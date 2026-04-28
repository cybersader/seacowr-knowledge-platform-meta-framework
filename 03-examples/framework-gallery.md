---
title: Framework Instantiations Gallery
publish: true
---

# Framework Instantiations Gallery

A side-by-side gallery of organizational frameworks with their **concrete
folder/tag trees**, the **starter kits** that ship them, and a **SEACOW(r)
mapping** for each.

Conventions used in this page:

- **"Tree"** quotes the exact folder layout from a real starter kit or
  reference repo where one exists; otherwise it shows the canonical layout from the framework's primary source.
- **"SEACOW(r) mapping"** is a 7-row table — System / Entity / Activities / Capture / Output / Work / relation — showing which platform structure addresses each component.
- **"Where it lives in your stack"** points to your local starter kits,
  GitHub repos, or cyberbase content that instantiates the framework.
- This page is a *gallery*, not a tutorial. For depth, follow the per-framework page in [../04-comparisons/](../04-comparisons/).

---

## Table of contents

- [Personal knowledge management (PKM) frameworks](#personal-knowledge-management-pkm-frameworks)
  - [PARA](#para--projects--areas--resources--archive)
  - [PARAUT](#paraut--corporate-para-extension)
  - [Building a Second Brain (BASB) + CODE](#building-a-second-brain-basb--code)
  - [Zettelkasten (Luhmann / Ahrens)](#zettelkasten-luhmann--ahrens)
  - [Atomic-notes / FLAP](#atomic-notes--flap-fleeting--literature--atomic--project)
  - [Linking Your Thinking (LYT) / Ideaverse / Maps of Content](#linking-your-thinking-lyt--ideaverse--maps-of-content)
  - [evergreen notes (Andy Matuschak)](#evergreen-notes-andy-matuschak)
- [Process / workflow frameworks](#process--workflow-frameworks)
  - [ARC (Add, Relate, Communicate)](#arc-add-relate-communicate)
  - [ACE (Atlas, Calendar, Efforts)](#ace-atlas-calendar-efforts)
  - [STIR (Space, Time, Importance, Relatedness)](#stir-space-time-importance-relatedness)
  - [ARCO (Atlas, Reference, Calendar, Organizer)](#arco-atlas-reference-calendar-organizer)
  - [e-ACCESS](#e-access-encounters--atlas--calendar--cards--extras--sources--spaces)
  - [WO(R)C(S) / SEACOW lineage](#worcs--seacow-lineage)
  - [Capture-Work-Output (CWO)](#capture-work-output-cwo)
- [Hierarchical / numeric / retrieval frameworks](#hierarchical--numeric--retrieval-frameworks)
  - [Johnny Decimal](#johnny-decimal)
  - [LATCH (Wurman)](#latch-wurman)
  - [DIKW pyramid](#dikw-pyramid)
  - [Numbered + emoji prefix (cyberbase variant)](#numbered--emoji-prefix-cyberbase-variant)
- [Library science / formal classification](#library-science--formal-classification)
  - [Library of Congress Classification (LCC)](#library-of-congress-classification-lcc)
  - [Library of Congress Subject Headings (LCSH)](#library-of-congress-subject-headings-lcsh)
  - [Dewey Decimal Classification (DDC)](#dewey-decimal-classification-ddc)
  - [Universal Decimal Classification (UDC)](#universal-decimal-classification-udc)
  - [Ranganathan's Colon Classification (PMEST)](#ranganathans-colon-classification-pmest)
  - [Controlled vocabulary types (8 forms)](#controlled-vocabulary-types-8-forms)
  - [Folksonomy](#folksonomy)
- [Domain-specific vault starters](#domain-specific-vault-starters)
  - [obsidian-secops-vault-template (cybersader)](#obsidian-secops-vault-template-cybersader)
  - [cyberbase (cybersader)](#cyberbase-cybersader)
  - [Ideaverse Lite 1.5 (LYT)](#ideaverse-lite-15-lyt)
  - [Weave (corporate, cuken)](#weave-corporate-cuken)
  - [The Good Parts v2 (FLAP)](#the-good-parts-v2-flap)
  - [Other starters in your collection](#other-starters-in-your-collection)
- [Cybersecurity compliance frameworks (specialized)](#cybersecurity-compliance-frameworks-specialized)
  - [NIST Cybersecurity Framework 2.0 (CSF 2.0)](#nist-cybersecurity-framework-20-csf-20)
  - [NIST SP 800-53 control families](#nist-sp-800-53-control-families)
  - [CIS Controls (IG1 / IG2 / IG3)](#cis-controls-ig1--ig2--ig3)
  - [MITRE ATT&CK / D3FEND / Engage](#mitre-attck--d3fend--engage)
  - [Cyber Kill Chain](#cyber-kill-chain)
  - [Diamond Model](#diamond-model)
  - [Crosswalking — CSF 2.0 → 800-53 → CRI](#crosswalking--csf-20--800-53--cri)
- [Other frameworks (concise)](#other-frameworks-concise)
  - [D.E.E.Z.N.U.T.S.](#deeznuts)
  - [EJK (Efforts, Journal, Knowledge)](#ejk-efforts-journal-knowledge)

---

# Personal knowledge management (PKM) frameworks

## PARA — Projects · Areas · Resources · Archive

**Origin:** Tiago Forte (Forte Labs) · [fortelabs.com/blog/para/](https://fortelabs.com/blog/para/)

**Core principle:** order folders by **actionability** — most-actionable
(Projects) on top, least (Archive) on the bottom.

**Tree (verbatim from `PARA_Starter_Kit_v2/`):**

```
1. Projects/
   ├── Notes Migration/
   ├── Obsidian Theme/
   └── PARA Starter Kit/

2. Areas/
   ├── Blog/
   ├── Finance/
   ├── Health/
   ├── House/
   ├── Job/
   ├── Personal Development/
   └── Productivity/

3. Resouces/                  # (typo in original starter)
   ├── Community/
   ├── Cooking/
   ├── Development/
   ├── Drawing/
   ├── Gaming/
   ├── Marketing/
   ├── Personal Knowledge Management/
   ├── Productivity/
   ├── Travel/
   └── Writing/

4. Archive/
   ├── 2020-05-05-Archive/
   ├── Apartment/
   ├── Moving to new city/
   └── Summer vacation 2019/
```

**SEACOW(r) mapping:**

| SEACOW(r) | PARA expression |
|---|---|
| **System** | Folder-only; relies on Dataview for relation surfaces. |
| **Entity** | Single user, implicit. |
| **Capture** | Not explicit — PARA expects you to land things in `1. Projects/` or `3. Resources/` directly. Many users add an `0. Inbox/` ahead. |
| **Output** | Not explicit — published items live wherever (typically inside Projects or Archive). |
| **Work** | Mostly inside `1. Projects/` and `2. Areas/`. |
| **relation** | Wikilinks + folder hierarchy; tags optional. |

**Where it lives in your stack:**

- `cybersader-vault-starters/starters (not mine)/PARA_Starter_Kit_v2/`
- Numbered SecOps variant in `obsidian-secops-vault-template/` uses `01 - Projects, Workspaces/` + `02 - Areas, Objectives, Initiatives, Ongoing/` + `05 - Archive, Admin/`.

**Variants in the wild:**

- **PARAUT** — adds Unstructured + Taxonomies (next entry).
- **PARA + Inbox** — `0. Inbox/` ahead of Projects.
- **CODE-PARA** — pairs PARA with Forte's CODE workflow (Capture, Organize, Distill, Express).

**Detail page:** [../04-comparisons/vs-para.md](../04-comparisons/vs-para.md)

---

## PARAUT — corporate PARA extension

**Origin:** community variant referenced in cyberbase's `Knowledge Organization.md`.

**Tree:**

```
1. Projects, Workspaces/
2. Areas, Initiatives/
3. Resources, Topics/
4. Archive, Admin/
5. Unstructured/
6. Taxonomies, Ontologies/
```

**SEACOW(r) mapping:**

| SEACOW(r) | PARAUT expression |
|---|---|
| Capture | `5. Unstructured/` (explicit, unlike vanilla PARA) |
| Work | 1, 2, 3 |
| Output | implicit, often in Archive or a dedicated published-folder |
| relation | `6. Taxonomies, Ontologies/` (the explicit graph layer) |

**Why it matters:** PARAUT adds the two layers vanilla PARA omits — explicit Capture and explicit relation. Closer to SEACOW(r) in spirit.

**Source quote (cyberbase):**

> 1. Projects, Workspaces  2. Areas, Initiatives  3. Resources, Topics  4. Archive, Admin  5. Unstructured  6. Taxonomies, Ontologies — *Cyberbase, 📁 17 - Knowledge Engineering / Knowledge Organization.md*

---

## Building a Second Brain (BASB) + CODE

**Origin:** Tiago Forte, *Building a Second Brain* (2022).

**The CODE workflow** (Forte's process layer that pairs with PARA):

| Letter | Meaning | SEACOW(r) |
|---|---|---|
| **C** | **C**apture — keep what resonates | Capture |
| **O** | **O**rganize — by actionability into PARA | Work (placement decision) |
| **D** | **D**istill — find essence (progressive summarization) | Work |
| **E** | **E**xpress — show your work, ship | Output |

**Tree:** PARA (above) is BASB's storage layer; CODE is the verb layer.

**Where it lives in your stack:**

- Implicit in your *FLAP* tag system (next-next entry) which fuses CODE-style verbs with Zettelkasten's note types.
- Referenced in cyberbase's `Knowledge Organization.md` (link to fortelabs.com).

**Variants:**

- **Just-In-Time PM** — Forte's lighter-weight project-management spin.
- **Progressive summarization** — the D step rendered as bold + highlight + summary tiers in the same note.

---

## Zettelkasten (Luhmann / Ahrens)

**Origin:** Niklas Luhmann's slip-box; modernized by Sönke Ahrens, *How to Take Smart Notes* (2017).

**Tree (from `Obsidian-Zettelkasten-Starter-Kit-3.0.0/`):**

```
Starter-Kit/
├── 1_Fleeting Notes/         # raw captures, pre-atomic
├── 2_Literature Notes/       # quotes from books, articles, videos (sourced)
├── 3_Permanent Notes/        # atomic, in your own words — the slip-box itself
├── 4_Bibliographical Notes/  # source metadata
├── 5_Structure Notes/        # hub / index notes (MOCs)
├── 6_Project Notes/          # output preparation
├── Assets/
├── Canvases/
├── Templates/
└── Visuals/
```

**SEACOW(r) mapping:**

| SEACOW(r) | Zettelkasten expression |
|---|---|
| System | Originally paper slip-box (Luhmann numbered 12.4a3); now Obsidian / The Archive / Roam |
| Entity | Single thinker; eventually published — implicit Output Entity |
| Capture | `1_Fleeting Notes/` + `2_Literature Notes/` |
| Work | `3_Permanent Notes/` (atomic, written in own words) |
| Output | `6_Project Notes/` + dense linking-graph that *eventually* yields papers / books |
| relation | The whole point — wikilinks + structure notes + ID system |

**Numbering scheme (Luhmann original):**

- Sequential IDs: `1`, `2`, `3` for top-level entries.
- Branch IDs: `1a`, `1b`, `1c` are continuations of `1`.
- Sub-branch: `1a1`, `1a2` continue `1a`.
- Result: a forest of depth-unlimited threads, each note locatable by ID.

**Where it lives in your stack:**

- `cybersader-vault-starters/starters (not mine)/Obsidian-Zettelkasten-Starter-Kit-3.0.0/`
- Referenced from cyberbase's `Knowledge Organization.md`.
- Adjacent: [groepl/Take-Useful-Notes](https://github.com/groepl/Take-Useful-Notes) (minimalist Zettelkasten ebook + kit).

**Detail page:** [../04-comparisons/vs-zettelkasten.md](../04-comparisons/vs-zettelkasten.md)

---

## Atomic-notes / FLAP (Fleeting · Literature · Atomic · Project)

**Origin:** community synthesis of PARA + Zettelkasten + GTD; appears in `cybersader-vault-starters/starters (not mine)/The Good Parts v2/`.

**This system uses tags, not folders:**

```
#fleeting             — raw captures; processed into atomic
#literature/unfiled   — unprocessed quotes from Readwise, books, videos, podcasts
#atomic               — processed, publishable unit of knowledge
#project              — items with a start AND end date
                        (areas have only start; archive has neither)
```

**SEACOW(r) mapping:**

| SEACOW(r) | FLAP expression |
|---|---|
| Capture | `#fleeting`, `#literature/unfiled` |
| Work | `#atomic` (synthesis), `#project` (action) |
| Output | publishable items (often `#atomic` items pulled into a `#project`) |
| relation | tag overlap + wikilinks |

**Why interesting:** tag-driven rather than folder-driven; Readwise-native (heavy literature-note inflow); makes the *publication contract* explicit (atomic = publishable unit).

---

## Linking Your Thinking (LYT) / Ideaverse / Maps of Content

**Origin:** Nick Milo · [linkingyourthinking.com](https://www.linkingyourthinking.com/) · the LYT Workshop and Ideaverse.

**Tree (verbatim from `Ideaverse Lite 1.5/`):**

```
Ideaverse Lite 1.5/
├── +/                       # templates, utilities (sorts to top)
├── Atlas/
│   ├── Dots/               # atomic notes / individual ideas
│   └── Maps/               # MOCs — index/navigation structures
├── Calendar/
│   ├── Logs/
│   └── Notes/
├── Efforts/                # Milo's "Efforts" replaces PARA's "Projects"
│   ├── Notes/
│   ├── On/                 # active
│   ├── Ongoing/            # simmering
│   └── Sleeping/           # paused
├── x/                      # admin / utility
│   ├── Excalidraw/
│   ├── Images/
│   └── Templates/
└── Home.md / Home Basic.md
```

**Frontmatter conventions (Ideaverse):**

```yaml
---
up: "[[Parent Note]]"
created: YYYY-MM-DD
obsidianUIMode: preview
in:
  - "[[Maps]]"
---
```

**Callout types (visual emphasis):** `[!Planet]`, `[!Network]`, `[!Joystick]`, `[!Snowflake]`, `[!Castle]`, `[!Puzzle]`, `[!Play]`, `[!Trees]`, `[!palette]`, `[!Link]`.

**SEACOW(r) mapping:**

| SEACOW(r) | Ideaverse expression |
|---|---|
| System | Obsidian, plugin-heavy (callouts, Dataview, Templater) |
| Entity | Single thinker; Home note is the entry point |
| Capture | `Calendar/Logs/`, `+/Inbox/` (if added) |
| Work | `Efforts/On/`, `Atlas/Dots/` |
| Output | `Atlas/Maps/`, published items |
| relation | The whole `Atlas/` — Dots + Maps form the bidirectional graph |

**Variants:**

- **Ideaverse Lite** (community, free) — minimal version above.
- **Ideaverse for Obsidian** — Milo's full course-companion vault.

**MOC plugin:** [IdreesInc/Waypoint](https://github.com/IdreesInc/Waypoint) auto-generates folder-MOC tables of contents and adds "Landmarks" as intermediary indexes.

**Where it lives in your stack:** `cybersader-vault-starters/starters (not mine)/Ideaverse Lite 1.5/`.

---

## evergreen notes (Andy Matuschak)

**Origin:** [notes.andymatuschak.org](https://notes.andymatuschak.org/) — Andy Matuschak's published note-garden + writing on the practice.

**Core principles (paraphrased):**

- **Evergreen notes should be atomic** — one concept per note.
- **Evergreen notes should be concept-oriented** — not source-oriented.
- **Evergreen notes should be densely linked.**
- **Prefer associative ontologies to hierarchical taxonomies** — the graph beats the tree.

**Tree:** flat. Matuschak's published vault is essentially flat with rich
linking — the *file system* expresses no hierarchy; the *link graph* does.

**SEACOW(r) mapping:**

| SEACOW(r) | evergreen-notes expression |
|---|---|
| System | Custom static-site renderer + flat folder |
| Entity | Public reader (Matuschak intentionally writes in public) |
| Capture | minimal — drafts in private; flow goes raw → polished evergreen |
| Work | the writing-and-rewriting loop — Matuschak edits notes for years |
| Output | the entire flat vault is the Output; Capture and Work happen *in place* via revision |
| relation | dense wikilinks; no folders |

**Why interesting:** the cleanest example of "let the graph be the structure." Pairs with Zettelkasten in spirit; very different from PARA.

**Where to encounter it:** referenced in cyberbase's `Knowledge Organization.md` link list ("Building a Second Brain illustrated notes — Maggie Appleton" + Matuschak's own site).

---

# Process / workflow frameworks

These aren't folder schemes — they're *rhythms* that overlay any folder scheme.

## ARC (Add, Relate, Communicate)

**Origin:** Nick Milo (LYT).

**Three verbs:**

- **A**dd — capture new information.
- **R**elate — connect to existing knowledge (links, MOCs, tags).
- **C**ommunicate — output for consumption.

**SEACOW(r) mapping (ARC is essentially SEACOW(r)'s Activities row):**

| ARC | SEACOW(r) Activity |
|---|---|
| Add | Capture (+ early Work) |
| Relate | Work + relation |
| Communicate | Output |

**Where it lives in your stack:** referenced in `cyberbase/📁 54 - Obsidian Vault Organization/Vault Folder & Tag Structure/` and migrated into [`../03-examples/cyberbase/vault-folder-and-tag-structure.md`](cyberbase/vault-folder-and-tag-structure.md).

---

## ACE (Atlas, Calendar, Efforts)

**Origin:** community insight from STIR — "the STI of STIR maps to ACE." Discussed in [The Ultimate Folder System: A quixotic journey to ACE](https://forum.obsidian.md/t/the-ultimate-folder-system-a-quixotic-journey-to-ace/63483).

**Tree:**

```
Atlas/        # SPACE of knowledge — MOCs, ontologies, conceptual maps
Calendar/     # TIME — daily notes, journals, meetings
Efforts/      # IMPORTANCE — projects, action-bound work
```

The "R" in STIR (Relatedness) = **the links you draw between Atlas/Calendar/Efforts entries.**

**SEACOW(r) mapping:**

| SEACOW(r) | ACE expression |
|---|---|
| Capture | typically pre-ACE (an Inbox added on top) |
| Work | `Efforts/` |
| Output | typically `Atlas/` (audience-facing maps) |
| relation | links between A/C/E + the implicit STIR-R |

---

## STIR (Space, Time, Importance, Relatedness)

**Origin:** community / forum discussion on the same Obsidian thread.

**Four organizing axes:**

- **S**pace — where the knowledge lives conceptually (Atlas).
- **T**ime — when it's relevant (Calendar).
- **I**mportance — how actionable / valuable (Efforts).
- **R**elatedness — how it connects to other items.

**Mapping:** STIR is the *retrieval* counterpart of LATCH — five (LATCH) or four (STIR) ways to make finished content findable. **Orthogonal** to SEACOW(r). Apply STIR or LATCH *inside* your Output layer to decide sort and navigation.

---

## ARCO (Atlas, Reference, Calendar, Organizer)

**Origin:** book-metaphor framework (community).

**Tree:**

```
Atlas/      # book of maps — relations, MOCs
Reference/  # book of facts and external links
Calendar/   # book of events — time-based
Organizer/  # book of tasks and projects
```

**SEACOW(r) mapping:**

| SEACOW(r) | ARCO expression |
|---|---|
| Capture | `Reference/` (sourced material) |
| Work | `Organizer/`, `Calendar/` |
| Output | `Atlas/` |
| relation | `Atlas/` (made explicit) + cross-links |

---

## e-ACCESS — Encounters · Atlas · Calendar · Cards · Extras · Sources · Spaces

**Origin:** extended community framework documented in your `Ideas for Knowledge Organization.md`.

**Tree:**

```
Encounters/   # cooling pad, unsorted, raw inputs (Capture)
Atlas/        # MOCs, dashboards, directories, overviews, consumption
Calendar/     # daily, meetings, journals
Cards/        # ideas, things, concepts, statements, atomic (Zettel-style)
Extras/       # support materials and images
Sources/      # clippings, articles, sources
Spaces/       # areas of life — each Space has its own PARA or sub-structure
```

**Why interesting:** this is one of the *most explicit* SEACOW(r)-shaped community frameworks — Encounters is pure Capture, Atlas is Output, Cards is Work, Sources is Capture, and Spaces is essentially Entity-scoping ("areas of life" = different audiences-of-self).

**SEACOW(r) mapping:**

| SEACOW(r) | e-ACCESS expression |
|---|---|
| Entity | `Spaces/<area-of-life>/` |
| Capture | `Encounters/` + `Sources/` |
| Work | `Cards/` + `Calendar/` + `Extras/` |
| Output | `Atlas/` |
| relation | links between Cards and Atlas |

**Where it lives in your stack:** quoted in [`../05-deep-dives/ideas-for-knowledge-organization.md`](../05-deep-dives/ideas-for-knowledge-organization.md).

---

## WO(R)C(S) / SEACOW lineage

**Origin:** your own working-notes — predecessor acronyms before SEACOW(r) settled.

| Acronym | Components | Status |
|---|---|---|
| **COW** | Capture, Output, Work | earliest sketch |
| **COWS** | Capture, Output, Work, System | second iteration |
| **WORCS** | Work, Output, Relation, Capture, System | "cause it just works" — explicit Relation |
| **WO(R)C(S)** | same as WORCS, parens around the optional pieces | published variant |
| **SEA(COWr)** | System, Entity, Activities (Capture, Output, Work, relation) | current |

**Where it lives in your stack:** [`../01-framework/meta-framework.md § Building my acronym`](../01-framework/meta-framework.md).

---

## Capture-Work-Output (CWO)

**Origin:** the bare three-verb engineering reduction underneath SEACOW(r).

The pure triplet — inputs / function / outputs. SEACOW(r) is what you get when you add Entity (audience) and System (platform) on top.

---

# Hierarchical / numeric / retrieval frameworks

## Johnny Decimal

**Origin:** [johnnydecimal.com](https://johnnydecimal.com/) — a numeric folder system designed for predictable retrieval.

**Tree:**

```
10-19 - Health/                # Area (10–19, 20–29, …, 90–99)
├── 11 - Fitness/              # Category (one digit inside the area)
│   ├── 11.01 - Running log/   # ID — every item has a stable address
│   ├── 11.02 - Lifting log/
│   └── 11.03 - Climbing log/
├── 12 - Nutrition/
│   ├── 12.01 - Recipes/
│   └── 12.02 - Macros/
└── 13 - Sleep/
    └── 13.01 - Sleep logs/
20-29 - Finance/
30-39 - …
```

**Rules:**

- Up to 10 areas (10–19, 20–29, …, 90–99).
- Up to 10 categories per area.
- Up to 100 IDs per category (`11.01` … `11.99`).
- The numbers are *stable addresses* — `11.04` keeps that name forever.

**SEACOW(r) mapping:**

| SEACOW(r) | JD expression |
|---|---|
| System | folder-only; no graph layer in JD itself |
| Entity | single user typically; can scope multi-user with separate JD systems |
| Capture | not addressed (JD is for cooled content) |
| Work / Output | both live inside JD addresses; JD is content-agnostic about their separation |
| relation | not addressed; people add wikilinks on top |

**When JD is the right answer:** bounded, slow-moving content (your home filing cabinet, finances, infrastructure inventory). When it's not: fluid evolving knowledge.

**Where it lives in your stack:**

- The cyberbase `📁 01 - Projects` … `📁 17 - Knowledge Engineering` folder convention is JD-flavored (one digit per area, no `.01` IDs).
- The SecOps starter `00 - Tasks, Planning/` … `99 - ARCHIVE/` is JD-flavored too.

**Detail page:** [`../04-comparisons/vs-johnny-decimal.md`](../04-comparisons/vs-johnny-decimal.md)

---

## LATCH (Wurman)

**Origin:** Richard Saul Wurman, *Information Anxiety* — five fundamental ways to organize information.

| Letter | Dimension | Example use |
|---|---|---|
| **L** | **L**ocation | maps; shop departments; geographic indexes |
| **A** | **A**lphabet | dictionaries; phone books; directories |
| **T** | **T**ime | timelines; journals; changelogs |
| **C** | **C**ategory | taxonomies; subject indexes; product types |
| **H** | **H**ierarchy | (originally "Continuum") rankings; magnitudes; trees |

**SEACOW(r) mapping:** LATCH is the *retrieval* axis. Apply it inside the Output layer of your SEACOW(r) instantiation.

**Where it lives in your stack:** [`../04-comparisons/vs-latch.md`](../04-comparisons/vs-latch.md) + cited throughout `📁 54 - Obsidian Vault Organization` notes.

---

## DIKW pyramid

**Origin:** information science (commonly attributed to Russell Ackoff, 1989).

```
            Wisdom        ← applied judgment
          Knowledge       ← synthesized, contextualized
       Information        ← processed, structured
     Data                 ← raw signals
```

**SEACOW(r) mapping:** DIKW is *vertical* (abstraction maturity); SEACOW(r) is *horizontal* (where content lives in a platform). They're orthogonal — a piece of "data" can sit in your Capture layer; the "information" derived from it sits in Work; the "knowledge" you publish sits in Output.

---

## Numbered + emoji prefix (cyberbase variant)

**Origin:** your own cyberbase convention.

**Tree:**

```
✅ TASKS                            (SYSTEM)
⬇️ Clipping                          (CAPTURE)
⬇️ INBOX, DROPZONE                   (CAPTURE)
📁 01 - Projects                     (OUTPUT, JD-flavored)
📁 02 - CyberNews                    (OUTPUT)
📁 03 - Curations, Stacks            (OUTPUT)
📁 04 - Cyber & Digital Trust        (OUTPUT)
📁 05 - Organizational Cyber         (OUTPUT)
📁 06 - Learning, Notes              (OUTPUT)
📁 07 - Cybersader Arsenal           (OUTPUT)
📁 09 - Personal                     (OUTPUT, Entity-scoped)
📁 10 - My Obsidian Stack            (SYSTEM + OUTPUT)
📁 11 - Community                    (Entity)
📁 12 - Content Creation             (WORK + OUTPUT)
📁 13 - Religion, Ontology, Philosophy
📁 14 - Journal, Diary               (CAPTURE + WORK)
📁 15 - Finance, Economy
📁 16 - Society, Culture, Politics, Government
📁 17 - Knowledge Engineering        (the meta-stuff itself)
📁 18 - Information Science, Ontology Traversal
📅 Changelog                         (OUTPUT)
🕸️ UNSTRUCTURED                      (CAPTURE + WORK)
🕸️ Daily Notes                       (CAPTURE + RELATION)
_attachments                         (SYSTEM)
_excalidraw                          (SYSTEM)
```

**Why the emojis:** ASCII/emoji codepoints control sort order. `_` (underscore) sorts first, then digits, then letters, then emojis. By prefixing with emojis, the user creates *intentional* groupings at the top and bottom of the file explorer.

**Detail page:** [`./cyberbase/folder-structure.md`](cyberbase/folder-structure.md)

---

# Library science / formal classification

The most rigorous tradition of organization. Mostly Output-layer techniques (how to make a corpus findable by a public).

## Library of Congress Classification (LCC)

**Origin:** US Library of Congress, late 1800s.

**Top-level letters (selection):**

```
A — General works                       L — Education
B — Philosophy, Psychology, Religion    M — Music
C — Auxiliary sciences of history       N — Fine arts
D — World history                       P — Language and literature
E — History of America                  Q — Science
F — Local US history                    R — Medicine
G — Geography, Anthropology             S — Agriculture
H — Social sciences                     T — Technology
J — Political science                   U — Military science
K — Law                                 V — Naval science
                                        Z — Bibliography
```

Each letter has a sub-classification (e.g. `QA` is Mathematics under Science). Specific items get a Cutter number (`QA76.73 .P98` for *Python: Programming*).

**SEACOW(r) mapping:** pure Output — designed for a public Entity browsing a physical library.

---

## Library of Congress Subject Headings (LCSH)

**Origin:** US Library of Congress controlled vocabulary for subject access (not the same as LCC, which is shelving).

**Form:** subject headings like `Computer security`, `Cryptography`, `Cyberterrorism — Prevention`. Subdivisions appear after `—` (em dash).

**SEACOW(r) mapping:** the controlled-vocabulary side of relation — explicitly named, hierarchically organized topics that any item can be tagged with.

**Where it lives in your stack:**

- Your `cybersader-vaults/_BACKUPS/awesome-cyber/📁 17 - Knowledge Engineering/Knowledge Organization.md` documents an integration approach: download the MADS/RDF JSONLD from `id.loc.gov/download/`, point the [linked-data-vocabularies plugin](https://github.com/kometenstaub/linked-data-vocabularies) at it, then `Ctrl+P > LCSH > category lookup`.

---

## Dewey Decimal Classification (DDC)

**Origin:** Melvil Dewey, 1876.

**Ten main classes:**

```
000 — General knowledge
100 — Philosophy and psychology
200 — Religion
300 — Social sciences
400 — Language
500 — Pure science
600 — Technology and applied science
700 — Arts and recreation
800 — Literature
900 — History and geography
```

Each class subdivides into 10 (e.g. `500` → `510 Mathematics`, `520 Astronomy`, etc.) and again into 10 (e.g. `510` → `516 Geometry`).

**SEACOW(r) mapping:** Output layer for public-library Entities. The decimal nesting is depth-bounded (typically 6 digits + decimal extension).

---

## Universal Decimal Classification (UDC)

**Origin:** International Federation for Information and Documentation, late 1800s — extension of DDC.

**Difference from DDC:** UDC is **faceted** — you can combine classes with auxiliary signs (`+`, `:`, `/`, `=`, `(`, `)`) to express *complex* topics. E.g. `004:621.39` means "computer science *applied to* telecommunications."

**SEACOW(r) mapping:** UDC is the closest formal classification system to SEACOW(r)'s relation layer — it explicitly supports cross-cutting combinations rather than forcing single-parent hierarchy.

**Where it lives in your stack:** referenced in cyberbase `Knowledge Organization.md`.

---

## Ranganathan's Colon Classification (PMEST)

**Origin:** S. R. Ranganathan, India, 1933 — the first faceted classification system.

**The five fundamental categories** (PMEST):

| Letter | Facet | Example |
|---|---|---|
| **P** | **P**ersonality | the entity (a thing, person, place, concept) |
| **M** | **M**atter | what it's made of |
| **E** | **E**nergy | what's done to / by it (action, activity, process) |
| **S** | **S**pace | where |
| **T** | **T**ime | when |

You combine facets with `:` (and other separators) to build a class number for *any* item.

**SEACOW(r) mapping:** PMEST overlaps with SEACOW(r) but speaks to the *content* (what's the item about?) where SEACOW(r) speaks to the *workflow position* (where does it sit in capture-work-output?). Use PMEST inside Output to classify; use SEACOW(r) outside to decide *where* the classified item lives.

**Why interesting:** PMEST is the *grandparent* of modern faceted classification (which Notion's properties, schema.org, and Wikidata all descend from).

---

## Controlled vocabulary types (8 forms)

**From your cyberbase `Knowledge Organization.md`:**

1. **Simple Term Lists** (Pick Lists) — flat enumeration.
2. **Thesauri** — terms + broader/narrower/related relations + synonyms.
3. **Subject Heading Lists** (e.g. LCSH, SLSH) — pre-coordinated headings.
4. **Authority Files** (e.g. LCNAF — Library of Congress Name Authority File) — canonical names for people, organizations, places.
5. **Taxonomies** — hierarchical classification.
6. **Alphanumeric Classification Schemes** (e.g. LCC, DDC, UDC) — coded shelf addresses.
7. **Ontologies** — formal logical schemas (RDF, OWL); supports inference.
8. **Folksonomies** — user-driven tagging; emergent rather than authored.

**SEACOW(r) mapping:** these are all **relation-layer** instruments, ordered roughly from least-structured (folksonomy) to most-structured (ontology).

---

## Folksonomy

**Origin:** community / web 2.0; tagging on Delicious, Flickr, Twitter, etc.

**Definition:** the *emergent* classification produced by users tagging things with whatever terms they want, with no controlled vocabulary or authority.

**Why it matters in PKM:** Obsidian tags are folksonomies by default. The *value* is low effort + high coverage; the *cost* is inconsistency (`#machine-learning`, `#machinelearning`, `#ml`, `#ML` will not collate).

**Tools to introduce structure to folksonomies:**

- Tag Wrangler (rename / merge tags).
- LinkedTagging — promoting tags into structured types.
- Crosswalker (your plugin) — ingesting an authoritative ontology and relating folksonomy tags to it.

---

# Domain-specific vault starters

These are *applications* of one or more frameworks above to a specific Entity.

## obsidian-secops-vault-template (cybersader)

**URL:** [github.com/cybersader/obsidian-secops-vault-template](https://github.com/cybersader/obsidian-secops-vault-template)

**Tree (verbatim, condensed):**

```
00 - Tasks, Planning/
  ├── ALL TASKS
  ├── Planning Sources
  ├── TRACKER (USER_1)
  ├── TRACKER (USER_2)
  └── Wishlist, Budget
01 - Projects, Workspaces/
02 - Areas, Objectives, Initiatives, Ongoing/
03 - Docs, Internal Info, SOPs, Resources/
04 - Topics, Knowledge, External/
05 - Archive, Admin/
06 - Ideation, Sandbox/
07 - Vault Config & Management/
08 - Frameworks/
   ├── Cyber Intel, Risk Intel/
   └── Frameworks, Ontologies, Mappings/
99 - ARCHIVE/
Framework Mapping/
   ├── Frameworker_Example/
   └── Links to Frameworks/
SYSTEM - SCRIPTS, QUERIES/
   ├── Templates/
   └── Templates_Pandoc/
Tag Usage Examples/
Testing/
User DB/
_STARTER_GUIDE/  (15+ sections)
⬇️ or 📥 DROPZONE, Inbox/
⭐ VAULT GUIDE, README (example)/
🔎 Index, Navigator, Map, MOCs, Atlas/
```

**Frameworks composed:** Johnny Decimal-flavored numbering + PARAUT (00 inbox + 99 archive + 08 frameworks) + cybersecurity domain customization.

**Frontmatter convention:**

```yaml
---
type: [note_type]
status: [draft | published | archived]
tags: [tag_namespace/subtag]
created: YYYY-MM-DD
updated: YYYY-MM-DD
---
```

**Notable extensions:** `08 - Frameworks/` for compliance crosswalking; multi-user `TRACKER (USER_1/2)`; emoji-prefixed indexes (⬇️, ⭐, 🔎).

---

## cyberbase (cybersader)

**URL:** [github.com/cybersader/cyberbase](https://github.com/cybersader/cyberbase)

See the [Numbered + emoji prefix](#numbered--emoji-prefix-cyberbase-variant) section above for the tree. This is the canonical SEACOW(r) instantiation.

---

## Ideaverse Lite 1.5 (LYT)

See the [LYT section](#linking-your-thinking-lyt--ideaverse--maps-of-content) above.

---

## Weave (corporate, cuken)

**URL:** [github.com/cuken/obsidian-weave](https://github.com/cuken/obsidian-weave)

**Tree (verbatim from `cybersader-vault-starters/starters (not mine)/Weave_clean/`):**

```
Weave/
├── Applications/    # apps you use, accounts, integrations
├── Contacts/        # CRM-lite — people you work with
├── Daily/           # daily journal entries
├── Meetings/        # meeting logs
└── System/
    ├── Media/
    └── Templates/
```

**Plugin stack:** Buttons, Calendar, Dataview, NLDates, Checklist, Excalidraw, Icon Folder, Outliner, Tasks, Text Expander JS, QuickAdd, Table Editor, Templater.

**SEACOW(r) mapping:**

| SEACOW(r) | Weave expression |
|---|---|
| System | Obsidian + extensive plugin stack |
| Entity | Corporate / synchronous-team setting |
| Capture | `Daily/` (daily journal) + meeting captures |
| Work | `Applications/` + `Meetings/` cross-linked via Dataview |
| Output | not explicit — Weave is mostly Capture+Work, output happens elsewhere |
| relation | Dataview-backed cross-references between Daily / Meetings / Applications / Contacts |

**Why interesting:** the *flattest* serious starter — only 4 top-level content folders. Optimized for high-frequency capture (daily standup culture).

---

## The Good Parts v2 (FLAP)

See the [FLAP section](#atomic-notes--flap-fleeting--literature--atomic--project) above.

---

## Other starters in your collection

Quick listing of additional starters present at `cybersader-vault-starters/starters/` and `starters (not mine)/`:

| Starter | Status | Framework family |
|---|---|---|
| `obsidian-cyberbase-template` | active | Numbered + JD-flavored, FileOrganizer2000-augmented |
| `obsidian-grc-vault-template` | draft | (planned) GRC application of SecOps pattern |
| `obsidian-devops-vault-template` | draft | (planned) DevOps application |
| `obsidian-advanced-linking-vault-template` | active | SecOps-pattern + advanced linking |
| `obsidian-cyber-frameworks-vault-template` | draft | Pre-built compliance frameworks (CIS, NIST, MITRE) — pairs with Crosswalker |
| `obsidian-community-vault-template` | draft | Community-vault pattern |
| `couple-vault-template` | draft | Personal — two-Entity household |
| `obsidian-catechesis-vault-template` | draft | Religious education |
| `Obsidian Starter Vault Free` | reference | Generic minimal |
| `Obsidian-Templates-10.1.0` | reference | Template collection |
| `obsidian-hub-main` | reference | Community hub |

---

# Cybersecurity compliance frameworks (specialized)

These are domain-specific to your cybersecurity work but represent some of
the most rigorous *real-world* hierarchical taxonomies. They illustrate how
SEACOW(r) accommodates compliance / GRC use-cases.

## NIST Cybersecurity Framework 2.0 (CSF 2.0)

**Origin:** NIST, 2024 update. [csrc.nist.gov/projects/cybersecurity-framework](https://csrc.nist.gov/projects/cybersecurity-framework).

**Six functions** (a.k.a. the top-level taxonomy):

```
GV — Govern    (new in 2.0)
ID — Identify
PR — Protect
DE — Detect
RS — Respond
RC — Recover
```

Each function has **categories** (e.g. `ID.AM` Asset Management) and **subcategories** (e.g. `ID.AM-01` Inventories of physical devices...).

**Concrete mapping example (from your `Home_IT_cyber_taxonomy.md`):**

| Domain | Quick Wins | CSF 2.0 alignment |
|---|---|---|
| Govern & Inventory | Family rules, asset list, data classification | Govern |
| Identity & Access | MFA, password manager | Identify |
| Devices & OS | Auto-updates, encryption | Protect |
| Network & Edge | WPA3, guest SSID | Protect |
| Monitoring & Logging | Router/NAS telemetry | Detect |
| Incident Response | Playbooks (lost phone, takeover) | Respond/Recover |

**SEACOW(r) mapping:** CSF 2.0 is a pure relation/taxonomy used to *categorize* security activities. The functions ID/PR/DE/RS/RC act as a controlled vocabulary applied to your security Output (policies, runbooks, SOPs).

---

## NIST SP 800-53 control families

**Origin:** NIST Special Publication 800-53, Revision 5 (Update 1).

**Control families (selection):**

```
AC — Access Control          PE — Physical and Environmental Protection
AT — Awareness and Training  PL — Planning
AU — Audit and Accountability PM — Program Management
CA — Assessment, Authorization, and Monitoring
                              PS — Personnel Security
CM — Configuration Management PT — PII Processing and Transparency
CP — Contingency Planning    RA — Risk Assessment
IA — Identification and Authentication
                              SA — System and Services Acquisition
IR — Incident Response       SC — System and Communications Protection
MA — Maintenance             SI — System and Information Integrity
MP — Media Protection        SR — Supply Chain Risk Management
```

Controls are addressed as `AC-1`, `AC-2`, etc., with control enhancements like `AC-2(1)`.

**SEACOW(r) mapping:** another taxonomy applied to Output (the controls themselves are documented artifacts). Crosswalks to CSF 2.0 (next section) link tactical control to strategic outcome.

---

## CIS Controls (IG1 / IG2 / IG3)

**Origin:** Center for Internet Security.

**Tiered maturity:**

| Tier | Audience |
|---|---|
| **IG1** — Implementation Group 1 | Small businesses, basic hygiene |
| **IG2** — Implementation Group 2 | Mid-size organizations, hardening |
| **IG3** — Implementation Group 3 | Large enterprises, advanced |

**18 CIS Controls** (as of v8): Inventory of Hardware, Inventory of Software, Data Protection, Secure Configuration, Account Management, Access Control Management, Continuous Vulnerability Management, Audit Log Management, Email and Web Browser Protections, Malware Defenses, Data Recovery, Network Infrastructure Management, Network Monitoring and Defense, Security Awareness, Service Provider Management, Application Software Security, Incident Response Management, Penetration Testing.

**SEACOW(r) mapping:** like CSF 2.0, a relation-layer taxonomy. The IG-tier system is interesting — it adds an *Entity-aware* dimension (different recommendations for different organization sizes).

---

## MITRE ATT&CK / D3FEND / Engage

**Origin:** MITRE Corporation. [attack.mitre.org](https://attack.mitre.org/) · [d3fend.mitre.org](https://d3fend.mitre.org/) · [engage.mitre.org](https://engage.mitre.org/)

**ATT&CK structure:**

```
Tactics       — high-level adversary objectives (Initial Access, Execution, Persistence, …)
  Techniques  — how the tactic is achieved (Spearphishing Attachment, Command and Scripting Interpreter, …)
    Sub-techniques — specific variants
Procedures   — observed real-world implementations
```

**Three flavors:**

| Framework | Direction | Purpose |
|---|---|---|
| **ATT&CK** | adversary | catalog of attacker tactics, techniques, procedures |
| **D3FEND** | defender | counter-measures, ontology of defensive techniques |
| **Engage** | engagement | deception, disruption, response engagements |

**SEACOW(r) mapping:** all three are relation-layer ontologies. ATT&CK is one of the most-crosswalked frameworks in cybersecurity — your `Crosswalker` plugin ingests these.

---

## Cyber Kill Chain

**Origin:** Lockheed Martin.

**Seven phases:**

```
1. Reconnaissance     (gather intel)
2. Weaponization      (build the malicious payload)
3. Delivery           (deliver via email, web, USB)
4. Exploitation       (execute in target)
5. Installation       (establish persistence)
6. Command & Control  (remote access)
7. Actions on Objectives (the actual bad thing)
```

**SEACOW(r) mapping:** a process / Activities-style framework — like ARC or CODE but for adversary lifecycle.

---

## Diamond Model

**Origin:** Center for Cyber Threat Intelligence.

**Four vertices:**

```
        Adversary
           |
Capability — Victim
           |
       Infrastructure
```

Each adversary intrusion is described as a quadruple of (Adversary, Capability, Infrastructure, Victim).

**SEACOW(r) mapping:** a relation-layer model for *describing* threat intelligence. Useful for SecOps Output (incident reports, threat profiles).

---

## Crosswalking — CSF 2.0 → 800-53 → CRI

**Source:** your `cybersader-vaults/_BACKUPS/awesome-cyber/📁 05 - Organizational Cyber/Frameworks, Standards/Framework Mapping.md`.

**Pattern:** map CSF 2.0 outcomes → 800-53 control families → CRI (Cyber Risk Institute) Community Profile risk scenarios.

**Toolchain:**

```
CSF 2.0 Core JSON
   ↓ (download from csrc.nist.gov/extensions/nudp/services/json/csf/download)
LibreBase / spreadsheet
   ↓
800-53 control mapping
   ↓
CRI Community Profile v2.0 Structure sheet
   ↓
RCSA process templates
```

**SEACOW(r) mapping:** crosswalking *is* the relation layer made explicit — formal mappings between competing taxonomies. This is what your [Crosswalker plugin](https://github.com/cybersader/Crosswalker) automates inside Obsidian.

**External resources:**

- [center-for-threat-informed-defense.github.io/mappings-explorer/](https://center-for-threat-informed-defense.github.io/mappings-explorer/)
- [github.com/center-for-threat-informed-defense/attack-control-framework-mappings](https://github.com/center-for-threat-informed-defense/attack-control-framework-mappings)

---

# Other frameworks (concise)

## D.E.E.Z.N.U.T.S.

**Origin:** Reddit (r/ObsidianMD), [thread](https://www.reddit.com/r/ObsidianMD/comments/1j66utn/introducing_deeznuts_not_a_meme/).

**Tree:**

```
D — Dashboards          (Maps of Content, navigation hubs)
E — Efforts             (active work)
E — Extras              (Templates, Archive)
Z — Zettelkasten        (atomic ideas)
N — Network & People    (notes on real people, social connections)
U — Unsorted/Unfinished (inbox)
T — Thoughts & Journal  (personal reflections, daily logs)
S — Sources             (raw materials: books, PDFs, articles, videos)
```

**SEACOW(r) mapping:**

| SEACOW(r) | DEEZ expression |
|---|---|
| Capture | U (Unsorted), T (Journal), S (Sources) |
| Work | E (Efforts), Z (Zettelkasten) |
| Output | D (Dashboards) |
| Entity | N (Network & People) — explicit Entity layer |
| relation | D (Dashboards) + Z (Zettelkasten) |

**Why interesting:** explicitly carves out an Entity layer (`N — Network & People`).

---

## EJK (Efforts, Journal, Knowledge)

**Origin:** community variant referenced in your `Vault Folder & Tag Structure.md`.

**Tree:**

```
Efforts/    — action-bound work (PARA's Projects+Areas)
Journal/    — time-based (PARA has no equivalent)
Time/       — explicit temporal organization
Knowledge/  — synthesis, evergreen (PARA's Resources+Archive merged)
```

**SEACOW(r) mapping:** simpler than PARA — collapses to three buckets that map cleanly to Work / Capture-time / Output.

---

# See also

- [`../INDEXES/by-comparison.md`](../INDEXES/by-comparison.md) — compact one-row-per-framework matrix.
- [`../04-comparisons/`](../04-comparisons/) — per-framework deep-dive pages.
- [`../05-deep-dives/knowledge-organization.md`](../05-deep-dives/knowledge-organization.md) — broader landscape with external links.
- [`../05-deep-dives/ideas-for-knowledge-organization.md`](../05-deep-dives/ideas-for-knowledge-organization.md) — your own brainstorm with e-ACCESS, EJK, time-based structures.
- [`../ROADMAP.md`](../ROADMAP.md) — frameworks not yet covered (GTD, Eisenhower Matrix, Bullet Journal, Forte's PARA-CODE in depth, Roam-style daily notes flow, IBIS, Kanban, OKRs, KonMari, schema.org, Dublin Core, FOAF, IDEF, Bates numbering, more).
