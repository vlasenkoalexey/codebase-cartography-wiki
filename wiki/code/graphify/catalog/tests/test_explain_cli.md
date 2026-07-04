---
title: 'Module: tests/test_explain_cli.py'
type: catalog
provenance: extracted
module: tests/test_explain_cli.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_explain_cli`/
symbols:
  _run: _run().
  test_explain_shows_preferred_lesson_line: test_explain_shows_preferred_lesson_line().
  test_explain_shows_contested_and_stale_lesson: test_explain_shows_contested_and_stale_lesson().
  _write_graph: _write_graph().
  test_callee_shows_callers_as_inbound: test_callee_shows_callers_as_inbound().
  test_caller_shows_callee_as_outbound: test_caller_shows_callee_as_outbound().
  test_explain_no_lesson_line_for_unannotated_node: test_explain_no_lesson_line_for_unannotated_node().
  test_explain_source_file_path_prefers_file_level_node: test_explain_source_file_path_prefers_file_level_node().
  _write_sidecar: _write_sidecar().
---
# Module: [`tests/test_explain_cli.py`](../../../../../raw/code/graphify/tests/test_explain_cli.py)

## Functions
- `_run(monkeypatch, graph_path, label, capsys)` — [`L34`](../../../../../raw/code/graphify/tests/test_explain_cli.py#L34)
- `_write_graph(tmp_path)` — [`L7`](../../../../../raw/code/graphify/tests/test_explain_cli.py#L7)
- `_write_sidecar(tmp_path, nodes)` — [`L87`](../../../../../raw/code/graphify/tests/test_explain_cli.py#L87)
- `test_callee_shows_callers_as_inbound(monkeypatch, tmp_path, capsys)` — [`L42`](../../../../../raw/code/graphify/tests/test_explain_cli.py#L42)
- `test_caller_shows_callee_as_outbound(monkeypatch, tmp_path, capsys)` — [`L52`](../../../../../raw/code/graphify/tests/test_explain_cli.py#L52)
- `test_explain_no_lesson_line_for_unannotated_node(monkeypatch, tmp_path, capsys)` — [`L121`](../../../../../raw/code/graphify/tests/test_explain_cli.py#L121) — No sidecar => no Lesson line; output identical to pre-feature.
- `test_explain_shows_contested_and_stale_lesson(monkeypatch, tmp_path, capsys)` — [`L107`](../../../../../raw/code/graphify/tests/test_explain_cli.py#L107)
- `test_explain_shows_preferred_lesson_line(monkeypatch, tmp_path, capsys)` — [`L95`](../../../../../raw/code/graphify/tests/test_explain_cli.py#L95)
- `test_explain_source_file_path_prefers_file_level_node(monkeypatch, tmp_path, capsys)` — [`L59`](../../../../../raw/code/graphify/tests/test_explain_cli.py#L59)

