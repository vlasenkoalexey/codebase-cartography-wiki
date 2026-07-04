---
slug: codegraph
commit: f8cdbe3c6748ef3f93d2f436ee89b79a05789191
scip_tool: scip-python
updated: 2026-07-04
---

# codegraph internals wiki

Generated, grounded wiki. Start from a concept (or an area); drill into cited symbols.
The commit pin above is the single source version for every page in this silo.

**Start here → [Overview](overview.md)** — the whole system in one page (main concepts + core diagrams + a map of the wiki).

## Concepts (deep)
| Concept | Page | Status |
|---|---|---|
| db-queries.ts | [db-queries.ts](concepts/db-queries.ts.md) | fresh |
| db-sqlite-adapter.ts | [db-sqlite-adapter.ts](concepts/db-sqlite-adapter.ts.md) | fresh |
| directory.ts | [directory.ts](concepts/directory.ts.md) | fresh |
| extraction-function-ref.ts | [extraction-function-ref.ts](concepts/extraction-function-ref.ts.md) | fresh |
| extraction-index.ts | [extraction-index.ts](concepts/extraction-index.ts.md) | fresh |
| extraction-parse-pool.ts | [extraction-parse-pool.ts](concepts/extraction-parse-pool.ts.md) | fresh |
| extraction-tree-sitter-helpers.ts | [extraction-tree-sitter-helpers.ts](concepts/extraction-tree-sitter-helpers.ts.md) | fresh |
| extraction-tree-sitter-types.ts | [extraction-tree-sitter-types.ts](concepts/extraction-tree-sitter-types.ts.md) | fresh |
| extraction-tree-sitter.ts | [extraction-tree-sitter.ts](concepts/extraction-tree-sitter.ts.md) | fresh |
| index.ts | [index.ts](concepts/index.ts.md) | fresh |
| installer-targets-shared.ts | [installer-targets-shared.ts](concepts/installer-targets-shared.ts.md) | fresh |
| installer-targets-types.ts | [installer-targets-types.ts](concepts/installer-targets-types.ts.md) | fresh |
| mcp-daemon.ts | [mcp-daemon.ts](concepts/mcp-daemon.ts.md) | fresh |
| mcp-query-pool.ts | [mcp-query-pool.ts](concepts/mcp-query-pool.ts.md) | fresh |
| mcp-tools.ts | [mcp-tools.ts](concepts/mcp-tools.ts.md) | fresh |
| mcp-transport.ts | [mcp-transport.ts](concepts/mcp-transport.ts.md) | fresh |
| resolution-callback-synthesizer.ts | [resolution-callback-synthesizer.ts](concepts/resolution-callback-synthesizer.ts.md) | fresh |
| resolution-index.ts | [resolution-index.ts](concepts/resolution-index.ts.md) | fresh |
| resolution-types.ts | [resolution-types.ts](concepts/resolution-types.ts.md) | fresh |
| sync-watcher.ts | [sync-watcher.ts](concepts/sync-watcher.ts.md) | fresh |
| telemetry-index.ts | [telemetry-index.ts](concepts/telemetry-index.ts.md) | fresh |
| types.ts | [types.ts](concepts/types.ts.md) | fresh |
| utils.ts | [utils.ts](concepts/utils.ts.md) | fresh |
| web-tree-sitter.d.ts | [web-tree-sitter.d.ts](concepts/web-tree-sitter.d.ts.md) | fresh |

## Doc-derived concepts
Concepts extracted from the project's own docs (README / `docs/`), grounded to the symbol catalog. The source docs stay in place.
- [adaptive-explore-sizing](doc-concepts/adaptive-explore-sizing.md)
- [agent-adoption](doc-concepts/agent-adoption.md)
- [chained-call-resolution](doc-concepts/chained-call-resolution.md)
- [cross-language-native-bridging](doc-concepts/cross-language-native-bridging.md)
- [dynamic-dispatch-coverage](doc-concepts/dynamic-dispatch-coverage.md)
- [function-ref-capture](doc-concepts/function-ref-capture.md)
- [init-and-autosync](doc-concepts/init-and-autosync.md)
- [local-first-grounding](doc-concepts/local-first-grounding.md)
- [mcp-tool-surface](doc-concepts/mcp-tool-surface.md)
- [template-markup-parsing](doc-concepts/template-markup-parsing.md)
- [value-reference-edges](doc-concepts/value-reference-edges.md)

## Coverage
Two tiers: **concept pages** explain mechanisms deeply (selective); **module
catalogs** represent the rest so the whole repo is navigable. Coverage is a
set-difference over the SCIP symbol table, not a graph walk — every documentable
symbol is enumerated and represented.

- documentable symbols: **3674** across 152 modules
- deep (concept pages): **668** (18.2%)
- catalog-only: **3006**
- represented total: **3674** (100.0%)
- classes represented: **227/227**

See [`catalog/`](catalog/) for the generated per-module structural index.

## Provenance
`extracted` = from SCIP / source. `inferred` = LLM judgment, treat as such.
Design-intent dynamics are labeled; none are runtime-measured (no L4 pass run).
Callers/callees are reference-scoped (SCIP has no call role), labeled "calls/refs".
