---
slug: understand-anything
commit: 0e8ad84a2a5236dca533beef618d71ee3f4568f6
scip_tool: scip-python
updated: 2026-07-04
---

# understand-anything internals wiki

Generated, grounded wiki. Start from a concept (or an area); drill into cited symbols.
The commit pin above is the single source version for every page in this silo.

**Start here → [Overview](overview.md)** — the whole system in one page (main concepts + core diagrams + a map of the wiki).

## Concepts (deep)
| Concept | Page | Status |
|---|---|---|
| understand-anything-plugin-packages-core-src-analyzer-graph-builder.ts | [understand-anything-plugin-packages-core-src-analyzer-graph-builder.ts](concepts/understand-anything-plugin-packages-core-src-analyzer-graph-builder.ts.md) | fresh |
| understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts | [understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts](concepts/understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts.md) | fresh |
| understand-anything-plugin-packages-core-src-fingerprint.ts | [understand-anything-plugin-packages-core-src-fingerprint.ts](concepts/understand-anything-plugin-packages-core-src-fingerprint.ts.md) | fresh |
| understand-anything-plugin-packages-core-src-languages-types.ts | [understand-anything-plugin-packages-core-src-languages-types.ts](concepts/understand-anything-plugin-packages-core-src-languages-types.ts.md) | fresh |
| understand-anything-plugin-packages-core-src-persistence-index.ts | [understand-anything-plugin-packages-core-src-persistence-index.ts](concepts/understand-anything-plugin-packages-core-src-persistence-index.ts.md) | fresh |
| understand-anything-plugin-packages-core-src-plugins-extractors-base-extractor.ts | [understand-anything-plugin-packages-core-src-plugins-extractors-base-extractor.ts](concepts/understand-anything-plugin-packages-core-src-plugins-extractors-base-extractor.ts.md) | fresh |
| understand-anything-plugin-packages-core-src-plugins-extractors-dart-extractor.ts | [understand-anything-plugin-packages-core-src-plugins-extractors-dart-extractor.ts](concepts/understand-anything-plugin-packages-core-src-plugins-extractors-dart-extractor.ts.md) | fresh |
| understand-anything-plugin-packages-core-src-plugins-extractors-swift-extractor.ts | [understand-anything-plugin-packages-core-src-plugins-extractors-swift-extractor.ts](concepts/understand-anything-plugin-packages-core-src-plugins-extractors-swift-extractor.ts.md) | fresh |
| understand-anything-plugin-packages-core-src-plugins-extractors-types.ts | [understand-anything-plugin-packages-core-src-plugins-extractors-types.ts](concepts/understand-anything-plugin-packages-core-src-plugins-extractors-types.ts.md) | fresh |
| understand-anything-plugin-packages-core-src-plugins-registry.ts | [understand-anything-plugin-packages-core-src-plugins-registry.ts](concepts/understand-anything-plugin-packages-core-src-plugins-registry.ts.md) | fresh |
| understand-anything-plugin-packages-core-src-plugins-tree-sitter-plugin.ts | [understand-anything-plugin-packages-core-src-plugins-tree-sitter-plugin.ts](concepts/understand-anything-plugin-packages-core-src-plugins-tree-sitter-plugin.ts.md) | fresh |
| understand-anything-plugin-packages-core-src-schema.ts | [understand-anything-plugin-packages-core-src-schema.ts](concepts/understand-anything-plugin-packages-core-src-schema.ts.md) | fresh |
| understand-anything-plugin-packages-core-src-types.ts | [understand-anything-plugin-packages-core-src-types.ts](concepts/understand-anything-plugin-packages-core-src-types.ts.md) | fresh |
| understand-anything-plugin-packages-dashboard-src-components-CustomNode.tsx | [understand-anything-plugin-packages-dashboard-src-components-CustomNode.tsx](concepts/understand-anything-plugin-packages-dashboard-src-components-CustomNode.tsx.md) | fresh |
| understand-anything-plugin-packages-dashboard-src-components-FileExplorer.tsx | [understand-anything-plugin-packages-dashboard-src-components-FileExplorer.tsx](concepts/understand-anything-plugin-packages-dashboard-src-components-FileExplorer.tsx.md) | fresh |
| understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx | [understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx](concepts/understand-anything-plugin-packages-dashboard-src-components-GraphView.tsx.md) | fresh |
| understand-anything-plugin-packages-dashboard-src-contexts-I18nContext.tsx | [understand-anything-plugin-packages-dashboard-src-contexts-I18nContext.tsx](concepts/understand-anything-plugin-packages-dashboard-src-contexts-I18nContext.tsx.md) | fresh |
| understand-anything-plugin-packages-dashboard-src-store.ts | [understand-anything-plugin-packages-dashboard-src-store.ts](concepts/understand-anything-plugin-packages-dashboard-src-store.ts.md) | fresh |
| understand-anything-plugin-packages-dashboard-src-themes-types.ts | [understand-anything-plugin-packages-dashboard-src-themes-types.ts](concepts/understand-anything-plugin-packages-dashboard-src-themes-types.ts.md) | fresh |
| understand-anything-plugin-packages-dashboard-src-utils-containers.ts | [understand-anything-plugin-packages-dashboard-src-utils-containers.ts](concepts/understand-anything-plugin-packages-dashboard-src-utils-containers.ts.md) | fresh |
| understand-anything-plugin-packages-dashboard-src-utils-edgeAggregation.ts | [understand-anything-plugin-packages-dashboard-src-utils-edgeAggregation.ts](concepts/understand-anything-plugin-packages-dashboard-src-utils-edgeAggregation.ts.md) | fresh |
| understand-anything-plugin-packages-dashboard-src-utils-elk-layout.ts | [understand-anything-plugin-packages-dashboard-src-utils-elk-layout.ts](concepts/understand-anything-plugin-packages-dashboard-src-utils-elk-layout.ts.md) | fresh |
| understand-anything-plugin-packages-dashboard-src-utils-layout.ts | [understand-anything-plugin-packages-dashboard-src-utils-layout.ts](concepts/understand-anything-plugin-packages-dashboard-src-utils-layout.ts.md) | fresh |
| understand-anything-plugin-skills-understand-merge-batch-graphs | [understand-anything-plugin-skills-understand-merge-batch-graphs](concepts/understand-anything-plugin-skills-understand-merge-batch-graphs.md) | fresh |

## Doc-derived concepts
Concepts extracted from the project's own docs (README / `docs/`), grounded to the symbol catalog. The source docs stay in place.
- [business-domain-extraction](doc-concepts/business-domain-extraction.md)
- [incremental-reconcile](doc-concepts/incremental-reconcile.md)
- [knowledge-base-analysis](doc-concepts/knowledge-base-analysis.md)
- [knowledge-graph-schema](doc-concepts/knowledge-graph-schema.md)
- [language-agnostic-extraction](doc-concepts/language-agnostic-extraction.md)
- [multi-agent-pipeline](doc-concepts/multi-agent-pipeline.md)
- [output-language-detection](doc-concepts/output-language-detection.md)
- [semantic-batching-output-chunking](doc-concepts/semantic-batching-output-chunking.md)
- [token-reduction](doc-concepts/token-reduction.md)
- [tree-sitter-llm-hybrid](doc-concepts/tree-sitter-llm-hybrid.md)
- [understandignore](doc-concepts/understandignore.md)

## Coverage
Two tiers: **concept pages** explain mechanisms deeply (selective); **module
catalogs** represent the rest so the whole repo is navigable. Coverage is a
set-difference over the SCIP symbol table, not a graph walk — every documentable
symbol is enumerated and represented.

- documentable symbols: **1801** across 203 modules
- deep (concept pages): **441** (24.5%)
- catalog-only: **1360**
- represented total: **1801** (100.0%)
- classes represented: **174/174**

See [`catalog/`](catalog/) for the generated per-module structural index.

## Provenance
`extracted` = from SCIP / source. `inferred` = LLM judgment, treat as such.
Design-intent dynamics are labeled; none are runtime-measured (no L4 pass run).
Callers/callees are reference-scoped (SCIP has no call role), labeled "calls/refs".
