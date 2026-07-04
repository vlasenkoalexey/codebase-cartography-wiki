---
title: 'Module: tests/test_ts_generators.py'
type: catalog
provenance: extracted
module: tests/test_ts_generators.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_ts_generators`/
symbols:
  test_generator_declaration_is_node_ts: test_generator_declaration_is_node_ts().
  test_generator_body_calls_are_attributed: test_generator_body_calls_are_attributed().
  _has_node: _has_node().
  test_generator_declaration_is_node_js: test_generator_declaration_is_node_js().
  test_generator_expression_is_node: test_generator_expression_is_node().
  test_async_generator_declaration_is_node: test_async_generator_declaration_is_node().
  _contains: _contains().
  _write: _write().
---
# Module: [`tests/test_ts_generators.py`](../../../../../raw/code/graphify/tests/test_ts_generators.py)

## Functions
- `_contains(result: dict, file: str, sym: str)` — [`L25`](../../../../../raw/code/graphify/tests/test_ts_generators.py#L25)
- `_has_node(result: dict, file: str, sym: str)` — [`L20`](../../../../../raw/code/graphify/tests/test_ts_generators.py#L20)
- `_write(path: Path, text: str)` — [`L14`](../../../../../raw/code/graphify/tests/test_ts_generators.py#L14)
- `test_async_generator_declaration_is_node(tmp_path)` — [`L70`](../../../../../raw/code/graphify/tests/test_ts_generators.py#L70)
- `test_generator_body_calls_are_attributed(tmp_path)` — [`L55`](../../../../../raw/code/graphify/tests/test_ts_generators.py#L55) — A call inside a generator's body should be attributed to the generator,
- `test_generator_declaration_is_node_js(tmp_path)` — [`L41`](../../../../../raw/code/graphify/tests/test_ts_generators.py#L41)
- `test_generator_declaration_is_node_ts(tmp_path)` — [`L33`](../../../../../raw/code/graphify/tests/test_ts_generators.py#L33)
- `test_generator_expression_is_node(tmp_path)` — [`L48`](../../../../../raw/code/graphify/tests/test_ts_generators.py#L48)

