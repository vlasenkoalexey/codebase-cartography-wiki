---
title: 'Module: tests/test_ts_namespace.py'
type: catalog
provenance: extracted
module: tests/test_ts_namespace.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_ts_namespace`/
symbols:
  _has_node: _has_node().
  _node_label: _node_label().
  test_namespace_is_node: test_namespace_is_node().
  test_module_keyword_is_node: test_module_keyword_is_node().
  test_nested_namespace_name: test_nested_namespace_name().
  test_namespace_members_still_extracted: test_namespace_members_still_extracted().
  test_ambient_string_module_quotes_stripped: test_ambient_string_module_quotes_stripped().
  test_namespace_node_not_emitted_in_js: test_namespace_node_not_emitted_in_js().
  _write: _write().
---
# Module: [`tests/test_ts_namespace.py`](../../../../../raw/code/graphify/tests/test_ts_namespace.py)

## Functions
- `_has_node(result: dict, file: str, sym: str)` — [`L24`](../../../../../raw/code/graphify/tests/test_ts_namespace.py#L24)
- `_node_label(result: dict, file: str, sym: str)` — [`L19`](../../../../../raw/code/graphify/tests/test_ts_namespace.py#L19)
- `_write(path: Path, text: str)` — [`L13`](../../../../../raw/code/graphify/tests/test_ts_namespace.py#L13)
- `test_ambient_string_module_quotes_stripped(tmp_path)` — [`L62`](../../../../../raw/code/graphify/tests/test_ts_namespace.py#L62)
- `test_module_keyword_is_node(tmp_path)` — [`L35`](../../../../../raw/code/graphify/tests/test_ts_namespace.py#L35)
- `test_namespace_is_node(tmp_path)` — [`L28`](../../../../../raw/code/graphify/tests/test_ts_namespace.py#L28)
- `test_namespace_members_still_extracted(tmp_path)` — [`L49`](../../../../../raw/code/graphify/tests/test_ts_namespace.py#L49) — The container node must not cost us the members the default recurse reached.
- `test_namespace_node_not_emitted_in_js(tmp_path)` — [`L69`](../../../../../raw/code/graphify/tests/test_ts_namespace.py#L69) — The handler is TS-only; plain JS has no namespace syntax to confuse it.
- `test_nested_namespace_name(tmp_path)` — [`L42`](../../../../../raw/code/graphify/tests/test_ts_namespace.py#L42)

