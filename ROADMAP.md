# Roadmap

Things this repo will grow into. Not commitments — a parking lot.

## Frameworks not yet in the gallery

The [framework gallery](03-examples/framework-gallery.md) covers **~110+ frameworks**. The ones below are still queued.

### Cybersecurity / GRC (more depth)

- **NIST SP 800-171** — protecting Controlled Unclassified Information (CUI).
- **NIST SP 800-218 (SSDF)** — Secure Software Development Framework.
- **FedRAMP** — controls baselines (Low, Moderate, High, LI-SaaS).
- **HITRUST CSF** — healthcare-focused control framework that crosswalks to many others.
- **MITRE ATT&CK for ICS / for Mobile / for Containers / for Cloud** — domain variants.
- **OWASP MASVS** (Mobile Application Security Verification Standard).
- **OWASP SAMM** (Software Assurance Maturity Model) — 5 business functions × 3 levels.
- **BSIMM** (Building Security In Maturity Model) — observed-practice equivalent of SAMM.
- **OWASP API Top 10** (current edition).
- **NIST Zero Trust Architecture (SP 800-207)** — 7 tenets.
- **CISA Zero Trust Maturity Model** — 5 pillars × 4 maturity levels.
- **Australian ASD Essential Eight** — 8 mitigation strategies × 3 maturity levels.
- **UK Cyber Essentials** — 5 technical control areas.
- **CMMC 2.0** — DoD Cybersecurity Maturity Model Certification.

### Engineering / dev practices

- **Kanban** — to-do / doing / done columns + WIP limits + class of service. (Currently only mentioned in passing.)
- **Scrum** — Sprint / Backlog / Increment / 5 events / 3 artifacts.
- **DORA Four Keys** — deployment frequency, lead time, change failure rate, MTTR.
- **SPACE framework** — developer productivity (Satisfaction, Performance, Activity, Communication, Efficiency).
- **Team Topologies** — four team types (Stream-aligned, Enabling, Complicated-Subsystem, Platform).

### Data / metadata

- **OASIS DITA** — Darwin Information Typing Architecture for technical content.
- **DocBook** — documentation XML schema.
- **JATS** (Journal Article Tag Suite, NISO Z39.96).

### Visual / spatial

- **Mind maps** (Tony Buzan) — radial idea expansion.
- **Concept maps** (Joseph Novak) — propositions linked by labeled edges.
- **Knowledge graphs** (RDF/OWL property-graph) — formal semantic linking.
- **Sketchnoting** (Mike Rohde / Sunni Brown).

### Personal / domestic

- **Kondo's joy-test** as a SEACOW(r) Capture-vs-Archive rule (already in gallery; could deserve its own deep-dive).
- **Inbox Zero** (Merlin Mann) as a Capture-discipline rule.
- **One-Touch / Two-Minute** as Capture rules.
- **GTD weekly review** as a process artifact.

### Niche / historical

- **Vannevar Bush's Memex** — the prehistoric link-based hypertext idea.
- **Doug Engelbart's NLS / Augment** — outliner ancestry.
- **Ted Nelson's Xanadu** — bidirectional links and transclusion.
- **Project Cybersyn** — Stafford Beer's Viable System Model applied to economic management.
- **Beer's Viable System Model (VSM)** itself — five subsystems for organizational viability.

### Knowledge representation (formal)

- **First-order logic ontology forms.**
- **Description Logic (DL).**
- **OWL profiles** (OWL 2 EL, OWL 2 QL, OWL 2 RL).
- **RDF triple stores and SPARQL.**

### Domain-specific (other)

- **GS1 product classifications** (UPC / GTIN, GPC).
- **NAICS / SIC codes** for industry classification.
- **ICD-10 / ICD-11** medical diagnosis codes.
- **CPT codes** for medical procedures.
- **GAAP / IFRS** accounting taxonomies.
- **XBRL** for financial reporting.

---

## Repo structural follow-ups

- **`MIGRATION_LOG.md`** — track the last-synced commit per file from cyberbase upstream, so editorial drift is auditable.
- **GitHub Pages or static site** (Astro / Starlight or MkDocs) — better search UX than browsing GitHub markdown. Especially valuable now that the gallery has 110+ frameworks.
- **Obsidian Publish parity** — verify all frontmatter still works for the user's `cyberbase`-style publish flow.
- **Diagrams** — populate `assets/diagrams/` with SVGs of:
  - The SEACOW(r) flow (Capture → Work → Output, with Entity / System framing).
  - The hierarchy-vs-graph tension diagram.
  - PARA / Zettelkasten / SEACOW(r) Venn / mapping overlays.
  - The temperature gradient (00-inbox → 04-archive).
  - The framework-family taxonomy that the gallery describes.
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
- **Index regeneration** — the `INDEXES/by-comparison.md` matrix is small relative to the gallery now; consider regenerating it as a more comprehensive table.

---

## Possible new top-level pages

- **`07-anti-patterns/`** — common ways SEACOW(r) instantiations go wrong. (Currently anti-patterns are scattered across component pages.)
- **`08-evolution/`** — how a SEACOW(r) instantiation matures over time (start minimal, observe, refactor). Currently mentioned in `01-framework/design-principles.md` but deserves its own treatment.
- **`09-glossary/`** — single-source glossary of every term used across the gallery (entry per term with primary section pointer).

---

## Editorial / hygiene

- Audit external links in the gallery quarterly (especially Forte Labs URLs — several were 404 during research).
- Add anchor links in long pages so the INDEXES can deep-link into specific sections.
- Consider whether some compact framework entries should be promoted to dedicated `04-comparisons/vs-X.md` pages once they're frequently referenced.
- Decide whether to fork off a separate "exhaustive registry" page (current gallery) vs a curated "essentials" page for newcomers.

---

*The roadmap is live — modify it freely.*
