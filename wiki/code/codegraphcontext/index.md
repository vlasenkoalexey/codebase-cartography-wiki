---
slug: codegraphcontext
commit: 8bd1a8f7214a3bdb2788106a6949c60dd83dd5be
scip_tool: scip-python
updated: 2026-07-04
---

# codegraphcontext internals wiki

Generated, grounded wiki. Start from a concept (or an area); drill into cited symbols.
The commit pin above is the single source version for every page in this silo.

**Start here → [Overview](overview.md)** — the whole system in one page (main concepts + core diagrams + a map of the wiki).

## Concepts (deep)
| Concept | Page | Status |
|---|---|---|
| codegraphcontext-cli-cli_helpers | [codegraphcontext-cli-cli_helpers](concepts/codegraphcontext-cli-cli_helpers.md) | fresh |
| codegraphcontext-cli-config_manager | [codegraphcontext-cli-config_manager](concepts/codegraphcontext-cli-config_manager.md) | fresh |
| codegraphcontext-cli-main | [codegraphcontext-cli-main](concepts/codegraphcontext-cli-main.md) | fresh |
| codegraphcontext-core-database_embedded_kuzu | [codegraphcontext-core-database_embedded_kuzu](concepts/codegraphcontext-core-database_embedded_kuzu.md) | fresh |
| codegraphcontext-core-jobs | [codegraphcontext-core-jobs](concepts/codegraphcontext-core-jobs.md) | fresh |
| codegraphcontext-server | [codegraphcontext-server](concepts/codegraphcontext-server.md) | fresh |
| codegraphcontext-tools-code_finder | [codegraphcontext-tools-code_finder](concepts/codegraphcontext-tools-code_finder.md) | fresh |
| codegraphcontext-tools-graph_builder | [codegraphcontext-tools-graph_builder](concepts/codegraphcontext-tools-graph_builder.md) | fresh |
| codegraphcontext-tools-indexing-persistence-utils | [codegraphcontext-tools-indexing-persistence-utils](concepts/codegraphcontext-tools-indexing-persistence-utils.md) | fresh |
| codegraphcontext-tools-indexing-persistence-writer | [codegraphcontext-tools-indexing-persistence-writer](concepts/codegraphcontext-tools-indexing-persistence-writer.md) | fresh |
| codegraphcontext-tools-indexing-resolution-calls | [codegraphcontext-tools-indexing-resolution-calls](concepts/codegraphcontext-tools-indexing-resolution-calls.md) | fresh |
| codegraphcontext-tools-languages-elisp | [codegraphcontext-tools-languages-elisp](concepts/codegraphcontext-tools-languages-elisp.md) | fresh |
| codegraphcontext-tools-languages-kotlin | [codegraphcontext-tools-languages-kotlin](concepts/codegraphcontext-tools-languages-kotlin.md) | fresh |
| codegraphcontext-tools-languages-typescript | [codegraphcontext-tools-languages-typescript](concepts/codegraphcontext-tools-languages-typescript.md) | fresh |
| codegraphcontext-tools-scip_pb2 | [codegraphcontext-tools-scip_pb2](concepts/codegraphcontext-tools-scip_pb2.md) | fresh |
| codegraphcontext-utils-debug_log | [codegraphcontext-utils-debug_log](concepts/codegraphcontext-utils-debug_log.md) | fresh |
| codegraphcontext-utils-tree_sitter_manager | [codegraphcontext-utils-tree_sitter_manager](concepts/codegraphcontext-utils-tree_sitter_manager.md) | fresh |
| extensions-vscode-src-mcp-client.ts | [extensions-vscode-src-mcp-client.ts](concepts/extensions-vscode-src-mcp-client.ts.md) | fresh |
| extensions-vscode-src-mcp-service.ts | [extensions-vscode-src-mcp-service.ts](concepts/extensions-vscode-src-mcp-service.ts.md) | fresh |
| extensions-vscode-src-types-cgc.ts | [extensions-vscode-src-types-cgc.ts](concepts/extensions-vscode-src-types-cgc.ts.md) | fresh |
| website-src-components-CodeGraphViewer.tsx | [website-src-components-CodeGraphViewer.tsx](concepts/website-src-components-CodeGraphViewer.tsx.md) | fresh |
| website-src-components-PRReviewer.tsx | [website-src-components-PRReviewer.tsx](concepts/website-src-components-PRReviewer.tsx.md) | fresh |
| website-src-lib-pr-mock-data.ts | [website-src-lib-pr-mock-data.ts](concepts/website-src-lib-pr-mock-data.ts.md) | fresh |
| website-src-lib-repo-provider.ts | [website-src-lib-repo-provider.ts](concepts/website-src-lib-repo-provider.ts.md) | fresh |

## Coverage
Two tiers: **concept pages** explain mechanisms deeply (selective); **module
catalogs** represent the rest so the whole repo is navigable. Coverage is a
set-difference over the SCIP symbol table, not a graph walk — every documentable
symbol is enumerated and represented.

- documentable symbols: **5482** across 373 modules
- deep (concept pages): **700** (12.8%)
- catalog-only: **4782**
- represented total: **5482** (100.0%)
- classes represented: **578/578**

See [`catalog/`](catalog/) for the generated per-module structural index.

## Provenance
`extracted` = from SCIP / source. `inferred` = LLM judgment, treat as such.
Design-intent dynamics are labeled; none are runtime-measured (no L4 pass run).
Callers/callees are reference-scoped (SCIP has no call role), labeled "calls/refs".
