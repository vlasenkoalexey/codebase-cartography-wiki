---
title: Semantic batching & output chunking
type: doc-concept
provenance: doc
source: docs/superpowers/specs/2026-05-24-semantic-batching-and-output-chunking-design.md
updated: 2026-07-04
status: fresh
---
# Semantic batching & output chunking

## Definition
Two compounding problems on output-constrained backends (notably Bedrock OPUS):
count-based batching splits files that belong to the same module across batches
(so cross-module `calls`/`related`/`inherits`/`implements` edges get dropped),
and a single dense batch can exceed the per-turn write budget, making the agent
silently drop nodes. The fix replaces count batching with **Louvain community
detection on the import graph** (a new Phase 1.5 that groups files that import
each other into one batch, and hands each `file-analyzer` a `neighborMap` of
cross-batch neighbors + their exported symbols to boost edge confidence), and adds
**output chunking**: an analyzer splits its result into `batch-<i>-part-<k>.json`
parts when it exceeds ~60 nodes / ~120 edges.

## In understand-anything (grounded)
> [!inferred]
> The core of this spec — `compute-batches.mjs` (Phase 1.5) and the `neighborMap`
> — is a proposed/draft file. It exists in the pinned source at
> `understand-anything-plugin/skills/understand/compute-batches.mjs`, but is a
> `.mjs` skill script not covered by the symbol catalog, so it has no citable
> anchor; it is described here in prose.

What *is* grounded is the merge side, which the spec confirms needs no code change
because it already tolerates multi-part input. The reducer
[`merge_and_normalize`](../catalog/understand-anything-plugin/skills/understand/merge-batch-graphs.md#merge_and_normalize)
loads every `batch-*.json` (its
[`load_batch`](../catalog/understand-anything-plugin/skills/understand/merge-batch-graphs.md#load_batch)
glob already matches `batch-3-part-1.json` and sorts parts under their logical
batch), and its final defenses hold regardless of how files were batched:
[`recover_imports_from_scan`](../catalog/understand-anything-plugin/skills/understand/merge-batch-graphs.md#recover_imports_from_scan)
restores `imports` edges from the scan, and the dangling-edge dropper removes any
edge whose target didn't survive
([`link_tests`](../catalog/understand-anything-plugin/skills/understand/merge-batch-graphs.md#link_tests)
similarly reconnects tests post-merge). The Louvain algorithm the spec adopts
(`graphology-communities-louvain`) is the same family already used on the
dashboard for clustering,
[`detectCommunities`](../catalog/understand-anything-plugin/packages/dashboard/src/utils/louvain.ts.md#detectCommunities).

## Why it matters / when it applies
This is the reliability-at-scale axis: token-reduction made runs *cheaper*;
semantic batching makes them *complete correctly* on large projects and OPUS-class
output caps, and it improves cross-module edge coverage that count batching lost.
The design is defensive by contract — every fallback (Louvain crash →
count-fallback, oversized community → split, exports failure → empty symbols,
missing part → merge warning) must emit a `Warning:` line that bubbles to the
user; silent `catch {}` is a review blocker. `scan-result.json` remains the source
of truth and the dangling-edge dropper the final guarantee, so no batching change
can produce an edge to a nonexistent node.

## Connections
- Code concepts: [merge-batch-graphs](../concepts/understand-anything-plugin-skills-understand-merge-batch-graphs.md), [normalize-graph](../concepts/understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts.md)
- Module catalogs: [skills/understand/merge-batch-graphs.py](../catalog/understand-anything-plugin/skills/understand/merge-batch-graphs.md), [dashboard/utils/louvain.ts](../catalog/understand-anything-plugin/packages/dashboard/src/utils/louvain.ts.md)
- Related doc-concepts: [token-reduction](token-reduction.md), [multi-agent-pipeline](multi-agent-pipeline.md), [knowledge-base-analysis](knowledge-base-analysis.md)

## Source
Extracted from `docs/superpowers/specs/2026-05-24-semantic-batching-and-output-chunking-design.md`
(kept in place).
