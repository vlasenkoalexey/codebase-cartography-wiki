---
slug: gitgalaxy
commit: 845400be8cb4ed973064956eacbd1013af10a0ff
scip_tool: scip-python
updated: 2026-07-04
---

# gitgalaxy internals wiki

Generated, grounded wiki. Start from a concept (or an area); drill into cited symbols.
The commit pin above is the single source version for every page in this silo.

**Start here → [Overview](overview.md)** — the whole system in one page (main concepts + core diagrams + a map of the wiki).

## Concepts (deep)
| Concept | Page | Status |
|---|---|---|
| gitgalaxy-cobol_refractor_controller | [gitgalaxy-cobol_refractor_controller](concepts/gitgalaxy-cobol_refractor_controller.md) | fresh |
| gitgalaxy-core-aperture | [gitgalaxy-core-aperture](concepts/gitgalaxy-core-aperture.md) | fresh |
| gitgalaxy-core-detector | [gitgalaxy-core-detector](concepts/gitgalaxy-core-detector.md) | fresh |
| gitgalaxy-core-guidestar_lens | [gitgalaxy-core-guidestar_lens](concepts/gitgalaxy-core-guidestar_lens.md) | fresh |
| gitgalaxy-core-prism | [gitgalaxy-core-prism](concepts/gitgalaxy-core-prism.md) | fresh |
| gitgalaxy-galaxyscope | [gitgalaxy-galaxyscope](concepts/gitgalaxy-galaxyscope.md) | fresh |
| gitgalaxy-licensing | [gitgalaxy-licensing](concepts/gitgalaxy-licensing.md) | fresh |
| gitgalaxy-metrics-chronometer | [gitgalaxy-metrics-chronometer](concepts/gitgalaxy-metrics-chronometer.md) | fresh |
| gitgalaxy-metrics-signal_processor | [gitgalaxy-metrics-signal_processor](concepts/gitgalaxy-metrics-signal_processor.md) | fresh |
| gitgalaxy-security-security_auditor | [gitgalaxy-security-security_auditor](concepts/gitgalaxy-security-security_auditor.md) | fresh |
| gitgalaxy-security-security_lens | [gitgalaxy-security-security_lens](concepts/gitgalaxy-security-security_lens.md) | fresh |
| gitgalaxy-standards-analysis_lens | [gitgalaxy-standards-analysis_lens](concepts/gitgalaxy-standards-analysis_lens.md) | fresh |
| gitgalaxy-standards-gitgalaxy_config | [gitgalaxy-standards-gitgalaxy_config](concepts/gitgalaxy-standards-gitgalaxy_config.md) | fresh |
| gitgalaxy-standards-language_lens | [gitgalaxy-standards-language_lens](concepts/gitgalaxy-standards-language_lens.md) | fresh |
| gitgalaxy-standards-language_standards | [gitgalaxy-standards-language_standards](concepts/gitgalaxy-standards-language_standards.md) | fresh |
| site-app | [site-app](concepts/site-app.md) | fresh |

## Doc-derived concepts
Concepts extracted from the project's own docs (README / `docs/`), grounded to the symbol catalog. The source docs stay in place.
- [active-matter-vs-ghost-mass](doc-concepts/active-matter-vs-ghost-mass.md)
- [ast-vs-heuristic-tradeoffs](doc-concepts/ast-vs-heuristic-tradeoffs.md)
- [atomic-literal-shield](doc-concepts/atomic-literal-shield.md)
- [blast-paradigm](doc-concepts/blast-paradigm.md)
- [cobol-legacy-migration-pipeline](doc-concepts/cobol-legacy-migration-pipeline.md)
- [delta-mission-vs-incremental-scan](doc-concepts/delta-mission-vs-incremental-scan.md)
- [domain-dialect-patching](doc-concepts/domain-dialect-patching.md)
- [ecosystem-gravity-and-confidence-override](doc-concepts/ecosystem-gravity-and-confidence-override.md)
- [empirical-validation-of-heuristic-parsing](doc-concepts/empirical-validation-of-heuristic-parsing.md)
- [guidestar-intent-vs-identity](doc-concepts/guidestar-intent-vs-identity.md)
- [identity-deception-and-extension-mismatch](doc-concepts/identity-deception-and-extension-mismatch.md)
- [language-lens-bayesian-trust-tiers](doc-concepts/language-lens-bayesian-trust-tiers.md)
- [linguistic-trust-tiers-and-biaxial-drift](doc-concepts/linguistic-trust-tiers-and-biaxial-drift.md)
- [neighborhood-micro-mass-quota](doc-concepts/neighborhood-micro-mass-quota.md)
- [network-and-agent-security-tools](doc-concepts/network-and-agent-security-tools.md)
- [optical-pipeline-metaphor](doc-concepts/optical-pipeline-metaphor.md)
- [polyglot-handshake-detection](doc-concepts/polyglot-handshake-detection.md)
- [risk-exposure-physics](doc-concepts/risk-exposure-physics.md)
- [satellite-physics-and-naming-shields](doc-concepts/satellite-physics-and-naming-shields.md)
- [structural-rag-graph](doc-concepts/structural-rag-graph.md)
- [supernova-injection](doc-concepts/supernova-injection.md)
- [supply-chain-and-compliance-tools](doc-concepts/supply-chain-and-compliance-tools.md)
- [systemic-bottleneck-taxonomy](doc-concepts/systemic-bottleneck-taxonomy.md)
- [the-cartographer-spatial-positioning](doc-concepts/the-cartographer-spatial-positioning.md)
- [xray-binary-inspection](doc-concepts/xray-binary-inspection.md)
- [zero-trust-deployment-and-licensing-model](doc-concepts/zero-trust-deployment-and-licensing-model.md)

## Coverage
Two tiers: **concept pages** explain mechanisms deeply (selective); **module
catalogs** represent the rest so the whole repo is navigable. Coverage is a
set-difference over the SCIP symbol table, not a graph walk — every documentable
symbol is enumerated and represented.

- documentable symbols: **1189** across 113 modules
- deep (concept pages): **335** (28.2%)
- catalog-only: **854**
- represented total: **1189** (100.0%)
- classes represented: **52/52**

See [`catalog/`](catalog/) for the generated per-module structural index.

## Provenance
`extracted` = from SCIP / source. `inferred` = LLM judgment, treat as such.
Design-intent dynamics are labeled; none are runtime-measured (no L4 pass run).
Callers/callees are reference-scoped (SCIP has no call role), labeled "calls/refs".
