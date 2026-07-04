---
title: 'Module: tests/test_query_cli.py'
type: catalog
provenance: extracted
module: tests/test_query_cli.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_query_cli`/
symbols:
  test_query_cli_explicit_context_filter: test_query_cli_explicit_context_filter().
  test_query_cli_heuristic_context_filter: test_query_cli_heuristic_context_filter().
  test_query_cli_rejects_oversized_graph: test_query_cli_rejects_oversized_graph().
  _write_graph: _write_graph().
---
# Module: [`tests/test_query_cli.py`](../../../../../raw/code/graphify/tests/test_query_cli.py)

## Functions
- `_write_graph(tmp_path)` — [`L12`](../../../../../raw/code/graphify/tests/test_query_cli.py#L12)
- `test_query_cli_explicit_context_filter(monkeypatch, tmp_path, capsys)` — [`L24`](../../../../../raw/code/graphify/tests/test_query_cli.py#L24)
- `test_query_cli_heuristic_context_filter(monkeypatch, tmp_path, capsys)` — [`L39`](../../../../../raw/code/graphify/tests/test_query_cli.py#L39)
- `test_query_cli_rejects_oversized_graph(monkeypatch, tmp_path, capsys)` — [`L54`](../../../../../raw/code/graphify/tests/test_query_cli.py#L54) — #F4: query CLI must refuse to parse a graph.json that exceeds the cap.

