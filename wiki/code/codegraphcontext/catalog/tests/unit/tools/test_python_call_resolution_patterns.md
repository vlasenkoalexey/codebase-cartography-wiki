---
title: 'Module: tests/unit/tools/test_python_call_resolution_patterns.py'
type: catalog
provenance: extracted
module: tests/unit/tools/test_python_call_resolution_patterns.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `tests.unit.tools.test_python_call_resolution_patterns`/
symbols:
  _resolve_file: _resolve_file().
  TestPythonCallResolutionPatterns.test_list_comprehension_calls_square: TestPythonCallResolutionPatterns#test_list_comprehension_calls_square().
  TestPythonCallResolutionPatterns.test_higher_order_calls_parameter_func: TestPythonCallResolutionPatterns#test_higher_order_calls_parameter_func().
  TestPythonCallResolutionPatterns.test_super_greet_resolves_to_parent_class: TestPythonCallResolutionPatterns#test_super_greet_resolves_to_parent_class().
  _fn_edges: _fn_edges().
  SAMPLE_PROJECT: SAMPLE_PROJECT.
  parser: parser().
  TestPythonCallResolutionPatterns: TestPythonCallResolutionPatterns#
---
# Module: [`tests/unit/tools/test_python_call_resolution_patterns.py`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_python_call_resolution_patterns.py)

## Classes
### `TestPythonCallResolutionPatterns`
- def: [`tests/unit/tools/test_python_call_resolution_patterns.py:50`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_python_call_resolution_patterns.py#L50)
- signature: `class TestPythonCallResolutionPatterns:`
- members:
  - `test_higher_order_calls_parameter_func(self, parser)` — [`L60`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_python_call_resolution_patterns.py#L60) — ID 2: higher_order(func, data) -> CALLS Parameter:func.
  - `test_list_comprehension_calls_square(self, parser)` — [`L51`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_python_call_resolution_patterns.py#L51) — ID 1: calls() -> square inside list comprehension.
  - `test_super_greet_resolves_to_parent_class(self, parser)` — [`L70`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_python_call_resolution_patterns.py#L70) — ID 3: B.greet super().greet() -> A.greet.
- uses (calls/refs, reference-scoped): (2 test-only callers)

## Functions
- `_fn_edges(groups)` — [`L44`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_python_call_resolution_patterns.py#L44)
- `_resolve_file(parser, relative_path: str)` — [`L30`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_python_call_resolution_patterns.py#L30)
- `parser()` — [`L21`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_python_call_resolution_patterns.py#L21)

## Module values
- `SAMPLE_PROJECT` — [`L12`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_python_call_resolution_patterns.py#L12)

