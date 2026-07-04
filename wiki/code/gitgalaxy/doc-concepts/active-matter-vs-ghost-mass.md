---
title: Active Matter vs. Ghost Mass — why the Detector never lets logic and prose mix
type: doc-concept
provenance: doc
source: docs/wiki/02-08-the-detector.md
updated: 2026-07-04
status: fresh
---
# Active Matter vs. Ghost Mass — why the Detector never lets logic and prose mix

## Definition
The doc names the Detector's strict separation between executable logic ("Active Matter") and
developer literature ("Ghost Mass") as the primary defense against "Logic Erosion" — the
failure mode where a commented-out `if` statement inflates a file's complexity score because a
scanner didn't distinguish code from comments. Three claims follow from this separation: (1)
the coding-analysis engine is bound to a fixed, 51-element schema so its output dictionary can
never drift in length or key order; (2) the comment-analysis engine runs a *different*,
narrower rule set over Ghost Mass only, tracking `planned_debt` (TODOs), `fragile_debt`
(HACKs), and `graveyard` (dead code hidden in comments); and (3) even a file that fails the
structural confidence floor and is relegated entirely to "Dark Matter" still has its Ghost
Mass decoded for **Ownership** and **Architectural Purpose**, so unparsed config files and
monolithic scripts still contribute human context to the repository map.

## In gitgalaxy (grounded)
All three claims are real, and the third is confirmed by reading `splice`'s call order
directly rather than only its documented behavior:
- **The 51-element schema guarantee.** [`StructuralExtractor.coding_analysis`](../catalog/gitgalaxy/core/detector.md#StructuralExtractor.coding_analysis)
  initializes its counting dictionary as `{key: 0 for key in
  self.UNIVERSAL_METRICS_SCHEMA}`, where [`UNIVERSAL_METRICS_SCHEMA`](../catalog/gitgalaxy/core/detector.md#StructuralExtractor.UNIVERSAL_METRICS_SCHEMA)
  is itself set at class-definition time from `RECORDING_SCHEMAS.get("SIGNAL_SCHEMA", [])` —
  a custom language definition cannot inject an unregistered key because the dictionary is
  never grown beyond this fixed key set, matching the doc's "Anti-Hallucination Binding."
- **The separate comment-analysis pass.** [`StructuralExtractor.comment_analysis`](../catalog/gitgalaxy/core/detector.md#StructuralExtractor.comment_analysis)
  is a distinct method taking the `comment_stream` (never the code stream) plus the counts
  dict `coding_analysis` already populated, folding debt/graveyard/doc signals into the same
  vector without ever re-scanning executable text.
- **Metadata survives the Dark Matter bypass.** Inside [`splice`](../catalog/gitgalaxy/core/detector.md#StructuralExtractor.splice),
  reading the pinned source directly: `ghost_meta = self._decode_comment_stream(comment_stream)`
  runs *before* the confidence-floor/format bypass check, with an inline comment reading "We
  always extract the metadata first, even for Unparsable Artifacts." Every early-return path
  in `splice` — the confidence bypass and the empty-code-stream bypass alike — still packs
  `"metadata": ghost_meta` into its otherwise-empty result.
  [`StructuralExtractor._decode_comment_stream`](../catalog/gitgalaxy/core/detector.md#StructuralExtractor._decode_comment_stream)
  itself hard-caps its scan to the first 15,000 characters of the comment stream specifically
  to bound cost on huge license blocks or generated data, and defaults `ownership` to
  `"Unknown Architect"` rather than raising when no author tag is found.

## Why it matters / when it applies
The Dark Matter exception is the sharpest point here: it means a config file, a data dump, or
any file that structurally fails to parse is never *fully* invisible to the repository map —
it still contributes an author and an inferred purpose, extracted from whatever comments or
header text it carries, even though it contributes zero risk-vector or function-level signal.
This is a deliberate asymmetry: gitgalaxy trusts prose-derived metadata (ownership, purpose)
more cheaply and unconditionally than it trusts structural signal, because extracting a
comment-block author tag has none of the ambiguity that counting branches in unparseable text
would.

## Connections
- Code concepts: [The Detector](../concepts/gitgalaxy-core-detector.md) — owns `splice`,
  `coding_analysis`, `comment_analysis`, and `_decode_comment_stream`; [The Prism](../concepts/gitgalaxy-core-prism.md) —
  the upstream stage that produces the `code_stream`/`comment_stream` split this separation
  depends on being mutually exclusive in the first place.
- Module catalogs: [detector](../catalog/gitgalaxy/core/detector.md).
- Related doc-concepts: [atomic-literal-shield](atomic-literal-shield.md),
  [satellite-physics-and-naming-shields](satellite-physics-and-naming-shields.md).

## Source
Extracted from `docs/wiki/02-08-the-detector.md` ("Coding vs. Comment Analysis" section);
`docs/wiki/02-07-the-prism.md` carries an earlier draft of the same material under the
same misleading filename (see [atomic-literal-shield](atomic-literal-shield.md)'s Source note).
Both kept in place.
