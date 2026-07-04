---
title: The three extraction passes
type: doc-concept
provenance: doc
source: docs/how-it-works.md
updated: 2026-07-04
status: fresh
---
# The three extraction passes

## Definition
graphify separates extraction into three passes by input type, so most of a project is turned into a graph without any API calls. **Pass 1 — code structure** parses code files locally with tree-sitter (classes, functions, imports, call graphs, comments), no LLM. **Pass 2 — video/audio** transcribes media locally with faster-whisper. **Pass 3 — docs/papers/images** runs LLM subagents in parallel over markdown, PDFs, images, and transcripts. If a corpus is code-only, Pass 3 is skipped entirely — semantic extraction is reserved for prose.

## In graphify (grounded)
- **Pass 1 (code, local)** is the tree-sitter path in `extract.py`: the `extract()` dispatcher [`extract`](../catalog/graphify/extract.md#extract) routes each suffix through its `_DISPATCH` table ([`_DISPATCH`](../catalog/graphify/extract.md#_DISPATCH._DISPATCH)) to a per-language `extract_<lang>` (e.g. [`extract_python`](../catalog/graphify/extract.md#extract_python)), then a call-graph second pass ([`walk_calls`](../catalog/graphify/extract.md#_extract_generic.walk_calls)) adds inferred `calls` edges. `detect.py` decides what counts as code via [`CODE_EXTENSIONS`](../catalog/graphify/detect.md#CODE_EXTENSIONS) and [`classify_file`](../catalog/graphify/detect.md#classify_file).
- **Pass 2 (media, local)** is `transcribe.py`: [`transcribe_all`](../catalog/graphify/transcribe.md#transcribe_all) / [`transcribe`](../catalog/graphify/transcribe.md#transcribe), with the whisper prompt seeded by top god nodes via [`build_whisper_prompt`](../catalog/graphify/transcribe.md#build_whisper_prompt).
- **Pass 3 (semantic, LLM)** is dispatched to the assistant's model; before it runs, converters turn pointer/binary formats into Markdown sidecars — e.g. [`convert_office_file`](../catalog/graphify/detect.md#convert_office_file) / [`docx_to_markdown`](../catalog/graphify/detect.md#docx_to_markdown).

## Why it matters / when it applies
The split is graphify's core privacy and cost story: code — the bulk of most repos — never leaves the machine and costs no tokens, and a code-only corpus runs fully offline. LLM spend is confined to the docs/papers/images that genuinely need semantic reading.

## Connections
- Code concepts: [extract](../concepts/graphify-extract.md), [detect](../concepts/graphify-detect.md)
- Module catalogs: [extract](../catalog/graphify/extract.md), [detect](../catalog/graphify/detect.md), [transcribe](../catalog/graphify/transcribe.md)
- Related doc-concepts: [ingest-pipeline](ingest-pipeline.md), [parallel-extraction](parallel-extraction.md), [multi-source-ingestion](multi-source-ingestion.md), [content-hash-cache](content-hash-cache.md)

## Source
Extracted from `docs/how-it-works.md` (kept in place).
