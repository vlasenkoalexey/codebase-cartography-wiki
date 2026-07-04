---
title: 'Module: graphify/ingest.py'
type: catalog
provenance: extracted
module: graphify/ingest.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `graphify.ingest`/
symbols:
  save_query_result: save_query_result().
  ingest: ingest().
  _yaml_str: _yaml_str().
  _fetch_webpage: _fetch_webpage().
  _fetch_arxiv: _fetch_arxiv().
  _fetch_tweet: _fetch_tweet().
  out: out.
  parser: parser.
  _download_binary: _download_binary().
  args: args.
  OUTCOMES: OUTCOMES.
  _fetch_html: _fetch_html().
  _safe_filename: _safe_filename().
  _detect_url_type: _detect_url_type().
  _html_to_markdown: _html_to_markdown().
---
# Module: [`graphify/ingest.py`](../../../../../raw/code/graphify/graphify/ingest.py)

## Functions
- `_detect_url_type(url: str)` — [`L64`](../../../../../raw/code/graphify/graphify/ingest.py#L64) — Classify the URL for targeted extraction.
- `_download_binary(url: str, suffix: str, target_dir: Path)` — [`L210`](../../../../../raw/code/graphify/graphify/ingest.py#L210) — Download a binary file (PDF, image) directly.
- `_fetch_arxiv(url: str, author: str | None, contributor: str | None)` — [`L165`](../../../../../raw/code/graphify/graphify/ingest.py#L165) — Fetch arXiv abstract page.
- `_fetch_html(url: str)` — [`L84`](../../../../../raw/code/graphify/graphify/ingest.py#L84)
- `_fetch_tweet(url: str, author: str | None, contributor: str | None)` — [`L103`](../../../../../raw/code/graphify/graphify/ingest.py#L103) — Fetch a tweet URL. Returns (content, filename).
- `_fetch_webpage(url: str, author: str | None, contributor: str | None)` — [`L136`](../../../../../raw/code/graphify/graphify/ingest.py#L136) — Fetch a generic webpage and convert to markdown.
- `_html_to_markdown(html: str, url: str)` — [`L88`](../../../../../raw/code/graphify/graphify/ingest.py#L88) — Convert HTML to clean markdown. Uses markdownify if available, else basic strip.
- `_safe_filename(url: str, suffix: str)` — [`L55`](../../../../../raw/code/graphify/graphify/ingest.py#L55) — Turn a URL into a safe filename.
- `_yaml_str(s: str)` — [`L13`](../../../../../raw/code/graphify/graphify/ingest.py#L13) — Escape a string for embedding in a YAML double-quoted scalar.
- `ingest(url: str, target_dir: Path, author: str | None = None, contributor: str | None = None)` — [`L218`](../../../../../raw/code/graphify/graphify/ingest.py#L218) — Fetch a URL and save it into target_dir as a graphify-ready file.
- `save_query_result(question: str, answer: str, memory_dir: Path, query_type: str = "query", source_nodes: list[str] | None = None, outcome: str | None = None, correction: str | None = None)` — [`L274`](../../../../../raw/code/graphify/graphify/ingest.py#L274) — Save a Q&A result as markdown so it gets extracted into the graph on next --update. — documented in [graphify-__main__](../../concepts/graphify-__main__.md)

## Module values
- `OUTCOMES` — [`L271`](../../../../../raw/code/graphify/graphify/ingest.py#L271) — documented in [graphify-reflect](../../concepts/graphify-reflect.md)
- `args` — [`L351`](../../../../../raw/code/graphify/graphify/ingest.py#L351)
- `out` — [`L352`](../../../../../raw/code/graphify/graphify/ingest.py#L352)
- `parser` — [`L346`](../../../../../raw/code/graphify/graphify/ingest.py#L346)

