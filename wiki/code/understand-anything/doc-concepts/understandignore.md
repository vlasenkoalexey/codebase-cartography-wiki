---
title: .understandignore file exclusion
type: doc-concept
provenance: doc
source: docs/superpowers/specs/2026-04-10-understandignore-design.md
updated: 2026-07-04
status: fresh
---
# .understandignore file exclusion

## Definition
`.understandignore` lets users exclude files/directories from analysis using
familiar `.gitignore` syntax. It layers **on top of** hardcoded defaults
(node_modules/, dist/, lock files, binaries, …) rather than replacing them, and
supports `!` negation to force-include something the defaults dropped. On first
run the tool deterministically generates a fully commented-out starter file
(suggestions based on what it finds in the project) and pauses for the user to
review before analysis. This is the tool's scoping/coverage-control knob — what a
codebase-comprehension survey would compare against wikify-repo's coverage
catalogs.

## In understand-anything (grounded)
Pattern matching is `packages/core/src/ignore-filter.ts`:
[`createIgnoreFilter`](../catalog/understand-anything-plugin/packages/core/src/ignore-filter.ts.md#createIgnoreFilter)
builds an [`IgnoreFilter`](../catalog/understand-anything-plugin/packages/core/src/ignore-filter.ts.md#IgnoreFilter)
whose [`isIgnored`](../catalog/understand-anything-plugin/packages/core/src/ignore-filter.ts.md#IgnoreFilter.isIgnored)
merges [`DEFAULT_IGNORE_PATTERNS`](../catalog/understand-anything-plugin/packages/core/src/ignore-filter.ts.md#DEFAULT_IGNORE_PATTERNS)
(the built-ins) with the project- and root-level `.understandignore` files,
additively and in override order (built on the `ignore` npm package).

Starter-file generation is `packages/core/src/ignore-generator.ts`:
[`generateStarterIgnoreFile`](../catalog/understand-anything-plugin/packages/core/src/ignore-generator.ts.md#generateStarterIgnoreFile)
scans the tree ([`detectDirectories`](../catalog/understand-anything-plugin/packages/core/src/ignore-generator.ts.md#detectDirectories))
and emits commented suggestions from
[`TEST_PATTERN_GROUPS`](../catalog/understand-anything-plugin/packages/core/src/ignore-generator.ts.md#TEST_PATTERN_GROUPS)
/ [`EXACT_DIR_NAMES`](../catalog/understand-anything-plugin/packages/core/src/ignore-generator.ts.md#EXACT_DIR_NAMES)
/ [`SUFFIX_DIR_GLOBS`](../catalog/understand-anything-plugin/packages/core/src/ignore-generator.ts.md#SUFFIX_DIR_GLOBS),
skipping anything already excluded
([`isCoveredByDefaults`](../catalog/understand-anything-plugin/packages/core/src/ignore-generator.ts.md#isCoveredByDefaults)),
under a fixed [`HEADER`](../catalog/understand-anything-plugin/packages/core/src/ignore-generator.ts.md#HEADER).
Both feed the two-layer scan filter: the `project-scanner` agent's coarse
hardcoded patterns (Layer 1) plus this deterministic `IgnoreFilter` (Layer 2),
reported as a `filteredByIgnore` count.

> [!inferred]
> No existing per-subsystem code concept page covers file exclusion; the two
> modules above are the whole feature, so this doc-concept links their module
> catalogs directly rather than a deeper concept page.

## Why it matters / when it applies
Excluding vendor code, generated output, and test fixtures makes analysis faster
and cheaper and keeps the graph focused on code the user actually owns. Two
design choices matter for trust: suggestions are generated but never
auto-activated (all commented out — the user opts in), and the run pauses for
review so exclusions are a deliberate, visible decision rather than a silent
default.

## Connections
- Code concepts: none directly cover file exclusion (the two modules below are the feature); adjacent scan-phase concepts appear in the sibling doc-concepts.
- Module catalogs: [ignore-filter.ts](../catalog/understand-anything-plugin/packages/core/src/ignore-filter.ts.md), [ignore-generator.ts](../catalog/understand-anything-plugin/packages/core/src/ignore-generator.ts.md)
- Related doc-concepts: [multi-agent-pipeline](multi-agent-pipeline.md), [token-reduction](token-reduction.md), [semantic-batching-output-chunking](semantic-batching-output-chunking.md)

## Source
Extracted from `docs/superpowers/specs/2026-04-10-understandignore-design.md`
(kept in place).
