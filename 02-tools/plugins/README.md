# Plugins

Plugin documentation for tools that **implement or enable** SEACOW(r). The
canonical example is `dynamic-tags-folders` (folder ↔ tag bridging), which
makes polyhierarchy practical on a hierarchical file system.

| Plugin | Status | Purpose |
|---|---|---|
| [dynamic-tags-folders/](dynamic-tags-folders/) | Active development at [cybersader/obsidian-folder-tag-sync](https://github.com/cybersader/obsidian-folder-tag-sync) | Bidirectional folder ↔ tag mapping with regex transformation rules. Solves the strict-hierarchy problem. |

## Why plugins matter for SEACOW(r)

SEACOW(r) treats the **System** component as a constraint set. Plugins extend
that constraint set — what the system *affords*. A vault with
`obsidian-folder-tag-sync` installed has a different SEACOW(r) profile than
one without: polyhierarchy becomes practical, and the rules-vocabulary can
include "this folder is also tagged X."

When documenting a plugin here, include:

1. The **System** affordance it adds.
2. Which SEACOW(r) **components** the plugin most affects.
3. A worked example showing it in use.
4. Limitations / known issues.
