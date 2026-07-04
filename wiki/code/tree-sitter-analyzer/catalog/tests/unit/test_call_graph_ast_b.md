---
title: 'Module: tests/unit/test_call_graph_ast_b.py'
type: catalog
provenance: extracted
module: tests/unit/test_call_graph_ast_b.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_call_graph_ast_b`/
symbols:
  _parse_source: _parse_source().
  TestExtractCall.test_c_call: TestExtractCall#test_c_call().
  TestFindParentClassJava.test_finds_parent_class: TestFindParentClassJava#test_finds_parent_class().
  TestFindParentClassJava.test_no_parent_class_top_level: TestFindParentClassJava#test_no_parent_class_top_level().
  _find_first_node: _find_first_node().
  TestGetFuncName.test_python_function: TestGetFuncName#test_python_function().
  TestGetFuncName.test_js_function: TestGetFuncName#test_js_function().
  TestGetFuncName.test_c_function: TestGetFuncName#test_c_function().
  TestGetFuncName.test_unsupported_language_returns_none: TestGetFuncName#test_unsupported_language_returns_none().
  TestExtractCall.test_python_call: TestExtractCall#test_python_call().
  TestExtractCall.test_python_method_call: TestExtractCall#test_python_method_call().
  TestExtractCall.test_js_call: TestExtractCall#test_js_call().
  TestFindParentClassPython.test_finds_parent_class: TestFindParentClassPython#test_finds_parent_class().
  TestFindParentClassPython.test_no_parent_class: TestFindParentClassPython#test_no_parent_class().
  _collect_nodes: _collect_nodes().
  PY_PROJECT: PY_PROJECT.
  TestGetFuncName.test_go_method_name_falls_back_to_field_identifier_child: TestGetFuncName#test_go_method_name_falls_back_to_field_identifier_child().
  TestGetFuncName.test_go_method_name_accepts_text_from_name_field: TestGetFuncName#test_go_method_name_accepts_text_from_name_field().
  TestGetFuncName.test_go_method_name_decodes_bytes_from_name_field: TestGetFuncName#test_go_method_name_decodes_bytes_from_name_field().
  TestGetFuncName.test_no_func_name_returns_none: TestGetFuncName#test_no_func_name_returns_none().
  TestExtractCall.test_returns_none_for_non_call: TestExtractCall#test_returns_none_for_non_call().
  FIXTURES_DIR: FIXTURES_DIR.
  TestGetFuncName: TestGetFuncName#
  TestExtractCall: TestExtractCall#
  TestFindParentClassPython: TestFindParentClassPython#
  TestFindParentClassJava: TestFindParentClassJava#
---
# Module: [`tests/unit/test_call_graph_ast_b.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_b.py)

## Classes
### `TestExtractCall`
- def: [`tests/unit/test_call_graph_ast_b.py:121`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_b.py#L121)
- signature: `class TestExtractCall:`
- members:
  - `test_c_call(self)` — [`L153`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_b.py#L153)
  - `test_js_call(self)` — [`L143`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_b.py#L143)
  - `test_python_call(self)` — [`L122`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_b.py#L122)
  - `test_python_method_call(self)` — [`L133`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_b.py#L133)
  - `test_returns_none_for_non_call(self)` — [`L163`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_b.py#L163)
- uses (calls/refs, reference-scoped): [`extract_call`](../../tree_sitter_analyzer/function_extraction.md#extract_call)  (2 test-only)

### `TestFindParentClassJava`
- def: [`tests/unit/test_call_graph_ast_b.py:199`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_b.py#L199)
- signature: `class TestFindParentClassJava:`
- members:
  - `test_finds_parent_class(self)` — [`L200`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_b.py#L200)
  - `test_no_parent_class_top_level(self)` — [`L209`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_b.py#L209)
- uses (calls/refs, reference-scoped): [`find_parent_class_java`](../../tree_sitter_analyzer/function_extraction.md#find_parent_class_java)  (2 test-only)

### `TestFindParentClassPython`
- def: [`tests/unit/test_call_graph_ast_b.py:174`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_b.py#L174)
- signature: `class TestFindParentClassPython:`
- members:
  - `test_finds_parent_class(self)` — [`L175`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_b.py#L175)
  - `test_no_parent_class(self)` — [`L187`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_b.py#L187)
- uses (calls/refs, reference-scoped): [`find_parent_class_python`](../../tree_sitter_analyzer/function_extraction.md#find_parent_class_python)  (1 test-only)

### `TestGetFuncName`
- def: [`tests/unit/test_call_graph_ast_b.py:55`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_b.py#L55)
- signature: `class TestGetFuncName:`
- members:
  - `test_c_function(self)` — [`L70`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_b.py#L70)
  - `test_go_method_name_accepts_text_from_name_field(self)` — [`L86`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_b.py#L86)
  - `test_go_method_name_decodes_bytes_from_name_field(self)` — [`L94`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_b.py#L94)
  - `test_go_method_name_falls_back_to_field_identifier_child(self)` — [`L76`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_b.py#L76)
  - `test_js_function(self)` — [`L63`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_b.py#L63)
  - `test_no_func_name_returns_none(self)` — [`L102`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_b.py#L102)
  - `test_python_function(self)` — [`L56`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_b.py#L56)
  - `test_unsupported_language_returns_none(self)` — [`L107`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_b.py#L107)
- uses (calls/refs, reference-scoped): [`get_func_name`](../../tree_sitter_analyzer/function_extraction.md#get_func_name)  (1 test-only)

## Functions
- `_collect_nodes(node, node_type, result_list)` — [`L31`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_b.py#L31)
- `_find_first_node(node, node_type, result)` — [`L39`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_b.py#L39)
- `_parse_source(source: str, language: str)` — [`L24`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_b.py#L24)

## Module values
- `FIXTURES_DIR` — [`L20`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_b.py#L20)
- `PY_PROJECT` — [`L21`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_b.py#L21)

