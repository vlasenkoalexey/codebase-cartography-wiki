---
slug: claude-context
commit: 627eb2be339723926d5b468698a8f5cc0da21167
scip_tool: scip-python
updated: 2026-07-04
---

# claude-context internals wiki

Generated, grounded wiki. Start from a concept (or an area); drill into cited symbols.
The commit pin above is the single source version for every page in this silo.

**Start here → [Overview](overview.md)** — the whole system in one page (main concepts + core diagrams + a map of the wiki).

## Concepts (deep)
| Concept | Page | Status |
|---|---|---|
| packages-chrome-extension-src-background.ts | [packages-chrome-extension-src-background.ts](concepts/packages-chrome-extension-src-background.ts.md) | fresh |
| packages-chrome-extension-src-config-milvusConfig.ts | [packages-chrome-extension-src-config-milvusConfig.ts](concepts/packages-chrome-extension-src-config-milvusConfig.ts.md) | fresh |
| packages-chrome-extension-src-milvus-chromeMilvusAdapter.ts | [packages-chrome-extension-src-milvus-chromeMilvusAdapter.ts](concepts/packages-chrome-extension-src-milvus-chromeMilvusAdapter.ts.md) | fresh |
| packages-chrome-extension-src-storage-indexedRepoManager.ts | [packages-chrome-extension-src-storage-indexedRepoManager.ts](concepts/packages-chrome-extension-src-storage-indexedRepoManager.ts.md) | fresh |
| packages-chrome-extension-src-stubs-milvus-vectordb-stub.ts | [packages-chrome-extension-src-stubs-milvus-vectordb-stub.ts](concepts/packages-chrome-extension-src-stubs-milvus-vectordb-stub.ts.md) | fresh |
| packages-core-src-context.ts | [packages-core-src-context.ts](concepts/packages-core-src-context.ts.md) | fresh |
| packages-core-src-embedding-base-embedding.ts | [packages-core-src-embedding-base-embedding.ts](concepts/packages-core-src-embedding-base-embedding.ts.md) | fresh |
| packages-core-src-embedding-gemini-embedding.ts | [packages-core-src-embedding-gemini-embedding.ts](concepts/packages-core-src-embedding-gemini-embedding.ts.md) | fresh |
| packages-core-src-embedding-ollama-embedding.ts | [packages-core-src-embedding-ollama-embedding.ts](concepts/packages-core-src-embedding-ollama-embedding.ts.md) | fresh |
| packages-core-src-embedding-openai-embedding.ts | [packages-core-src-embedding-openai-embedding.ts](concepts/packages-core-src-embedding-openai-embedding.ts.md) | fresh |
| packages-core-src-embedding-voyageai-embedding.ts | [packages-core-src-embedding-voyageai-embedding.ts](concepts/packages-core-src-embedding-voyageai-embedding.ts.md) | fresh |
| packages-core-src-splitter-ast-splitter.ts | [packages-core-src-splitter-ast-splitter.ts](concepts/packages-core-src-splitter-ast-splitter.ts.md) | fresh |
| packages-core-src-splitter-index.ts | [packages-core-src-splitter-index.ts](concepts/packages-core-src-splitter-index.ts.md) | fresh |
| packages-core-src-sync-merkle.ts | [packages-core-src-sync-merkle.ts](concepts/packages-core-src-sync-merkle.ts.md) | fresh |
| packages-core-src-sync-synchronizer.ts | [packages-core-src-sync-synchronizer.ts](concepts/packages-core-src-sync-synchronizer.ts.md) | fresh |
| packages-core-src-vectordb-milvus-restful-vectordb.ts | [packages-core-src-vectordb-milvus-restful-vectordb.ts](concepts/packages-core-src-vectordb-milvus-restful-vectordb.ts.md) | fresh |
| packages-core-src-vectordb-milvus-vectordb.ts | [packages-core-src-vectordb-milvus-vectordb.ts](concepts/packages-core-src-vectordb-milvus-vectordb.ts.md) | fresh |
| packages-core-src-vectordb-types.ts | [packages-core-src-vectordb-types.ts](concepts/packages-core-src-vectordb-types.ts.md) | fresh |
| packages-core-src-vectordb-zilliz-utils.ts | [packages-core-src-vectordb-zilliz-utils.ts](concepts/packages-core-src-vectordb-zilliz-utils.ts.md) | fresh |
| packages-mcp-src-config.ts | [packages-mcp-src-config.ts](concepts/packages-mcp-src-config.ts.md) | fresh |
| packages-mcp-src-handlers.ts | [packages-mcp-src-handlers.ts](concepts/packages-mcp-src-handlers.ts.md) | fresh |
| packages-mcp-src-snapshot.ts | [packages-mcp-src-snapshot.ts](concepts/packages-mcp-src-snapshot.ts.md) | fresh |
| packages-mcp-src-sync.ts | [packages-mcp-src-sync.ts](concepts/packages-mcp-src-sync.ts.md) | fresh |
| packages-vscode-extension-src-config-configManager.ts | [packages-vscode-extension-src-config-configManager.ts](concepts/packages-vscode-extension-src-config-configManager.ts.md) | fresh |

## Doc-derived concepts
Concepts extracted from the project's own docs (README / `docs/`), grounded to the symbol catalog. The source docs stay in place.
- [architecture-packages](doc-concepts/architecture-packages.md)
- [async-indexing-workflow](doc-concepts/async-indexing-workflow.md)
- [async-progress-tracking](doc-concepts/async-progress-tracking.md)
- [async-snapshot-state](doc-concepts/async-snapshot-state.md)
- [embedding-and-vector-backends](doc-concepts/embedding-and-vector-backends.md)
- [env-embedding-provider](doc-concepts/env-embedding-provider.md)
- [env-global-config](doc-concepts/env-global-config.md)
- [env-splitter](doc-concepts/env-splitter.md)
- [env-tuning-knobs](doc-concepts/env-tuning-knobs.md)
- [env-vector-db-connection](doc-concepts/env-vector-db-connection.md)
- [faq-codebase-path-keying](doc-concepts/faq-codebase-path-keying.md)
- [faq-file-inclusion](doc-concepts/faq-file-inclusion.md)
- [faq-indexing-status](doc-concepts/faq-indexing-status.md)
- [files-ignore-patterns](doc-concepts/files-ignore-patterns.md)
- [files-inclusion-rules](doc-concepts/files-inclusion-rules.md)
- [files-supported-extensions](doc-concepts/files-supported-extensions.md)
- [hybrid-search](doc-concepts/hybrid-search.md)
- [mcp-integration](doc-concepts/mcp-integration.md)
- [prereq-embedding-provider](doc-concepts/prereq-embedding-provider.md)
- [prereq-vector-database](doc-concepts/prereq-vector-database.md)
- [quickstart-index-then-search-workflow](doc-concepts/quickstart-index-then-search-workflow.md)
- [quickstart-mcp-server-setup](doc-concepts/quickstart-mcp-server-setup.md)
- [semantic-code-search](doc-concepts/semantic-code-search.md)

## Coverage
Two tiers: **concept pages** explain mechanisms deeply (selective); **module
catalogs** represent the rest so the whole repo is navigable. Coverage is a
set-difference over the SCIP symbol table, not a graph walk — every documentable
symbol is enumerated and represented.

- documentable symbols: **1111** across 63 modules
- deep (concept pages): **559** (50.3%)
- catalog-only: **552**
- represented total: **1111** (100.0%)
- classes represented: **109/109**

See [`catalog/`](catalog/) for the generated per-module structural index.

## Provenance
`extracted` = from SCIP / source. `inferred` = LLM judgment, treat as such.
Design-intent dynamics are labeled; none are runtime-measured (no L4 pass run).
Callers/callees are reference-scoped (SCIP has no call role), labeled "calls/refs".
