---
slug: openwiki
commit: 58b4bd33a3e824e09c082e1b6f0764d97666b856
scip_tool: scip-python
updated: 2026-07-04
---

# openwiki internals wiki

Generated, grounded wiki. Start from a concept (or an area); drill into cited symbols.
The commit pin above is the single source version for every page in this silo.

**Start here → [Overview](overview.md)** — the whole system in one page (main concepts + core diagrams + a map of the wiki).

## Concepts (deep)
| Concept | Page | Status |
|---|---|---|
| openwiki-agent-index.ts | [openwiki-agent-index.ts](concepts/openwiki-agent-index.ts.md) | fresh |
| openwiki-agent-types.ts | [openwiki-agent-types.ts](concepts/openwiki-agent-types.ts.md) | fresh |
| openwiki-cli.tsx | [openwiki-cli.tsx](concepts/openwiki-cli.tsx.md) | fresh |
| openwiki-commands.ts | [openwiki-commands.ts](concepts/openwiki-commands.ts.md) | fresh |
| openwiki-constants.ts | [openwiki-constants.ts](concepts/openwiki-constants.ts.md) | fresh |
| openwiki-credentials.tsx | [openwiki-credentials.tsx](concepts/openwiki-credentials.tsx.md) | fresh |
| openwiki-env.ts | [openwiki-env.ts](concepts/openwiki-env.ts.md) | fresh |

## Doc-derived concepts
Concepts extracted from the project's own docs (README / `docs/`), grounded to the symbol catalog. The source docs stay in place.
- [agent-native-documentation](doc-concepts/agent-native-documentation.md)
- [development-and-dry-run](doc-concepts/development-and-dry-run.md)
- [documentation-lifecycle](doc-concepts/documentation-lifecycle.md)
- [provider-configuration](doc-concepts/provider-configuration.md)
- [scheduled-documentation-updates](doc-concepts/scheduled-documentation-updates.md)

## Coverage
Two tiers: **concept pages** explain mechanisms deeply (selective); **module
catalogs** represent the rest so the whole repo is navigable. Coverage is a
set-difference over the SCIP symbol table, not a graph walk — every documentable
symbol is enumerated and represented.

- documentable symbols: **459** across 9 modules
- deep (concept pages): **132** (28.8%)
- catalog-only: **327**
- represented total: **459** (100.0%)
- classes represented: **44/44**

See [`catalog/`](catalog/) for the generated per-module structural index.

## Provenance
`extracted` = from SCIP / source. `inferred` = LLM judgment, treat as such.
Design-intent dynamics are labeled; none are runtime-measured (no L4 pass run).
Callers/callees are reference-scoped (SCIP has no call role), labeled "calls/refs".
