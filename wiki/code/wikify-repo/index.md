---
slug: wikify-repo
commit: 05228d70489dd5d3963a6bb74460bf670f4c1d9f
scip_tool: scip-python
updated: 2026-07-04
---

# wikify-repo internals wiki

Generated, grounded wiki. Start from a concept (or an area); drill into cited symbols.
The commit pin above is the single source version for every page in this silo.

**Start here → [Overview](overview.md)** — the whole system in one page (main concepts + core diagrams + a map of the wiki).

## Concepts (deep)
| Concept | Page | Status |
|---|---|---|
| wikify-acquire | [wikify-acquire](concepts/wikify-acquire.md) | fresh |
| wikify-ast_fallback | [wikify-ast_fallback](concepts/wikify-ast_fallback.md) | fresh |
| wikify-cli | [wikify-cli](concepts/wikify-cli.md) | fresh |
| wikify-config | [wikify-config](concepts/wikify-config.md) | fresh |
| wikify-connect | [wikify-connect](concepts/wikify-connect.md) | fresh |
| wikify-coverage | [wikify-coverage](concepts/wikify-coverage.md) | fresh |
| wikify-diff | [wikify-diff](concepts/wikify-diff.md) | fresh |
| wikify-discover | [wikify-discover](concepts/wikify-discover.md) | fresh |
| wikify-docs | [wikify-docs](concepts/wikify-docs.md) | fresh |
| wikify-graph | [wikify-graph](concepts/wikify-graph.md) | fresh |
| wikify-languages | [wikify-languages](concepts/wikify-languages.md) | fresh |
| wikify-lint | [wikify-lint](concepts/wikify-lint.md) | fresh |
| wikify-monikers | [wikify-monikers](concepts/wikify-monikers.md) | fresh |
| wikify-scip_index | [wikify-scip_index](concepts/wikify-scip_index.md) | fresh |
| wikify-state | [wikify-state](concepts/wikify-state.md) | fresh |
| wikify-verify | [wikify-verify](concepts/wikify-verify.md) | fresh |

## Doc-derived concepts
Concepts extracted from the project's own docs (README / `docs/`), grounded to the symbol catalog. The source docs stay in place.
- [adversarial-verify](doc-concepts/adversarial-verify.md)
- [citation-linter-grounding-gate](doc-concepts/citation-linter-grounding-gate.md)
- [concept-driven-synthesis-and-coverage](doc-concepts/concept-driven-synthesis-and-coverage.md)
- [devirtualization-dispatch-seam](doc-concepts/devirtualization-dispatch-seam.md)
- [docs-mode](doc-concepts/docs-mode.md)
- [idempotent-reconcile](doc-concepts/idempotent-reconcile.md)
- [indexing-at-scale](doc-concepts/indexing-at-scale.md)
- [markdown-as-interface](doc-concepts/markdown-as-interface.md)
- [multi-repo-connect](doc-concepts/multi-repo-connect.md)
- [packet-based-synthesis](doc-concepts/packet-based-synthesis.md)
- [python-llm-split](doc-concepts/python-llm-split.md)
- [scip-vs-ast-grounding](doc-concepts/scip-vs-ast-grounding.md)
- [three-layer-architecture](doc-concepts/three-layer-architecture.md)
- [tool-positioning-comparison](doc-concepts/tool-positioning-comparison.md)

## Coverage
Two tiers: **concept pages** explain mechanisms deeply (selective); **module
catalogs** represent the rest so the whole repo is navigable. Coverage is a
set-difference over the SCIP symbol table, not a graph walk — every documentable
symbol is enumerated and represented.

- documentable symbols: **664** across 48 modules
- deep (concept pages): **347** (52.3%)
- catalog-only: **317**
- represented total: **664** (100.0%)
- classes represented: **25/25**

See [`catalog/`](catalog/) for the generated per-module structural index.

## Provenance
`extracted` = from SCIP / source. `inferred` = LLM judgment, treat as such.
Design-intent dynamics are labeled; none are runtime-measured (no L4 pass run).
Callers/callees are reference-scoped (SCIP has no call role), labeled "calls/refs".
