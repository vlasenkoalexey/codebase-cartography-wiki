---
slug: graphify
commit: 983da3c15f3eb31862bca4c9977ff5329a6b12d4
scip_tool: scip-python
updated: 2026-07-04
---

# graphify internals wiki

Generated, grounded wiki. Start from a concept (or an area); drill into cited symbols.
The commit pin above is the single source version for every page in this silo.

**Start here → [Overview](overview.md)** — the whole system in one page (main concepts + core diagrams + a map of the wiki).

## Concepts (deep)
| Concept | Page | Status |
|---|---|---|
| graphify-__main__ | [graphify-__main__](concepts/graphify-__main__.md) | fresh |
| graphify-_minhash | [graphify-_minhash](concepts/graphify-_minhash.md) | fresh |
| graphify-analyze | [graphify-analyze](concepts/graphify-analyze.md) | fresh |
| graphify-build | [graphify-build](concepts/graphify-build.md) | fresh |
| graphify-cache | [graphify-cache](concepts/graphify-cache.md) | fresh |
| graphify-callflow_html | [graphify-callflow_html](concepts/graphify-callflow_html.md) | fresh |
| graphify-cluster | [graphify-cluster](concepts/graphify-cluster.md) | fresh |
| graphify-dedup | [graphify-dedup](concepts/graphify-dedup.md) | fresh |
| graphify-detect | [graphify-detect](concepts/graphify-detect.md) | fresh |
| graphify-export | [graphify-export](concepts/graphify-export.md) | fresh |
| graphify-extract | [graphify-extract](concepts/graphify-extract.md) | fresh |
| graphify-extractors-base | [graphify-extractors-base](concepts/graphify-extractors-base.md) | fresh |
| graphify-file_slice | [graphify-file_slice](concepts/graphify-file_slice.md) | fresh |
| graphify-hooks | [graphify-hooks](concepts/graphify-hooks.md) | fresh |
| graphify-llm | [graphify-llm](concepts/graphify-llm.md) | fresh |
| graphify-multigraph_compat | [graphify-multigraph_compat](concepts/graphify-multigraph_compat.md) | fresh |
| graphify-paths | [graphify-paths](concepts/graphify-paths.md) | fresh |
| graphify-prs | [graphify-prs](concepts/graphify-prs.md) | fresh |
| graphify-reflect | [graphify-reflect](concepts/graphify-reflect.md) | fresh |
| graphify-scip_ingest | [graphify-scip_ingest](concepts/graphify-scip_ingest.md) | fresh |
| graphify-security | [graphify-security](concepts/graphify-security.md) | fresh |
| graphify-serve | [graphify-serve](concepts/graphify-serve.md) | fresh |
| graphify-symbol_resolution | [graphify-symbol_resolution](concepts/graphify-symbol_resolution.md) | fresh |
| graphify-watch | [graphify-watch](concepts/graphify-watch.md) | fresh |

## Doc-derived concepts
Concepts extracted from the project's own docs (README / `docs/`), grounded to the symbol catalog. The source docs stay in place.
- [adding-a-language](doc-concepts/adding-a-language.md)
- [always-on-graph](doc-concepts/always-on-graph.md)
- [community-detection](doc-concepts/community-detection.md)
- [confidence-labels](doc-concepts/confidence-labels.md)
- [content-hash-cache](doc-concepts/content-hash-cache.md)
- [extraction-schema](doc-concepts/extraction-schema.md)
- [god-nodes-report](doc-concepts/god-nodes-report.md)
- [graph-query-interface](doc-concepts/graph-query-interface.md)
- [ingest-pipeline](doc-concepts/ingest-pipeline.md)
- [mcp-server](doc-concepts/mcp-server.md)
- [multi-source-ingestion](doc-concepts/multi-source-ingestion.md)
- [node-summaries](doc-concepts/node-summaries.md)
- [output-artifacts](doc-concepts/output-artifacts.md)
- [parallel-extraction](doc-concepts/parallel-extraction.md)
- [pr-dashboard](doc-concepts/pr-dashboard.md)
- [security-validation](doc-concepts/security-validation.md)
- [three-pass-extraction](doc-concepts/three-pass-extraction.md)
- [token-benchmark](doc-concepts/token-benchmark.md)
- [work-memory](doc-concepts/work-memory.md)

## Coverage
Two tiers: **concept pages** explain mechanisms deeply (selective); **module
catalogs** represent the rest so the whole repo is navigable. Coverage is a
set-difference over the SCIP symbol table, not a graph walk — every documentable
symbol is enumerated and represented.

- documentable symbols: **4849** across 184 modules
- deep (concept pages): **621** (12.8%)
- catalog-only: **4228**
- represented total: **4849** (100.0%)
- classes represented: **78/78**

See [`catalog/`](catalog/) for the generated per-module structural index.

## Provenance
`extracted` = from SCIP / source. `inferred` = LLM judgment, treat as such.
Design-intent dynamics are labeled; none are runtime-measured (no L4 pass run).
Callers/callees are reference-scoped (SCIP has no call role), labeled "calls/refs".
