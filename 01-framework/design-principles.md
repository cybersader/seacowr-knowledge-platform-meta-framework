---
title: SEACOW(r) Design Principles
publish: true
source: cybersader/cyberbase — 📁 54 - Obsidian Vault Organization/.claude/CLAUDE.md (split — framework-level content) + KNOWLEDGE_BASE_PHILOSOPHY.md (appendix)
---

# SEACOW(r) design principles

Cross-cutting principles that aren't specific to one component. Read these
after the [meta-framework](meta-framework.md) and the [components/](components/)
pages.

---

## 1. Start with purpose and audience

Every structural decision should trace back to an answer to *why are you
organizing this?* and *who is it for?* Without these answers, you're guessing.
This is the same opening move described in the [meta-framework](meta-framework.md);
it bears repeating because it's the principle people skip.

## 2. The core problem: hierarchy vs. graph

**Knowledge is networked. File systems aren't.** Most knowledge platforms
(Obsidian, file shares, Notion's pages, Git repos) are built on hierarchical
storage even though human knowledge doesn't fit a single hierarchy. SEACOW(r)
makes the design tension explicit and gives you a vocabulary for resolving it.

The resolution is almost always: **use folders for the dominant
Entity-perspective, and use tags / links / properties to recover the graph
layer that the file system suppresses.** When the file system *itself* needs
to express polyhierarchy, you need a bridging tool — see
[../02-tools/plugins/dynamic-tags-folders/concept.md](../02-tools/plugins/dynamic-tags-folders/concept.md).

## 3. Separate process from content

Folders should structure your **knowledge work process**, not your content.
Tags, links, and properties structure your **content**. The single most
important application: don't build deep folder hierarchies for topics —
that's what tags / properties / links are for.

## 4. Polyhierarchy is the norm, not the exception

Most knowledge has multiple parents. A note about "encryption in healthcare"
belongs under both `Cybersecurity` and `Healthcare`. Folder systems force you
to pick one parent; tag and link systems let you have many. SEACOW(r) is
neutral about which primitive you use — but it expects you to make the
poly-hierarchy decision *deliberately* in light of System constraints.

The [obsidian-folder-tag-sync plugin](https://github.com/cybersader/obsidian-folder-tag-sync)
solves this for the Obsidian System; see
[../02-tools/plugins/dynamic-tags-folders/concept.md](../02-tools/plugins/dynamic-tags-folders/concept.md).

## 5. LATCH for retrieval

Once content exists, retrieval is the second-half of the organization problem.
[LATCH](../04-comparisons/vs-latch.md) (Wurman: Location, Alphabet, Time,
Category, Hierarchy) is a useful pairing — SEACOW(r) decides *what to organize*,
LATCH decides *how to make it findable*. They compose; they don't compete.

Apply LATCH especially to the **Output** layer — it's the audience-facing
surface that needs to be findable.

## 6. ARC: Add, Relate, Communicate

Nick Milo's ARC (Add → Relate → Communicate) is a Work-area rhythm that maps
naturally to SEACOW(r): **Add** is Capture+Work, **Relate** is the Relation
layer, **Communicate** is Output. ARC is a useful daily-practice rhythm;
SEACOW(r) is the structural lens.

## 7. The temperature gradient (when used)

Some applications of SEACOW(r) use a temperature-gradient pacing model:

```
hot  → 00-inbox/        (raw captures, session notes)
       01-working/      (active synthesis)
       02-learnings/    (patterns extracted)
       03-reference/    (cool reference material)
cold → 04-archive/      (frozen, Johnny Decimal by domain)
```

Content moves from hot to cold over time. This is a *Work-area* pacing
discipline — it lives inside the Work component, not as a top-level layer.
Use it when you have multi-session persistence and want to track maturity.
The `knowledge-curator` skill (in
[~/.claude/skills/](https://github.com/cybersader/cybersader-agentic-workflow-and-tech-stack)
and mirrored at [../02-tools/skills/](../02-tools/skills/)) is the AI-side
enforcement layer.

## 8. Best practices (distilled from real instantiations)

### Start simple, scale up

- Don't over-engineer initially.
- Let structure emerge from use.
- Refactor incrementally as your understanding deepens.

### Design for recall

Apply LATCH to the audience-facing layer. Where will a reader (your future
self included) look for this?

### Separate process from content

Folders → workflow stages. Tags → content ontology. Don't duplicate without a
reason.

### Multiple perspectives

- Folders for primary audience.
- Tags for alternative views.
- Links for specific relationships.
- Frontmatter for structured attributes.

### Consistent naming

- Choose a case convention (snake_case, Title Case, kebab-case) per primitive.
- Stick to it within each system.
- Document the convention so collaborators (human or AI) can follow it.

### Folder notes (optional)

- Index folders with notes of the same name.
- Pros: show up in graph view, provide context.
- Cons: discipline cost.

---

## Appendix: Knowledge-base-as-the-project's-brain

> The KB is **not** documentation created after the fact — it **IS** the
> project's brain.

A philosophy from cyberbase that pairs naturally with SEACOW(r). Reproduced
here from `cyberbase/📁 54 - Obsidian Vault Organization/.claude/KNOWLEDGE_BASE_PHILOSOPHY.md`.

### Core principle

All projects follow a living markdown KB pattern, designed for both human and
LLM-agent collaboration. The KB evolves as understanding deepens, decisions
are made, and implementation progresses. It serves as **persistent memory
across sessions and agents.**

### Why this pattern

**For humans:** searchable (grep, Obsidian, VS Code all work), portable (no
vendor lock-in), Git-friendly (diffs, history, collaboration), human-readable.

**For LLM agents:** context loading at session start, persistent memory
across sessions, structured output (research goes INTO files, not just chat),
multi-agent friendly, auditable.

### Working with LLM agents

**Session start pattern:**

1. Agent reads the project's `.claude/` folder for context.
2. Agent reads relevant KB files for the task at hand.
3. Agent has full context without re-explaining.

**During work:**

- **UPDATE** KB files as new information is learned.
- **CREATE** new files for new topics (don't dump in chat).
- **LINK** between related files.
- **DELETE** obsolete content.

**Research tasks — output goes INTO the KB, not just displayed in chat:**

> ❌ "Here's what I found about DNS filtering: [wall of text in chat]"
> ✅ "I've created `DNS_FILTERING_DEEP_DIVE.md` with my findings."

**Implementation tasks:**

1. Document decisions and rationale in the KB **before** coding.
2. Update architecture docs as implementation reveals new info.
3. KB explains **why**; code explains **how**.

**Multi-session continuity:**

```
Session 1: Research competitors → creates 02-competitors/*.md
Session 2: Agent reads competitor files → has full context
Session 3: Design architecture → creates 03-architecture/*.md
```

### File naming conventions

`SCREAMING_SNAKE_CASE.md`. Names should be descriptive, unique across project,
self-documenting, and specific enough to grep.

> Note: in *this* repo we use `kebab-case.md` because GitHub renders kebab-case URLs better. The SCREAMING_SNAKE_CASE convention applies to KB-philosophy projects (where SCREAMING names sort obviously and grep cleanly). Pick one per project and stay consistent.

### Standard project structure

```
project/
├── .claude/                    # Meta: how to work on this project
│   ├── PROJECT_CONTEXT.md      # What is this, who's it for, background
│   ├── KNOWLEDGE_BASE_PHILOSOPHY.md  # This file (or link to global)
│   └── [project-specific guidance]
│
├── 00-overview/                # Vision, goals, principles
├── 01-problem/                 # Problem definition, constraints, landscape
├── 02-research/                # Or 02-competitors/ — analysis of existing work
├── 03-architecture/            # Technical designs, decisions
├── 04-implementation/          # Or platform-specific folders
└── ...
```

Numbered prefixes ensure consistent ordering in file explorers — and they map
nicely to SEACOW(r): `00-overview` is OUTPUT (what's this for an outsider?),
`01-problem` is the framing for Work, `02-research` is Capture-becoming-Work,
`03-architecture` is Output of synthesis.

### KB evolution principles

1. **Create files early.** Don't wait until you "know enough." Create a file when you start exploring a topic — it will grow.
2. **Split when large.** If a file exceeds ~500 lines or covers multiple distinct topics, split it.
3. **Update, don't append.** When understanding changes, update existing content rather than appending "UPDATE: actually..." notes. The KB reflects *current* understanding.
4. **Link between files.** Use relative links — `See [DNS Services](../02-competitors/DNS_FILTERING_SERVICES_DEEP_DIVE.md)`.
5. **Delete obsolete content.** Git history has the old version if you need it back.
6. **Index files are valuable.** Create index / overview files that link to detailed files. `TOOLS_INDEX.md` links to individual tool analyses.

### The `.claude/` folder

Every project should have a `.claude/` folder with at minimum a
`PROJECT_CONTEXT.md` that an agent reads first. Optional but recommended:
`RESEARCH_SOURCES.md`, `CONVENTIONS.md`, `CURRENT_STATUS.md`. The folder is
**the first thing an agent reads** when starting work — it provides the
meta-context needed to work effectively.

### Anti-patterns

**Don't:**

- Create one giant file for everything.
- Use generic names like `notes.md` or `info.md`.
- Leave outdated information in files.
- Put temporary thoughts in permanent files.
- Keep research only in chat (it disappears).
- Expect agents to remember previous sessions without a KB.

**Do:**

- One topic per file (roughly).
- Descriptive, searchable names.
- Update as understanding evolves.
- Use consistent structure.
- Cross-link related files.
- Write findings to files, not just chat.

### How this pattern relates to SEACOW(r)

The KB-as-the-project's-brain principle is itself an instance of SEACOW(r):

- **System** — markdown files in a Git repo (sometimes also an Obsidian vault).
- **Entity** — humans + LLM agents, each reading the same files.
- **Capture** — research notes, session logs, raw findings (the inbox / hot zone).
- **Work** — synthesis files, architecture decisions (warm zone).
- **Output** — the published KB itself; the README; the canonical-decision files (cooled).
- **relation** — cross-links between KB files, MOCs, index files.

Applying SEACOW(r) thinking to the KB makes it self-consistent: the
*structure of the project's brain* obeys the same framework that the brain is
designed to teach.

## Cross-references

- Meta-framework: [meta-framework.md](meta-framework.md).
- Rules: [rules.md](rules.md).
- Choosing among primitives: [../05-deep-dives/folders-vs-tags-vs-links-vs-metadata.md](../05-deep-dives/folders-vs-tags-vs-links-vs-metadata.md).
- LATCH comparison: [../04-comparisons/vs-latch.md](../04-comparisons/vs-latch.md).
- Obsidian application: [../06-applications/obsidian.md](../06-applications/obsidian.md).
