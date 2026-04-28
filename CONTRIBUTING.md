# Contributing

This repo is a curated knowledge base. Contributions are welcome — but please
keep the editorial standard high: prefer **cooled, finished** content on `main`.

## Where things go

- **Concepts / canonical definitions** — `01-framework/`. Edit existing pages first; new pages need a clear reason.
- **Tools / skills / agents / plugin docs** — `02-tools/`. Tools applying SEACOW(r), not theory.
- **Examples** — `03-examples/`. Worked instances. New case studies welcome under `03-examples/case-studies/`.
- **Comparisons** — `04-comparisons/`. SEACOW(r) vs other organizational framework.
- **Long-form** — `05-deep-dives/`. Theory or decision matrices that don't fit elsewhere.
- **Platform-specific** — `06-applications/`. "SEACOW(r) for X."

The `INDEXES/` files re-curate existing content for different audiences. Don't
add new primary content there.

## Editorial standard

- Every claim about the framework should trace back to `01-framework/`.
- Every example should reference the framework component it illustrates.
- Comparisons should be **fair** — describe the other framework on its own terms first, then map to SEACOW(r).

## Style

- See [AGENTS.md](AGENTS.md) for technical conventions (links, frontmatter, kebab-case, numbered folders).
- Voice: precise, opinionated, but not preachy. Show your work.

## Half-baked ideas welcome — but as issues, not PRs

This repo deliberately omits a `00-inbox/` "warm zone." Raw observations,
counter-examples, and "did anyone consider X" should land as issues; maintainers
will cool them into deep-dives.

## Commits

- Subject form: `area: imperative subject`. Example: `04-comparisons: stub vs-johnny-decimal page`.
- **No AI attribution** — never include `Co-Authored-By: Claude`, `Generated with`, or any AI/LLM co-author footer. Commit as the human contributor only.

## License

By contributing, you agree your contributions are released under [CC BY 4.0](LICENSE).
