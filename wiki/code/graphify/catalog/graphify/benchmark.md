---
title: 'Module: graphify/benchmark.py'
type: catalog
provenance: extracted
module: graphify/benchmark.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `graphify.benchmark`/
symbols:
  run_benchmark: run_benchmark().
  _query_subgraph_tokens: _query_subgraph_tokens().
  print_benchmark: print_benchmark().
  _hr: _hr().
  _safe: _safe().
  _estimate_tokens: _estimate_tokens().
  _SAMPLE_QUESTIONS: _SAMPLE_QUESTIONS.
  _CHARS_PER_TOKEN: _CHARS_PER_TOKEN.
---
# Module: [`graphify/benchmark.py`](../../../../../raw/code/graphify/graphify/benchmark.py)

## Functions
- `_estimate_tokens(text: str)` — [`L36`](../../../../../raw/code/graphify/graphify/benchmark.py#L36)
- `_hr(width: int = 50)` — [`L31`](../../../../../raw/code/graphify/graphify/benchmark.py#L31) — Horizontal rule that survives non-UTF-8 stdout (e.g. Windows cp1252 console).
- `_query_subgraph_tokens(G: nx.Graph, question: str, depth: int = 3)` — [`L40`](../../../../../raw/code/graphify/graphify/benchmark.py#L40) — Run BFS from best-matching nodes and return estimated tokens in the subgraph context.
- `_safe(unicode_char: str, ascii_fallback: str)` — [`L17`](../../../../../raw/code/graphify/graphify/benchmark.py#L17) — Return unicode_char if stdout can encode it, else ascii_fallback.
- `print_benchmark(result: dict)` — [`L141`](../../../../../raw/code/graphify/graphify/benchmark.py#L141) — Print a human-readable benchmark report.
- `run_benchmark(graph_path: str | None = None, corpus_words: int | None = None, questions: list[str] | None = None)` — [`L88`](../../../../../raw/code/graphify/graphify/benchmark.py#L88) — Measure token reduction: corpus tokens vs graphify query tokens. — documented in [graphify-paths](../../concepts/graphify-paths.md)

## Module values
- `_CHARS_PER_TOKEN` — [`L14`](../../../../../raw/code/graphify/graphify/benchmark.py#L14)
- `_SAMPLE_QUESTIONS` — [`L79`](../../../../../raw/code/graphify/graphify/benchmark.py#L79)

