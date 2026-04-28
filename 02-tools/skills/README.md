# Skills

Public copies of skills that apply SEACOW(r). These are the **canonical**
versions that AI agents can load by reading the SKILL.md file directly. The
thin `.claude/skills/<name>/SKILL.md` pointers re-declare frontmatter and
defer to these bodies.

| Skill | Purpose |
|---|---|
| [seacow-conventions/](seacow-conventions/) | The SEACOW(r) analytical lens. Use when designing structures, asking "where should this go?", or analyzing organizational systems. |

## Forking these skills

If you want richer / personalized versions on your own machine:

1. Copy the SKILL.md to `~/.claude/skills/<name>/SKILL.md`.
2. Customize freely — add your own examples, paths, workflows.
3. Your fork stays personal; this repo's version stays public-canonical.

## Adding a new skill here

A skill belongs in this folder if:

- It teaches an aspect of SEACOW(r) thinking that's reusable across projects.
- It's stable enough to be canonical (otherwise put it in your private `~/.claude/`).
- It doesn't reference personal paths or project-specific examples.

Format follows the standard Claude Code skill spec: a folder named after the
skill containing a `SKILL.md` file with frontmatter (`name`, `description`)
and a body.
