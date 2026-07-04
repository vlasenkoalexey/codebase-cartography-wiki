---
title: 'Module: tests/unit/test_call_graph_ast_a.py'
type: catalog
provenance: extracted
module: tests/unit/test_call_graph_ast_a.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_call_graph_ast_a`/
symbols:
  _parse_source: _parse_source().
  TestFunctionRef.test_qualified_name_without_receiver: TestFunctionRef#test_qualified_name_without_receiver().
  TestFunctionRef.test_qualified_name_with_receiver: TestFunctionRef#test_qualified_name_with_receiver().
  TestFunctionRef.test_equality_not_functionref: TestFunctionRef#test_equality_not_functionref().
  TestFunctionRef.test_to_dict_no_receiver: TestFunctionRef#test_to_dict_no_receiver().
  TestFunctionRef.test_to_dict_with_receiver: TestFunctionRef#test_to_dict_with_receiver().
  TestWalkTree.test_python_function_defs: TestWalkTree#test_python_function_defs().
  TestWalkTree.test_python_class_method: TestWalkTree#test_python_class_method().
  TestWalkTree.test_python_calls: TestWalkTree#test_python_calls().
  TestWalkTree.test_python_method_call: TestWalkTree#test_python_method_call().
  TestWalkTree.test_python_nested_class: TestWalkTree#test_python_nested_class().
  TestWalkTree.test_js_function_defs: TestWalkTree#test_js_function_defs().
  TestWalkTree.test_js_calls: TestWalkTree#test_js_calls().
  TestWalkTree.test_java_method_defs: TestWalkTree#test_java_method_defs().
  TestWalkTree.test_go_function_defs: TestWalkTree#test_go_function_defs().
  TestWalkTree.test_go_method_defs_and_selector_calls: TestWalkTree#test_go_method_defs_and_selector_calls().
  TestWalkTree.test_go_method_receiver_type_extracted: TestWalkTree#test_go_method_receiver_type_extracted().
  TestWalkTree.test_go_function_no_receiver: TestWalkTree#test_go_function_no_receiver().
  TestWalkTree.test_find_receiver_type_go_pointer: TestWalkTree#test_find_receiver_type_go_pointer().
  TestWalkTree.test_find_receiver_type_go_generic_pointer: TestWalkTree#test_find_receiver_type_go_generic_pointer().
  TestWalkTree.test_find_receiver_type_go_generic_multiline_pointer: TestWalkTree#test_find_receiver_type_go_generic_multiline_pointer().
  TestWalkTree.test_find_receiver_type_go_value_receiver: TestWalkTree#test_find_receiver_type_go_value_receiver().
  TestWalkTree.test_find_receiver_type_go_unnamed_pointer_receiver: TestWalkTree#test_find_receiver_type_go_unnamed_pointer_receiver().
  TestWalkTree.test_find_receiver_type_go_wrong_node_type: TestWalkTree#test_find_receiver_type_go_wrong_node_type().
  TestWalkTree.test_c_function_defs: TestWalkTree#test_c_function_defs().
  TestWalkTree.test_c_calls: TestWalkTree#test_c_calls().
  TestWalkTree.test_unsupported_language: TestWalkTree#test_unsupported_language().
  TestWalkTree.test_empty_source: TestWalkTree#test_empty_source().
  PY_PROJECT: PY_PROJECT.
  TestFunctionRef.test_basic_creation: TestFunctionRef#test_basic_creation().
  TestFunctionRef.test_creation_with_receiver: TestFunctionRef#test_creation_with_receiver().
  TestFunctionRef.test_equality_same_fields: TestFunctionRef#test_equality_same_fields().
  TestFunctionRef.test_equality_different_line: TestFunctionRef#test_equality_different_line().
  TestFunctionRef.test_equality_different_name: TestFunctionRef#test_equality_different_name().
  TestFunctionRef.test_hash_same_equal: TestFunctionRef#test_hash_same_equal().
  TestFunctionRef.test_hash_different: TestFunctionRef#test_hash_different().
  TestFunctionRef.test_slots: TestFunctionRef#test_slots().
  TestNodeText.test_extracts_text_from_node: TestNodeText#test_extracts_text_from_node().
  TestNodeText.test_extracts_text_from_middle: TestNodeText#test_extracts_text_from_middle().
  TestNodeText.test_fallback_to_text_attribute_bytes: TestNodeText#test_fallback_to_text_attribute_bytes().
  TestNodeText.test_fallback_to_text_attribute_str: TestNodeText#test_fallback_to_text_attribute_str().
  TestNodeText.test_fallback_to_text_attribute_unicode: TestNodeText#test_fallback_to_text_attribute_unicode().
  TestWalkTree.test_find_receiver_type_go_none_for_non_method: TestWalkTree#test_find_receiver_type_go_none_for_non_method().
  FIXTURES_DIR: FIXTURES_DIR.
  TestFunctionRef: TestFunctionRef#
  TestNodeText: TestNodeText#
  TestWalkTree: TestWalkTree#
---
# Module: [`tests/unit/test_call_graph_ast_a.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_a.py)

## Classes
### `TestFunctionRef`
- def: [`tests/unit/test_call_graph_ast_a.py:36`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_a.py#L36)
- signature: `class TestFunctionRef:`
- members:
  - `test_basic_creation(self)` — [`L37`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_a.py#L37)
  - `test_creation_with_receiver(self)` — [`L45`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_a.py#L45)
  - `test_equality_different_line(self)` — [`L62`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_a.py#L62)
  - `test_equality_different_name(self)` — [`L67`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_a.py#L67)
  - `test_equality_not_functionref(self)` — [`L72`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_a.py#L72)
  - `test_equality_same_fields(self)` — [`L57`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_a.py#L57)
  - `test_hash_different(self)` — [`L83`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_a.py#L83)
  - `test_hash_same_equal(self)` — [`L77`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_a.py#L77)
  - `test_qualified_name_with_receiver(self)` — [`L53`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_a.py#L53)
  - `test_qualified_name_without_receiver(self)` — [`L49`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_a.py#L49)
  - `test_slots(self)` — [`L103`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_a.py#L103)
  - `test_to_dict_no_receiver(self)` — [`L88`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_a.py#L88)
  - `test_to_dict_with_receiver(self)` — [`L98`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_a.py#L98)
- uses (calls/refs, reference-scoped): [`FunctionRef`](../../tree_sitter_analyzer/call_graph.md#FunctionRef), [`qualified_name`](../../tree_sitter_analyzer/call_graph.md#FunctionRef.qualified_name), [`to_dict`](../../tree_sitter_analyzer/call_graph.md#FunctionRef.to_dict), [`__eq__`](../../tree_sitter_analyzer/call_graph.md#FunctionRef.__eq__)

### `TestNodeText`
- def: [`tests/unit/test_call_graph_ast_a.py:113`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_a.py#L113)
- signature: `class TestNodeText:`
- members:
  - `test_extracts_text_from_middle(self)` — [`L121`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_a.py#L121)
  - `test_extracts_text_from_node(self)` — [`L114`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_a.py#L114)
  - `test_fallback_to_text_attribute_bytes(self)` — [`L128`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_a.py#L128)
  - `test_fallback_to_text_attribute_str(self)` — [`L135`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_a.py#L135)
  - `test_fallback_to_text_attribute_unicode(self)` — [`L141`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_a.py#L141)
- uses (calls/refs, reference-scoped): [`node_text`](../../tree_sitter_analyzer/function_extraction.md#node_text)

### `TestWalkTree`
- def: [`tests/unit/test_call_graph_ast_a.py:153`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_a.py#L153)
- signature: `class TestWalkTree:`
- members:
  - `test_c_calls(self)` — [`L334`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_a.py#L334)
  - `test_c_function_defs(self)` — [`L326`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_a.py#L326)
  - `test_empty_source(self)` — [`L348`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_a.py#L348)
  - `test_find_receiver_type_go_generic_multiline_pointer(self)` — [`L293`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_a.py#L293)
  - `test_find_receiver_type_go_generic_pointer(self)` — [`L287`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_a.py#L287)
  - `test_find_receiver_type_go_none_for_non_method(self)` — [`L317`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_a.py#L317)
  - `test_find_receiver_type_go_pointer(self)` — [`L276`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_a.py#L276)
  - `test_find_receiver_type_go_unnamed_pointer_receiver(self)` — [`L311`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_a.py#L311)
  - `test_find_receiver_type_go_value_receiver(self)` — [`L305`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_a.py#L305)
  - `test_find_receiver_type_go_wrong_node_type(self)` — [`L320`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_a.py#L320)
  - `test_go_function_defs(self)` — [`L224`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_a.py#L224)
  - `test_go_function_no_receiver(self)` — [`L270`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_a.py#L270)
  - `test_go_method_defs_and_selector_calls(self)` — [`L233`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_a.py#L233)
  - `test_go_method_receiver_type_extracted(self)` — [`L256`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_a.py#L256)
  - `test_java_method_defs(self)` — [`L209`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_a.py#L209)
  - `test_js_calls(self)` — [`L202`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_a.py#L202)
  - `test_js_function_defs(self)` — [`L194`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_a.py#L194)
  - `test_python_calls(self)` — [`L170`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_a.py#L170)
  - `test_python_class_method(self)` — [`L162`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_a.py#L162)
  - `test_python_function_defs(self)` — [`L154`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_a.py#L154)
  - `test_python_method_call(self)` — [`L179`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_a.py#L179)
  - `test_python_nested_class(self)` — [`L187`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_a.py#L187)
  - `test_unsupported_language(self)` — [`L341`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_a.py#L341)
- uses (calls/refs, reference-scoped): [`walk_tree`](../../tree_sitter_analyzer/function_extraction.md#walk_tree), [`find_receiver_type_go`](../../tree_sitter_analyzer/function_extraction.md#find_receiver_type_go)  (1 test-only)

## Functions
- `_parse_source(source: str, language: str)` — [`L24`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_a.py#L24)

## Module values
- `FIXTURES_DIR` — [`L20`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_a.py#L20)
- `PY_PROJECT` — [`L21`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_ast_a.py#L21)

