---
title: Multi-source ingestion
type: doc-concept
provenance: doc
source: README.md
updated: 2026-07-04
status: fresh
---
# Multi-source ingestion

## Definition
graphify maps a whole project, not just its code: 36 tree-sitter code grammars plus Apex, Terraform/HCL, MCP configs, package manifests, docs (`.md .rst .html …`), Office files, Google Workspace, PDFs, images, and video/audio — all into one graph. Beyond files on disk, `graphify add <url>` fetches a paper (e.g. an arXiv link) or transcribes a YouTube/video URL and folds it in. This is what makes graphify a knowledge graph over "code, docs, PDFs, images, videos" rather than a code-only indexer.

## In graphify (grounded)
- File-type classification and the extension tables are `detect.py`: [`classify_file`](../catalog/graphify/detect.md#classify_file) over [`CODE_EXTENSIONS`](../catalog/graphify/detect.md#CODE_EXTENSIONS), [`DOC_EXTENSIONS`](../catalog/graphify/detect.md#DOC_EXTENSIONS), [`PAPER_EXTENSIONS`](../catalog/graphify/detect.md#PAPER_EXTENSIONS), [`IMAGE_EXTENSIONS`](../catalog/graphify/detect.md#IMAGE_EXTENSIONS), [`VIDEO_EXTENSIONS`](../catalog/graphify/detect.md#VIDEO_EXTENSIONS), [`OFFICE_EXTENSIONS`](../catalog/graphify/detect.md#OFFICE_EXTENSIONS).
- URL ingestion is `ingest.py`: [`ingest`](../catalog/graphify/ingest.md#ingest) dispatches by [`_detect_url_type`](../catalog/graphify/ingest.md#_detect_url_type) to [`_fetch_arxiv`](../catalog/graphify/ingest.md#_fetch_arxiv), [`_fetch_webpage`](../catalog/graphify/ingest.md#_fetch_webpage), [`_fetch_tweet`](../catalog/graphify/ingest.md#_fetch_tweet), or a binary download.
- Video/audio become transcripts via `transcribe.py` [`transcribe`](../catalog/graphify/transcribe.md#transcribe) / [`download_audio`](../catalog/graphify/transcribe.md#download_audio); Office/Google Workspace files are converted to Markdown sidecars by [`convert_office_file`](../catalog/graphify/detect.md#convert_office_file).
- Manifests, MCP configs, and SQL/Postgres are their own extractor paths (`manifest_ingest`, `mcp_ingest`, and `extract_sql` / `pg_introspect`).

## Why it matters / when it applies
Ingesting heterogeneous sources into one graph is what lets graphify surface *cross-source* connections — a design doc linked to the code it describes, a paper linked to its implementation — the "surprising connections" the report highlights. It is also the axis on which graphify differs from code-only comprehension tools in the survey.

## Connections
- Code concepts: [detect](../concepts/graphify-detect.md), [extractors-base](../concepts/graphify-extractors-base.md), [extract](../concepts/graphify-extract.md)
- Module catalogs: [detect](../catalog/graphify/detect.md), [ingest](../catalog/graphify/ingest.md), [transcribe](../catalog/graphify/transcribe.md)
- Related doc-concepts: [three-pass-extraction](three-pass-extraction.md), [security-validation](security-validation.md), [god-nodes-report](god-nodes-report.md)

## Source
Extracted from `README.md` ("What files it handles", "add") and `docs/how-it-works.md` (converters) (kept in place).
