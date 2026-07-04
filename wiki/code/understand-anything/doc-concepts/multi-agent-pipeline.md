---
title: Multi-agent analysis pipeline
type: doc-concept
provenance: doc
source: README.md
updated: 2026-07-04
status: fresh
---
# Multi-agent analysis pipeline

## Definition
`/understand` runs a multi-agent pipeline rather than one monolithic pass. Five
specialized agents each own one phase — `project-scanner` (discover files, detect
languages/frameworks), `file-analyzer` (extract functions/classes/imports →
nodes and edges, run in parallel batches), `architecture-analyzer` (assign
layers), `tour-builder` (generate guided tours), and `graph-reviewer` (validate
completeness and referential integrity) — with `domain-analyzer` and
`article-analyzer` added by the `/understand-domain` and `/understand-knowledge`
skills. Agents write intermediate results to disk (not back into context) and
the orchestrator assembles them into the final graph.

## In understand-anything (grounded)
The agent prompts live under `understand-anything-plugin/agents/` and
`skills/**` (markdown, not indexed as code symbols), but the deterministic
assembly they feed is grounded. Per-file results are turned into nodes/edges by
[`GraphBuilder`](../catalog/understand-anything-plugin/packages/core/src/analyzer/graph-builder.ts.md#GraphBuilder)
([`addFileWithAnalysis`](../catalog/understand-anything-plugin/packages/core/src/analyzer/graph-builder.ts.md#GraphBuilder.addFileWithAnalysis),
[`build`](../catalog/understand-anything-plugin/packages/core/src/analyzer/graph-builder.ts.md#GraphBuilder.build)).
The `architecture-analyzer` phase is backed by
[`detectLayers`](../catalog/understand-anything-plugin/packages/core/src/analyzer/layer-detector.ts.md#detectLayers)
/ [`applyLLMLayers`](../catalog/understand-anything-plugin/packages/core/src/analyzer/layer-detector.ts.md#applyLLMLayers);
`tour-builder` by [`buildTourGenerationPrompt`](../catalog/understand-anything-plugin/packages/core/src/analyzer/tour-generator.ts.md#buildTourGenerationPrompt),
[`parseTourGenerationResponse`](../catalog/understand-anything-plugin/packages/core/src/analyzer/tour-generator.ts.md#parseTourGenerationResponse),
and the deterministic fallback
[`generateHeuristicTour`](../catalog/understand-anything-plugin/packages/core/src/analyzer/tour-generator.ts.md#generateHeuristicTour).

Because `file-analyzer` runs in parallel batches, each writing its own
`batch-<N>.json`, the outputs are merged and normalized by the Python reducer
[`merge_and_normalize`](../catalog/understand-anything-plugin/skills/understand/merge-batch-graphs.md#merge_and_normalize)
(which also runs [`link_tests`](../catalog/understand-anything-plugin/skills/understand/merge-batch-graphs.md#link_tests)
and [`recover_imports_from_scan`](../catalog/understand-anything-plugin/skills/understand/merge-batch-graphs.md#recover_imports_from_scan)),
plus the TypeScript
[`normalizeBatchOutput`](../catalog/understand-anything-plugin/packages/core/src/analyzer/normalize-graph.ts.md#normalizeBatchOutput).
The `graph-reviewer` phase reduces to
[`validateGraph`](../catalog/understand-anything-plugin/packages/core/src/schema.ts.md#validateGraph)
/ [`autoFixGraph`](../catalog/understand-anything-plugin/packages/core/src/schema.ts.md#autoFixGraph)
on the happy path (the full LLM reviewer is gated behind `--review` — see
token-reduction).

## Why it matters / when it applies
The pipeline shape is what makes the tool scale to 200k-line codebases: work is
sharded across parallel `file-analyzer` batches (up to 5 concurrent, 20–30 files
each), agents pass state through disk so no single context holds the whole
project, and the deterministic reducer/validator guarantees a well-formed graph
even from partial or noisy agent output. This phased, disk-backed decomposition
is the operational counterpart to the tree-sitter+LLM split.

## Connections
- Code concepts: [graph-builder](../concepts/understand-anything-plugin-packages-core-src-analyzer-graph-builder.ts.md), [normalize-graph](../concepts/understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts.md), [schema](../concepts/understand-anything-plugin-packages-core-src-schema.ts.md), [merge-batch-graphs](../concepts/understand-anything-plugin-skills-understand-merge-batch-graphs.md)
- Module catalogs: [analyzer/graph-builder.ts](../catalog/understand-anything-plugin/packages/core/src/analyzer/graph-builder.ts.md), [analyzer/layer-detector.ts](../catalog/understand-anything-plugin/packages/core/src/analyzer/layer-detector.ts.md), [analyzer/tour-generator.ts](../catalog/understand-anything-plugin/packages/core/src/analyzer/tour-generator.ts.md), [skills/understand/merge-batch-graphs.py](../catalog/understand-anything-plugin/skills/understand/merge-batch-graphs.md), [schema.ts](../catalog/understand-anything-plugin/packages/core/src/schema.ts.md)
- Related doc-concepts: [tree-sitter-llm-hybrid](tree-sitter-llm-hybrid.md), [knowledge-graph-schema](knowledge-graph-schema.md), [token-reduction](token-reduction.md), [semantic-batching-output-chunking](semantic-batching-output-chunking.md), [incremental-reconcile](incremental-reconcile.md)

## Source
Extracted from `README.md` (§ Under the Hood — Multi-Agent Pipeline) and
`docs/superpowers/specs/2026-03-14-understand-anything-design.md` (§ Claude Code
Skill Commands, Implementation Phases) — kept in place.
