# 01 — Framework

The canonical concept layer. The **definitions** of SEACOW(r) live here. Everything else in the repo cites these pages.

| Read | What it covers |
|---|---|
| [meta-framework.md](meta-framework.md) | The full canonical definition. SEA(COWr) overview, framework breakdown, application notes, "Isn't PARA enough?" |
| [components/](components/) | One page per component (S / E / A / C / O / W / r) |
| [rules.md](rules.md) | The rule-setting language. Gain-not-lose, nesting limits, restrictions on activity stacking. |
| [design-principles.md](design-principles.md) | Cross-cutting principles: LATCH, polyhierarchy, separating process from content. |

## When to add a page here

- A new SEACOW(r) component (only if the framework genuinely changes)
- A clarification of an existing concept that's too long for an in-line note
- A formalization of a rule that's been informally applied in `03-examples/`

Don't add platform-specific content here — that goes in `06-applications/`.
Don't add comparisons here — that goes in `04-comparisons/`.
