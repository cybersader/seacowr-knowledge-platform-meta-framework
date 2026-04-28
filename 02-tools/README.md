# 02 — Tools

The apply-it layer. Skills, agents, plugins, and platform-operational notes.

| Folder | Contains |
|---|---|
| [skills/](skills/) | Reusable AI skills. Currently: `seacow-conventions` (the analytical lens as a Claude Code skill). |
| [agents/](agents/) | AI agent definitions. Currently: `seacow-scaffolder` (proactive agent for designing new project structures). |
| [plugins/](plugins/) | Documentation for plugins that implement or enable SEACOW(r). Currently: `dynamic-tags-folders` (bidirectional folder↔tag sync). |
| [platform-notes/](platform-notes/) | Platform-specific operational guidance — limitations, bugs, workarounds. Currently: Obsidian tag limitations, tag bugs, plugin ecosystem. |

## Public-vs-private skill / agent split

The canonical public copies of skills and agents live here under `02-tools/`.
Thin pointers in [../.claude/](../.claude/) re-declare their frontmatter and
defer to these public bodies for content. The user's `~/.claude/` versions on
their own machine may be richer and contain personal paths — that's intentional.

If you fork this repo and want richer versions of the skills/agents on your own
machine, copy `02-tools/skills/seacow-conventions/SKILL.md` to
`~/.claude/skills/seacow-conventions/SKILL.md` and customize from there.
