---
title: 'Module: graphify/querylog.py'
type: catalog
provenance: extracted
module: graphify/querylog.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `graphify.querylog`/
symbols:
  log_query: log_query().
  nodes_from_result: nodes_from_result().
  _NODES_RE: _NODES_RE.
  _log_path: _log_path().
  _log_responses: _log_responses().
---
# Module: [`graphify/querylog.py`](../../../../../raw/code/graphify/graphify/querylog.py)

## Functions
- `_log_path()` — [`L15`](../../../../../raw/code/graphify/graphify/querylog.py#L15)
- `_log_responses()` — [`L24`](../../../../../raw/code/graphify/graphify/querylog.py#L24)
- `log_query(*, kind: str, question: str, corpus: str, result: str | None = None, nodes_returned: int | None = None, duration_ms: float | None = None, **extra: Any)` — [`L33`](../../../../../raw/code/graphify/graphify/querylog.py#L33) — Append one JSONL record to the query log. Never raises. — documented in [graphify-serve](../../concepts/graphify-serve.md)
- `nodes_from_result(result: str)` — [`L28`](../../../../../raw/code/graphify/graphify/querylog.py#L28)

## Module values
- `_NODES_RE` — [`L12`](../../../../../raw/code/graphify/graphify/querylog.py#L12)

