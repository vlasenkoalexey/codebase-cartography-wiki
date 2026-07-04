---
title: Polyglot handshake detection — from lang_mix telemetry to Language Sliding
type: doc-concept
provenance: doc
source: docs/wiki/02-05-language-lens.md
updated: 2026-07-04
status: fresh
---
# Polyglot handshake detection — from lang_mix telemetry to Language Sliding

## Definition
Modern files are frequently multi-language (HTML embedding JavaScript, C embedding inline
assembly, PHP embedding HTML), and a single-language classification would misapply one
language's regex rules to another language's text. The Language Lens doc describes a
"Handshake Protocol": a registry of transition triggers (`<script>`, `asm!()`, `SELECT`, …)
that the Lens scans for, tracking paired-bracket nesting depth to measure the exact
byte-length of each embedded "alien" segment. The output is a `lang_mix` telemetry array
(e.g. "80% HTML, 20% JavaScript") that — the doc states — "is passed down the pipeline,
signaling the Primary Detector to actively swap its regular expressions (**Language
Sliding**) when processing the file's structural physics." This page traces that signal from
where it is produced (the Lens) to where it is consumed (the Detector).

## In gitgalaxy (grounded)
- **Production, in the Lens.** [`_detect_hybrids`](../catalog/gitgalaxy/standards/language_lens.md#LanguageDetector._detect_hybrids)
  walks the compiled [`HANDSHAKE_REGISTRY`](../catalog/gitgalaxy/standards/language_lens.md#LanguageDetector.HANDSHAKE_REGISTRY)
  (trigger/end/target/pair tuples) and, for paired delimiters, uses
  [`_find_balanced_end`](../catalog/gitgalaxy/standards/language_lens.md#LanguageDetector._find_balanced_end)
  (a string-aware bracket matcher bounded by the same lookahead limit as unpaired handshakes)
  to measure how much of the file is a secondary embedded language.
- **Consumption, in the Detector.** [`splice`](../catalog/gitgalaxy/core/detector.md#StructuralExtractor.splice)
  partitions its shielded stream into per-language segments via
  [`_partition_segments`](../catalog/gitgalaxy/core/detector.md#StructuralExtractor._partition_segments)
  (read directly from the pinned source; not previously cited in this silo's concept pages) —
  "so an embedded `<script>` or `asm!()` block is scanned under its own rules," in the words
  of the existing Detector concept page. [`test_detector_embedded_language_partitioning`](../catalog/tests/core_engine/test_detector.md#test_detector_embedded_language_partitioning)
  confirms the engine "dynamically swaps languages mid-file" — this is "Language Sliding" by
  another name, exercised as a real, tested behavior rather than only a docs claim. The
  `HANDSHAKE_LOOKAHEAD_LIMIT` (50,000 characters) that bounds this scan is shared machinery
  with the Lens's own handshake search.
- **A third, parallel implementation in the Prism.** [`_partition_embedded_languages`](../catalog/gitgalaxy/core/prism.md#Prism._partition_embedded_languages)
  performs the analogous split one stage earlier, before comment-stripping, guarded by its own
  cheap literal-substring pre-check (the "Universal Web Tax Shield") — the same architectural
  idea (detect a trigger, resolve its balanced end, treat the interior as a different
  language) is implemented independently in three different modules rather than shared as one
  utility.

## Why it matters / when it applies
This is a case where the same conceptual mechanism — "detect an embedded-language boundary
with a bounded, string-aware bracket scan" — recurs at three separate stages of the pipeline
(Language Lens, Prism, Detector) with three separate implementations rather than one shared
function. That is consistent with this survey's broader observation about gitgalaxy: each
module is independently defensive rather than composed from a shared parsing core, because
there is no shared AST or IR that a "parse once, reuse everywhere" design would need. The
`lang_mix` telemetry is also, per the doc, meant to feed the Cartographer's visualization (see
[the-cartographer-spatial-positioning](the-cartographer-spatial-positioning.md)) so a
polyglot file's structure is represented honestly in the 3D map rather than collapsed to one
language.

## Connections
- Code concepts: [Language lens](../concepts/gitgalaxy-standards-language_lens.md) — produces
  `lang_mix`; [The Detector](../concepts/gitgalaxy-core-detector.md) — consumes it via segment
  partitioning; [The Prism](../concepts/gitgalaxy-core-prism.md) — the third, independent
  embedded-language splitter.
- Module catalogs: [language_lens](../catalog/gitgalaxy/standards/language_lens.md),
  [detector](../catalog/gitgalaxy/core/detector.md), [prism](../catalog/gitgalaxy/core/prism.md).
- Related doc-concepts: [ecosystem-gravity-and-confidence-override](ecosystem-gravity-and-confidence-override.md),
  [atomic-literal-shield](atomic-literal-shield.md).

## Source
Extracted from `docs/wiki/02-05-language-lens.md` ("Hybrid Detection" section), cross-referenced
against `docs/wiki/02-08-the-detector.md`'s "Metric Vectorization" section for the consumer
side; both kept in place.
