---
title: 'Module: src/search/identifier-segments.ts'
type: catalog
provenance: extracted
module: src/search/identifier-segments.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/search/`identifier-segments.ts`/
symbols:
  extractProseCandidates: extractProseCandidates().
  splitIdentifierSegments: splitIdentifierSegments().
  segmentLookupVariants: segmentLookupVariants().
  MIN_PROSE_CHARS: MIN_PROSE_CHARS.
  MAX_PROSE_CHARS: MAX_PROSE_CHARS.
  MIN_SEGMENT_CHARS: MIN_SEGMENT_CHARS.
  MAX_SEGMENT_CHARS: MAX_SEGMENT_CHARS.
  MAX_SEGMENTS_PER_NAME: MAX_SEGMENTS_PER_NAME.
  normalizeProseWord: normalizeProseWord().
  MAX_PROSE_CANDIDATES: MAX_PROSE_CANDIDATES.
  ENGLISH_PROSE_STOPWORDS: ENGLISH_PROSE_STOPWORDS.
---
# Module: [`src/search/identifier-segments.ts`](../../../../../../raw/code/codegraph/src/search/identifier-segments.ts)

## Functions
- `extractProseCandidates(prompt: string)` — [`L114`](../../../../../../raw/code/codegraph/src/search/identifier-segments.ts#L114) — Candidate words from a prompt for segment-vocabulary lookup, in order of
- `normalizeProseWord(word: string)` — [`L56`](../../../../../../raw/code/codegraph/src/search/identifier-segments.ts#L56) — Normalize a prose word for segment lookup: lowercase + strip diacritics
- `segmentLookupVariants(word: string)` — [`L147`](../../../../../../raw/code/codegraph/src/search/identifier-segments.ts#L147) — Lookup variants for a prose word: the word itself plus light plural folding
- `splitIdentifierSegments(name: string)` — [`L30`](../../../../../../raw/code/codegraph/src/search/identifier-segments.ts#L30) — Split a symbol or file name into lowercase word segments.

## Module values
- `ENGLISH_PROSE_STOPWORDS` — [`L81`](../../../../../../raw/code/codegraph/src/search/identifier-segments.ts#L81) — English prompt words that are never evidence a symbol was NAMED, however
- `MAX_PROSE_CANDIDATES` — [`L62`](../../../../../../raw/code/codegraph/src/search/identifier-segments.ts#L62) — Candidate cap: a prompt's first words carry its subject; scanning an essay
- `MAX_PROSE_CHARS` — [`L64`](../../../../../../raw/code/codegraph/src/search/identifier-segments.ts#L64)
- `MAX_SEGMENTS_PER_NAME` — [`L20`](../../../../../../raw/code/codegraph/src/search/identifier-segments.ts#L20)
- `MAX_SEGMENT_CHARS` — [`L19`](../../../../../../raw/code/codegraph/src/search/identifier-segments.ts#L19)
- `MIN_PROSE_CHARS` — [`L63`](../../../../../../raw/code/codegraph/src/search/identifier-segments.ts#L63)
- `MIN_SEGMENT_CHARS` — [`L18`](../../../../../../raw/code/codegraph/src/search/identifier-segments.ts#L18) — Bounds keep degenerate identifiers (minified names, hashes) from bloating

