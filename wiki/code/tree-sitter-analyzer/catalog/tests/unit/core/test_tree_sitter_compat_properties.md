---
title: 'Module: tests/unit/core/test_tree_sitter_compat_properties.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_tree_sitter_compat_properties.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_tree_sitter_compat_properties`/
symbols:
  TestTreeSitterVersionCompatibilityProperties.test_property_14_api_version_result_equivalence: TestTreeSitterVersionCompatibilityProperties#test_property_14_api_version_result_equivalence().
  TestTreeSitterVersionCompatibilityProperties.test_property_14_newest_api_returns_consistent_format: TestTreeSitterVersionCompatibilityProperties#test_property_14_newest_api_returns_consistent_format().
  TestTreeSitterVersionCompatibilityProperties.test_property_14_modern_api_returns_consistent_format: TestTreeSitterVersionCompatibilityProperties#test_property_14_modern_api_returns_consistent_format().
  TestTreeSitterVersionCompatibilityProperties.test_property_14_legacy_api_returns_consistent_format: TestTreeSitterVersionCompatibilityProperties#test_property_14_legacy_api_returns_consistent_format().
  TestTreeSitterVersionCompatibilityProperties.test_property_14_get_node_text_safe_byte_extraction_consistency: TestTreeSitterVersionCompatibilityProperties#test_property_14_get_node_text_safe_byte_extraction_consistency().
  TestTreeSitterCompatEdgeCases.test_property_14_point_based_extraction_consistency: TestTreeSitterCompatEdgeCases#test_property_14_point_based_extraction_consistency().
  _assert_results_are_tuples: _assert_results_are_tuples().
  TestTreeSitterVersionCompatibilityProperties.test_property_14_safe_execute_query_fallback_consistency: TestTreeSitterVersionCompatibilityProperties#test_property_14_safe_execute_query_fallback_consistency().
  TestTreeSitterCompatEdgeCases.test_property_14_error_handling_consistency: TestTreeSitterCompatEdgeCases#test_property_14_error_handling_consistency().
  capture_names: capture_names.
  _normalize_capture_names: _normalize_capture_names().
  TestTreeSitterVersionCompatibilityProperties.test_property_14_get_node_text_safe_text_attribute_consistency: TestTreeSitterVersionCompatibilityProperties#test_property_14_get_node_text_safe_text_attribute_consistency().
  TestTreeSitterVersionCompatibilityProperties.test_property_14_create_query_safely_consistency: TestTreeSitterVersionCompatibilityProperties#test_property_14_create_query_safely_consistency().
  byte_positions: byte_positions.
  line_positions: line_positions.
  column_positions: column_positions.
  source_code_content: source_code_content.
  num_captures: num_captures.
  TestTreeSitterVersionCompatibilityProperties: TestTreeSitterVersionCompatibilityProperties#
  TestTreeSitterCompatEdgeCases: TestTreeSitterCompatEdgeCases#
---
# Module: [`tests/unit/core/test_tree_sitter_compat_properties.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat_properties.py)

## Classes
### `TestTreeSitterCompatEdgeCases`
- def: [`tests/unit/core/test_tree_sitter_compat_properties.py:493`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat_properties.py#L493)
- doc: Edge case tests for tree-sitter compatibility.
- signature: `class TestTreeSitterCompatEdgeCases:`
- members:
  - `test_property_14_error_handling_consistency(self, error_message: str)` — [`L566`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat_properties.py#L566) — **Feature: test-coverage-improvement, Property 14: Tree-sitter Version Compatibility**
  - `test_property_14_point_based_extraction_consistency(self, source_lines: list[str], start_line: int, end_line: int, start_col: int, end_col: int)` — [`L511`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat_properties.py#L511) — **Feature: test-coverage-improvement, Property 14: Tree-sitter Version Compatibility**
- uses (calls/refs, reference-scoped): [`get_node_text_safe`](../../../tree_sitter_analyzer/utils/tree_sitter_compat.md#get_node_text_safe), [`TreeSitterQueryCompat`](../../../tree_sitter_analyzer/utils/tree_sitter_compat.md#TreeSitterQueryCompat), [`execute_query`](../../../tree_sitter_analyzer/utils/tree_sitter_compat.md#TreeSitterQueryCompat.execute_query)  (2 test-only)

### `TestTreeSitterVersionCompatibilityProperties`
- def: [`tests/unit/core/test_tree_sitter_compat_properties.py:76`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat_properties.py#L76)
- doc: Property-based tests for tree-sitter version compatibility.
- signature: `class TestTreeSitterVersionCompatibilityProperties:`
- members:
  - `test_property_14_api_version_result_equivalence(self, capture_name_list: list[str])` — [`L418`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat_properties.py#L418) — **Feature: test-coverage-improvement, Property 14: Tree-sitter Version Compatibility**
  - `test_property_14_create_query_safely_consistency(self, query_string: str)` — [`L382`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat_properties.py#L382) — **Feature: test-coverage-improvement, Property 14: Tree-sitter Version Compatibility**
  - `test_property_14_get_node_text_safe_byte_extraction_consistency(self, source_code: str, start_byte: int, end_byte: int)` — [`L248`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat_properties.py#L248) — **Feature: test-coverage-improvement, Property 14: Tree-sitter Version Compatibility**
  - `test_property_14_get_node_text_safe_text_attribute_consistency(self, source_code: str)` — [`L288`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat_properties.py#L288) — **Feature: test-coverage-improvement, Property 14: Tree-sitter Version Compatibility**
  - `test_property_14_legacy_api_returns_consistent_format(self, capture_name_list: list[str])` — [`L198`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat_properties.py#L198) — **Feature: test-coverage-improvement, Property 14: Tree-sitter Version Compatibility**
  - `test_property_14_modern_api_returns_consistent_format(self, capture_name_list: list[str])` — [`L145`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat_properties.py#L145) — **Feature: test-coverage-improvement, Property 14: Tree-sitter Version Compatibility**
  - `test_property_14_newest_api_returns_consistent_format(self, capture_name_list: list[str])` — [`L88`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat_properties.py#L88) — **Feature: test-coverage-improvement, Property 14: Tree-sitter Version Compatibility**
  - `test_property_14_safe_execute_query_fallback_consistency(self, fallback_captures: list[tuple[str, str]])` — [`L344`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat_properties.py#L344) — **Feature: test-coverage-improvement, Property 14: Tree-sitter Version Compatibility**
- uses (calls/refs, reference-scoped): [`get_node_text_safe`](../../../tree_sitter_analyzer/utils/tree_sitter_compat.md#get_node_text_safe), [`TreeSitterQueryCompat`](../../../tree_sitter_analyzer/utils/tree_sitter_compat.md#TreeSitterQueryCompat), [`safe_execute_query`](../../../tree_sitter_analyzer/utils/tree_sitter_compat.md#TreeSitterQueryCompat.safe_execute_query), [`execute_query`](../../../tree_sitter_analyzer/utils/tree_sitter_compat.md#TreeSitterQueryCompat.execute_query), [`create_query_safely`](../../../tree_sitter_analyzer/utils/tree_sitter_compat.md#create_query_safely), [`_execute_legacy_api`](../../../tree_sitter_analyzer/utils/tree_sitter_compat.md#TreeSitterQueryCompat._execute_legacy_api), [`_execute_modern_api`](../../../tree_sitter_analyzer/utils/tree_sitter_compat.md#TreeSitterQueryCompat._execute_modern_api), [`_execute_newest_api`](../../../tree_sitter_analyzer/utils/tree_sitter_compat.md#TreeSitterQueryCompat._execute_newest_api)  (5 test-only)

## Functions
- `_assert_results_are_tuples(results: list, label: str = "")` — [`L60`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat_properties.py#L60) — Assert all items are (node, str) tuples.
- `_normalize_capture_names(names: list)` — [`L54`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat_properties.py#L54) — Filter invalid names and return at least one default.

## Module values
- `byte_positions` — [`L47`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat_properties.py#L47)
- `capture_names` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat_properties.py#L26)
- `column_positions` — [`L51`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat_properties.py#L51)
- `line_positions` — [`L50`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat_properties.py#L50)
- `num_captures` — [`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat_properties.py#L37)
- `source_code_content` — [`L40`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_tree_sitter_compat_properties.py#L40)

