---
title: 'Module: tests/test_corrupt_graph_json.py'
type: catalog
provenance: extracted
module: tests/test_corrupt_graph_json.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_corrupt_graph_json`/
symbols:
  test_valid_graph_still_loads: test_valid_graph_still_loads().
  _corrupt: _corrupt().
  test_build_merge_corrupt_graph_raises_runtimeerror: test_build_merge_corrupt_graph_raises_runtimeerror().
  test_affected_load_graph_corrupt_raises_runtimeerror: test_affected_load_graph_corrupt_raises_runtimeerror().
  test_diagnostics_read_corrupt_raises_runtimeerror: test_diagnostics_read_corrupt_raises_runtimeerror().
  _CORRUPT: _CORRUPT.
---
# Module: [`tests/test_corrupt_graph_json.py`](../../../../../raw/code/graphify/tests/test_corrupt_graph_json.py)

## Functions
- `_corrupt(tmp_path)` — [`L19`](../../../../../raw/code/graphify/tests/test_corrupt_graph_json.py#L19)
- `test_affected_load_graph_corrupt_raises_runtimeerror(tmp_path)` — [`L31`](../../../../../raw/code/graphify/tests/test_corrupt_graph_json.py#L31)
- `test_build_merge_corrupt_graph_raises_runtimeerror(tmp_path)` — [`L25`](../../../../../raw/code/graphify/tests/test_corrupt_graph_json.py#L25)
- `test_diagnostics_read_corrupt_raises_runtimeerror(tmp_path)` — [`L37`](../../../../../raw/code/graphify/tests/test_corrupt_graph_json.py#L37)
- `test_valid_graph_still_loads(tmp_path)` — [`L43`](../../../../../raw/code/graphify/tests/test_corrupt_graph_json.py#L43) — Happy path unchanged: a well-formed graph.json loads without raising.

## Module values
- `_CORRUPT` — [`L16`](../../../../../raw/code/graphify/tests/test_corrupt_graph_json.py#L16)

