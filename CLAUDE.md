---
skills: seacow-conventions, knowledge-curator, obsidian-markdown
---

# CLAUDE.md

Claude Code-specific instructions for this repo. Inherits everything in
[AGENTS.md](AGENTS.md) — read that first.

## Skills auto-loaded for this project

- `seacow-conventions` — apply the SEACOW(r) lens when asked "where should X go?" or "is this structure consistent?"
- `knowledge-curator` — temperature-gradient placement (this repo runs cooled-only by design; flag drafts that don't belong on `main`)
- `obsidian-markdown` — for frontmatter and wikilink-to-markdown conversion during migration

The user-level versions live in `~/.claude/skills/`. Public copies (scrubbed)
live at [02-tools/skills/](02-tools/skills/) and are intended to be readable by
anyone visiting the repo.

## Public scaffold (in this repo)

- [.claude/skills/seacow-conventions/SKILL.md](.claude/skills/seacow-conventions/SKILL.md) — thin pointer to the canonical public copy at `02-tools/skills/seacow-conventions/SKILL.md`
- [.claude/agents/seacow-scaffolder.md](.claude/agents/seacow-scaffolder.md) — thin pointer to the canonical public copy at `02-tools/agents/seacow-scaffolder.md`

The thin-pointer pattern lets the `.claude/` folder boot Claude Code with just
the frontmatter while the actual content lives in user-readable docs.

## Routing notes

- "Where should I put X?" → invoke `seacow-conventions` skill, then map to folder per [AGENTS.md § When asked 'where should X go?'](AGENTS.md).
- "What's the canonical SEACOW(r) definition?" → [01-framework/meta-framework.md](01-framework/meta-framework.md). Don't paraphrase.
- "Migrate this from cyberbase" → follow [AGENTS.md § Migration policy](AGENTS.md). Always flag substantive edits.
- "Compare SEACOW(r) to X" → [04-comparisons/](04-comparisons/) — add a stub if X isn't covered yet.

## Don't

- Don't invoke the `seacow-scaffolder` agent against this repo — its template-scaffolding flow is for *new* projects. This repo is its source-of-truth, not a target.
- Don't rewrite migrated cyberbase content without flagging diffs. Reference the source frontmatter line and explain the editorial change in the commit body.
- Don't commit with AI attribution. The maintainer's global commit-msg hook will reject `Co-Authored-By: Claude`, `Generated with`, `noreply@anthropic.com`, etc.
- Don't add wikilinks to committed files (see AGENTS.md).

## Quick references

- Canonical SEACOW(r) definition: [01-framework/meta-framework.md](01-framework/meta-framework.md)
- Public skill body: [02-tools/skills/seacow-conventions/SKILL.md](02-tools/skills/seacow-conventions/SKILL.md)
- Public agent body: [02-tools/agents/seacow-scaffolder.md](02-tools/agents/seacow-scaffolder.md)
- Multi-path indexes: [INDEXES/](INDEXES/)
