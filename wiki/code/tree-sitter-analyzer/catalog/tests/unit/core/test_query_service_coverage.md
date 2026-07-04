---
title: 'Module: tests/unit/core/test_query_service_coverage.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_query_service_coverage.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_query_service_coverage`/
symbols:
  query_service: query_service().
  test_query_service_basic: test_query_service_basic().
  test_query_service_execute_empty: test_query_service_execute_empty().
  TestExtractNodeName: TestExtractNodeName#
  TestExtractNodeName.test_name_field_found: TestExtractNodeName#test_name_field_found().
  TestExtractNodeName.test_declarator_field_with_inner_declarator: TestExtractNodeName#test_declarator_field_with_inner_declarator().
  TestExtractNodeName.test_declarator_field_with_inner_name: TestExtractNodeName#test_declarator_field_with_inner_name().
  TestExtractNodeName.test_no_child_by_field_name: TestExtractNodeName#test_no_child_by_field_name().
  TestExtractNodeName.test_empty_text_returns_none: TestExtractNodeName#test_empty_text_returns_none().
  TestExtractNodeName.test_very_long_name_ignored: TestExtractNodeName#test_very_long_name_ignored().
  TestExtractParentContext: TestExtractParentContext#
  TestExtractParentContext.test_no_parent_attr: TestExtractParentContext#test_no_parent_attr().
  TestExtractParentContext.test_parent_is_container: TestExtractParentContext#test_parent_is_container().
  TestExtractParentContext.test_parent_not_container: TestExtractParentContext#test_parent_not_container().
  TestExtractParentContext.test_grandparent_is_container: TestExtractParentContext#test_grandparent_is_container().
  TestExtractParentContext.test_parent_no_type_attr: TestExtractParentContext#test_parent_no_type_attr().
  TestExtractParentContext.test_container_with_empty_name: TestExtractParentContext#test_container_with_empty_name().
  TestExtractParentContext.test_container_with_no_name_node: TestExtractParentContext#test_container_with_no_name_node().
  TestCreateResultDictFull: TestCreateResultDictFull#
  TestCreateResultDictFull.test_with_name_and_parent: TestCreateResultDictFull#test_with_name_and_parent().
  TestCreateResultDictFull.test_node_missing_start_end_point: TestCreateResultDictFull#test_node_missing_start_end_point().
  TestExecutePluginQueryElementConversion: TestExecutePluginQueryElementConversion#
  TestExecutePluginQueryElementConversion.test_element_with_raw_text: TestExecutePluginQueryElementConversion#test_element_with_raw_text().
  TestExecutePluginQueryElementConversion.test_null_query_key_defaults: TestExecutePluginQueryElementConversion#test_null_query_key_defaults().
  TestExecutePluginQueryElementConversion.test_no_plugin_uses_fallback: TestExecutePluginQueryElementConversion#test_no_plugin_uses_fallback().
  TestExecutePluginQueryElementConversion.test_plugin_returns_none_elements: TestExecutePluginQueryElementConversion#test_plugin_returns_none_elements().
  TestReadFileAsync: TestReadFileAsync#
  TestReadFileAsync.test_read_file_async_actual: TestReadFileAsync#test_read_file_async_actual().
---
# Module: [`tests/unit/core/test_query_service_coverage.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_coverage.py)

## Classes
### `TestCreateResultDictFull`
- def: [`tests/unit/core/test_query_service_coverage.py:188`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_coverage.py#L188)
- doc: Cover _create_result_dict with name and parent extraction.
- signature: `class TestCreateResultDictFull:`
- members:
  - `test_node_missing_start_end_point(self, query_service)` — [`L221`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_coverage.py#L221)
  - `test_with_name_and_parent(self, mock_text, query_service)` — [`L195`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_coverage.py#L195)

### `TestExecutePluginQueryElementConversion`
- def: [`tests/unit/core/test_query_service_coverage.py:229`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_coverage.py#L229)
- doc: Cover MockNode creation and element conversion in _execute_plugin_query.
- signature: `class TestExecutePluginQueryElementConversion:`
- members:
  - `test_element_with_raw_text(self, query_service)` — [`L232`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_coverage.py#L232)
  - `test_no_plugin_uses_fallback(self, query_service)` — [`L271`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_coverage.py#L271)
  - `test_null_query_key_defaults(self, query_service)` — [`L254`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_coverage.py#L254)
  - `test_plugin_returns_none_elements(self, query_service)` — [`L282`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_coverage.py#L282)

### `TestExtractNodeName`
- def: [`tests/unit/core/test_query_service_coverage.py:33`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_coverage.py#L33)
- doc: Cover _extract_node_name branches.
- signature: `class TestExtractNodeName:`
- members:
  - `test_declarator_field_with_inner_declarator(self, mock_text, query_service)` — [`L53`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_coverage.py#L53)
  - `test_declarator_field_with_inner_name(self, mock_text, query_service)` — [`L70`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_coverage.py#L70)
  - `test_empty_text_returns_none(self, mock_text, query_service)` — [`L90`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_coverage.py#L90)
  - `test_name_field_found(self, mock_text, query_service)` — [`L40`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_coverage.py#L40)
  - `test_no_child_by_field_name(self, query_service)` — [`L83`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_coverage.py#L83)
  - `test_very_long_name_ignored(self, mock_text, query_service)` — [`L103`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_coverage.py#L103)

### `TestExtractParentContext`
- def: [`tests/unit/core/test_query_service_coverage.py:113`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_coverage.py#L113)
- doc: Cover _extract_parent_context branches.
- signature: `class TestExtractParentContext:`
- members:
  - `test_container_with_empty_name(self, mock_text, query_service)` — [`L168`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_coverage.py#L168)
  - `test_container_with_no_name_node(self, query_service)` — [`L178`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_coverage.py#L178)
  - `test_grandparent_is_container(self, mock_text, query_service)` — [`L145`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_coverage.py#L145)
  - `test_no_parent_attr(self, query_service)` — [`L116`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_coverage.py#L116)
  - `test_parent_is_container(self, mock_text, query_service)` — [`L124`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_coverage.py#L124)
  - `test_parent_no_type_attr(self, query_service)` — [`L158`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_coverage.py#L158)
  - `test_parent_not_container(self, query_service)` — [`L134`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_coverage.py#L134)

### `TestReadFileAsync`
- def: [`tests/unit/core/test_query_service_coverage.py:295`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_coverage.py#L295)
- doc: Cover _read_file_async with actual file.
- signature: `class TestReadFileAsync:`
- members:
  - `test_read_file_async_actual(self, query_service, tmp_path)` — [`L299`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_coverage.py#L299)

## Functions
- `query_service()` — [`L9`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_coverage.py#L9)
- `test_query_service_basic(query_service)` — [`L13`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_coverage.py#L13)
- `test_query_service_execute_empty(query_service)` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_service_coverage.py#L18)

