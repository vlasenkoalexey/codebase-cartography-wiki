---
title: 'Module: tests/test_querylog.py'
type: catalog
provenance: extracted
module: tests/test_querylog.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_querylog`/test_
symbols:
  test_nodes_from_result_parses_header: nodes_from_result_parses_header().
  test_nodes_from_result_singular: nodes_from_result_singular().
  test_nodes_from_result_missing: nodes_from_result_missing().
  test_nodes_from_result_empty: nodes_from_result_empty().
  test_log_query_writes_jsonl: log_query_writes_jsonl().
  test_log_query_appends: log_query_appends().
  test_disable_env: disable_env().
  test_disable_env_true: disable_env_true().
  test_responses_not_logged_by_default: responses_not_logged_by_default().
  test_responses_optin: responses_optin().
  test_log_never_raises: log_never_raises().
  test_log_creates_parent_dirs: log_creates_parent_dirs().
  test_nodes_returned_inferred_from_result: nodes_returned_inferred_from_result().
  test_explicit_nodes_returned_takes_precedence: explicit_nodes_returned_takes_precedence().
  test_kind_mcp_query: kind_mcp_query().
---
# Module: [`tests/test_querylog.py`](../../../../../raw/code/graphify/tests/test_querylog.py)

## Functions
- `test_disable_env(tmp_path, monkeypatch)` — [`L74`](../../../../../raw/code/graphify/tests/test_querylog.py#L74)
- `test_disable_env_true(tmp_path, monkeypatch)` — [`L84`](../../../../../raw/code/graphify/tests/test_querylog.py#L84)
- `test_explicit_nodes_returned_takes_precedence(tmp_path, monkeypatch)` — [`L159`](../../../../../raw/code/graphify/tests/test_querylog.py#L159)
- `test_kind_mcp_query(tmp_path, monkeypatch)` — [`L170`](../../../../../raw/code/graphify/tests/test_querylog.py#L170)
- `test_log_creates_parent_dirs(tmp_path, monkeypatch)` — [`L133`](../../../../../raw/code/graphify/tests/test_querylog.py#L133)
- `test_log_never_raises(tmp_path, monkeypatch)` — [`L122`](../../../../../raw/code/graphify/tests/test_querylog.py#L122)
- `test_log_query_appends(tmp_path, monkeypatch)` — [`L56`](../../../../../raw/code/graphify/tests/test_querylog.py#L56)
- `test_log_query_writes_jsonl(tmp_path, monkeypatch)` — [`L35`](../../../../../raw/code/graphify/tests/test_querylog.py#L35)
- `test_nodes_from_result_empty()` — [`L27`](../../../../../raw/code/graphify/tests/test_querylog.py#L27)
- `test_nodes_from_result_missing()` — [`L23`](../../../../../raw/code/graphify/tests/test_querylog.py#L23)
- `test_nodes_from_result_parses_header()` — [`L14`](../../../../../raw/code/graphify/tests/test_querylog.py#L14)
- `test_nodes_from_result_singular()` — [`L19`](../../../../../raw/code/graphify/tests/test_querylog.py#L19)
- `test_nodes_returned_inferred_from_result(tmp_path, monkeypatch)` — [`L147`](../../../../../raw/code/graphify/tests/test_querylog.py#L147)
- `test_responses_not_logged_by_default(tmp_path, monkeypatch)` — [`L94`](../../../../../raw/code/graphify/tests/test_querylog.py#L94)
- `test_responses_optin(tmp_path, monkeypatch)` — [`L106`](../../../../../raw/code/graphify/tests/test_querylog.py#L106)

