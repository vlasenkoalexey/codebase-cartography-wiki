---
title: 'Module: tests/unit/parsers/test_python_parser.py'
type: catalog
provenance: extracted
module: tests/unit/parsers/test_python_parser.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `tests.unit.parsers.test_python_parser`/TestPythonParser#
symbols:
  TestPythonParser: ''
  TestPythonParser.parser: parser().
  TestPythonParser.test_parse_simple_function: test_parse_simple_function().
  TestPythonParser.test_module_level_call_uses_module_context: test_module_level_call_uses_module_context().
  TestPythonParser.test_duplicate_import_keeps_earliest_source_line: test_duplicate_import_keeps_earliest_source_line().
  TestPythonParser.test_nested_module_level_calls_attribute_to_outer_callee: test_nested_module_level_calls_attribute_to_outer_callee().
  TestPythonParser.test_parse_class_with_method: test_parse_class_with_method().
---
# Module: [`tests/unit/parsers/test_python_parser.py`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_python_parser.py)

## Classes
### `TestPythonParser`
- def: [`tests/unit/parsers/test_python_parser.py:8`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_python_parser.py#L8)
- doc: Test the Python Parser logic.
- signature: `class TestPythonParser:`
- members:
  - `parser(self)` — [`L14`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_python_parser.py#L14)
  - `test_duplicate_import_keeps_earliest_source_line(self, parser, temp_test_dir)` — [`L70`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_python_parser.py#L70) — Duplicate imports should be stable regardless of capture traversal order.
  - `test_module_level_call_uses_module_context(self, parser, temp_test_dir)` — [`L49`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_python_parser.py#L49) — Top-level executable calls should be linked from a synthetic module frame.
  - `test_nested_module_level_calls_attribute_to_outer_callee(self, parser, temp_test_dir)` — [`L95`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_python_parser.py#L95) — Nested call expressions attribute inner calls to the outer callee.
  - `test_parse_class_with_method(self, parser, temp_test_dir)` — [`L115`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_python_parser.py#L115) — Parse a class with a method.
  - `test_parse_simple_function(self, parser, temp_test_dir)` — [`L28`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_python_parser.py#L28) — Parse a simple python file and verify output.

