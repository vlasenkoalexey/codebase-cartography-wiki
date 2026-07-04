---
title: Incremental reconcile & staleness detection
type: doc-concept
provenance: doc
source: docs/superpowers/specs/2026-03-14-understand-anything-design.md
updated: 2026-07-04
status: fresh
---
# Incremental reconcile & staleness detection

## Definition
The knowledge graph is persisted to `.understand-anything/` and kept current
without re-analyzing the whole project. On each run the skill compares the last
analyzed commit against `HEAD`, re-analyzes only the changed files, and **merges**
the new results into the existing graph. The graph is committable, so a team can
commit it once and skip the pipeline; a post-commit hook (`--auto-update`) keeps
it fresh incrementally. This is the tool's answer to "how does it stay current at
low cost" — the same axis as wikify-repo's `ingest --ref` delta rebuild.

## In understand-anything (grounded)
Change detection is structural, not just mtime-based. `packages/core/src/fingerprint.ts`
hashes each file's extracted structure —
[`extractFileFingerprint`](../catalog/understand-anything-plugin/packages/core/src/fingerprint.ts.md#extractFileFingerprint),
[`compareFingerprints`](../catalog/understand-anything-plugin/packages/core/src/fingerprint.ts.md#compareFingerprints),
[`analyzeChanges`](../catalog/understand-anything-plugin/packages/core/src/fingerprint.ts.md#analyzeChanges)
— and classifies each file by
[`ChangeLevel`](../catalog/understand-anything-plugin/packages/core/src/fingerprint.ts.md#ChangeLevel)
so a cosmetic-only edit doesn't trigger re-analysis. Git-level staleness is
`packages/core/src/staleness.ts`:
[`isStale`](../catalog/understand-anything-plugin/packages/core/src/staleness.ts.md#isStale),
[`getChangedFiles`](../catalog/understand-anything-plugin/packages/core/src/staleness.ts.md#getChangedFiles),
and the merge itself,
[`mergeGraphUpdate`](../catalog/understand-anything-plugin/packages/core/src/staleness.ts.md#mergeGraphUpdate).
The decision of *what* to rebuild (which files, whether to rerun architecture or
tour) is [`classifyUpdate`](../catalog/understand-anything-plugin/packages/core/src/change-classifier.ts.md#classifyUpdate)
→ [`UpdateDecision`](../catalog/understand-anything-plugin/packages/core/src/change-classifier.ts.md#UpdateDecision).

Persistence is `packages/core/src/persistence/index.ts`:
[`loadGraph`](../catalog/understand-anything-plugin/packages/core/src/persistence/index.ts.md#loadGraph)
/ [`saveGraph`](../catalog/understand-anything-plugin/packages/core/src/persistence/index.ts.md#saveGraph),
[`loadMeta`](../catalog/understand-anything-plugin/packages/core/src/persistence/index.ts.md#loadMeta)
/ [`saveMeta`](../catalog/understand-anything-plugin/packages/core/src/persistence/index.ts.md#saveMeta)
(the last-analyzed commit hash), and the fingerprint store
[`loadFingerprints`](../catalog/understand-anything-plugin/packages/core/src/persistence/index.ts.md#loadFingerprints)
/ [`saveFingerprints`](../catalog/understand-anything-plugin/packages/core/src/persistence/index.ts.md#saveFingerprints)
under [`UA_DIR`](../catalog/understand-anything-plugin/packages/core/src/persistence/index.ts.md#UA_DIR).

## Why it matters / when it applies
The README calls out the cost asymmetry directly: the first `/understand` is
expensive, but "subsequent runs are incremental by default — only changed files
are re-analyzed — so they use far fewer tokens." Committing the graph turns
onboarding, PR review, and docs-as-code into a zero-pipeline experience for
teammates. Structural fingerprints are what make this safe: a reformatting-only
diff is recognized as cosmetic and skipped, so incremental runs stay cheap and
the graph stays trustworthy.

## Connections
- Code concepts: [fingerprint](../concepts/understand-anything-plugin-packages-core-src-fingerprint.ts.md), [persistence](../concepts/understand-anything-plugin-packages-core-src-persistence-index.ts.md)
- Module catalogs: [fingerprint.ts](../catalog/understand-anything-plugin/packages/core/src/fingerprint.ts.md), [staleness.ts](../catalog/understand-anything-plugin/packages/core/src/staleness.ts.md), [change-classifier.ts](../catalog/understand-anything-plugin/packages/core/src/change-classifier.ts.md), [persistence/index.ts](../catalog/understand-anything-plugin/packages/core/src/persistence/index.ts.md)
- Related doc-concepts: [multi-agent-pipeline](multi-agent-pipeline.md), [token-reduction](token-reduction.md), [semantic-batching-output-chunking](semantic-batching-output-chunking.md)

## Source
Extracted from `docs/superpowers/specs/2026-03-14-understand-anything-design.md`
(§ Persistence & Staleness Detection) and `README.md` (§ Share the Graph with
Your Team; token-usage note) — kept in place.
