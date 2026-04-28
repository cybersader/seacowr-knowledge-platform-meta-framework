# Roadmap

Things this repo will grow into. Not commitments — a parking lot.

## Frameworks not yet in the gallery

The [framework gallery](03-examples/framework-gallery.md) covers ~30 organizational frameworks. The ones below are queued for future research / addition:

### PKM and process

- **GTD** (Getting Things Done — David Allen) — the contexts (`@office`, `@calls`), the weekly review, the 2-minute rule. Maps to SEACOW(r) Work + relation.
- **GTD Horizons of Focus** — 50K (life), 40K (vision), 30K (goals), 20K (areas), 10K (projects), runway (actions). Vertical scope hierarchy.
- **Bullet Journal** (Ryder Carroll) — daily / monthly / future logs + collections + migration. Originally analog; portable to digital.
- **OKRs** (Objectives & Key Results) — quarterly goal-tracking. Hierarchical: organization → team → individual.
- **Eisenhower Matrix** — urgent × important 2x2. Filtering rule, not a folder scheme.
- **Kanban** — to-do / doing / done columns. Process visualization.
- **Forte's CODE** — already mentioned in gallery, but deserves its own deep-dive page.
- **Forte's "Just-In-Time PM"** — lighter-weight Project handling.
- **Andy Matuschak evergreen-notes principles** — already in gallery; full deep-dive worth doing.
- **Roam-style daily notes flow** — date as primary axis; backlinks emerge.
- **IBIS** (Issue-Based Information System) — Issue → Position → Argument. Specifically for collaborative reasoning.
- **Cynefin framework** — clear / complicated / complex / chaotic / disorder. Sense-making for *kind of problem* you have.

### Hierarchical / formal

- **schema.org / Dublin Core / FOAF / SKOS** — metadata vocabularies. Adjacent to Library Science but for the open web.
- **Bates numbering** — legal-discovery sequential ID system.
- **IDEF** family (IDEF0, IDEF1X, IDEF3) — DoD-origin process modeling.
- **OASIS metadata standards** (DITA, DocBook).
- **ISO 25964** (information-and-documentation thesauri).
- **EAD (Encoded Archival Description)** — archival finding aids.
- **MARC 21** — bibliographic records.

### Visual / spatial

- **Mind maps** (Tony Buzan).
- **Concept maps** (Joseph Novak).
- **Knowledge graphs** (formal RDF/OWL plus property graphs / Neo4j-style).
- **Faceted classification** in modern systems (Notion properties, Airtable views).

### Domain-specific

- **DAMA-DMBOK** for data management organization.
- **TOGAF / ArchiMate** for enterprise architecture artifacts.
- **C4 Model** for software architecture documentation.
- **OWASP ASVS / OWASP Top 10** mapping (would complement the Crosswalker examples).
- **CSA CCM** (Cloud Controls Matrix).

### Personal / domestic

- **KonMari** — for physical organization; interesting because it's anti-categorization (sort by category, not location).
- **Tiago Forte's "PARA in real life"** — extending PARA to physical filing cabinets.
- **Marie Kondo's joy-test** as a SEACOW(r) Capture-vs-Archive rule.

### Older / niche

- **"Lifehacker's Inbox-zero"** as a Capture rule.
- **Smart Notes** (Cal Newport's "deep work" frame on Zettelkasten).
- **Rakhshani-style commonplace book** — pre-digital atomic-note tradition.
- **Vannevar Bush's Memex** — the prehistoric link-based system.

---

## Repo structural follow-ups

- **`MIGRATION_LOG.md`** — track the last-synced commit per file from cyberbase upstream, so editorial drift is auditable.
- **GitHub Pages or static site** (Astro/Starlight or MkDocs) — better search UX than browsing GitHub markdown.
- **Obsidian Publish parity** — make sure all frontmatter still works for the user's `cyberbase`-style publish flow.
- **Diagrams** — populate `assets/diagrams/` with SVGs of:
  - The SEACOW(r) flow (Capture → Work → Output, with Entity / System framing).
  - The hierarchy-vs-graph tension diagram.
  - PARA / Zettelkasten / SEACOW(r) Venn / mapping overlays.
  - The temperature gradient (00-inbox → 04-archive).
- **Rule-pack examples for [obsidian-folder-tag-sync](https://github.com/cybersader/obsidian-folder-tag-sync)** — concrete rule-packs that translate each major framework into a folder-tag bridge.
- **Worked-example case studies** under `03-examples/case-studies/`:
  - `personal-research-vault.md`
  - `compliance-team-fileshare.md`
  - `student-homework-folder.md`
  - `software-product-team-repo.md`
  - `family-shared-drive.md`
- **Comparison-page completion** — `04-comparisons/*.md` are stubs; flesh out vs-para, vs-zettelkasten, vs-johnny-decimal, vs-latch with full worked examples.
- **`02-tools/skills/knowledge-curator/`** — copy in the public version of the temperature-gradient skill.
- **Crosswalker integration page** under `02-tools/plugins/crosswalker/` — docs for using Crosswalker to import compliance frameworks into a SEACOW(r)-organized vault.

---

## Possible new top-level pages

- **`07-anti-patterns/`** — common ways SEACOW(r) instantiations go wrong. (Currently anti-patterns are scattered across component pages.)
- **`08-evolution/`** — how a SEACOW(r) instantiation matures over time (start minimal, observe, refactor). Currently mentioned in `01-framework/design-principles.md` but deserves its own treatment.

---

## Editorial / hygiene

- Reduce duplication between `framework-gallery.md`, the `INDEXES/`, and the `04-comparisons/` stubs once the gallery has stabilized.
- Add anchor links in long pages so the INDEXES can deep-link into specific sections.
- Audit external links periodically (forum URLs especially).

---

*If you want one of these next, open an issue or just add a section. The roadmap is live — modify it freely.*
