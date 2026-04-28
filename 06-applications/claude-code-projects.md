---
title: SEACOW(r) for Claude Code projects
publish: true
---

# SEACOW(r) for Claude Code projects

How to apply the SEACOW(r) framework to a [Claude Code](https://claude.com/claude-code)
project — specifically the structure of the `.claude/` directory and the
surrounding repo.

## Claude Code's organizational primitives

- **Skills** (`.claude/skills/<name>/SKILL.md`) — reusable analytical / procedural capabilities loaded on demand.
- **Agents** (`.claude/agents/<name>.md`) — specialized sub-agents Claude can spawn.
- **Commands** (`.claude/commands/<name>.md`) — slash-commands that wrap prompts.
- **Hooks** (in `.claude/settings.json`) — shell hooks fired on tool events.
- **Settings** (`.claude/settings.json`, `.claude/settings.local.json`) — permissions, env, hooks.
- **CLAUDE.md** at any depth — instructions for Claude when working in that directory.
- **AGENTS.md** at any depth — universal cross-tool agent instructions.
- **Plans** (in `~/.claude/plans/` or per-project) — staged implementation plans.
- **Memory** (in `~/.claude/projects/<id>/memory/`) — persistent per-project memory.

## Mapping SEACOW(r) → Claude Code

| Component | Claude Code primitives |
|---|---|
| **System** | The `.claude/` folder itself; settings.json hooks; the skills/agents/commands runtime |
| **Entity** | The user, the AI agents (Claude, Cursor, etc.), the project's downstream readers |
| **Capture** | Plans (`~/.claude/plans/`); session logs; raw exploration outputs |
| **Work** | The project's source code + KB; in-progress design docs; staged plans |
| **Output** | Documentation; published code; READMEs; user-facing artifacts |
| **relation** | CLAUDE.md routing notes; cross-links between KB files; skill ↔ agent references |

## Two-level structure: user-level vs project-level

- **`~/.claude/`** is the user's personal scaffold — skills, agents, commands they bring to every project.
- **`<project>/.claude/`** is the project's scaffold — project-specific skills, agents, hooks, instructions.

Treat them as two separate **Systems** in SEACOW(r) terms — they have
different Entities (user-only vs project-readable) and often different
Capture / Work / Output rules.

## Public-vs-private skill / agent split

If your project is open-source, the `.claude/` folder is *public*. That
creates a tension with the "richer personal user-level skills" pattern —
your `~/.claude/skills/seacow-conventions/SKILL.md` may contain personal
paths and project-specific examples that don't belong in the public scaffold.

The pattern this repo uses:

- Canonical **public** copies of skills / agents live in `02-tools/skills/` and `02-tools/agents/`.
- Thin pointers in `.claude/skills/` and `.claude/agents/` re-declare frontmatter and defer to the canonical body.
- The user's `~/.claude/` versions stay richer with personal context.

## Recommended starter structure

```
project/
├── AGENTS.md                       # universal agent instructions
├── CLAUDE.md                       # Claude-specific (skill preloading)
├── README.md
├── .claude/
│   ├── settings.json               # permissions, hooks (committed)
│   ├── settings.local.json         # per-machine paths (gitignored)
│   ├── skills/
│   │   └── <skill>/SKILL.md        # public scaffold
│   └── agents/
│       └── <agent>.md
└── ...                             # source code, docs, KB
```

For a docs / KB-only project (like this repo), drop the source code; everything
else stays.

## Multi-session persistence

Long-lived projects often add a `knowledge-base/` folder with the
[temperature gradient](../01-framework/design-principles.md#7-the-temperature-gradient-when-used)
(00-inbox / 01-working / 02-learnings / 03-reference / 04-archive). The
`knowledge-curator` skill nudges the AI to respect the gradient.

This repo deliberately *omits* the gradient for v0.1.0 — see [README.md § Conventions](../README.md#conventions).

## Cross-references

- The KB-as-the-project's-brain principle: [../01-framework/design-principles.md](../01-framework/design-principles.md#appendix-knowledge-base-as-the-projects-brain).
- The user's broader workflow scaffold: [cybersader/agentic-workflow-and-tech-stack](https://github.com/cybersader/agentic-workflow-and-tech-stack) (public).
