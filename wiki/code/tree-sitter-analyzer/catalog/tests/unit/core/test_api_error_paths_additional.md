---
title: 'Module: tests/unit/core/test_api_error_paths_additional.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_api_error_paths_additional.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_api_error_paths_additional`/Test
symbols:
  TestAnalyzeFileAdditional.test_method_inside_class_assigns_class_name: AnalyzeFileAdditional#test_method_inside_class_assigns_class_name().
  TestAnalyzeFileAdditional.test_method_not_in_class_gets_none: AnalyzeFileAdditional#test_method_not_in_class_gets_none().
  TestAnalyzeFileAdditional.test_include_elements_false_removes_elements: AnalyzeFileAdditional#test_include_elements_false_removes_elements().
  TestAnalyzeFileAdditional.test_include_queries_false_removes_query_results: AnalyzeFileAdditional#test_include_queries_false_removes_query_results().
  TestAnalyzeFileAdditional.test_generic_exception_returns_error_dict: AnalyzeFileAdditional#test_generic_exception_returns_error_dict().
  TestAnalyzeFileAdditional.test_file_not_found_error_is_re_raised: AnalyzeFileAdditional#test_file_not_found_error_is_re_raised().
  TestAnalyzeCodeAdditional.test_method_inside_class_in_code: AnalyzeCodeAdditional#test_method_inside_class_in_code().
  TestAnalyzeCodeAdditional.test_include_elements_false: AnalyzeCodeAdditional#test_include_elements_false().
  TestAnalyzeCodeAdditional.test_include_queries_false: AnalyzeCodeAdditional#test_include_queries_false().
  TestAnalyzeCodeAdditional.test_failure_returns_error: AnalyzeCodeAdditional#test_failure_returns_error().
  TestValidateFileAdditional.test_readable_valid_file: ValidateFileAdditional#test_readable_valid_file().
  TestValidateFileAdditional.test_unreadable_file: ValidateFileAdditional#test_unreadable_file().
  TestGroupCapturesAdditional.test_empty_captures: GroupCapturesAdditional#test_empty_captures().
  TestGroupCapturesAdditional.test_stack_pop_when_child_beyond_parent: GroupCapturesAdditional#test_stack_pop_when_child_beyond_parent().
  TestGroupCapturesAdditional.test_sub_capture_without_parent: GroupCapturesAdditional#test_sub_capture_without_parent().
  TestExecuteQueryAdditional.test_execute_query_with_dict_captures: ExecuteQueryAdditional#test_execute_query_with_dict_captures().
  TestExecuteQueryAdditional.test_execute_query_with_list_captures: ExecuteQueryAdditional#test_execute_query_with_list_captures().
  TestExecuteQueryAdditional.test_execute_query_with_other_type_captures: ExecuteQueryAdditional#test_execute_query_with_other_type_captures().
  TestExecuteQueryAdditional.test_execute_query_failure: ExecuteQueryAdditional#test_execute_query_failure().
  TestExecuteQueryAdditional.test_execute_query_exception: ExecuteQueryAdditional#test_execute_query_exception().
  TestExtractElementsAdditional.test_extract_with_type_filtering: ExtractElementsAdditional#test_extract_with_type_filtering().
  TestExtractElementsAdditional.test_extract_no_matching_types: ExtractElementsAdditional#test_extract_no_matching_types().
  TestExtractElementsAdditional.test_extract_elements_no_elements_key: ExtractElementsAdditional#test_extract_elements_no_elements_key().
  TestAnalyzeFileAdditional: AnalyzeFileAdditional#
  TestAnalyzeCodeAdditional: AnalyzeCodeAdditional#
  TestValidateFileAdditional: ValidateFileAdditional#
  TestGroupCapturesAdditional: GroupCapturesAdditional#
  TestExecuteQueryAdditional: ExecuteQueryAdditional#
  TestExtractElementsAdditional: ExtractElementsAdditional#
---
# Module: [`tests/unit/core/test_api_error_paths_additional.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_api_error_paths_additional.py)

## Classes
### `TestAnalyzeCodeAdditional`
- def: [`tests/unit/core/test_api_error_paths_additional.py:149`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_api_error_paths_additional.py#L149)
- doc: Additional tests for analyze_code uncovered paths.
- signature: `class TestAnalyzeCodeAdditional:`
- members:
  - `test_failure_returns_error(self)` — [`L225`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_api_error_paths_additional.py#L225) — Lines 238-240: analyze_code failure with error_message.
  - `test_include_elements_false(self)` — [`L188`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_api_error_paths_additional.py#L188) — Line 315: analyze_code include_elements=False.
  - `test_include_queries_false(self)` — [`L207`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_api_error_paths_additional.py#L207) — Line 318: analyze_code include_queries=False.
  - `test_method_inside_class_in_code(self)` — [`L152`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_api_error_paths_additional.py#L152) — Lines 289-301: analyze_code method inside class.
- uses (calls/refs, reference-scoped): [`analyze_code`](../../../tree_sitter_analyzer/api.md#analyze_code)

### `TestAnalyzeFileAdditional`
- def: [`tests/unit/core/test_api_error_paths_additional.py:24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_api_error_paths_additional.py#L24)
- doc: Additional tests for analyze_file uncovered paths.
- signature: `class TestAnalyzeFileAdditional:`
- members:
  - `test_file_not_found_error_is_re_raised(self)` — [`L139`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_api_error_paths_additional.py#L139) — FileNotFoundError is a public API exception, not an error dict.
  - `test_generic_exception_returns_error_dict(self)` — [`L129`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_api_error_paths_additional.py#L129) — Lines 181-186: generic exception in analyze_file.
  - `test_include_elements_false_removes_elements(self)` — [`L93`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_api_error_paths_additional.py#L93) — Line 174: include_elements=False deletes elements key.
  - `test_include_queries_false_removes_query_results(self)` — [`L111`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_api_error_paths_additional.py#L111) — Line 177: include_queries=False deletes query_results key.
  - `test_method_inside_class_assigns_class_name(self)` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_api_error_paths_additional.py#L27) — Lines 148-160: method element inside a class gets class_name.
  - `test_method_not_in_class_gets_none(self)` — [`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_api_error_paths_additional.py#L65) — Lines 159-160: method element with no containing class.
- uses (calls/refs, reference-scoped): [`analyze_file`](../../../tree_sitter_analyzer/api.md#analyze_file)

### `TestExecuteQueryAdditional`
- def: [`tests/unit/core/test_api_error_paths_additional.py:330`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_api_error_paths_additional.py#L330)
- doc: Additional tests for execute_query uncovered paths.
- signature: `class TestExecuteQueryAdditional:`
- members:
  - `test_execute_query_exception(self)` — [`L410`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_api_error_paths_additional.py#L410) — Lines 674-681: execute_query exception handler.
  - `test_execute_query_failure(self)` — [`L398`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_api_error_paths_additional.py#L398) — Lines 666-672: execute_query when analyze_file fails.
  - `test_execute_query_with_dict_captures(self)` — [`L333`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_api_error_paths_additional.py#L333) — Line 648: captures from dict query_result_dict.
  - `test_execute_query_with_list_captures(self)` — [`L360`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_api_error_paths_additional.py#L360) — Line 649-650: captures as plain list.
  - `test_execute_query_with_other_type_captures(self)` — [`L384`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_api_error_paths_additional.py#L384) — Line 651-652: captures is neither dict-with-captures nor list.
- uses (calls/refs, reference-scoped): [`execute_query`](../../../tree_sitter_analyzer/api.md#execute_query)

### `TestExtractElementsAdditional`
- def: [`tests/unit/core/test_api_error_paths_additional.py:420`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_api_error_paths_additional.py#L420)
- doc: Additional tests for extract_elements uncovered paths.
- signature: `class TestExtractElementsAdditional:`
- members:
  - `test_extract_elements_no_elements_key(self)` — [`L457`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_api_error_paths_additional.py#L457) — Lines 727-732: successful analysis but no elements key.
  - `test_extract_no_matching_types(self)` — [`L442`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_api_error_paths_additional.py#L442) — No elements match the filter.
  - `test_extract_with_type_filtering(self)` — [`L423`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_api_error_paths_additional.py#L423) — Lines 707-720: extract_elements filters by element_types.
- uses (calls/refs, reference-scoped): [`extract_elements`](../../../tree_sitter_analyzer/api.md#extract_elements)

### `TestGroupCapturesAdditional`
- def: [`tests/unit/core/test_api_error_paths_additional.py:277`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_api_error_paths_additional.py#L277)
- doc: Additional tests for _group_captures_by_main_node.
- signature: `class TestGroupCapturesAdditional:`
- members:
  - `test_empty_captures(self)` — [`L280`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_api_error_paths_additional.py#L280) — Line 559: empty captures list.
  - `test_stack_pop_when_child_beyond_parent(self)` — [`L287`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_api_error_paths_additional.py#L287) — Line 582: stack pop when child extends beyond parent.
  - `test_sub_capture_without_parent(self)` — [`L312`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_api_error_paths_additional.py#L312) — Sub-capture with no containing main node is ignored.
- uses (calls/refs, reference-scoped): [`_group_captures_by_main_node`](../../../tree_sitter_analyzer/api.md#_group_captures_by_main_node)

### `TestValidateFileAdditional`
- def: [`tests/unit/core/test_api_error_paths_additional.py:241`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_api_error_paths_additional.py#L241)
- doc: Additional tests for validate_file uncovered paths.
- signature: `class TestValidateFileAdditional:`
- members:
  - `test_readable_valid_file(self)` — [`L244`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_api_error_paths_additional.py#L244) — Lines 475-503: validate_file with existing readable file.
  - `test_unreadable_file(self)` — [`L263`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_api_error_paths_additional.py#L263) — Lines 482-484: validate_file with unreadable file.
- uses (calls/refs, reference-scoped): [`validate_file`](../../../tree_sitter_analyzer/api.md#validate_file)

