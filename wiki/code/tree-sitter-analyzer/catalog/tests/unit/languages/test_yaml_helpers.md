---
title: 'Module: tests/unit/languages/test_yaml_helpers.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_yaml_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_yaml_helpers`/
symbols:
  FakeNode: FakeNode#
  test_build_document_mapping_and_sequence_elements: test_build_document_mapping_and_sequence_elements().
  FakeNode.children: FakeNode#children.
  test_build_anchor_alias_and_comment_elements: test_build_anchor_alias_and_comment_elements().
  test_analyze_yaml_file_success_path: test_analyze_yaml_file_success_path().
  _text: _text().
  test_tree_navigation_helpers: test_tree_navigation_helpers().
  test_sequence_element_extracts_parent_mapping_key: test_sequence_element_extracts_parent_mapping_key().
  test_append_element_wrappers_add_successful_builds: test_append_element_wrappers_add_successful_builds().
  _document_index: _document_index().
  _nesting_level: _nesting_level().
  test_mapping_extraction_handles_flow_nodes_and_anchors: test_mapping_extraction_handles_flow_nodes_and_anchors().
  test_extract_node_text_uses_byte_offsets: test_extract_node_text_uses_byte_offsets().
  test_extract_value_info_collection_types: test_extract_value_info_collection_types().
  test_count_children_helpers_ignore_syntax_nodes: test_count_children_helpers_ignore_syntax_nodes().
  test_append_mapping_element_swallows_helper_failures: test_append_mapping_element_swallows_helper_failures().
  FakeNode.start_byte: FakeNode#start_byte.
  test_extract_value_info_scalar_types: test_extract_value_info_scalar_types().
  test_analyze_yaml_file_failure_paths: test_analyze_yaml_file_failure_paths().
  FakeNode.start_point: FakeNode#start_point.
  FakeNode.end_point: FakeNode#end_point.
  FakeNode.__post_init__: FakeNode#__post_init__().
  FakeNode.parent: FakeNode#parent.
  FakeNode.prev_sibling: FakeNode#prev_sibling.
  FakeExtractor.extract_yaml_elements: FakeExtractor#extract_yaml_elements().
  FakeNode.text: FakeNode#text.
  FakeNode.end_byte: FakeNode#end_byte.
  FakeParser: FakeParser#
  FakeExtractor: FakeExtractor#
  FakeExtractor.elements: FakeExtractor#elements.
  FakeParser.parse: FakeParser#parse().
  FakeExtractor.__init__: FakeExtractor#__init__().
---
# Module: [`tests/unit/languages/test_yaml_helpers.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_helpers.py)

## Classes
### `FakeExtractor`
- def: [`tests/unit/languages/test_yaml_helpers.py:58`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_helpers.py#L58)
- signature: `class FakeExtractor:`
- members:
  - `extract_yaml_elements(self, tree: object, content: str)` — [`L62`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_helpers.py#L62)
  - `elements` — [`L60`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_helpers.py#L60)
- protocol/private: `__init__`[`L59`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_helpers.py#L59)
- used by: (1 test-only callers)

### `FakeNode`
- def: [`tests/unit/languages/test_yaml_helpers.py:37`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_helpers.py#L37)
- signature: `class FakeNode:`
- members:
  - `children` — [`L40`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_helpers.py#L40)
  - `end_byte` — [`L44`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_helpers.py#L44)
  - `end_point` — [`L42`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_helpers.py#L42)
  - `parent` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_helpers.py#L45)
  - `prev_sibling` — [`L46`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_helpers.py#L46)
  - `start_byte` — [`L43`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_helpers.py#L43)
  - `start_point` — [`L41`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_helpers.py#L41)
  - `text` — [`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_helpers.py#L39)
- protocol/private: `__post_init__`[`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_helpers.py#L48)
- used by: (15 test-only callers)

### `FakeParser`
- def: [`tests/unit/languages/test_yaml_helpers.py:53`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_helpers.py#L53)
- signature: `class FakeParser:`
- members:
  - `parse(self, content: bytes)` — [`L54`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_helpers.py#L54)
- used by: (1 test-only callers)

## Functions
- `_document_index(_node: FakeNode)` — [`L71`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_helpers.py#L71)
- `_nesting_level(_node: FakeNode)` — [`L75`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_helpers.py#L75)
- `_text(node: FakeNode)` — [`L67`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_helpers.py#L67)
- `test_analyze_yaml_file_failure_paths(tmp_path)` — [`L390`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_helpers.py#L390)
- `test_analyze_yaml_file_success_path(tmp_path)` — [`L368`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_helpers.py#L368)
- `test_append_element_wrappers_add_successful_builds()` — [`L310`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_helpers.py#L310)
- `test_append_mapping_element_swallows_helper_failures()` — [`L354`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_helpers.py#L354)
- `test_build_anchor_alias_and_comment_elements()` — [`L226`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_helpers.py#L226)
- `test_build_document_mapping_and_sequence_elements()` — [`L188`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_helpers.py#L188)
- `test_count_children_helpers_ignore_syntax_nodes()` — [`L158`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_helpers.py#L158)
- `test_extract_node_text_uses_byte_offsets()` — [`L79`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_helpers.py#L79)
- `test_extract_value_info_collection_types()` — [`L133`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_helpers.py#L133)
- `test_extract_value_info_scalar_types()` — [`L110`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_helpers.py#L110)
- `test_mapping_extraction_handles_flow_nodes_and_anchors()` — [`L250`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_helpers.py#L250)
- `test_sequence_element_extracts_parent_mapping_key()` — [`L280`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_helpers.py#L280)
- `test_tree_navigation_helpers()` — [`L86`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_helpers.py#L86)

