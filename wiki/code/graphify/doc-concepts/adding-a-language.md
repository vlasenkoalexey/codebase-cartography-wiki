---
title: Adding a language extractor
type: doc-concept
provenance: doc
source: ARCHITECTURE.md
updated: 2026-07-04
status: fresh
---
# Adding a language extractor

## Definition
graphify's code coverage is extensible through a fixed five-step recipe. To add a language you (1) write an `extract_<lang>(path) -> dict` in `extract.py` following the existing pattern — tree-sitter parse → walk nodes → collect `nodes` and `edges` → call-graph second pass for INFERRED `calls` edges; (2) register the suffix in the `extract()` dispatch and `collect_files()`; (3) add the suffix to `CODE_EXTENSIONS` in `detect.py` and `_WATCHED_EXTENSIONS` in `watch.py`; (4) add the tree-sitter package to `pyproject.toml`; (5) add a fixture and tests.

## In graphify (grounded)
- The pattern to copy is any existing `extract_<lang>` — e.g. [`extract_python`](../catalog/graphify/extract.md#extract_python), [`extract_go`](../catalog/graphify/extract.md#extract_go), [`extract_rust`](../catalog/graphify/extract.md#extract_rust) — plus the shared call-graph pass [`walk_calls`](../catalog/graphify/extract.md#_extract_generic.walk_calls).
- Dispatch registration is the [`_DISPATCH`](../catalog/graphify/extract.md#_DISPATCH._DISPATCH) table consumed by [`extract`](../catalog/graphify/extract.md#extract) (via [`_get_extractor`](../catalog/graphify/extract.md#_get_extractor)); newer languages live under `graphify/extractors/` (see the [extractors base](../concepts/graphify-extractors-base.md)).
- Detection and watching are updated through [`CODE_EXTENSIONS`](../catalog/graphify/detect.md#CODE_EXTENSIONS) in `detect.py` and [`_WATCHED_EXTENSIONS`](../catalog/graphify/watch.md#_WATCHED_EXTENSIONS) in `watch.py`.

## Why it matters / when it applies
The uniform extractor contract (see [extraction-schema](extraction-schema.md)) is what makes this recipe short: a new grammar only has to emit the standard `{nodes, edges}` shape to join every downstream stage. This is graphify's answer to breadth — 36 tree-sitter grammars today, each added by the same steps.

## Connections
- Code concepts: [extract](../concepts/graphify-extract.md), [extractors-base](../concepts/graphify-extractors-base.md), [detect](../concepts/graphify-detect.md), [watch](../concepts/graphify-watch.md)
- Module catalogs: [extract](../catalog/graphify/extract.md), [detect](../catalog/graphify/detect.md), [watch](../catalog/graphify/watch.md), [extractors base](../catalog/graphify/extractors/base.md)
- Related doc-concepts: [extraction-schema](extraction-schema.md), [three-pass-extraction](three-pass-extraction.md)

## Source
Extracted from `ARCHITECTURE.md` ("Adding a new language extractor") (kept in place).
