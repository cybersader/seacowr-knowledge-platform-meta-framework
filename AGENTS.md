# AGENTS.md

Universal agent instructions for this repo. Applies to Claude Code, OpenCode,
Cursor, Cline, Codex, and any other AI coding assistant. Tool-specific
addendums live in their own files (e.g. [CLAUDE.md](CLAUDE.md)).

## What this repo is

A documentation / knowledge base for the **SEACOW(r) Knowledge Platform
Organization Meta-Framework**. There is **no build system, no test suite, no
runtime code** to ship. Treat it as a publication, not a coding project.

## Read order for orientation

1. [README.md](README.md) — what's here and where to start
2. [00-start-here/quick-start.md](00-start-here/quick-start.md) — 5-minute SEACOW(r) primer
3. [01-framework/meta-framework.md](01-framework/meta-framework.md) — the canonical definition
4. The `INDEXES/` files — multiple navigation paths
5. The folder relevant to the user's question (`02-tools/`, `03-examples/`, etc.)

## Editing conventions

- **Relative-path markdown links** — e.g. `[meta-framework](../01-framework/meta-framework.md)`. Not wikilinks. GitHub must render every link clickable.
- **Preserve frontmatter** on migrated files — `publish`, `aliases`, `permalink`, `date created`, `date modified`. These exist so the same files can be re-published via Obsidian Publish.
- **Kebab-case file names** — exception: top-level numbered folders (`00-start-here/`, etc.) keep their `NN-name/` shape.
- **Numbered top-level folders are stable** — do not renumber once published. Numbers encode reading order.
- **No emojis in committed file paths** (cyberbase uses `📁 NN - Name/` — that aesthetic stays in cyberbase; this repo is GitHub-clean).

## Migration policy

When porting content from `cybersader/cyberbase` (the upstream working vault):

- Convert wikilinks `[[Foo]]` → relative markdown links.
- URL-decode any percent-encoded paths (e.g. `Knowledge%20Platform` → just rewrite the link to the new repo path).
- Strip cyberbase-specific paths (e.g. `📁 54 - Obsidian Vault Organization/`).
- Preserve the original frontmatter; add a `source:` line pointing back to the cyberbase path so we can audit drift.
- Don't rewrite migrated content silently — flag substantive edits in the commit message.

## When asked "where should X go?"

Use the [seacow-conventions skill](.claude/skills/seacow-conventions/SKILL.md)
(Claude Code) or apply the same reasoning manually:

1. Is this raw input or processed? (Capture vs Work)
2. Is this finished or in progress? (Output vs Work)
3. Who is this for? (Entity)
4. What are platform constraints? (System)
5. How does it connect? (Relation)

Then map to a folder:

- `00-start-here/` — only if it's an entry-point doc (TL;DR, quick-start, glossary)
- `01-framework/` — concept-layer canon (definitions, components, rules)
- `02-tools/` — skills, agents, plugins, platform-specific operational notes
- `03-examples/` — concrete instantiations (real vaults, rule-packs, fixtures)
- `04-comparisons/` — SEACOW(r) vs other framework
- `05-deep-dives/` — long-form theory or decision matrices
- `06-applications/` — "SEACOW(r) for X" — applying it to a specific platform
- `INDEXES/` — only re-curation of existing files; no new primary content here

## Commit conventions

- **Subject** — `area: imperative subject`, e.g. `01-framework: split activities into per-component pages`. Areas: `00-start-here`, `01-framework`, `02-tools`, `03-examples`, `04-comparisons`, `05-deep-dives`, `06-applications`, `indexes`, `meta`, `tools`.
- **No AI / LLM attribution.** Commit as the human contributor only. Do not add any `Co-Authored-By:` trailer for an AI tool or LLM service, and do not include "generated with…" footers. The maintainer enforces this via a global commit-msg hook.
- **Group migrations** — one commit per migration group (entry / components / examples / deep-dives / platform-notes / split-redistribute). Keeps `git log` readable.

## What NOT to do

- Don't run `npm install`, `npm run build`, `bun install`, or any other build/install commands. There's no package.json by design.
- Don't create a `package.json`, `tsconfig.json`, `Cargo.toml`, etc. — this is a docs repo.
- Don't restructure numbered folders without a tracked decision (see commit message conventions).
- Don't introduce wikilinks in committed files. Obsidian users can still wikilink from their own vault that imports this repo; the committed files stay GitHub-friendly.
- Don't auto-sync from cyberbase — migrations are intentional editorial events. A `MIGRATION_LOG.md` will track sync points (post-v0.1.0).

## When you finish a session

If you split, merged, or substantially edited migrated content, append a one-line note to a commit message body explaining the editorial diff from the cyberbase source. This makes the public/private divergence auditable.
