# Agents

Public copies of agents that apply SEACOW(r). These are the **canonical**
versions; thin `.claude/agents/<name>.md` pointers re-declare frontmatter
and defer to these bodies.

| Agent | Purpose |
|---|---|
| [seacow-scaffolder.md](seacow-scaffolder.md) | Proactively used when setting up a new project, vault, or workspace. Designs organizational structures via SEACOW(r) analysis (not template copying). |

## Forking these agents

If you want richer / personalized versions on your own machine:

1. Copy the `.md` file to `~/.claude/agents/<name>.md`.
2. Customize freely — add your own context, paths, model preferences.
3. Your fork stays personal; this repo's version stays public-canonical.

## Adding a new agent here

An agent belongs in this folder if:

- It applies SEACOW(r) directly (not just SEACOW(r)-flavored).
- It's stable and useful across projects.
- It doesn't reference personal paths or project-specific scaffolds.

Format: standard Claude Code agent spec — frontmatter (`name`, `description`,
`tools`, `model`, optionally `skills`, `memory`) and a body describing the
agent's process.
