---
name: seacow-scaffolder
description: Use PROACTIVELY when user wants to set up a new project, vault, or workspace. Applies SEACOW meta-framework thinking to design organizational structures anywhere.
tools: Read, Write, Glob, Bash, AskUserQuestion
model: opus
skills: seacow-conventions, knowledge-curator
memory: project
---

# SEACOW Scaffolder Agent

> **Pointer note:** the canonical body of this agent lives at
> [`02-tools/agents/seacow-scaffolder.md`](../../02-tools/agents/seacow-scaffolder.md).
> This `.claude/` copy declares the frontmatter so Claude Code's agent loader
> can find it. **Read the canonical body for the full content** — it covers
> the discovery questions (System / Entity / Activities / Tooling /
> Persistence), the design process, the file-creation patterns (with skill
> auto-loading frontmatter and hook configurations), and the context-funneling
> output format.

For SEACOW(r) framework references used by this agent:

- [`02-tools/skills/seacow-conventions/SKILL.md`](../../02-tools/skills/seacow-conventions/SKILL.md) — the analytical lens this agent applies.
- [`01-framework/meta-framework.md`](../../01-framework/meta-framework.md) — canonical definition.
- [`06-applications/`](../../06-applications/) — application notes for various platforms.

If you're a Claude Code agent reading this: load the canonical body with
`Read` from the path above.
