---
slug: tree-sitter-analyzer
commit: c5a4ae0fc7f5a2d266f877f542a8625e1944e93c
scip_tool: scip-python
updated: 2026-07-04
---

# tree-sitter-analyzer internals wiki

Generated, grounded wiki. Start from a concept (or an area); drill into cited symbols.
The commit pin above is the single source version for every page in this silo.

**Start here → [Overview](overview.md)** — the whole system in one page (main concepts + core diagrams + a map of the wiki).

## Concepts (deep)
| Concept | Page | Status |
|---|---|---|
| tree_sitter_analyzer-ast_cache | [tree_sitter_analyzer-ast_cache](concepts/tree_sitter_analyzer-ast_cache.md) | fresh |
| tree_sitter_analyzer-ast_diff | [tree_sitter_analyzer-ast_diff](concepts/tree_sitter_analyzer-ast_diff.md) | fresh |
| tree_sitter_analyzer-call_graph | [tree_sitter_analyzer-call_graph](concepts/tree_sitter_analyzer-call_graph.md) | fresh |
| tree_sitter_analyzer-core-parser | [tree_sitter_analyzer-core-parser](concepts/tree_sitter_analyzer-core-parser.md) | fresh |
| tree_sitter_analyzer-core-request | [tree_sitter_analyzer-core-request](concepts/tree_sitter_analyzer-core-request.md) | fresh |
| tree_sitter_analyzer-formatters-toon_encoder | [tree_sitter_analyzer-formatters-toon_encoder](concepts/tree_sitter_analyzer-formatters-toon_encoder.md) | fresh |
| tree_sitter_analyzer-graph-edge_store | [tree_sitter_analyzer-graph-edge_store](concepts/tree_sitter_analyzer-graph-edge_store.md) | fresh |
| tree_sitter_analyzer-languages-csharp_plugin | [tree_sitter_analyzer-languages-csharp_plugin](concepts/tree_sitter_analyzer-languages-csharp_plugin.md) | fresh |
| tree_sitter_analyzer-languages-scala_plugin | [tree_sitter_analyzer-languages-scala_plugin](concepts/tree_sitter_analyzer-languages-scala_plugin.md) | fresh |
| tree_sitter_analyzer-legacy_table_formatter | [tree_sitter_analyzer-legacy_table_formatter](concepts/tree_sitter_analyzer-legacy_table_formatter.md) | fresh |
| tree_sitter_analyzer-mcp-server | [tree_sitter_analyzer-mcp-server](concepts/tree_sitter_analyzer-mcp-server.md) | fresh |
| tree_sitter_analyzer-mcp-tools-base_tool | [tree_sitter_analyzer-mcp-tools-base_tool](concepts/tree_sitter_analyzer-mcp-tools-base_tool.md) | fresh |
| tree_sitter_analyzer-mcp-tools-facade_tool | [tree_sitter_analyzer-mcp-tools-facade_tool](concepts/tree_sitter_analyzer-mcp-tools-facade_tool.md) | fresh |
| tree_sitter_analyzer-mcp-tools-read_partial_tool | [tree_sitter_analyzer-mcp-tools-read_partial_tool](concepts/tree_sitter_analyzer-mcp-tools-read_partial_tool.md) | fresh |
| tree_sitter_analyzer-mcp-utils-error_handler | [tree_sitter_analyzer-mcp-utils-error_handler](concepts/tree_sitter_analyzer-mcp-utils-error_handler.md) | fresh |
| tree_sitter_analyzer-models-base | [tree_sitter_analyzer-models-base](concepts/tree_sitter_analyzer-models-base.md) | fresh |
| tree_sitter_analyzer-models-markup_models | [tree_sitter_analyzer-models-markup_models](concepts/tree_sitter_analyzer-models-markup_models.md) | fresh |
| tree_sitter_analyzer-models-result | [tree_sitter_analyzer-models-result](concepts/tree_sitter_analyzer-models-result.md) | fresh |
| tree_sitter_analyzer-models-sql_models | [tree_sitter_analyzer-models-sql_models](concepts/tree_sitter_analyzer-models-sql_models.md) | fresh |
| tree_sitter_analyzer-plugins-base | [tree_sitter_analyzer-plugins-base](concepts/tree_sitter_analyzer-plugins-base.md) | fresh |
| tree_sitter_analyzer-plugins-manager | [tree_sitter_analyzer-plugins-manager](concepts/tree_sitter_analyzer-plugins-manager.md) | fresh |
| tree_sitter_analyzer-security-validator | [tree_sitter_analyzer-security-validator](concepts/tree_sitter_analyzer-security-validator.md) | fresh |
| tree_sitter_analyzer-uml_export | [tree_sitter_analyzer-uml_export](concepts/tree_sitter_analyzer-uml_export.md) | fresh |
| tree_sitter_analyzer-utils-logging | [tree_sitter_analyzer-utils-logging](concepts/tree_sitter_analyzer-utils-logging.md) | fresh |

## Doc-derived concepts
Concepts extracted from the project's own docs (README / `docs/`), grounded to the symbol catalog. The source docs stay in place.
- [cross-language-miswire-benchmark](doc-concepts/cross-language-miswire-benchmark.md)
- [mcp-facade-and-verdict-envelopes](doc-concepts/mcp-facade-and-verdict-envelopes.md)
- [supported-language-tiers](doc-concepts/supported-language-tiers.md)
- [toon-output-format](doc-concepts/toon-output-format.md)

## Coverage
Two tiers: **concept pages** explain mechanisms deeply (selective); **module
catalogs** represent the rest so the whole repo is navigable. Coverage is a
set-difference over the SCIP symbol table, not a graph walk — every documentable
symbol is enumerated and represented.

- documentable symbols: **43362** across 1883 modules
- deep (concept pages): **481** (1.1%)
- catalog-only: **42881**
- represented total: **43362** (100.0%)
- classes represented: **4881/4881**

See [`catalog/`](catalog/) for the generated per-module structural index.

## Provenance
`extracted` = from SCIP / source. `inferred` = LLM judgment, treat as such.
Design-intent dynamics are labeled; none are runtime-measured (no L4 pass run).
Callers/callees are reference-scoped (SCIP has no call role), labeled "calls/refs".
