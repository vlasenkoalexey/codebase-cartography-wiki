---
title: 'Module: tests/unit/languages/test_go_function_helpers.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_go_function_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_go_function_helpers`/
symbols:
  TestExtractGoFunction.test_basic_function_extraction: TestExtractGoFunction#test_basic_function_extraction().
  TestExtractGoMethod.test_basic_method_extraction: TestExtractGoMethod#test_basic_method_extraction().
  TestExtractGoMethod.test_method_receiver_extraction: TestExtractGoMethod#test_method_receiver_extraction().
  TestExtractGoFunction.test_private_function: TestExtractGoFunction#test_private_function().
  TestExtractGoFunction.test_no_result_node: TestExtractGoFunction#test_no_result_node().
  TestExtractGoFunction.test_with_docstring: TestExtractGoFunction#test_with_docstring().
  FakeNode.child_by_field_name: FakeNode#child_by_field_name().
  TestExtractGoFunction.test_no_docstring: TestExtractGoFunction#test_no_docstring().
  FakeNode: FakeNode#
  FakeNode._name_text: FakeNode#_name_text.
  TestExtractGoFunction.test_empty_name_returns_none: TestExtractGoFunction#test_empty_name_returns_none().
  TestExtractGoFunction.get_text: TestExtractGoFunction#get_text().
  TestExtractGoFunction.test_no_name_node_returns_none: TestExtractGoFunction#test_no_name_node_returns_none().
  TestExtractGoFunction.test_exception_returns_none: TestExtractGoFunction#test_exception_returns_none().
  TestExtractGoMethod.test_method_no_name_returns_none: TestExtractGoMethod#test_method_no_name_returns_none().
  TestExtractGoMethod.test_method_exception_returns_none: TestExtractGoMethod#test_method_exception_returns_none().
  FakeNode.start_point: FakeNode#start_point.
  FakeNode.end_point: FakeNode#end_point.
  TestExtractGoFunction.patched: TestExtractGoFunction#patched().
  TestExtractGoMethod.mock_receiver_extractor: TestExtractGoMethod#mock_receiver_extractor().
  _NameNode: _NameNode#
  _TextNode: _TextNode#
  _ParamsNode: _ParamsNode#
  FakeNode.children: FakeNode#children.
  _NameNode.text: _NameNode#text.
  _NameNode.child_by_field_name: _NameNode#child_by_field_name().
  _TextNode.text: _TextNode#text.
  _TextNode.children: _TextNode#children.
  _TextNode.child_by_field_name: _TextNode#child_by_field_name().
  _ParamsNode.children: _ParamsNode#children.
  _ParamsNode.child_by_field_name: _ParamsNode#child_by_field_name().
  TestExtractGoFunction: TestExtractGoFunction#
  TestExtractGoMethod: TestExtractGoMethod#
---
# Module: [`tests/unit/languages/test_go_function_helpers.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_function_helpers.py)

## Classes
### `FakeNode`
- def: [`tests/unit/languages/test_go_function_helpers.py:16`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_function_helpers.py#L16)
- signature: `class FakeNode:`
- members:
  - `child_by_field_name(self, name: str)` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_function_helpers.py#L23)
  - `children` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_function_helpers.py#L20)
  - `end_point` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_function_helpers.py#L19)
  - `start_point` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_function_helpers.py#L18)
- protocol/private: `_name_text`[`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_function_helpers.py#L21)
- uses (calls/refs, reference-scoped): (3 test-only callers)
- used by: (7 test-only callers)

### `TestExtractGoFunction`
- def: [`tests/unit/languages/test_go_function_helpers.py:61`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_function_helpers.py#L61)
- signature: `class TestExtractGoFunction:`
- members:
  - `get_text(n)` — [`L72`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_function_helpers.py#L72)
  - `patched(name)` — [`L188`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_function_helpers.py#L188)
  - `test_basic_function_extraction(self)` — [`L62`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_function_helpers.py#L62)
  - `test_empty_name_returns_none(self)` — [`L120`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_function_helpers.py#L120)
  - `test_exception_returns_none(self)` — [`L143`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_function_helpers.py#L143)
  - `test_no_docstring(self)` — [`L154`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_function_helpers.py#L154)
  - `test_no_name_node_returns_none(self)` — [`L109`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_function_helpers.py#L109)
  - `test_no_result_node(self)` — [`L183`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_function_helpers.py#L183)
  - `test_private_function(self)` — [`L92`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_function_helpers.py#L92)
  - `test_with_docstring(self)` — [`L165`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_function_helpers.py#L165)
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`start_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`end_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.end_line), [`language`](../../../tree_sitter_analyzer/models/base.md#CodeElement.language), [`return_type`](../../../tree_sitter_analyzer/models/base.md#Function.return_type), [`visibility`](../../../tree_sitter_analyzer/models/base.md#Function.visibility), [`docstring`](../../../tree_sitter_analyzer/models/base.md#CodeElement.docstring), [`is_method`](../../../tree_sitter_analyzer/models/base.md#Function.is_method), [`extract_go_function`](../../../tree_sitter_analyzer/languages/_go_function_helpers.md#extract_go_function), [`is_public`](../../../tree_sitter_analyzer/models/base.md#Function.is_public)  (5 test-only)

### `TestExtractGoMethod`
- def: [`tests/unit/languages/test_go_function_helpers.py:203`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_function_helpers.py#L203)
- signature: `class TestExtractGoMethod:`
- members:
  - `mock_receiver_extractor(n, get_text)` — [`L215`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_function_helpers.py#L215)
  - `test_basic_method_extraction(self)` — [`L204`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_function_helpers.py#L204)
  - `test_method_exception_returns_none(self)` — [`L248`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_function_helpers.py#L248)
  - `test_method_no_name_returns_none(self)` — [`L237`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_function_helpers.py#L237)
  - `test_method_receiver_extraction(self)` — [`L259`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_function_helpers.py#L259)
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`receiver_type`](../../../tree_sitter_analyzer/models/base.md#Function.receiver_type), [`is_method`](../../../tree_sitter_analyzer/models/base.md#Function.is_method), [`extract_go_method`](../../../tree_sitter_analyzer/languages/_go_function_helpers.md#extract_go_method), [`extract_method_receiver`](../../../tree_sitter_analyzer/languages/_go_common_helpers.md#extract_method_receiver), [`receiver`](../../../tree_sitter_analyzer/models/base.md#Function.receiver)  (2 test-only)

### `_NameNode`
- def: [`tests/unit/languages/test_go_function_helpers.py:34`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_function_helpers.py#L34)
- members:
  - `child_by_field_name(self, name: str)` — [`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_function_helpers.py#L38)
  - `text` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_function_helpers.py#L35)
- used by: (1 test-only callers)

### `_ParamsNode`
- def: [`tests/unit/languages/test_go_function_helpers.py:53`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_function_helpers.py#L53)
- members:
  - `child_by_field_name(self, name: str)` — [`L57`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_function_helpers.py#L57)
  - `children` — [`L54`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_function_helpers.py#L54)
- used by: (1 test-only callers)

### `_TextNode`
- def: [`tests/unit/languages/test_go_function_helpers.py:43`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_function_helpers.py#L43)
- members:
  - `child_by_field_name(self, name: str)` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_function_helpers.py#L48)
  - `children` — [`L46`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_function_helpers.py#L46)
  - `text` — [`L44`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_function_helpers.py#L44)
- used by: (1 test-only callers)

