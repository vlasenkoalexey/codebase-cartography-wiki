---
title: 'Module: tests/unit/test_api_query_helpers.py'
type: catalog
provenance: extracted
module: tests/unit/test_api_query_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_api_query_helpers`/Test
symbols:
  TestGroupCapturesByMainNode.test_empty_captures_returns_empty_list: GroupCapturesByMainNode#test_empty_captures_returns_empty_list().
  TestGroupCapturesByMainNode.test_single_main_capture: GroupCapturesByMainNode#test_single_main_capture().
  TestGroupCapturesByMainNode.test_nested_child_attached_to_parent: GroupCapturesByMainNode#test_nested_child_attached_to_parent().
  TestGroupCapturesByMainNode.test_overlapping_main_nodes_stacked: GroupCapturesByMainNode#test_overlapping_main_nodes_stacked().
  TestGroupCapturesByMainNode.test_multiple_children_same_capture_name_becomes_list: GroupCapturesByMainNode#test_multiple_children_same_capture_name_becomes_list().
  TestGroupCapturesByMainNode.test_child_without_active_parent_is_ignored: GroupCapturesByMainNode#test_child_without_active_parent_is_ignored().
  TestGroupCapturesByMainNode.test_end_line_calculation_counts_newlines: GroupCapturesByMainNode#test_end_line_calculation_counts_newlines().
  TestGroupCapturesByMainNode.test_sorted_by_start_byte_then_nested_first: GroupCapturesByMainNode#test_sorted_by_start_byte_then_nested_first().
  TestQueryCapturesForResult.test_dict_captures_key: QueryCapturesForResult#test_dict_captures_key().
  TestQueryCapturesForResult.test_list_query_result: QueryCapturesForResult#test_list_query_result().
  TestQueryCapturesForResult.test_missing_query_name_returns_empty: QueryCapturesForResult#test_missing_query_name_returns_empty().
  TestQueryCapturesForResult.test_non_dict_non_list_returns_empty: QueryCapturesForResult#test_non_dict_non_list_returns_empty().
  TestQueryExecutionResult.test_failed_analysis: QueryExecutionResult#test_failed_analysis().
  TestQueryExecutionResult.test_successful_execution: QueryExecutionResult#test_successful_execution().
  TestQueryExecutionResult.test_no_query_results_key: QueryExecutionResult#test_no_query_results_key().
  TestQueryExecutionResult.test_file_path_preserved: QueryExecutionResult#test_file_path_preserved().
  TestFilterElementsByType.test_none_types_returns_all: FilterElementsByType#test_none_types_returns_all().
  TestFilterElementsByType.test_empty_types_returns_all: FilterElementsByType#test_empty_types_returns_all().
  TestFilterElementsByType.test_case_insensitive_match: FilterElementsByType#test_case_insensitive_match().
  TestFilterElementsByType.test_fuzzy_substring_match: FilterElementsByType#test_fuzzy_substring_match().
  TestFilterElementsByType.test_multiple_types_any_match: FilterElementsByType#test_multiple_types_any_match().
  TestFilterElementsByType.test_no_match_returns_empty: FilterElementsByType#test_no_match_returns_empty().
  TestFilterElementsByType.test_class_filter_includes_interface: FilterElementsByType#test_class_filter_includes_interface().
  TestFilterElementsByType.test_class_filter_includes_enum: FilterElementsByType#test_class_filter_includes_enum().
  TestFilterElementsByType.test_class_filter_includes_namespace: FilterElementsByType#test_class_filter_includes_namespace().
  TestFilterElementsByType.test_class_filter_includes_type_alias: FilterElementsByType#test_class_filter_includes_type_alias().
  TestFilterElementsByType.test_class_filter_includes_abstract_class: FilterElementsByType#test_class_filter_includes_abstract_class().
  TestFilterElementsByType.test_interface_filter_does_not_widen_to_all_class_family: FilterElementsByType#test_interface_filter_does_not_widen_to_all_class_family().
  TestGroupCapturesByMainNode: GroupCapturesByMainNode#
  TestQueryCapturesForResult: QueryCapturesForResult#
  TestQueryExecutionResult: QueryExecutionResult#
  TestFilterElementsByType: FilterElementsByType#
---
# Module: [`tests/unit/test_api_query_helpers.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_query_helpers.py)

## Classes
### `TestFilterElementsByType`
- def: [`tests/unit/test_api_query_helpers.py:232`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_query_helpers.py#L232)
- doc: Tests for filter_elements_by_type.
- signature: `class TestFilterElementsByType:`
- members:
  - `test_case_insensitive_match(self)` — [`L243`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_query_helpers.py#L243)
  - `test_class_filter_includes_abstract_class(self)` — [`L292`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_query_helpers.py#L292)
  - `test_class_filter_includes_enum(self)` — [`L274`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_query_helpers.py#L274)
  - `test_class_filter_includes_interface(self)` — [`L267`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_query_helpers.py#L267) — #795 P2: filtering by 'class' must still return interface elements.
  - `test_class_filter_includes_namespace(self)` — [`L280`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_query_helpers.py#L280)
  - `test_class_filter_includes_type_alias(self)` — [`L286`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_query_helpers.py#L286)
  - `test_empty_types_returns_all(self)` — [`L239`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_query_helpers.py#L239)
  - `test_fuzzy_substring_match(self)` — [`L249`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_query_helpers.py#L249)
  - `test_interface_filter_does_not_widen_to_all_class_family(self)` — [`L297`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_query_helpers.py#L297) — Filtering by 'interface' should NOT return plain 'class' elements.
  - `test_multiple_types_any_match(self)` — [`L255`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_query_helpers.py#L255)
  - `test_no_match_returns_empty(self)` — [`L260`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_query_helpers.py#L260)
  - `test_none_types_returns_all(self)` — [`L235`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_query_helpers.py#L235)
- uses (calls/refs, reference-scoped): [`filter_elements_by_type`](../../tree_sitter_analyzer/_api_query_helpers.md#filter_elements_by_type)

### `TestGroupCapturesByMainNode`
- def: [`tests/unit/test_api_query_helpers.py:11`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_query_helpers.py#L11)
- doc: Tests for group_captures_by_main_node.
- signature: `class TestGroupCapturesByMainNode:`
- members:
  - `test_child_without_active_parent_is_ignored(self)` — [`L112`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_query_helpers.py#L112)
  - `test_empty_captures_returns_empty_list(self)` — [`L14`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_query_helpers.py#L14)
  - `test_end_line_calculation_counts_newlines(self)` — [`L126`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_query_helpers.py#L126)
  - `test_multiple_children_same_capture_name_becomes_list(self)` — [`L79`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_query_helpers.py#L79)
  - `test_nested_child_attached_to_parent(self)` — [`L33`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_query_helpers.py#L33)
  - `test_overlapping_main_nodes_stacked(self)` — [`L56`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_query_helpers.py#L56)
  - `test_single_main_capture(self)` — [`L17`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_query_helpers.py#L17)
  - `test_sorted_by_start_byte_then_nested_first(self)` — [`L141`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_query_helpers.py#L141)
- uses (calls/refs, reference-scoped): [`group_captures_by_main_node`](../../tree_sitter_analyzer/_api_query_helpers.md#group_captures_by_main_node)

### `TestQueryCapturesForResult`
- def: [`tests/unit/test_api_query_helpers.py:166`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_query_helpers.py#L166)
- doc: Tests for query_captures_for_result.
- signature: `class TestQueryCapturesForResult:`
- members:
  - `test_dict_captures_key(self)` — [`L169`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_query_helpers.py#L169)
  - `test_list_query_result(self)` — [`L174`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_query_helpers.py#L174)
  - `test_missing_query_name_returns_empty(self)` — [`L179`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_query_helpers.py#L179)
  - `test_non_dict_non_list_returns_empty(self)` — [`L183`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_query_helpers.py#L183)
- uses (calls/refs, reference-scoped): [`query_captures_for_result`](../../tree_sitter_analyzer/_api_query_helpers.md#query_captures_for_result)

### `TestQueryExecutionResult`
- def: [`tests/unit/test_api_query_helpers.py:188`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_query_helpers.py#L188)
- doc: Tests for query_execution_result.
- signature: `class TestQueryExecutionResult:`
- members:
  - `test_failed_analysis(self)` — [`L191`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_query_helpers.py#L191)
  - `test_file_path_preserved(self)` — [`L226`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_query_helpers.py#L226)
  - `test_no_query_results_key(self)` — [`L221`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_query_helpers.py#L221)
  - `test_successful_execution(self)` — [`L197`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_query_helpers.py#L197)
- uses (calls/refs, reference-scoped): [`query_execution_result`](../../tree_sitter_analyzer/_api_query_helpers.md#query_execution_result)

