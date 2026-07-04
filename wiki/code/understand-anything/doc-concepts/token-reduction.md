---
title: Token reduction for /understand
type: doc-concept
provenance: doc
source: docs/superpowers/specs/2026-03-27-token-reduction-design.md
updated: 2026-07-04
status: fresh
---
# Token reduction for /understand

## Definition
On large codebases most of `/understand`'s tokens go to **repeated context
injection** — the same data resent to every subagent. The spec targets an ~83%
input-token cut on a 500-file project via five independent changes (C1–C5): (C1)
pre-resolve imports once in the scanner into an `importMap` instead of shipping
the full file list to every batch; (C2) increase batch size 5–10 → 20–30 files
and concurrency 3 → 5; (C3) drop per-language/framework prompt addendums from
batches in favor of one inline hint table; (C4) slim the tour/architecture
payloads to file-only nodes and imports/calls-only edges; (C5) gate the LLM
graph-reviewer behind `--review`, using an inline deterministic validator by
default. This is the efficiency axis of the tool's grounding pipeline.

## In understand-anything (grounded)
Most of these changes live in the skill/agent markdown (`SKILL.md`,
`project-scanner-prompt.md`, `file-analyzer-prompt.md`), but they rest on typed
and deterministic code. Pre-resolved imports (C1) are the
[`ImportResolution`](../catalog/understand-anything-plugin/packages/core/src/types.ts.md#ImportResolution)
shape (source →
[`resolvedPath`](../catalog/understand-anything-plugin/packages/core/src/types.ts.md#ImportResolution.resolvedPath))
that [`AnalyzerPlugin.resolveImports`](../catalog/understand-anything-plugin/packages/core/src/types.ts.md#AnalyzerPlugin.resolveImports)
produces; the `importMap` written by the scanner is what the merge reducer later
uses as a safety net —
[`recover_imports_from_scan`](../catalog/understand-anything-plugin/skills/understand/merge-batch-graphs.md#recover_imports_from_scan)
restores `imports` edges even if a slimmed batch dropped them, via
[`merge_and_normalize`](../catalog/understand-anything-plugin/skills/understand/merge-batch-graphs.md#merge_and_normalize).
Batch results are coerced to the schema by
[`normalizeBatchOutput`](../catalog/understand-anything-plugin/packages/core/src/analyzer/normalize-graph.ts.md#normalizeBatchOutput).

The C5 default path replaces the LLM reviewer with the deterministic
[`validateGraph`](../catalog/understand-anything-plugin/packages/core/src/schema.ts.md#validateGraph)
/ [`autoFixGraph`](../catalog/understand-anything-plugin/packages/core/src/schema.ts.md#autoFixGraph).
Token reduction also compounds with incremental runs: fewer files to analyze at
all, decided by
[`classifyUpdate`](../catalog/understand-anything-plugin/packages/core/src/change-classifier.ts.md#classifyUpdate)
and the fingerprint diff
[`analyzeChanges`](../catalog/understand-anything-plugin/packages/core/src/fingerprint.ts.md#analyzeChanges).

## Why it matters / when it applies
The root cause is quantified: for a 500-file project, injecting the full file
list into 67 batches costs ~167k tokens of pure redundancy. Because each change
is independent, they ship separately (recommended order C5 → C4 → C3 → C1+C2) and
the savings scale with project size — bigger repos have more batches and thus more
repetition to eliminate. Backward compatibility with the existing
`knowledge-graph.json` schema is a stated goal, so none of this changes the
output representation.

## Connections
- Code concepts: [core types](../concepts/understand-anything-plugin-packages-core-src-types.ts.md), [merge-batch-graphs](../concepts/understand-anything-plugin-skills-understand-merge-batch-graphs.md), [normalize-graph](../concepts/understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts.md), [fingerprint](../concepts/understand-anything-plugin-packages-core-src-fingerprint.ts.md)
- Module catalogs: [types.ts](../catalog/understand-anything-plugin/packages/core/src/types.ts.md), [skills/understand/merge-batch-graphs.py](../catalog/understand-anything-plugin/skills/understand/merge-batch-graphs.md), [analyzer/normalize-graph.ts](../catalog/understand-anything-plugin/packages/core/src/analyzer/normalize-graph.ts.md), [schema.ts](../catalog/understand-anything-plugin/packages/core/src/schema.ts.md), [change-classifier.ts](../catalog/understand-anything-plugin/packages/core/src/change-classifier.ts.md), [fingerprint.ts](../catalog/understand-anything-plugin/packages/core/src/fingerprint.ts.md)
- Related doc-concepts: [semantic-batching-output-chunking](semantic-batching-output-chunking.md), [multi-agent-pipeline](multi-agent-pipeline.md), [incremental-reconcile](incremental-reconcile.md)

## Source
Extracted from `docs/superpowers/specs/2026-03-27-token-reduction-design.md`
(kept in place).
