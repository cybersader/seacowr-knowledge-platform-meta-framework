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
- [Cybersecurity compliance frameworks](#cybersecurity-compliance-frameworks)
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
- [Productivity & lifecycle frameworks](#productivity--lifecycle-frameworks)
  - GTD · GTD Horizons · Bullet Journal · OKRs · Eisenhower · Cynefin · IBIS · Pomodoro · KonMari · PDCA · OODA · Six Sigma DMAIC · AAR · 5 Whys / Ishikawa / 5W1H · Business Model Canvas
- [More PKM frameworks](#more-pkm-frameworks)
  - Forte CODE · Forte Intermediate Packets · Forte PARA-in-Real-Life · Ahrens Smart Notes · Matuschak evergreen-notes · Luhmann Folgezettel · Roam daily-notes flow · Appleton Stream/Garden/Campfire · Commonplace book
- [More library science / metadata standards](#more-library-science--metadata-standards)
  - Dublin Core · schema.org · FOAF · SKOS · MARC 21 · MeSH · AAT · EAD · ISO 25964 · Bates · IDEF0 · IDEF1X · OAIS · OAI-PMH · CIDOC-CRM · BIBFRAME · METS · Wikidata · ISO/IEC 11179 · PREMIS
- [Enterprise architecture & strategy](#enterprise-architecture--strategy)
  - DAMA-DMBOK · TOGAF ADM · ArchiMate · Zachman · C4 Model · arc42 · 4+1 · Garrett UX · Norman design · Wardley Mapping
- [IT governance / GRC](#it-governance--grc)
  - ITIL 4 · COBIT 2019 · IIA Three Lines · ISO 27001/27002 · NIST RMF · NIST Privacy · FAIR · SABSA · OWASP ASVS · OWASP Top 10 · CSA CCM · PCI DSS · HIPAA Security Rule
- [Project & delivery management](#project--delivery-management)
  - PRINCE2 · PMBOK 7 · SAFe · GitHub Flow / GitFlow / Trunk-Based · Twelve-Factor App
- [Threat modeling](#threat-modeling)
  - STRIDE · PASTA · ICS Cyber Kill Chain
- [Educational / cognitive taxonomies](#educational--cognitive-taxonomies)
  - Bloom (revised) · Webb DOK · SOLO · Costa · Marzano
- [Academic discipline classifications](#academic-discipline-classifications)
  - ACM CCS · AMS MSC2020 · JEL · PACS · arXiv · PhilPapers
- [Narrative / creative structures](#narrative--creative-structures)
  - Hero's Journey · Three-Act · Save the Cat · Pixar 22 Rules · Story Circle · Freytag · Polti 36
- [Business process notation](#business-process-notation)
  - BPMN 2.0 · RACI · Value Stream Map
- [Philosophical / classical taxonomies](#philosophical--classical-taxonomies)
  - Aristotelian Categories · Porphyrian Tree · Kant · Five Aggregates · Confucian Five

> **~110+ frameworks total.** Each entry has a concrete structural backbone and a SEACOW(r) mapping. Use Ctrl-F (or your editor's outline pane) to jump to a framework.

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
- Numbered-PARA variants common in compliance / corporate vaults use `01 - Projects, Workspaces/` + `02 - Areas, Objectives, Initiatives, Ongoing/` + `05 - Archive, Admin/` style numbering.

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

**Visual:**

```
                  ┌─────────────────────┐
                  │   BASB = PARA + CODE │
                  └──────────┬──────────┘
                             │
            ┌────────────────┴────────────────┐
            │                                 │
       PARA (storage)                   CODE (verbs)
            │                                 │
   ┌────┬───┴───┬────┐               ┌────┬───┴───┬────┐
   P    A      R    A                C    O      D    E
Projects Areas Resources Archive    Capture Org. Distill Express
```

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

**Visual** (deliberately graph, not tree):

```
            ┌─[atomic note]
            │       ↕                  no folders.
   [atomic note]──[atomic note]        the link graph
        ↕            ↕                  *is* the structure.
  [atomic note]──[atomic note]──[atomic note]
        ↕            ↕            ↕
   [atomic note]──[atomic note]
            ↕
        [atomic note]
```

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

**Visual:**

```
   raw input        ━━ Add ━━━━━━━▶  [your vault]
                                          │
                          ━━ Relate ━━━━━━┤  (links, MOCs, tags)
                                          │
   audience  ◀━━ Communicate ━━━━━━━━━━━━━┘
```

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

**Visual:**

```
                    ╔═══════════════╗
                    ║      STIR      ║
                    ╚═══════╤═══════╝
                            │
        ┌───────────┬───────┴────────┬───────────┐
        │           │                │           │
       (S)         (T)              (I)         (R)
       Space       Time            Importance   Relatedness
        │           │                │           │
       Atlas    Calendar          Efforts     (the links you draw)
       (in ACE)  (in ACE)         (in ACE)    (between A/C/E)
```

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

**Visual** (acronym evolution):

```
         COW                              ─── 3 verbs (Capture, Output, Work)
          │
          ▼
        COWS                              ─── + System
          │
          ▼
       WORCS                              ─── + Relation, reordered
          │  "cause it just works"
          ▼
      WO(R)C(S)                           ─── parens for optional pieces
          │
          ▼
      SEA(COWr)         ◀── current       ─── + Entity (audience)
          │                                    + Activities umbrella
          │                                    lower-case r (debatable)
   System / Entity / Activities (Capture, Output, Work, relation)
```

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

**Visual:**

```
   ┌───────────┐    ┌───────────┐    ┌───────────┐
   │  CAPTURE  │ ──▶│   WORK    │ ──▶│  OUTPUT   │
   │  (inputs) │    │ (function)│    │ (outputs) │
   └───────────┘    └───────────┘    └───────────┘
                          ↑
                    + SYSTEM (platform)
                    + ENTITY (audience)
                    + relation (graph layer)
                    = SEACOW(r)
```

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

**Detail page:** [`../04-comparisons/vs-johnny-decimal.md`](../04-comparisons/vs-johnny-decimal.md)

---

## LATCH (Wurman)

**Origin:** Richard Saul Wurman, *Information Anxiety* — five fundamental ways to organize information.

**Visual:**

```
                  Same content,
                   five rotations:

   By LOCATION    [North] [South] [East] [West]
   By ALPHABET    [A]  [B]  [C]  [D]  [E]  ...
   By TIME        2020 → 2021 → 2022 → 2023 → 2024
   By CATEGORY    [Books] [Videos] [Articles] [Podcasts]
   By HIERARCHY   ╔═══╗→╔═══╗→╔═══╗→╔═══╗   (rank/magnitude)
                  ║ 5 ║  ║ 4 ║  ║ 3 ║  ║ 2 ║
                  ╚═══╝  ╚═══╝  ╚═══╝  ╚═══╝
```

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

**Visual** (heading hierarchy + subdivisions):

```
Computer security
├── Computer security — Government policy
├── Computer security — Law and legislation
├── Computer security — Standards
│   └── Computer security — Standards — United States
└── Computer security — Vocational guidance

Cryptography
├── Cryptography — Bibliography
├── Cryptography — Data processing
├── Cryptography — Mathematical models
└── Public key cryptography

Cyberterrorism
├── Cyberterrorism — Prevention
└── Cyberterrorism — United States — Prevention
```

**SEACOW(r) mapping:** the controlled-vocabulary side of relation — explicitly named, hierarchically organized topics that any item can be tagged with.

**Where it lives in your stack:**

- LCSH is loadable into Obsidian via the [linked-data-vocabularies plugin](https://github.com/kometenstaub/linked-data-vocabularies): download the MADS/RDF JSONLD from `id.loc.gov/download/`, point the plugin at it, then `Ctrl+P > LCSH > category lookup`.

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

**Visual** (auxiliary signs + a worked example):

```
   Top classes:    0  Generalities, computer science
                   1  Philosophy, psychology
                   2  Religion, theology
                   3  Social sciences
                   5  Mathematics, natural sciences
                   6  Applied sciences, technology, medicine
                   7  Arts, recreation, sports
                   8  Linguistics, literature
                   9  Geography, biography, history

   Auxiliary signs (the faceted-classification magic):
       +   coordination ("and"):     59 + 636        — zoology AND animal husbandry
       /   consecutive extension:    592/599         — invertebrate to vertebrate zoology
       :   relation:                 02:34           — librarianship related to law
       []  subgrouping:              02:[34+33]      — librarianship related to law and economics
       =   language:                 ...=111         — in English
       (0...) form:                  ...(02)         — handbook form
       (1/9) place:                  ...(44)         — France
       "..." time:                   ..."20"         — 21st century

   Worked example:
       004 : 621.39 = 111 (44) "20"
        │     │       │   │     │
        │     │       │   │     └── 21st century
        │     │       │   └────── France
        │     │       └────── in English
        │     └────────────── telecommunications
        └────────────────── computer science
       "Computer-science-applied-to-telecommunications, in English, France, 21st century"
```

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

**Visual** (compose any subject from PMEST facets):

```
   Subject heading = MAIN_CLASS [, P] [; M] [: E] [. S] [' T]
                                  │     │     │     │     │
                                  P     M     E     S     T

   Worked example: "X-ray therapy of tuberculosis of lungs, in India, 1950"
       L   ,   45     ;   421       :   6        .   44     '   N5
       │       │          │             │            │          │
   Medicine  Lungs    Tuberculosis   Therapy       India        1950
   (main)    (P)      (M — disease)  (E — by-X-ray)(S — place)   (T — date)

   Reads left-to-right as the work's "shelf address":
   ┌───────────────────────────────────────────────────────────────────┐
   │  Medicine ▶ Lungs ▶ TB ▶ X-ray therapy ▶ India ▶ 1950             │
   └───────────────────────────────────────────────────────────────────┘
```

**SEACOW(r) mapping:** PMEST overlaps with SEACOW(r) but speaks to the *content* (what's the item about?) where SEACOW(r) speaks to the *workflow position* (where does it sit in capture-work-output?). Use PMEST inside Output to classify; use SEACOW(r) outside to decide *where* the classified item lives.

**Why interesting:** PMEST is the *grandparent* of modern faceted classification (which Notion's properties, schema.org, and Wikidata all descend from).

---

## Controlled vocabulary types (8 forms)

**Eight forms** (per the standard library-science taxonomy of vocabulary types):

**Visual** (least → most structured):

```
   FLAT ◀──────────────────────── STRUCTURE LADDER ────────────────────▶ FORMAL

   Folksonomy   →  Pick List  →  Authority File  →  Subject Headings  →  Taxonomy  →  Thesaurus  →  Classification Scheme  →  Ontology
   ─────────       ─────────     ──────────────     ────────────────     ────────     ─────────     ────────────────────     ────────
   user-driven    flat enum     canonical names    pre-coordinated      tree         + synonyms     coded addresses          formal logic
   emergent       no rels       (people, places)   ("Computer security  hierarchy    + broader/     (LCC, DDC, UDC)          (RDF, OWL)
                                                    — Standards")       only         narrower/                                inference!
                                                                                     related
   #obsidian      [draft|        John Smith        Computer security    Security     synonym:       QA76.73                   :Person rdf:type
   #ml            published]      → "Smith, John   Cryptography           ├─ AppSec  "Cybersec"     QA76.9                       owl:Class
                                     1965-"        Cyberterrorism         └─ NetSec   broader:                                 :knows owl:domain
                                                                                     "InfoSec"                                   :Person
```

The 8 forms in detail:

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

**Visual** (the cost of emergence):

```
   What users actually type:
   ┌──────────────────────────────────────────┐
   │ #ml          #ML            #m.l.        │
   │ #machinelearning            #MachineLearning
   │ #machine-learning           #machine_learning
   │ #ai/ml       #ai_ml         #aiml        │
   │ #deeplearning                #deep-learning
   │ #DL          #neuralnets    #nn          │
   └──────────────────────────────────────────┘
                      │
                      ▼  (tag-cleanup pass)
                      │
   Crosswalker / Tag Wrangler / SKOS-mapping
                      │
                      ▼
   Canonical:  #machine-learning
   Aliases:    #ml, #machinelearning, #machine_learning
   Children:   #machine-learning/deep-learning
               #machine-learning/neural-networks
```

**Why it matters in PKM:** Obsidian tags are folksonomies by default. The *value* is low effort + high coverage; the *cost* is inconsistency (`#machine-learning`, `#machinelearning`, `#ml`, `#ML` will not collate).

**Tools to introduce structure to folksonomies:**

- Tag Wrangler (rename / merge tags).
- LinkedTagging — promoting tags into structured types.
- Crosswalker — a plugin that ingests an authoritative ontology and relates folksonomy tags to it.

---

# Cybersecurity compliance frameworks

A worked example of how SEACOW(r) handles a domain with **rigorous,
real-world hierarchical taxonomies and crosswalks**. The cybersec compliance
ecosystem is one of the densest crosswalking environments in modern
information work — useful as a reference even outside the security domain,
because it shows how multiple competing taxonomies (CSF 2.0 / 800-53 / CIS /
ATT&CK / ISO / etc.) coexist via explicit relation-layer mappings.

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

**SEACOW(r) mapping:** CSF 2.0 is a pure relation/taxonomy used to *categorize* security activities. The functions GV/ID/PR/DE/RS/RC act as a controlled vocabulary applied to security Output (policies, runbooks, SOPs).

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

**Visual** (controls × IG-tier):

```
                                                    IG1   IG2   IG3
   01  Inventory of Enterprise Assets                ●     ●     ●
   02  Inventory of Software Assets                  ●     ●     ●
   03  Data Protection                               ●     ●     ●
   04  Secure Configuration                          ●     ●     ●
   05  Account Management                            ●     ●     ●
   06  Access Control Management                     ●     ●     ●
   07  Continuous Vulnerability Management           ●     ●     ●
   08  Audit Log Management                          ●     ●     ●
   09  Email and Web Browser Protections             ●     ●     ●
   10  Malware Defenses                              ●     ●     ●
   11  Data Recovery                                 ●     ●     ●
   12  Network Infrastructure Management             ─     ●     ●
   13  Network Monitoring and Defense                ─     ●     ●
   14  Security Awareness and Skills Training        ●     ●     ●
   15  Service Provider Management                   ─     ●     ●
   16  Application Software Security                 ─     ●     ●
   17  Incident Response Management                  ●     ●     ●
   18  Penetration Testing                           ─     ─     ●

   Each control has Safeguards (sub-controls);
   ~56 safeguards in IG1, ~130 in IG2, ~153 in IG3.
```

**Tiered maturity:**

| Tier | Audience |
|---|---|
| **IG1** — Implementation Group 1 | Small businesses, basic hygiene |
| **IG2** — Implementation Group 2 | Mid-size organizations, hardening |
| **IG3** — Implementation Group 3 | Large enterprises, advanced |

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

**SEACOW(r) mapping:** all three are relation-layer ontologies. ATT&CK is one of the most-crosswalked frameworks in cybersecurity — the [Crosswalker plugin](https://github.com/cybersader/Crosswalker) ingests these into Obsidian vaults.

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

**SEACOW(r) mapping:** a relation-layer model for *describing* threat intelligence — incident reports, threat profiles.

---

## Crosswalking — CSF 2.0 → 800-53 → CRI

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

**SEACOW(r) mapping:** crosswalking *is* the relation layer made explicit — formal mappings between competing taxonomies. The [Crosswalker plugin](https://github.com/cybersader/Crosswalker) automates this inside Obsidian.

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

# Productivity & lifecycle frameworks

These aren't folder schemes (mostly) — they're rhythms, triage filters, and lifecycle loops that overlay any folder scheme. They tend to map to SEACOW(r)'s **Activities** row.

## GTD — Getting Things Done (David Allen, 2001)

**Source:** [gettingthingsdone.com/five-steps/](https://gettingthingsdone.com/five-steps/) · book *Getting Things Done* (2001).

**Five steps:**

```
CAPTURE — Collect what has your attention
CLARIFY — Process what it means
ORGANIZE — Put it where it belongs
REFLECT — Review frequently
ENGAGE — Simply do
```

**Canonical lists:** Inbox / Next Actions / Waiting For / Someday-Maybe / Calendar / Reference / Trash.

**Contexts** (relation tags on actions): `@home`, `@office`, `@calls`, `@errands`, `@computer`, `@agenda`.

**SEACOW(r) mapping:** verb-driven Capture→Work pipeline; lists are Containers, contexts are Relations on actions. Pairs naturally with PARA (PARA = where, GTD = how).

**Notable variants:** "Weekly Review" cadence; "two-minute rule" (if it takes <2 min, do it now); often paired with Eisenhower for prioritization inside Next Actions.

---

## GTD Horizons of Focus (David Allen)

**Source:** [gettingthingsdone.com — 6 Horizons of Focus](https://gettingthingsdone.com/2011/01/the-6-horizons-of-focus/).

**Six altitudes:**

```
Ground (Calendar / Actions)            "actions and information you currently have to do"
Horizon 1 — 10,000 ft  Projects        commitments to finish (more than one action step)
Horizon 2 — 20,000 ft  Areas of Focus  4-7 major areas of responsibility
Horizon 3 — 30,000 ft  1-2 yr Goals
Horizon 4 — 40,000 ft  3-5 yr Vision
Horizon 5 — 50,000 ft  Purpose & Principles    "why are you here?"
```

**SEACOW(r) mapping:** vertical System scaffold — altitude = abstraction layer over Work and Entities (goals, areas).

**Notable for:** Maps cleanly onto PARA's Project/Area distinction at H1/H2; gives you a "zoom level" vocabulary for life-design conversations.

---

## Bullet Journal (Ryder Carroll, 2013)

**Source:** [bulletjournal.com](https://bulletjournal.com).

**Modules:** **Index** / **Future Log** / **Monthly Log** / **Daily Log** / **Collections**.

**Rapid Logging signifiers:**

```
•  Task           ○  Event           —  Note
✗  Task complete  >  Migrated         <  Scheduled
*  Priority       !  Inspiration      👁  Eye on it
```

**SEACOW(r) mapping:** Capture-first analog system; **Index** = Entity registry; signifiers = micro-typology of work items; **Migration** ritual replaces software's automatic carry-forward.

**Notable for:** Famously analog-first, but ports to digital (e.g. Notion / Obsidian Daily Notes plugin).

---

## OKRs — Objectives & Key Results (Andy Grove → John Doerr, ~1970s/2000s)

**Source:** [rework.withgoogle.com](https://rework.withgoogle.com/) · *Measure What Matters* (Doerr, 2017).

**Structure:**

```
OBJECTIVE   = a significant, concrete, clearly-defined goal (qualitative)
KEY RESULTS = 3-5 measurable outcomes per objective
              measured 0.0 - 1.0; target ≈ 0.7 (stretch)
CASCADE:     org-level → team-level → (sometimes) individual
CADENCE:     usually quarterly, with weekly check-ins
```

**SEACOW(r) mapping:** Output measurement layer — Objective is intent (System-aligned), Key Results are countable Outputs.

**Notable variants:** "Committed" vs "Aspirational" OKRs (Google); the "0.7 is success, 1.0 means you didn't stretch" calibration norm.

---

## Eisenhower Matrix

**Source:** popularized in Stephen Covey's *7 Habits*; attributed to Dwight D. Eisenhower.

**2×2 (Urgent × Important):**

```
                Urgent              Not urgent
Important     | DO              | SCHEDULE / DECIDE  |
              | (do now)        | (plan it in)       |
              |-----------------|--------------------|
Not important | DELEGATE        | DELETE             |
              | (someone else)  | (drop it)          |
```

**SEACOW(r) mapping:** triage filter — assigns Work-item Relations (urgency × importance) to one of four verbs.

**Notable for:** Covey's "Quadrant II" reframe argues most value lives in Important+Not-urgent; commonly layered onto GTD Next Actions.

---

## Cynefin Framework (Dave Snowden, 1999; "Clear" rename 2014)

**Source:** [thecynefin.co](https://thecynefin.co).

**Five domains:**

```
Clear (formerly "Obvious"):  sense - categorize - respond  (best practice)
Complicated:                 sense - analyze    - respond  (good practice)
Complex:                     probe - sense      - respond  (emergent practice)
Chaotic:                     act   - sense      - respond  (novel practice)
Confusion / Disorder:        central — unclear which applies
```

**SEACOW(r) mapping:** sense-making typology over Systems — picks the action verb (categorize / analyze / probe / act) based on the *kind of problem* you have.

**Notable for:** the right framework for *choosing* a framework. Use Cynefin to decide whether your situation needs PARA-style categories or Zettelkasten-style emergence.

---

## IBIS — Issue-Based Information System (Kunz & Rittel, 1970)

**Source:** [en.wikipedia.org/wiki/Issue-based_information_system](https://en.wikipedia.org/wiki/Issue-based_information_system).

**Three-node graph:**

```
Issue (?)         — questions requiring answers
  ↓
Position (!)       — proposed solutions / ideas
  ↓
Argument (+/−)    — pros and cons attached to positions
  ↓
(sub-issues branch from any node — "directed edges, forming a graph")
```

**SEACOW(r) mapping:** typed-edge relation graph over deliberation Entities — pure argumentation schema.

**Notable variants:** Dialogue Mapping (Jeff Conklin); the Compendium tool; gIBIS / D-Agree.

---

## Pomodoro Technique (Francesco Cirillo, late 1980s)

**Source:** [francescocirillo.com](https://francescocirillo.com/pages/pomodoro-technique).

**Loop:**

```
1. Decide on task
2. Set timer for 25 min ("a Pomodoro")
3. Work until timer rings
4. Short break (5 min)
5. After 4 Pomodori, long break (20-30 min)
```

**SEACOW(r) mapping:** Work-time temporal Container; 25/5/4×/long-break is the only structure.

**Notable for:** scope discipline — forces a "what am I going to do in the next 25 min?" articulation.

---

## KonMari Method (Marie Kondo)

**Source:** *The Life-Changing Magic of Tidying Up* (2011).

**Order (deliberate easiest → hardest):**

```
1. Clothes
2. Books
3. Papers
4. Komono (miscellaneous)
5. Sentimental items
```

**Rule:** keep only items that "spark joy" (*tokimeku*); sort *by category, not by location*.

**SEACOW(r) mapping:** Entity-by-category sweep with a binary keep/discard verb (joy-test); the joy-test is a *rule* applied during the cooled-Output review pass.

**Notable for:** anti-categorization in placement (don't have a "books shelf" alongside "papers desk" — gather all books in one pile first).

---

## PDCA / Deming Cycle (Walter Shewhart → W. Edwards Deming)

**Source:** Shewhart 1939, popularized by Deming.

**Loop:**

```
PLAN  → DO  → CHECK  → ACT  → (repeat)
                            (a.k.a. PDSA: Plan / Do / Study / Act)
```

**SEACOW(r) mapping:** Activities loop — applied to any improvement initiative, business process, or scientific experiment.

**Notable for:** the canonical continuous-improvement cycle; underneath ITIL, Six Sigma, and most process-improvement frameworks.

---

## OODA Loop (John Boyd, US Air Force)

**Source:** Boyd's *Discourse on Winning and Losing* briefings.

**Four-phase loop:**

```
OBSERVE  → ORIENT  → DECIDE  → ACT  → (repeat)
              ↑                           |
              ←————— feedback —————————————
```

**SEACOW(r) mapping:** Activities (decision-cycle); Boyd argued **Orient** is the dominant phase — your mental model determines what you can perceive and what options you'll consider.

**Notable for:** military decision-making; widely borrowed in cybersecurity (incident response) and competitive strategy.

---

## Six Sigma DMAIC

**Source:** Motorola → GE — popularized 1980s/90s.

**Phases:**

```
DEFINE   → MEASURE   → ANALYZE   → IMPROVE   → CONTROL
```

**SEACOW(r) mapping:** Activities — improvement-cycle phases for process-defect reduction.

**Notable for:** the rigor expectation: Define has a SIPOC; Measure has Cp/Cpk capability indices; Analyze has Pareto / Ishikawa / hypothesis tests; Improve has DOE; Control has SPC.

---

## AAR — After-Action Review (US Army)

**Source:** US Army TC 25-20.

**Four questions** (sometimes six):

```
1. What was supposed to happen?
2. What actually happened?
3. What went well? (and why)
4. What can be improved? (and how)
   (5. What did we learn?)
   (6. What will we do differently next time?)
```

**SEACOW(r) mapping:** Activities — retrospective phases applied to any completed effort.

**Notable for:** psychological-safety construct — "no rank in the AAR." The closest formal cousin to Agile retrospectives.

---

## 5 Whys / Ishikawa Fishbone / 5W1H

**Origin:** Toyota Production System (5 Whys / Sakichi Toyoda); Kaoru Ishikawa (Fishbone, 1968); journalism (5W1H).

**Visual — 5 Whys:**

```
   Symptom:    "Customer's order shipped late."
       │  Why?
       ▼
   Why 1:      "Picker missed the SLA window."
       │  Why?
       ▼
   Why 2:      "Truck dock was full."
       │  Why?
       ▼
   Why 3:      "Outbound dock blocked by inbound returns."
       │  Why?
       ▼
   Why 4:      "Returns hadn't been processed in 4 days."
       │  Why?
       ▼
   Why 5:      "Returns staff was reassigned to inventory count."
       │
       ▼
   Root cause: scheduling rule lacks priority for returns processing.
```

**Visual — Ishikawa Fishbone (6Ms):**

```
   Man     Machine    Method
     \      |        /
      \     |       /
       \    |      /
        \   |     /
         \  |    /
          \ |   /
           \|  /
   ─────────────────────►  PROBLEM
           /|  \
          / |   \
         /  |    \
        /   |     \
       /    |      \
      /     |       \
     /      |        \
   Material Measurement Milieu (Environment)
```

**Visual — 5W1H** (single row of probes):

```
   PROBLEM
   ──┬──┬──┬──┬──┬──
     ▼  ▼  ▼  ▼  ▼  ▼
    Who What Where When Why How
```

**5 Whys:** iterate the question "why?" 5 times to drill from symptom to root cause.

**Ishikawa 6Ms (cause categories):** **M**an / **M**achine / **M**ethod / **M**aterial / **M**easurement / **M**ilieu (Environment).

**5W1H:** **W**ho / **W**hat / **W**here / **W**hen / **W**hy / **H**ow.

**SEACOW(r) mapping:** all three are relation frames — causal attribution applied to a problem.

**Notable for:** the simplest tools that consistently outperform their complexity; pair well with PDCA's *Check* phase.

---

## Business Model Canvas (Osterwalder & Pigneur, 2010)

**Source:** *Business Model Generation* — [strategyzer.com/canvas/business-model-canvas](https://www.strategyzer.com/canvas/business-model-canvas).

**Nine blocks:**

```
KEY PARTNERS       │ KEY ACTIVITIES   │              │ CUSTOMER         │ CUSTOMER
                   │                  │              │ RELATIONSHIPS    │ SEGMENTS
                   ├──────────────────│ VALUE         ├──────────────────│
                   │ KEY RESOURCES    │ PROPOSITIONS  │ CHANNELS         │
                   │                  │              │                  │
─────────────────────────────────────────────────────────────────────────
COST STRUCTURE                                  │ REVENUE STREAMS
```

**SEACOW(r) mapping:** System (whole-business surface in one frame) — every block touches Entities (Segments / Partners) and Activities (Key Activities).

**Notable variants:** **Lean Canvas** (Ash Maurya, 2012) replaces Key Partners / Key Activities / Key Resources / Customer Relationships with Problem / Solution / Key Metrics / Unfair Advantage. Better for early-stage startups.

---

# More PKM frameworks

(Building on the [PKM section](#personal-knowledge-management-pkm-frameworks) at the top of this gallery.)

## Forte's CODE (Tiago Forte)

**Source:** [fortelabs.com/blog/basboverview/](https://fortelabs.com/blog/basboverview/) · *Building a Second Brain* (2022).

**Four verbs:**

```
CAPTURE   — keep what resonates
ORGANIZE  — by actionability into PARA
DISTILL   — find essence (progressive summarization)
EXPRESS   — show your work, ship
```

**Progressive Summarization layers** (the D step):

```
Layer 0: raw note
Layer 1: bold key passages
Layer 2: highlight the bolded
Layer 3: executive summary
Layer 4: remix into new artifact
```

**SEACOW(r) mapping:** PARA = Container taxonomy by actionability; CODE = Capture/Work/Output verb pipeline that *uses* PARA.

---

## Forte's Intermediate Packets (IPs) — Just-In-Time PM

**Source:** Tiago Forte, *Building a Second Brain*.

**Five IP types:**

```
1. Distilled Notes      — your processed notes (Layer 3 above)
2. Outtakes             — material cut from past projects, reusable
3. Work-in-Process      — current intermediate artifacts
4. Final Deliverables   — what you've already shipped, modular
5. Documentation        — how-to / SOP / reference
```

**SEACOW(r) mapping:** Output lifecycle — reusable mid-stage Entities between raw Capture and finished Output.

**Notable for:** the explicit *re-use* discipline. Every project deliverable is potentially an IP for the next one.

---

## Tiago Forte — PARA in Real Life

**Source:** Tiago Forte, *Building a Second Brain*.

**Pattern:** mirror the same 4-folder PARA structure across **every** container — desktop file system, cloud drive, email folders, note app, physical filing cabinet — so cross-platform navigation is isomorphic.

**Visual (mirror-PARA across every System):**

```
   ┌──────────────┬──────────────┬──────────────┬──────────────┬──────────────┐
   │   DESKTOP    │  CLOUD DRIVE │     EMAIL    │    NOTES     │   PHYSICAL   │
   ├──────────────┼──────────────┼──────────────┼──────────────┼──────────────┤
   │ /Projects    │ /Projects    │ /Projects    │ /Projects    │ Cab 1: Proj. │
   │ /Areas       │ /Areas       │ /Areas       │ /Areas       │ Cab 2: Areas │
   │ /Resources   │ /Resources   │ /Resources   │ /Resources   │ Cab 3: Res.  │
   │ /Archive     │ /Archive     │ /Archive     │ /Archive     │ Cab 4: Arch. │
   └──────────────┴──────────────┴──────────────┴──────────────┴──────────────┘
                                       ▲
                                       │
                          isomorphic across every System
                          → muscle memory cross-platform
                          → search trains the same vocabulary
```

**SEACOW(r) mapping:** same Container schema across every System surface. *Mirror-PARA*.

**Notable for:** explicit System-spanning convention. Every Capture surface and every Output surface uses the same four-folder shape.

---

## Sönke Ahrens — How to Take Smart Notes (2017)

**Source:** *How to Take Smart Notes* (Ahrens, 2017).

**Three note types:**

```
Fleeting notes      — transient capture, pre-permanent
Literature notes    — notes-on-source, in your own words
Permanent notes     — atomic, written for the slip-box
```

**Principle:** "writing is thinking" — only what you can rewrite, you understand.

**SEACOW(r) mapping:** Capture → Work pipeline staged by note-Entity type; permanence = promotion criterion.

**Notable for:** the modern (Obsidian-era) reformulation of Luhmann's Zettelkasten in language that doesn't require knowing German index-card filing.

---

## Andy Matuschak — Evergreen Notes

**Source:** [notes.andymatuschak.org/Evergreen_notes](https://notes.andymatuschak.org/Evergreen_notes).

**Five principles (verbatim):**

```
1. Evergreen notes should be ATOMIC.
2. Evergreen notes should be CONCEPT-ORIENTED.
3. Evergreen notes should be DENSELY LINKED.
4. Prefer ASSOCIATIVE ONTOLOGIES to HIERARCHICAL TAXONOMIES.
5. Write notes for YOURSELF by default, disregarding audience.
```

**SEACOW(r) mapping:** Entity-shape rules (1-3) + relation-density rule (3) + an *anti-Container* stance (4); explicitly rejects hierarchical taxonomy.

**Notable for:** principle #4 is the most influential anti-folder argument in modern PKM. Pairs well with Zettelkasten and Roam-style daily-notes flow.

---

## Niklas Luhmann's Folgezettel (numbering scheme)

**Source:** [zettelkasten.de/posts/luhmann-folgezettel-truth/](https://zettelkasten.de/posts/luhmann-folgezettel-truth/).

**Alphanumeric branching IDs:**

```
1, 2, 3                — top-level entries
1a, 1b, 1c            — branches off 1
1a1, 1a2              — sub-branches off 1a
1a1a, 1a1b            — and so on, alternating digits and letters
```

**Rules:** sibling = increment final character (1 → 2; 1a → 1b); child = append next-tier character (1 → 1a → 1a1).

**SEACOW(r) mapping:** physical-medium relation encoding — IDs *are* the link graph; positions Entities in a branching sequence without imposing categories.

**Notable for:** Luhmann's own quote: "It is not important where you store a Zettel as long as you can reference it from every other point." The numbering existed because card position couldn't.

---

## Roam Research / daily-notes flow (Conor White-Sullivan, 2019)

**Source:** [roamresearch.com](https://roamresearch.com).

**Structure:**

```
Daily Note (date page)        — primary capture surface; the date is the default page
[[wikilink]]                  — creates a page on first reference
((block ref))                 — transcludes any bullet from anywhere
backlinks pane                — unlinked + linked references aggregator
outliner-native               — every line is a referenceable block
```

**SEACOW(r) mapping:** date axis = Capture spine; block = atomic Entity; backlinks = bidirectional relation surface.

**Notable for:** the Roam pattern is the closest most users come to a "no Containers" knowledge system. Logseq, Obsidian Daily Notes, and Tana all descend from it.

---

## Maggie Appleton — Stream / Garden / Campfire

**Source:** [maggieappleton.com/garden-history](https://maggieappleton.com/garden-history).

**Three publishing modes:**

```
Stream   — collapse to single-track timeline; ephemeral, algorithmic, chronological
           (Twitter, Facebook feed, blog reverse-chrono)

Garden   — richly linked landscape that grows slowly over time; non-chronological
           (digital gardens, wikis, evergreen-note sites)

Campfire — private Slack groups, casual blog rings, "Cozy Web" intimacies
           (Tom Critchlow's coinage)
```

**SEACOW(r) mapping:** three publishing-System modes distinguished by **time-axis** vs **link-axis** vs **intimacy-axis**.

**Notable variants:** "Torch" sometimes used in place of Campfire in PKM circles.

---

## Commonplace book (17th c.; Locke's method 1706)

**Source:** [en.wikipedia.org/wiki/Commonplace_book](https://en.wikipedia.org/wiki/Commonplace_book).

**Structure:**

- Organized by **subject headings** ("heads") — ethics, theology, love, politics, religion, etc.
- Content types: notes, proverbs, adages, aphorisms, maxims, recipes, quotes, letters, poems, tables, prayers, professional references.
- **Locke's 1706 indexing method:** index by *first letter* + *first vowel* of each head (so all "Politics" entries land in `Pi`, "Patience" in `Pa`).

**Visual** (Locke's index — first letter + first vowel of each head):

```
   Index page (the front of the book):

       │ a │ e │ i │ o │ u │
   ────┼───┼───┼───┼───┼───┤
    A  │p2 │p7 │   │p11│   │  ← entries starting with 'A' indexed by next vowel
    B  │   │   │   │p3 │   │
    P  │p5 │p8 │p13│p20│   │  ← Pa = "Patience" → p5
                              │   Pe = "Persistence" → p8
                              │   Pi = "Politics" → p13   (per Locke's example)
                              │   Po = "Power" → p20

   Page 5 (first available "Pa..." page):
   ┌──────────────────────────────────────────┐
   │ Patience                                  │
   │ ─────────                                  │
   │ "He that can have patience, can have       │
   │  what he will." — Franklin                 │
   │                                              │
   │ "Patience is bitter, but its fruit          │
   │  is sweet." — Aristotle                    │
   └──────────────────────────────────────────┘
```

**SEACOW(r) mapping:** thematic-head Container taxonomy of quote/observation Entities — Zettelkasten's direct ancestor, *hierarchical* rather than associative.

**Notable for:** the prehistoric Output-first organization scheme that influenced both Locke's *Essay Concerning Human Understanding* and modern Zettelkasten advocates (Ahrens cites it).

---

# More library science / metadata standards

(Building on the [Library science / formal classification](#library-science--formal-classification) section above.)

## Dublin Core Metadata Element Set (DCMI, 1995 / RFC 2413, 1998)

**Source:** [dublincore.org/specifications/dublin-core/dces/](https://www.dublincore.org/specifications/dublin-core/dces/).

**15 core elements:**

```
Title         Creator      Subject      Description   Publisher
Contributor   Date         Type         Format        Identifier
Source        Language     Relation     Coverage      Rights
```

**SEACOW(r) mapping:** flat property-set spanning Entity (Creator/Contributor/Publisher), Output (Title/Description/Type/Format), and relation (Source/Relation/Coverage).

**Where it shows up:** Obsidian / Hugo frontmatter conventions; OAI-PMH default schema; the most-copied metadata vocabulary in the world.

---

## schema.org (Google / Bing / Yahoo / Yandex, 2011)

**Source:** [schema.org](https://schema.org/docs/full.html).

**Top-level types** (direct children of `Thing`):

```
Action     — verbs
BioChemEntity
CreativeWork — books, articles, blog posts, software
Event      — concerts, lectures, sports matches
Intangible — services, ratings, contact points
MedicalEntity
Organization
Person
Place
Product
Taxon (some versions)
```

**SEACOW(r) mapping:** full SEACOW spread — Entity (Person/Organization), Activities (Action/Event), Output (CreativeWork/Product), relation via Intangible.

**Where it shows up:** JSON-LD page metadata, knowledge-graph publishing, Obsidian frontmatter `@type`.

---

## FOAF — Friend of a Friend (Brickley & Miller, 2000-2014)

**Source:** [xmlns.com/foaf/spec/](http://xmlns.com/foaf/spec/).

**Visual** (class hierarchy + property edges):

```
                     foaf:Agent
                    /     │     \
              Person   Organization  Group
                │           │           │
        ┌───────┼───────┐   │           │
       knows   made    interest         │
        │       │        │              │
      Person  Document  Concept         │
              (foaf:Document)
              ├── foaf:Image
              ├── foaf:PersonalProfileDocument
              └── (any web doc)

   Properties: name · homepage · mbox · weblog · interest · depiction · depicts
```

**Classes:** `Agent` / `Person` / `Organization` / `Group` / `Document` / `Image` / `Project` / `OnlineAccount`.

**Properties:** `name`, `homepage`, `knows`, `made`/`maker`, `mbox`, `weblog`, `interest`, `depiction`/`depicts`.

**SEACOW(r) mapping:** pure Entity layer (people / organizations / projects) with light Output (Document) and relation (`knows` / `made`).

**Where it shows up:** personal websites' RDF metadata; the social-graph ancestor before walled-garden social networks.

---

## SKOS — Simple Knowledge Organization System (W3C, 2009)

**Source:** [w3.org/TR/skos-reference/](https://www.w3.org/TR/skos-reference/).

**Visual** (concepts + relationships):

```
                     skos:ConceptScheme
                    "Cybersecurity Topics"
                            │
                            │ hasTopConcept
                            ▼
   ┌─────────────────────  Concept  ─────────────────────┐
   │                                                      │
   │  prefLabel:   "Cryptography"                          │
   │  altLabel:    "Crypto", "Cipher systems"              │
   │  hiddenLabel: "kryptography" (typo redirect)          │
   │                                                      │
   └──────┬─────────────┬──────────────┬─────────────────┘
          │             │              │
   broader │     narrower │     related │
          ▼             ▼              ▼
       Information     Public-key      Network
       security        cryptography    security
       (parent)        (child)         (sibling concept)
```

**Classes:** `skos:Concept` / `skos:ConceptScheme` / `skos:Collection` / `skos:OrderedCollection`.

**Properties:** `broader` / `narrower` / `broaderTransitive` / `narrowerTransitive` / `related` / `prefLabel` / `altLabel` / `hiddenLabel` / `inScheme` / `topConceptOf` / `hasTopConcept`.

**SEACOW(r) mapping:** the relation/Capture layer made formal — controlled vocabularies and the wiring between concepts.

**Where it shows up:** tag taxonomies, library subject thesauri, ontology bridging. Most MOC plugins map cleanly to SKOS.

---

## MARC 21 (LoC + LAC, 1999)

**Source:** [loc.gov/marc](https://www.loc.gov/marc).

**Tag blocks:**

```
0XX  control / numbers (008 fixed-length data, 020 ISBN, 022 ISSN)
1XX  main entry (100 personal name, 110 corporate)
2XX  titles (245 title statement, 250 edition)
3XX  physical description
4XX  series
5XX  notes
6XX  subject access (650 topical heading)
7XX  added entries
8XX  series added entries
9XX  local
```

**SEACOW(r) mapping:** Output-centric — fielded record-per-Output (book / serial) with Entity (1XX/7XX) and relation (6XX) attached.

**Where it shows up:** library ILS systems (Aleph, Sierra, Alma); not common in PKM but the *grammar* (control fields + data fields + subfields) is influential.

---

## MeSH — Medical Subject Headings (NLM, annual)

**Source:** [meshb.nlm.nih.gov/treeView](https://meshb.nlm.nih.gov/treeView).

**Top-level categories:**

```
A  Anatomy                           L  Information Science
B  Organisms                         M  Named Groups
C  Diseases                          N  Health Care
D  Chemicals and Drugs               V  Publication Characteristics
E  Diagnostic & Therapeutic           Z  Geographicals
F  Psychiatry and Psychology
G  Phenomena and Processes
H  Disciplines and Occupations
I  Anthropology, Education, Sociology
J  Technology, Industry, Agriculture
K  Humanities
```

**SEACOW(r) mapping:** domain-specific Capture vocabulary — controlled subject tagging for biomedical Output.

**Where it shows up:** PubMed indexing; templates for tag schemas in research vaults.

---

## AAT — Getty Art & Architecture Thesaurus

**Source:** [getty.edu/research/tools/vocabularies/aat](https://www.getty.edu/research/tools/vocabularies/aat/about.html).

**Seven facets** (verbatim):

```
Associated Concepts
Physical Attributes
Styles and Periods
Agents
Activities
Materials
Objects
```

**SEACOW(r) mapping:** **a near-explicit SEACOW** — Agents = Entity, Activities = Activities, Objects/Materials = Output, Styles/Concepts = relation/Capture.

**Notable for:** if you're building a personal taxonomy and want a faceted-classification template, AAT is one of the cleanest models in existence.

---

## EAD — Encoded Archival Description (LoC + SAA, 1998)

**Source:** [loc.gov/ead](https://www.loc.gov/ead/).

**`<archdesc>` children:**

```
did              — Descriptive Identification (creator, size, dates, language, abstract)
bioghist         — biography / history
scopecontent     — scope and content
controlaccess    — controlled-access subjects, names, places
accessrestrict   — access restrictions
userestrict      — use restrictions
arrangement      — how the collection is arranged
relatedmaterial
separatedmaterial
dsc              — subordinate components inventory (the nested folder/file tree)
```

**SEACOW(r) mapping:** hierarchical Output description with Entity (creator) and Capture (controlaccess) slots.

**Where it shows up:** archival finding aids; nested folder-note patterns in PKM.

---

## ISO 25964 — Thesauri & Interoperability (ISO 2011/2013)

**Source:** [niso.org/schemas/iso25964](https://www.niso.org/schemas/iso25964).

**Relationship types:**

```
Equivalence:        USE / UF (Used For)
Hierarchical:       BT / NT  (Broader Term / Narrower Term)
                    BT-G / NT-G   generic
                    BT-P / NT-P   partitive (whole/part)
                    BT-I / NT-I   instantial
Associative:        RT (Related Term)
Multilingual:       cross-language equivalences
```

**SEACOW(r) mapping:** the *grammar* of the relation layer — formal link types for any controlled vocabulary.

**Where it shows up:** SKOS extensions; Tag Wrangler-style alias/synonym handling.

---

## Bates numbering (Bates Manufacturing Co., 1891 patent)

**Source:** [en.wikipedia.org/wiki/Bates_numbering](https://en.wikipedia.org/wiki/Bates_numbering).

**Format:** `PREFIX-000001` — originally a 4-digit sequence (0000–9999), modern use 4-7 digits.

```
ABC-DEF-0001234
└─ prefix ─┘└── ID ──┘
```

**SEACOW(r) mapping:** pure Output identifier convention — stable per-artifact IDs.

**Where it shows up:** legal discovery; analog for stable note IDs in Zettelkasten and frontmatter `id:` fields.

---

## IDEF0 — Function Modeling (FIPS PUB 183, NIST 1993)

**Source:** [en.wikipedia.org/wiki/IDEF0](https://en.wikipedia.org/wiki/IDEF0).

**ICOM (every function box has):**

```
        Controls (top)        — governing constraints, policies
            ↓
Inputs ───►[ FUNCTION ]───► Outputs
(left)                     (right)
            ↑
        Mechanisms (bottom)   — supporting means (people, tools, systems)
```

**SEACOW(r) mapping:** Activities-layer notation — every box is a Capture/Work step with explicit Inputs → Outputs and Mechanisms (System / Entity) and Controls (rules).

**Where it shows up:** process docs; SOP diagrams; the visual ancestor of BPMN.

---

## IDEF1X — Data Modeling (FIPS PUB 184, NIST 1993)

**Source:** [en.wikipedia.org/wiki/IDEF1X](https://en.wikipedia.org/wiki/IDEF1X).

**Concepts:**

```
Entity types:        Independent / Dependent
Relationships:       Identifying / Non-Identifying / Specific / Non-Specific / Categorization
Keys:                Primary / Alternate / Foreign
```

**SEACOW(r) mapping:** schema for Entity layer + relation cardinality.

**Where it shows up:** ER diagrams; Bases / Dataview schema sketches; the canonical pre-UML data-modeling notation.

---

## OAIS — Open Archival Information System (ISO 14721:2012, CCSDS)

**Source:** [public.ccsds.org/Pubs/650x0m2.pdf](https://public.ccsds.org/Pubs/650x0m2.pdf).

**Information Packages:**

```
SIP — Submission Information Package    (producer → archive)
AIP — Archival Information Package      (stored by archive)
DIP — Dissemination Information Package (archive → user)
```

**Functional entities:**

```
Ingest          Archival Storage   Data Management
Administration  Preservation Planning   Access
```

**SEACOW(r) mapping:** Activities / Capture pipeline for Output preservation — inbox → archive → retrieval.

**Where it shows up:** vault inbox → processing → archive folders; the formal model behind the temperature gradient idea.

---

## OAI-PMH (Open Archives Initiative, 1999)

**Source:** [openarchives.org/OAI/openarchivesprotocol.html](https://www.openarchives.org/OAI/openarchivesprotocol.html).

**Six verbs:**

```
Identify              ListMetadataFormats   ListSets
ListIdentifiers       ListRecords           GetRecord
```

**SEACOW(r) mapping:** protocol for harvesting Output metadata across Systems — pure relation / transport layer.

**Where it shows up:** repository federation; analog for vault-to-vault sync APIs.

---

## CIDOC-CRM (ISO 21127:2014, CIDOC/ICOM)

**Source:** [cidoc-crm.org](https://www.cidoc-crm.org/).

**~92 entity classes (E1 – E92):**

```
E1 CRM Entity              E2 Temporal Entity         E5 Event
E18 Physical Thing         E21 Person                 E39 Actor
E52 Time-Span              E53 Place                  E70 Thing
E77 Persistent Item        E89 Propositional Object   …
```

**SEACOW(r) mapping:** Event-centric ontology — Activities (Event) connect Actor / Place / Time-Span / Thing across all SEACOW layers.

**Where it shows up:** cultural-heritage linked data; the richest event-modeling reference in formal ontology.

---

## BIBFRAME (Library of Congress, 2014→)

**Source:** [loc.gov/bibframe](https://www.loc.gov/bibframe/).

**Three core classes:**

```
Work      — the intellectual / artistic content (e.g. "Hamlet" the play)
Instance  — a specific manifestation (e.g. the 1623 First Folio, or a 2020 paperback)
Item      — a single physical or digital copy (the one in this library)
```

**SEACOW(r) mapping:** Output stratified — abstract Work / concrete Instance / specific Item.

**Where it shows up:** modern library linked data (MARC's RDF successor); analog for note-vs-rendered-page-vs-export distinction in PKM.

---

## METS (LoC / DLF, 2001)

**Source:** [loc.gov/standards/mets/](https://www.loc.gov/standards/mets/).

**Seven sections:**

```
metsHdr      — header
dmdSec       — descriptive metadata
amdSec       — administrative metadata
fileSec      — file inventory
structMap    — hierarchical structure (the only mandatory section)
structLink
behaviorSec
```

**SEACOW(r) mapping:** container for digital Output — wraps content + Capture metadata + relation map.

**Where it shows up:** digital library packages; analog for vault-export bundles (`.zip` of vault + manifest.json).

---

## Wikidata data model (Wikimedia Foundation, 2012)

**Source:** [wikidata.org/wiki/Help:Statements](https://www.wikidata.org/wiki/Help:Statements).

**Building blocks:**

```
Item (Q-ID)         — a concept (Q42 = Douglas Adams)
Property (P-ID)     — a category of data (P31 = "instance of")
Statement           = property-value pair + (qualifiers + references + ranks)
  property-value alone = "claim"
  without qualifiers   = "snak"
```

**SEACOW(r) mapping:** Entity + relation + provenance — every fact is reified with sources.

**Where it shows up:** Dataview / Bases-style frontmatter with provenance fields.

---

## ISO/IEC 11179 — Metadata Registry (ISO/IEC, 2003-2019)

**Source:** [en.wikipedia.org/wiki/ISO/IEC_11179](https://en.wikipedia.org/wiki/ISO/IEC_11179).

**Visual** (Data Element decomposition):

```
                   Data Element
                  (e.g. "PersonAge_Years")
                         │
            ┌────────────┴────────────┐
            │                         │
   Data Element Concept       Value Domain
   "Age of a Person"          "Integer years, 0-150"
            │                         │
            │                         │
   Conceptual Domain           Permissible Values
   "Age"                       {0, 1, 2, …, 150}

   The 7 parts of ISO/IEC 11179:
   Part 1: Framework
   Part 2: Classification                     ◀── what kinds of metadata exist
   Part 3: Registry metamodel                 ◀── relationships between metadata
   Part 4: Formulation of definitions
   Part 5: Naming and identification          ◀── conventions for IDs
   Part 6: Registration                       ◀── lifecycle: proposed → approved → retired
   Part 7: Metamodel for data set registration
```

**Parts 1-7:** Framework / Classification / Registry metamodel / Formulation of definitions / Naming and identification / Registration / Metamodel for data set registration.

**Concepts:** Data Element Concept / Conceptual Domain / Value Domain / Data Element.

**SEACOW(r) mapping:** meta-System layer — registry of *how field definitions themselves* are governed.

**Where it shows up:** property registries; canonical-frontmatter governance.

---

## PREMIS — Preservation Metadata (LoC, v3 2015)

**Source:** [loc.gov/standards/premis/](https://www.loc.gov/standards/premis/).

**Semantic units:**

```
Object    (with subtypes File / Bitstream / Representation / Intellectual Entity)
Event
Agent
Rights
```

**SEACOW(r) mapping:** **direct SEACOW(r) analog** — Object = Output, Event = Activities, Agent = Entity, Rights = relation / governance.

**Where it shows up:** digital preservation; analog for change-log / event-stream patterns in PKM.

---

# Enterprise architecture & strategy

## DAMA-DMBOK2 (DAMA International, 2nd ed., 2017)

**Source:** [dama.org/cpages/body-of-knowledge](https://www.dama.org/cpages/body-of-knowledge).

**11 knowledge areas around Data Governance:**

```
                    DATA GOVERNANCE (hub)
                    /        |        \
Data Architecture  Data Modeling  Data Storage & Operations
Data Security      Data Integration & Interoperability
Documents & Content   Reference & Master Data
Data Warehousing & BI    Metadata    Data Quality
```

**SEACOW(r) mapping:** information / data layer (with Governance as cross-cut).

**Notable for:** canonical taxonomy for data-management roles, RACI, and CDMP certification crosswalks.

---

## TOGAF ADM (The Open Group, v9.2 / v10, 2022)

**Source:** [pubs.opengroup.org/togaf-standard/adm/](https://pubs.opengroup.org/togaf-standard/adm/).

**Architecture Development Method phases:**

```
Preliminary
A.  Architecture Vision
B.  Business Architecture
C.  Information Systems Architectures (Data + Application)
D.  Technology Architecture
E.  Opportunities & Solutions
F.  Migration Planning
G.  Implementation Governance
H.  Architecture Change Management
+   Requirements Management (cross-cutting, in the center)
```

**SEACOW(r) mapping:** capability / architecture layer (process for traversing all SEACOW layers).

**Notable for:** de facto EA method; ADM phases map to lifecycle gates.

---

## ArchiMate (The Open Group, v3.2, 2023)

**Source:** [pubs.opengroup.org/architecture/archimate3-doc/](https://pubs.opengroup.org/architecture/archimate3-doc/).

**Layers (top to bottom):**

```
Strategy
Business
Application
Technology
Physical
Implementation & Migration
Motivation                  (cross-cutting)
```

Aspects (per layer): Active Structure / Behavior / Passive Structure.

**SEACOW(r) mapping:** modeling notation spanning Strategy → Operations.

**Notable for:** visual EA modeling; pairs with TOGAF.

---

## Zachman Framework (Zachman International, v3.0)

**Source:** [zachman.com/about-the-zachman-framework](https://www.zachman.com/about-the-zachman-framework).

**6 × 6 ontology grid:**

```
                    What    How    Where  Who    When   Why
                    (Inv)   (Proc) (Net)  (Org)  (Time) (Mot)
Executive (Scope)    □       □      □      □      □      □
Business Mgmt        □       □      □      □      □      □
Architect (System)   □       □      □      □      □      □
Engineer (Tech)      □       □      □      □      □      □
Technician (Detail)  □       □      □      □      □      □
Enterprise (Func)    □       □      □      □      □      □
```

**SEACOW(r) mapping:** cross-cutting ontology (every SEACOW layer × 6 interrogatives).

**Notable for:** pure classification ontology; not a method. The original meta-grid that everything else descends from.

---

## C4 Model (Simon Brown)

**Source:** [c4model.com](https://c4model.com).

**Four zoom levels:**

```
Level 1: System Context   — your software in the world
Level 2: Container        — apps, databases, services
Level 3: Component        — internal modules
Level 4: Code             — class diagrams (rarely needed)
+ Supplementary:          System Landscape, Dynamic, Deployment
```

**SEACOW(r) mapping:** architecture (zoom levels of system structure).

**Notable for:** simple, code-aligned diagramming for software teams. Diagrams-as-code via Structurizr.

---

## arc42 (Starke & Hruschka)

**Source:** [arc42.org/overview](https://arc42.org/overview).

**12 sections:**

```
1.  Introduction & Goals      7.  Deployment View
2.  Constraints                8.  Cross-cutting Concepts
3.  Context & Scope            9.  Architecture Decisions
4.  Solution Strategy         10.  Quality Requirements
5.  Building Block View       11.  Risks & Technical Debt
6.  Runtime View              12.  Glossary
```

**SEACOW(r) mapping:** architecture documentation template (Output-layer schema).

**Notable for:** open-source, language-agnostic; pairs with C4 for views.

---

## 4+1 architectural view model (Kruchten, 1995)

**Source:** [cs.ubc.ca/~gregor/teaching/papers/4+1view-architecture.pdf](https://www.cs.ubc.ca/~gregor/teaching/papers/4+1view-architecture.pdf).

**Five views:**

```
Logical View       — design / class diagrams
Process View       — concurrency, runtime
Development View   — code organization, modules
Physical View      — deployment topology
+ Scenarios        — use cases tying the above together
```

**SEACOW(r) mapping:** architecture (multi-stakeholder views).

**Notable for:** foundational for RUP and IEEE 1471.

---

## Garrett's 5 Elements of UX (Jesse James Garrett, 2000)

**Source:** *The Elements of User Experience* (Garrett, 2002).

**Five layers (bottom → top):**

```
Strategy   — user needs + product objectives
Scope      — functional specs + content requirements
Structure  — interaction design + information architecture
Skeleton   — interface, navigation, information design
Surface    — visual / sensory design
```

**SEACOW(r) mapping:** System (layered UX abstraction stack — every layer maps to a SEACOW component, with Surface = Output).

**Notable for:** foundational UX text; the layers framing is reused across product organizations.

---

## Norman's Design Principles (Don Norman, *Design of Everyday Things*)

**Source:** *Design of Everyday Things* (Norman, 1988 / 2013).

**Visual** (the principles applied to a single artifact):

```
                          [ ARTIFACT (e.g. a door) ]
                                   │
        ┌───────────┬───────┬─────┴─────┬────────┬──────────┐
        │           │       │           │        │          │
   Affordance  Signifier Mapping  Feedback  Constraint  Conceptual
   "I can grab "Pull"     "push side"  "click   "won't open
   this handle" sticker   feel right    sound"   if locked"  Model
                                       (the user's
                                        mental story
                                        of how it works)
        │           │       │           │        │          │
        └────── all support ─┼─ Visibility ─┼─ Consistency ─┘
                              │              │
                              ▼              ▼
                            Discoverability + Learnability
```

**Principles:** Visibility / Feedback / Constraints / Mapping / Consistency / Affordance (sometimes also Discoverability / Signifiers / Conceptual Model).

**SEACOW(r) mapping:** relations (Entity ↔ Object usability properties).

**Notable for:** the lingua franca of UX critique. Affordance + signifier is the indispensable language pair.

---

## Wardley Mapping (Simon Wardley)

**Source:** [learnwardleymapping.com](https://learnwardleymapping.com/).

**Map structure:**

```
Y-axis: Value Chain (Visible ↑ to Invisible ↓ to user)
X-axis: Evolution (Genesis → Custom-built → Product → Commodity)
```

Components plotted by **dependency** (Y) and **maturity** (X).

**SEACOW(r) mapping:** strategy map combining dependency + maturity. Output-layer reasoning at the System level.

**Notable for:** unique among strategy frameworks for explicitly modeling component evolution over time.

---

# IT governance / GRC

## ITIL 4 (AXELOS / PeopleCert, 2019+)

**Source:** [axelos.com](https://www.axelos.com/certifications/itil-service-management).

**Service Value System (SVS):**

```
4 Dimensions:        Organizations & People / Information & Technology /
                     Partners & Suppliers / Value Streams & Processes
7 Guiding Principles
Service Value Chain: Plan / Improve / Engage / Design&Transition / Obtain / Build / Deliver&Support
34 Management Practices in 3 groups:
  - General Management   (14 practices)
  - Service Management   (17 practices)
  - Technical Management (3 practices)
```

**SEACOW(r) mapping:** operations / service layer.

**Notable for:** mainstream ITSM; maps to COBIT and ISO 20000.

---

## COBIT 2019 (ISACA)

**Source:** [isaca.org/resources/cobit](https://www.isaca.org/resources/cobit).

**40 Governance / Management objectives across 5 domains:**

```
Governance:
  EDM — Evaluate, Direct, Monitor          (5 objectives)
Management:
  APO — Align, Plan, Organize              (14)
  BAI — Build, Acquire, Implement          (11)
  DSS — Deliver, Service, Support          (6)
  MEA — Monitor, Evaluate, Assess          (4)
```

**SEACOW(r) mapping:** governance / capability layer.

**Notable for:** audit-grade IT governance; integrates with ITIL, NIST, ISO.

---

## IIA Three Lines Model (Institute of Internal Auditors)

**Source:** [theiia.org/en/content/guidance/mandatory/standards/three-lines-model](https://www.theiia.org/) · also documented in your `cyberbase/⬇ INBOX, DROPZONE/Governance, Mgmt/IIA 3 Lines Model/`.

**Four roles:**

```
Governing Body        — sets objectives, delegates, expects assurance
1st Line (Management) — leads actions, manages risk, applies resources, owns controls
2nd Line (Risk/Compliance) — expertise, support, monitoring, challenge (specialist advisory)
3rd Line (Internal Audit)  — independent assurance, reports to governing body
```

**SEACOW(r) mapping:** Entity-stratification across an organization — accountability roles for governance and oversight.

**Notable for:** the canonical model for assurance and audit independence in any GRC program.

---

## ISO/IEC 27001 / 27002:2022

**Source:** [iso.org/standard/27001](https://www.iso.org/standard/27001).

**Annex A — 93 controls in 4 themes (2022 update):**

```
Organizational  (37 controls)
People          (8)
Physical        (14)
Technological   (34)
```

**14 control attribute categories** (for tagging/filtering controls): control type, information-security properties (CIA), cybersecurity concepts mapped to NIST CSF, operational capabilities, security domains.

**SEACOW(r) mapping:** controls / risk layer.

**Notable for:** certifiable ISMS standard; baseline for global compliance.

---

## NIST RMF (Risk Management Framework, SP 800-37 Rev. 2)

**Source:** [csrc.nist.gov/projects/risk-management](https://csrc.nist.gov/projects/risk-management).

**Seven steps:**

```
PREPARE → CATEGORIZE → SELECT → IMPLEMENT → ASSESS → AUTHORIZE → MONITOR
                                                                    │
                                                                    └─► (loop back)
```

**SEACOW(r) mapping:** risk / compliance lifecycle.

**Notable for:** federal ATO process; pairs with SP 800-53 control catalog.

---

## NIST Privacy Framework v1.0 (2020)

**Source:** [nist.gov/privacy-framework](https://www.nist.gov/privacy-framework).

**Core (5 functions):**

```
Identify-P    Govern-P    Control-P    Communicate-P    Protect-P
```

Plus Profiles and Implementation Tiers (1-4).

**SEACOW(r) mapping:** risk / compliance layer (privacy-specific).

**Notable for:** companion to NIST CSF; aligns with GDPR / CCPA mappings.

---

## FAIR — Factor Analysis of Information Risk (FAIR Institute / Open Group O-RA)

**Source:** [fairinstitute.org](https://www.fairinstitute.org/fair-risk-management).

**Decomposition tree:**

```
Risk
 ├── Loss Event Frequency (LEF)
 │    ├── Threat Event Frequency
 │    │    ├── Contact Frequency
 │    │    └── Probability of Action
 │    └── Vulnerability
 │         ├── Threat Capability
 │         └── Resistance Strength
 └── Loss Magnitude (LM)
      ├── Primary Loss
      └── Secondary Risk
           ├── Secondary LEF
           └── Secondary LM
```

**SEACOW(r) mapping:** risk quantification layer.

**Notable for:** quantitative risk in $ rather than qualitative red/yellow/green; complements ISO 27005.

---

## SABSA (Sherwood Applied Business Security Architecture)

**Source:** [sabsa.org](https://sabsa.org).

**6 layers × 6 questions matrix:**

```
                     What    Why    How    Who    Where  When
                     (Assets)(Mot)  (Proc) (Pple) (Loc)  (Time)
Contextual            □       □      □      □      □      □
(Business view)
Conceptual            □       □      □      □      □      □
(Architect's view)
Logical               □       □      □      □      □      □
Physical              □       □      □      □      □      □
Component             □       □      □      □      □      □
Operational           □       □      □      □      □      □
(Service Manager)
```

**SEACOW(r) mapping:** security architecture (Zachman-style for security).

**Notable for:** business-driven security architecture; traceability assets → controls.

---

## OWASP ASVS v4.0.3

**Source:** [owasp.org/www-project-application-security-verification-standard](https://owasp.org/www-project-application-security-verification-standard/).

**14 categories × 3 levels** (L1 Opportunistic / L2 Standard / L3 Advanced):

```
V1   Architecture, Design & Threat Modeling
V2   Authentication
V3   Session Management
V4   Access Control
V5   Validation, Sanitization & Encoding
V6   Stored Cryptography
V7   Error Handling & Logging
V8   Data Protection
V9   Communication
V10  Malicious Code
V11  Business Logic
V12  Files & Resources
V13  API & Web Service
V14  Configuration
```

**SEACOW(r) mapping:** application controls layer.

**Notable for:** verification checklist for AppSec; pairs with Top 10.

---

## OWASP Top 10 (2021)

**Source:** [owasp.org/Top10/](https://owasp.org/Top10/).

```
A01  Broken Access Control
A02  Cryptographic Failures
A03  Injection
A04  Insecure Design
A05  Security Misconfiguration
A06  Vulnerable & Outdated Components
A07  Identification & Authentication Failures
A08  Software & Data Integrity Failures
A09  Security Logging & Monitoring Failures
A10  Server-Side Request Forgery (SSRF)
```

**SEACOW(r) mapping:** application risks layer.

**Notable for:** awareness doc, not a standard; widely cited in policy.

---

## CSA CCM v4 (Cloud Security Alliance Cloud Controls Matrix)

**Source:** [cloudsecurityalliance.org/research/cloud-controls-matrix](https://cloudsecurityalliance.org/research/cloud-controls-matrix).

**17 domains, 197 controls:**

```
A&AC   Audit & Assurance
AIS    Application & Interface Security
BCR    Business Continuity & Operational Resilience
CCC    Change Control & Configuration Management
CEK    Cryptography, Encryption & Key Management
DCS    Datacenter Security
DSP    Data Security & Privacy Lifecycle Management
GRC    Governance, Risk & Compliance
HRS    Human Resources
IAM    Identity & Access Management
IPY    Interoperability & Portability
IVS    Infrastructure & Virtualization Security
LOG    Logging & Monitoring
SEF    Security Incident Mgmt, E-Discovery & Cloud Forensics
STA    Supply Chain Mgmt, Transparency & Accountability
TVM    Threat & Vulnerability Management
UEM    Universal Endpoint Management
```

**SEACOW(r) mapping:** cloud controls layer.

**Notable for:** CAIQ-mapped; crosswalks to ISO 27017, NIST 800-53, PCI DSS.

---

## PCI DSS v4.0 (PCI SSC, 2022)

**Source:** [pcisecuritystandards.org](https://www.pcisecuritystandards.org).

**6 goals / 12 requirements:**

```
Build & Maintain a Secure Network
  R1  Install/maintain network security controls (firewalls)
  R2  Apply secure configurations
Protect Account Data
  R3  Protect stored cardholder data
  R4  Protect cardholder data in transmission
Vulnerability Management
  R5  Protect against malicious software
  R6  Develop & maintain secure systems
Strong Access Control
  R7  Restrict access by need-to-know
  R8  Identify users & authenticate access
  R9  Restrict physical access
Regular Monitoring & Testing
  R10 Log & monitor all access
  R11 Test security
Information Security Policy
  R12 Support InfoSec with org policies
```

**SEACOW(r) mapping:** compliance layer (payments).

**Notable for:** mandated for cardholder data; v4 adds the customized approach option.

---

## HIPAA Security Rule (45 CFR Part 164, Subpart C)

**Source:** [hhs.gov/hipaa/for-professionals/security](https://www.hhs.gov/hipaa/for-professionals/security/).

**3 safeguard categories:**

```
Administrative (9 standards):  Security Mgmt Process / Workforce Security /
                               Access Mgmt / Awareness & Training /
                               Incident Procedures / Contingency Plan /
                               Evaluation / BAAs / Assigned Responsibility

Physical (4):                   Facility Access / Workstation Use /
                               Workstation Security / Device & Media Controls

Technical (5):                  Access Control / Audit Controls / Integrity /
                               Authentication / Transmission Security
```

Specs are either **Required** or **Addressable**.

**SEACOW(r) mapping:** compliance layer (US healthcare ePHI).

**Notable for:** foundational for HITRUST.

---

# Project & delivery management

## PRINCE2 (AXELOS, 7th ed., 2023)

**Source:** [axelos.com](https://www.axelos.com/certifications/propath/prince2-project-management).

**7 + 7 + 7 structure:**

```
7 Principles:  Continued business justification / Learn from experience /
               Defined roles & responsibilities / Manage by stages /
               Manage by exception / Focus on products / Tailor to suit project

7 Practices:   Business Case / Organizing / Plans / Quality / Risk / Issues / Progress

7 Processes:   Starting Up / Directing / Initiating / Controlling a Stage /
               Managing Product Delivery / Managing Stage Boundaries / Closing
```

**SEACOW(r) mapping:** operations / project layer.

**Notable for:** stage-gated governance; UK-government default.

---

## PMI PMBOK 7th Edition (2021)

**Source:** [pmi.org/pmbok-guide-standards](https://www.pmi.org/pmbok-guide-standards).

**12 Principles + 8 Performance Domains:**

```
Principles:   Stewardship / Team / Stakeholders / Value / Systems Thinking /
              Leadership / Tailoring / Quality / Complexity / Risk /
              Adaptability & Resilience / Change

Performance   Stakeholders / Team / Development Approach & Life Cycle /
Domains:      Planning / Project Work / Delivery / Measurement / Uncertainty
```

**SEACOW(r) mapping:** operations / project layer.

**Notable for:** the 7th edition shifted from process-based (6th ed) to principle-based.

---

## SAFe (Scaled Agile Framework, v6.0)

**Source:** [scaledagileframework.com](https://scaledagileframework.com).

**4 configurations / levels:**

```
Team          — feature teams, Scrum / Kanban
Essential     — Agile Release Train (ART), 5-12 teams, Program Increment cadence
Large Solution — multiple ARTs cooperating on a single solution
Portfolio     — strategic themes, value streams, Lean budgets
              (Full SAFe combines all four)
```

**Core flow:** Strategic Themes → Portfolio Backlog → Solution Train → ART → Team Backlog.

**SEACOW(r) mapping:** operations / delivery layer.

**Notable for:** enterprise agile; PI Planning cadence.

---

## GitHub Flow / GitFlow / Trunk-Based Development

**Sources:** [docs.github.com — github-flow](https://docs.github.com/en/get-started/quickstart/github-flow) · [nvie.com — GitFlow](https://nvie.com/posts/a-successful-git-branching-model/) · [trunkbaseddevelopment.com](https://trunkbaseddevelopment.com).

**Visuals** (branch topology):

```
   GitHub Flow:
   main  ──●─────────●─────────●─────────●─────────●──▶
            \       / \       /
             feat-A    feat-B
              ●──●      ●──●
              (PR ↑)    (PR ↑)

   GitFlow (Vincent Driessen):
   main     ──●─────────────────●─────────────────●──▶  (production)
              │                 │                 │
              │  release/1.0    │  release/2.0    │
              │   ●──●          │   ●──●          │
              │  /    \         │  /    \         │
   develop  ─●─●──────●─────────●─●──────●────────●────▶  (integration)
                \      \         │      / \
                 feat   feat     │  feat    hotfix/1.0.1
                  ●──●   ●──●    │   ●──●     ●──● (off main, back to both)
                                 │

   Trunk-Based Development:
   trunk ──●──●──●──●──●──●──●──●──●──●──●──●──▶
            \  \  \  \                       │
             feat short feat                 │  release/2024-Q4
              ●  ●  ●  ●                      ●──▶ (cut from trunk)
              (each <1 day, behind feature flags)
```

| Model | Branches |
|---|---|
| **GitHub Flow** | `main` ← short-lived feature branches → PR → deploy. Web-app default. |
| **GitFlow (Vincent Driessen)** | `main` / `develop` / `feature/*` / `release/*` / `hotfix/*`. Heavy, release-based. |
| **Trunk-Based Development** | `trunk` (`main`) ← short-lived branches (<1 day) or direct commits, release branches cut from trunk. CD-friendly. |

**SEACOW(r) mapping:** engineering workflow layer (System affordance).

**Notable for:** branch-model choice maps to *System maturity* — startups / web apps tend to GitHub Flow or Trunk; mature SaaS with multiple environments tend to GitFlow.

---

## The Twelve-Factor App (Heroku, Adam Wiggins, 2011)

**Source:** [12factor.net](https://12factor.net).

**12 factors:**

```
I.    Codebase            VII.   Port binding
II.   Dependencies        VIII.  Concurrency
III.  Config              IX.    Disposability
IV.   Backing services    X.     Dev/prod parity
V.    Build, release, run XI.    Logs
VI.   Processes           XII.   Admin processes
```

**SEACOW(r) mapping:** engineering / architecture principles (System hygiene).

**Notable for:** SaaS-era app design; baseline for cloud-native maturity.

---

# Threat modeling

## STRIDE (Microsoft)

**Source:** [learn.microsoft.com — STRIDE](https://learn.microsoft.com/en-us/azure/security/develop/threat-modeling-tool-threats).

**Six threat types ↔ security properties:**

```
Spoofing                  ↔  Authentication
Tampering                 ↔  Integrity
Repudiation               ↔  Non-repudiation
Information disclosure    ↔  Confidentiality
Denial of service         ↔  Availability
Elevation of privilege    ↔  Authorization
```

**SEACOW(r) mapping:** risk / threat-modeling layer.

**Notable for:** used in MS SDL; pairs with Data Flow Diagrams.

---

## PASTA — Process for Attack Simulation & Threat Analysis (UcedaVelez & Morana)

**Source:** [owasp.org/www-pdf-archive/PASTA-Methodology-OWASP.pdf](https://owasp.org/www-pdf-archive/PASTA-Methodology-OWASP.pdf).

**Seven stages:**

```
I.    Define Objectives
II.   Define Technical Scope
III.  Application Decomposition
IV.   Threat Analysis
V.    Vulnerability & Weakness Analysis
VI.   Attack Modeling
VII.  Risk & Impact Analysis
```

**SEACOW(r) mapping:** risk / threat-modeling layer (business-aligned).

**Notable for:** risk-centric; aligns threats to business impact.

---

## ICS Cyber Kill Chain (SANS / Assante & Lee, 2015)

**Source:** [sans.org — ICS Cyber Kill Chain](https://www.sans.org/white-papers/36297/).

**Two-stage model for OT / ICS:**

```
Stage 1 — Cyber Intrusion
  Reconnaissance → Weaponization → Targeting → Delivery →
  Exploit → Install/Modify → C2 → Act (gain ICS access)

Stage 2 — ICS Attack
  Develop (custom capability for target ICS) →
  Test (in lab) →
  Deliver (to ICS) →
  Install/Modify →
  Execute ICS Attack (Loss of View / Loss of Control / Manipulation)
```

**SEACOW(r) mapping:** risk / threat-kill-chain layer (OT/ICS-specific).

**Notable for:** extends the Lockheed kill chain for ICS; pairs with MITRE ATT&CK for ICS.

---

# Educational / cognitive taxonomies

## Bloom's Taxonomy, Revised (Anderson & Krathwohl, 2001)

**Source:** *A Taxonomy for Learning, Teaching, and Assessing.*

**6 cognitive process verbs × 4 knowledge dimensions:**

```
Cognitive process (low → high):
  Remember → Understand → Apply → Analyze → Evaluate → Create

Knowledge dimension:
  Factual / Conceptual / Procedural / Metacognitive
```

**SEACOW(r) mapping:** Activities × Object — verbs an Entity (learner) performs on Objects (knowledge).

**Notable for:** the standard reference for designing assessment items at varying cognitive demand.

---

## Webb's Depth of Knowledge (Norman Webb, 1997)

**Source:** Webb, N.L. (1997). *Criteria for Alignment of Expectations and Assessments.*

**4 levels:**

```
Level 1  Recall and Reproduction
Level 2  Skills and Concepts
Level 3  Strategic Thinking
Level 4  Extended Thinking
```

**SEACOW(r) mapping:** Activities (cognitive depth ordinal scale).

**Notable for:** measures *depth* (not difficulty). Used heavily in K-12 standards alignment.

---

## SOLO Taxonomy (Biggs & Collis, 1982)

**Source:** Biggs, J. & Collis, K. (1982). *Evaluating the Quality of Learning: The SOLO Taxonomy.*

**5 levels:**

```
Pre-structural    — misses the point
Uni-structural    — one relevant point
Multi-structural  — several relevant points, unconnected
Relational        — points integrated into a coherent whole
Extended Abstract — generalized beyond the immediate problem
```

**SEACOW(r) mapping:** Activities — quality / structure of a learner's response.

**Notable for:** measures *structural complexity* of understanding, not just recall.

---

## Costa's Levels of Questioning (Arthur Costa)

**Source:** Costa, A.L. *Developing Minds: A Resource Book for Teaching Thinking.*

**3 levels:**

```
Level 1  Gathering   — define, identify, list, name, observe, recite
Level 2  Processing  — compare, contrast, classify, infer, analyze
Level 3  Applying    — evaluate, predict, hypothesize, judge, speculate
```

**SEACOW(r) mapping:** Activities (question-verb tiers).

**Notable for:** AVID's standard framework for student questioning.

---

## Marzano's New Taxonomy (Marzano & Kendall, 2007)

**Source:** *The New Taxonomy of Educational Objectives.*

**6 levels of processing:**

```
Cognitive system:
  Level 1  Retrieval
  Level 2  Comprehension
  Level 3  Analysis
  Level 4  Knowledge Utilization
Metacognitive system:
  Level 5  Goal-setting, monitoring, etc.
Self-system:
  Level 6  Importance, efficacy, emotion, motivation
```

**3 knowledge domains:** Information / Mental procedures / Psychomotor procedures.

**SEACOW(r) mapping:** Activities + System (the self-system layer adds motivation / identity).

**Notable for:** adds *will* (self-system) above *thinking* — rare among taxonomies.

---

# Academic discipline classifications

## ACM Computing Classification System (CCS 2012)

**Source:** [dl.acm.org/ccs](https://dl.acm.org/ccs).

**Top-level branches:**

```
General and reference                  Networks
Hardware                                Software and its engineering
Computer systems organization           Theory of computation
Mathematics of computing                Information systems
Security and privacy                    Human-centered computing
Computing methodologies                  Applied computing
Social and professional topics
Proper nouns: People, technologies and companies
```

**SEACOW(r) mapping:** Object (subject-matter taxonomy of CS artifacts).

**Notable for:** **poly-hierarchical** — items can sit in multiple branches. The polyhierarchy showcase.

---

## AMS MSC2020 (Mathematics Subject Classification)

**Source:** [mathscinet.ams.org/msc/msc2020.html](https://mathscinet.ams.org/msc/msc2020.html).

**Top codes (selected):**

```
00  General and overarching topics
03  Mathematical logic and foundations
05  Combinatorics
11  Number theory
14  Algebraic geometry
26  Real functions
35  Partial differential equations
46  Functional analysis
53  Differential geometry
60  Probability theory
62  Statistics
65  Numerical analysis
68  Computer science
90  Operations research
97  Mathematics education
```

**SEACOW(r) mapping:** Object (subject taxonomy, three-level codes XX-YY-ZZZ).

**Notable for:** used by *Mathematical Reviews* and *Zentralblatt MATH*.

---

## JEL Classification (Journal of Economic Literature)

**Source:** [aeaweb.org/jel/guide/jel.php](https://www.aeaweb.org/jel/guide/jel.php).

**Top-level letters:**

```
A  General Economics                    J  Labor and Demographic
B  History of Economic Thought          K  Law and Economics
C  Math and Quantitative Methods         L  Industrial Organization
D  Microeconomics                       M  Business Administration
E  Macroeconomics                       N  Economic History
F  International                        O  Economic Development
G  Financial Economics                  P  Economic Systems
H  Public Economics                     Q  Agricultural / Natural Resource
I  Health, Education, Welfare           R  Urban / Rural / Real Estate
                                         Y  Miscellaneous
                                         Z  Other Special Topics
```

**SEACOW(r) mapping:** Object (subject taxonomy of econ literature).

**Notable for:** three-level letter+digit codes (e.g., G21 = Banks; Depository Institutions).

---

## PACS (Physics and Astronomy Classification Scheme, AIP, retired 2010)

**Top decades:**

```
00  General                              60  Condensed matter — structure
10  Elementary particles & fields        70  Condensed matter — electronic
20  Nuclear physics                      80  Interdisciplinary
30  Atomic & molecular                   90  Geophysics, astronomy, astrophysics
40  Electromagnetism, optics, etc.
50  Plasma physics
```

Six-digit codes (e.g., `03.65.Ud`).

**SEACOW(r) mapping:** Object (subject taxonomy, retired in favor of PhySH).

---

## arXiv subject categories

**Source:** [arxiv.org/category_taxonomy](https://arxiv.org/category_taxonomy).

**Top archives:**

```
astro-ph  cond-mat  cs (cs.AI, cs.CL, cs.CV, cs.LG, cs.RO, ...)
econ      eess      gr-qc
hep-ex    hep-lat   hep-ph     hep-th
math      nlin      nucl-ex    nucl-th
physics   q-bio     q-fin      quant-ph    stat
```

**SEACOW(r) mapping:** Object (preprint subject taxonomy).

**Notable for:** **crosslisting allowed** — one paper, multiple categories. Polyhierarchy in production.

---

## PhilPapers Categorization

**Source:** [philpapers.org/categories.html](https://philpapers.org/categories.html).

**Top-level:**

```
Metaphysics and Epistemology
Value Theory
Science, Logic, and Mathematics
History of Western Philosophy
Philosophical Traditions
Philosophy, Misc
Other Academic Areas
```

**SEACOW(r) mapping:** Object (philosophy subject taxonomy).

**Notable for:** community-curated, deeply nested (5+ levels).

---

# Narrative / creative structures

## Hero's Journey (Joseph Campbell, 1949 / Christopher Vogler 12-stage)

**Source:** *The Writer's Journey* (Vogler, 1992).

**12 stages:**

```
1.  Ordinary World            7.  Approach to the Inmost Cave
2.  Call to Adventure          8.  Ordeal
3.  Refusal of the Call        9.  Reward (Seizing the Sword)
4.  Meeting the Mentor        10.  The Road Back
5.  Crossing the Threshold    11.  Resurrection
6.  Tests, Allies, Enemies    12.  Return with the Elixir
```

**SEACOW(r) mapping:** Activities (sequenced phases of an Entity-protagonist's transformation).

**Notable for:** monomyth template behind most Hollywood scripts.

---

## Three-Act Structure

**Structure:** Act 1 Setup / Act 2 Confrontation / Act 3 Resolution.

**Visual** (with relative duration):

```
   ╔════════════╗ ╔══════════════════════════════════╗ ╔════════════╗
   ║  ACT 1      ║ ║              ACT 2                ║ ║  ACT 3      ║
   ║   Setup     ║ ║          Confrontation             ║ ║ Resolution ║
   ╚════════════╝ ╚══════════════════════════════════╝ ╚════════════╝
   ~25%             ~50%                                  ~25%
   │                 │                                     │
   │  inciting      │  midpoint           climax          │  denouement
   │  incident      │     ●                 ●             │       ●
   ▼                ▼                                     ▼
   ────────────────●──────●──────────────────●────────────────●─▶
                  IP1                       IP2
                  (1st plot point)         (2nd plot point)
```

**SEACOW(r) mapping:** Activities (coarse phase scaffold).

**Notable for:** smallest viable narrative skeleton.

---

## Save the Cat (Blake Snyder, 2005) — 15 beats

**Source:** *Save the Cat!*

**15 beats** (with rough page targets in a 110-page screenplay):

```
1.  Opening Image (p. 1)
2.  Theme Stated (~p. 5)
3.  Set-Up (p. 1-10)
4.  Catalyst (p. 12)
5.  Debate (p. 12-25)
6.  Break Into Two (p. 25)
7.  B Story (p. 30)
8.  Fun and Games (p. 30-55)
9.  Midpoint (p. 55)
10. Bad Guys Close In (p. 55-75)
11. All Is Lost (p. 75)
12. Dark Night of the Soul (p. 75-85)
13. Break Into Three (p. 85)
14. Finale (p. 85-110)
15. Final Image (p. 110)
```

**SEACOW(r) mapping:** Activities (beat-by-beat phase grid with page targets).

**Notable for:** numerically-anchored template; popularized analytically the rhythm of mainstream movies.

---

## Pixar's 22 Storytelling Rules (Emma Coats, 2011)

**Source:** Emma Coats' Twitter thread; widely re-published.

**Flagship #4 — the Story Spine:**

```
Once upon a time there was ___.
Every day, ___.
One day ___.
Because of that, ___.
Because of that, ___.
Until finally ___.
```

**SEACOW(r) mapping:** Activities (writing-craft heuristics, not a phase model).

**Notable for:** the Story Spine is one of the cleanest minimal narrative templates.

---

## Dan Harmon's Story Circle (8 steps)

**Source:** Dan Harmon (creator of *Community*, *Rick and Morty*).

**8 steps** (compressed monomyth, circular):

```
1. YOU      — character in zone of comfort
2. NEED     — something is wanted
3. GO       — into unfamiliar situation
4. SEARCH   — adapt to it
5. FIND     — get what you wanted
6. TAKE     — pay the price
7. RETURN   — back to familiar situation
8. CHANGE   — having changed
```

**SEACOW(r) mapping:** Activities (circular Hero's-Journey compression).

**Notable for:** TV-writers' shorthand, mapped to a clock face.

---

## Freytag's Pyramid (Gustav Freytag, 1863)

**5 phases:**

```
Exposition → Rising Action → Climax → Falling Action → Denouement
                                                       (Catastrophe)
```

**SEACOW(r) mapping:** Activities (5-phase dramatic arc).

**Notable for:** origin of the "climax" terminology in narratology.

---

## The 36 Dramatic Situations (Georges Polti, 1895)

**Selected (by number):**

```
1  Supplication         13 Enmity of Kin             25 Adultery
2  Deliverance           14 Rivalry of Kin            26 Crimes of Love
3  Crime Pursued         15 Murderous Adultery        27 Discovery of Dishonor
4  Vengeance for Kin     16 Madness                   28 Obstacles to Love
5  Pursuit               17 Fatal Imprudence          29 An Enemy Loved
6  Disaster              18 Involuntary Crimes        30 Ambition
7  Falling Prey          19 Slaying of Kin            31 Conflict with a God
8  Revolt                20 Self-Sacrifice for Ideal  32 Mistaken Jealousy
9  Daring Enterprise     21 Self-Sacrifice for Kin    33 Erroneous Judgment
10 Abduction              22 Sacrificed for Passion    34 Remorse
11 The Enigma             23 Sacrificing Loved Ones    35 Recovery of a Lost One
12 Obtaining              24 Rivalry Sup. vs Inf.      36 Loss of Loved Ones
```

**SEACOW(r) mapping:** relations (each is a relational tension between Entities).

**Notable for:** the most reductionist take on what stories *are* — relational tensions.

---

# Business process notation

## BPMN 2.0 (Object Management Group)

**Source:** [omg.org/spec/BPMN/2.0](https://www.omg.org/spec/BPMN/2.0/).

**Element categories:**

```
Flow Objects:        Events / Activities / Gateways
Connecting Objects:  Sequence Flow / Message Flow / Association
Swimlanes:           Pool / Lane
Artifacts:           Data Object / Group / Annotation
```

**SEACOW(r) mapping:** Activities + relations (process notation grammar).

**Notable for:** tool-portable process-modeling standard. Camunda, Bizagi, Signavio all consume BPMN XML.

---

## RACI matrix

**Source:** project-management folklore; codified in PMI literature.

**Four roles per task:**

```
R — Responsible    (does the work)
A — Accountable    (owns the outcome — exactly one per task)
C — Consulted      (input is sought before)
I — Informed       (told after)
```

**Format:** matrix of tasks × people, each cell holding R/A/C/I.

**SEACOW(r) mapping:** relations (Entity ↔ Activity assignment matrix).

**Notable variants:** **RASCI** (adds Support); **DACI** (Driver, Approver, Contributor, Informed); **RACI-VS** (Verifier, Signatory).

---

## Value Stream Map (Lean / Toyota)

**Source:** Rother & Shook, *Learning to See* (1999).

**Three flow layers:**

```
Material Flow:    raw → process → process → ship
                  (with takt-time / WIP / inventory boxes)

Information Flow: forecast → schedule → kanban signals → daily orders
                  (PUSH vs PULL arrows)

Timeline:         process times / wait times / lead time
                  (typically: lead time vastly exceeds process time)
```

**SEACOW(r) mapping:** Activities + relations (flow + timing overlay).

**Notable for:** the canonical lean diagram for diagnosing where time goes in a process.

---

# Philosophical / classical taxonomies

## Aristotelian Categories

**Source:** Aristotle, *Categories* (~350 BC).

**10 categories:**

```
Substance     Quantity     Quality     Relation     Place
Time          Position     State       Action       Affection
(Posture)     (Habit)                                (Passion)
```

**SEACOW(r) mapping:** Object / Entity ontology primitives.

**Notable for:** the original metaphysical classification scheme. Influenced every formal ontology that came after.

---

## Porphyrian Tree (Porphyry, 3rd century AD)

**Source:** *Isagoge* (Porphyry).

**Genus-differentia hierarchy:**

```
Substance
├── Corporeal               Incorporeal
    ├── Living body         Non-living body
        ├── Sensitive       Insensitive
            ├── Animal      (other living things)
                ├── Rational animal      Irrational animal
                    ├── Man              (other rational beings)
                        ├── Socrates     Plato     ...
```

**SEACOW(r) mapping:** Entity (the genus-differentia hierarchy archetype).

**Notable for:** the prototype of every taxonomic classification ever drawn. Linnaean biology, Library of Congress Classification, OOP class hierarchies all descend from this shape.

---

## Kant's Categories (*Critique of Pure Reason*, 1781)

**Source:** Kant, *Kritik der reinen Vernunft*.

**4 headings × 3 each = 12:**

```
Quantity:   Unity / Plurality / Totality
Quality:    Reality / Negation / Limitation
Relation:   Inherence and Subsistence /
            Causality and Dependence /
            Community (reciprocity)
Modality:   Possibility–Impossibility /
            Existence–Non-existence /
            Necessity–Contingency
```

**SEACOW(r) mapping:** Entity (a-priori conceptual primitives).

**Notable for:** Kant's argument is that these aren't *empirical* categories — they're the conceptual structure the mind imposes on experience.

---

## Five Aggregates / Skandhas (Buddhism)

**Source:** Pali Canon; *Khandha-saṃyutta*.

**5 constituents of personhood:**

```
Form (rūpa)               — physical body / matter
Sensation (vedanā)        — feeling tone (pleasant / unpleasant / neutral)
Perception (saññā)        — recognition / cognition
Mental formations         — volition, intent, mental constructions
  (saṅkhāra)
Consciousness (viññāṇa)   — awareness
```

**SEACOW(r) mapping:** Entity decomposition (constituents of a "self").

**Notable for:** unusual among classification schemes — explicitly *anti-foundational* (the doctrine is that there's no enduring self that owns these aggregates).

---

## Confucian Five Relationships (五倫)

**Source:** *Mencius* and the Confucian classics.

**5 normative dyads:**

```
Ruler – Subject                    Father – Son
Husband – Wife                     Elder Brother – Younger Brother
Friend – Friend
```

**SEACOW(r) mapping:** relations (social-role dyads).

**Notable for:** an Entity-pair-centric view of social structure — relationships, not individuals, are the unit.

---

# See also

- [`../INDEXES/by-comparison.md`](../INDEXES/by-comparison.md) — compact one-row-per-framework matrix.
- [`../04-comparisons/`](../04-comparisons/) — per-framework deep-dive pages (stubs, will be filled in).
- [`../05-deep-dives/knowledge-organization.md`](../05-deep-dives/knowledge-organization.md) — broader landscape with external links.
- [`../05-deep-dives/ideas-for-knowledge-organization.md`](../05-deep-dives/ideas-for-knowledge-organization.md) — your own brainstorm with e-ACCESS, EJK, time-based structures.
- [`../ROADMAP.md`](../ROADMAP.md) — frameworks queued for future addition (still some! — Wardley map deep-dive, IBIS dialogue-mapping, more cybersecurity standards, NIST SP 800-171, FedRAMP, TLS Maturity Model, ATT&CK for ICS / for Mobile / for Containers, OWASP MASVS, OWASP SAMM, BSIMM, OWASP API Top 10, etc.).
