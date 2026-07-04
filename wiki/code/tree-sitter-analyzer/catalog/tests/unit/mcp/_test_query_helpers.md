---
title: 'Module: tests/unit/mcp/_test_query_helpers.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/_test_query_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp._test_query_helpers`/Test
symbols:
  TestFormatSummaryTestMixin: FormatSummaryTestMixin#
  TestExtractNameFromContentTestMixin: ExtractNameFromContentTestMixin#
  TestGetAvailableQueriesTestMixin: GetAvailableQueriesTestMixin#
  TestFormatSummaryAdditionalTestMixin: FormatSummaryAdditionalTestMixin#
  TestExtractNameAdditionalTestMixin: ExtractNameAdditionalTestMixin#
  TestFormatSummaryCoverageBoostTestMixin: FormatSummaryCoverageBoostTestMixin#
  TestExtractNameCoverageBoostTestMixin: ExtractNameCoverageBoostTestMixin#
  TestCategorizeQueriesTestMixin: CategorizeQueriesTestMixin#
  TestBuildNextStepsTestMixin: BuildNextStepsTestMixin#
  TestCategorizeQueriesTestMixin.test_common_keys_categorized: CategorizeQueriesTestMixin#test_common_keys_categorized().
  TestCategorizeQueriesTestMixin.test_declaration_keys_categorized: CategorizeQueriesTestMixin#test_declaration_keys_categorized().
  TestCategorizeQueriesTestMixin.test_control_flow_keys_categorized: CategorizeQueriesTestMixin#test_control_flow_keys_categorized().
  TestCategorizeQueriesTestMixin.test_framework_keys_categorized: CategorizeQueriesTestMixin#test_framework_keys_categorized().
  TestCategorizeQueriesTestMixin.test_other_keys_categorized: CategorizeQueriesTestMixin#test_other_keys_categorized().
  TestCategorizeQueriesTestMixin.test_empty_categories_removed: CategorizeQueriesTestMixin#test_empty_categories_removed().
  TestCategorizeQueriesTestMixin.test_mixed_categorization: CategorizeQueriesTestMixin#test_mixed_categorization().
  TestCategorizeQueriesTestMixin.test_empty_query_list: CategorizeQueriesTestMixin#test_empty_query_list().
  TestFormatSummaryTestMixin.test_format_summary_basic: FormatSummaryTestMixin#test_format_summary_basic().
  TestFormatSummaryTestMixin.test_format_summary_grouping: FormatSummaryTestMixin#test_format_summary_grouping().
  TestFormatSummaryTestMixin.test_format_summary_item_structure: FormatSummaryTestMixin#test_format_summary_item_structure().
  TestFormatSummaryTestMixin.test_format_summary_multiple_captures: FormatSummaryTestMixin#test_format_summary_multiple_captures().
  TestExtractNameFromContentTestMixin.test_extract_method_name: ExtractNameFromContentTestMixin#test_extract_method_name().
  TestExtractNameFromContentTestMixin.test_extract_class_name: ExtractNameFromContentTestMixin#test_extract_class_name().
  TestExtractNameFromContentTestMixin.test_extract_function_name: ExtractNameFromContentTestMixin#test_extract_function_name().
  TestExtractNameFromContentTestMixin.test_extract_markdown_header: ExtractNameFromContentTestMixin#test_extract_markdown_header().
  TestExtractNameFromContentTestMixin.test_extract_unnamed: ExtractNameFromContentTestMixin#test_extract_unnamed().
  TestExtractNameFromContentTestMixin.test_extract_empty_content: ExtractNameFromContentTestMixin#test_extract_empty_content().
  TestExtractNameFromContentTestMixin.test_extract_whitespace_only_content: ExtractNameFromContentTestMixin#test_extract_whitespace_only_content().
  TestExtractNameFromContentTestMixin.test_extract_private_method: ExtractNameFromContentTestMixin#test_extract_private_method().
  TestExtractNameFromContentTestMixin.test_extract_protected_method: ExtractNameFromContentTestMixin#test_extract_protected_method().
  TestExtractNameFromContentTestMixin.test_extract_subheading: ExtractNameFromContentTestMixin#test_extract_subheading().
  TestGetAvailableQueriesTestMixin.test_get_available_queries: GetAvailableQueriesTestMixin#test_get_available_queries().
  TestFormatSummaryAdditionalTestMixin.test_format_summary_empty_results: FormatSummaryAdditionalTestMixin#test_format_summary_empty_results().
  TestFormatSummaryAdditionalTestMixin.test_format_summary_single_result: FormatSummaryAdditionalTestMixin#test_format_summary_single_result().
  TestExtractNameAdditionalTestMixin.test_extract_interface_name: ExtractNameAdditionalTestMixin#test_extract_interface_name().
  TestExtractNameAdditionalTestMixin.test_extract_static_method_name: ExtractNameAdditionalTestMixin#test_extract_static_method_name().
  TestExtractNameAdditionalTestMixin.test_extract_deep_subheading: ExtractNameAdditionalTestMixin#test_extract_deep_subheading().
  TestFormatSummaryCoverageBoostTestMixin.test_format_summary_multi_capture_with_items: FormatSummaryCoverageBoostTestMixin#test_format_summary_multi_capture_with_items().
  TestExtractNameCoverageBoostTestMixin.test_extract_simple_function_call: ExtractNameCoverageBoostTestMixin#test_extract_simple_function_call().
  TestExtractNameCoverageBoostTestMixin.test_extract_private_static_class: ExtractNameCoverageBoostTestMixin#test_extract_private_static_class().
  TestExtractNameCoverageBoostTestMixin.test_extract_unnamed_no_pattern_match: ExtractNameCoverageBoostTestMixin#test_extract_unnamed_no_pattern_match().
  TestBuildNextStepsTestMixin.test_empty_results_returns_empty: BuildNextStepsTestMixin#test_empty_results_returns_empty().
  TestBuildNextStepsTestMixin.test_single_result_suggests_other_queries: BuildNextStepsTestMixin#test_single_result_suggests_other_queries().
  TestBuildNextStepsTestMixin.test_many_results_suggests_filter: BuildNextStepsTestMixin#test_many_results_suggests_filter().
  TestBuildNextStepsTestMixin.test_named_results_with_method_query_suggests_search: BuildNextStepsTestMixin#test_named_results_with_method_query_suggests_search().
  TestBuildNextStepsTestMixin.test_named_results_with_function_query_suggests_search: BuildNextStepsTestMixin#test_named_results_with_function_query_suggests_search().
  TestBuildNextStepsTestMixin.test_unnamed_results_no_search_suggestion: BuildNextStepsTestMixin#test_unnamed_results_no_search_suggestion().
  TestBuildNextStepsTestMixin.test_non_method_function_query_no_search: BuildNextStepsTestMixin#test_non_method_function_query_no_search().
  TestBuildNextStepsTestMixin.test_returns_at_most_three_steps: BuildNextStepsTestMixin#test_returns_at_most_three_steps().
  TestBuildNextStepsTestMixin.test_extractable_result_generates_extract_step: BuildNextStepsTestMixin#test_extractable_result_generates_extract_step().
  TestBuildNextStepsTestMixin.test_no_line_range_no_extract_step: BuildNextStepsTestMixin#test_no_line_range_no_extract_step().
  TestBuildNextStepsTestMixin.test_same_start_end_line_no_extract: BuildNextStepsTestMixin#test_same_start_end_line_no_extract().
---
# Module: [`tests/unit/mcp/_test_query_helpers.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_helpers.py)

## Classes
### `TestBuildNextStepsTestMixin`
- def: [`tests/unit/mcp/_test_query_helpers.py:311`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_helpers.py#L311)
- doc: Tests for _build_next_steps method.
- signature: `class TestBuildNextStepsTestMixin:`
- members:
  - `test_empty_results_returns_empty(self, tool)` — [`L314`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_helpers.py#L314)
  - `test_extractable_result_generates_extract_step(self, tool)` — [`L418`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_helpers.py#L418)
  - `test_many_results_suggests_filter(self, tool)` — [`L332`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_helpers.py#L332)
  - `test_named_results_with_function_query_suggests_search(self, tool)` — [`L366`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_helpers.py#L366)
  - `test_named_results_with_method_query_suggests_search(self, tool)` — [`L346`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_helpers.py#L346)
  - `test_no_line_range_no_extract_step(self, tool)` — [`L431`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_helpers.py#L431)
  - `test_non_method_function_query_no_search(self, tool)` — [`L391`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_helpers.py#L391)
  - `test_returns_at_most_three_steps(self, tool)` — [`L404`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_helpers.py#L404)
  - `test_same_start_end_line_no_extract(self, tool)` — [`L436`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_helpers.py#L436)
  - `test_single_result_suggests_other_queries(self, tool)` — [`L319`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_helpers.py#L319)
  - `test_unnamed_results_no_search_suggestion(self, tool)` — [`L379`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_helpers.py#L379)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `TestCategorizeQueriesTestMixin`
- def: [`tests/unit/mcp/_test_query_helpers.py:224`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_helpers.py#L224)
- doc: Tests for _categorize_queries helper function.
- signature: `class TestCategorizeQueriesTestMixin:`
- members:
  - `test_common_keys_categorized(self)` — [`L227`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_helpers.py#L227)
  - `test_control_flow_keys_categorized(self)` — [`L252`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_helpers.py#L252)
  - `test_declaration_keys_categorized(self)` — [`L242`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_helpers.py#L242)
  - `test_empty_categories_removed(self)` — [`L277`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_helpers.py#L277)
  - `test_empty_query_list(self)` — [`L304`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_helpers.py#L304)
  - `test_framework_keys_categorized(self)` — [`L261`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_helpers.py#L261)
  - `test_mixed_categorization(self)` — [`L285`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_helpers.py#L285)
  - `test_other_keys_categorized(self)` — [`L270`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_helpers.py#L270)
- uses (calls/refs, reference-scoped): [`_categorize_queries`](../../../tree_sitter_analyzer/mcp/tools/query_tool.md#_categorize_queries)  (1 test-only)
- used by: (1 test-only callers)

### `TestExtractNameAdditionalTestMixin`
- def: [`tests/unit/mcp/_test_query_helpers.py:149`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_helpers.py#L149)
- doc: Additional tests for _extract_name_from_content.
- signature: `class TestExtractNameAdditionalTestMixin:`
- members:
  - `test_extract_deep_subheading(self, tool)` — [`L162`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_helpers.py#L162)
  - `test_extract_interface_name(self, tool)` — [`L152`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_helpers.py#L152)
  - `test_extract_static_method_name(self, tool)` — [`L157`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_helpers.py#L157)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `TestExtractNameCoverageBoostTestMixin`
- def: [`tests/unit/mcp/_test_query_helpers.py:208`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_helpers.py#L208)
- doc: Tests targeting uncovered _extract_name_from_content branches.
- signature: `class TestExtractNameCoverageBoostTestMixin:`
- members:
  - `test_extract_private_static_class(self, tool)` — [`L215`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_helpers.py#L215)
  - `test_extract_simple_function_call(self, tool)` — [`L211`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_helpers.py#L211)
  - `test_extract_unnamed_no_pattern_match(self, tool)` — [`L219`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_helpers.py#L219)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `TestExtractNameFromContentTestMixin`
- def: [`tests/unit/mcp/_test_query_helpers.py:55`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_helpers.py#L55)
- doc: Tests for _extract_name_from_content method.
- signature: `class TestExtractNameFromContentTestMixin:`
- members:
  - `test_extract_class_name(self, tool)` — [`L63`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_helpers.py#L63)
  - `test_extract_empty_content(self, tool)` — [`L83`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_helpers.py#L83)
  - `test_extract_function_name(self, tool)` — [`L68`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_helpers.py#L68)
  - `test_extract_markdown_header(self, tool)` — [`L73`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_helpers.py#L73)
  - `test_extract_method_name(self, tool)` — [`L58`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_helpers.py#L58)
  - `test_extract_private_method(self, tool)` — [`L91`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_helpers.py#L91)
  - `test_extract_protected_method(self, tool)` — [`L96`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_helpers.py#L96)
  - `test_extract_subheading(self, tool)` — [`L101`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_helpers.py#L101)
  - `test_extract_unnamed(self, tool)` — [`L78`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_helpers.py#L78)
  - `test_extract_whitespace_only_content(self, tool)` — [`L87`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_helpers.py#L87)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `TestFormatSummaryAdditionalTestMixin`
- def: [`tests/unit/mcp/_test_query_helpers.py:120`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_helpers.py#L120)
- doc: Additional tests for _format_summary.
- signature: `class TestFormatSummaryAdditionalTestMixin:`
- members:
  - `test_format_summary_empty_results(self, tool)` — [`L123`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_helpers.py#L123)
  - `test_format_summary_single_result(self, tool)` — [`L129`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_helpers.py#L129)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `TestFormatSummaryCoverageBoostTestMixin`
- def: [`tests/unit/mcp/_test_query_helpers.py:168`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_helpers.py#L168)
- doc: Tests targeting uncovered _format_summary branches.
- signature: `class TestFormatSummaryCoverageBoostTestMixin:`
- members:
  - `test_format_summary_multi_capture_with_items(self, tool)` — [`L171`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_helpers.py#L171)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `TestFormatSummaryTestMixin`
- def: [`tests/unit/mcp/_test_query_helpers.py:6`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_helpers.py#L6)
- doc: Tests for _format_summary method.
- signature: `class TestFormatSummaryTestMixin:`
- members:
  - `test_format_summary_basic(self, tool, mock_query_results)` — [`L9`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_helpers.py#L9)
  - `test_format_summary_grouping(self, tool, mock_query_results)` — [`L17`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_helpers.py#L17)
  - `test_format_summary_item_structure(self, tool, mock_query_results)` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_helpers.py#L22)
  - `test_format_summary_multiple_captures(self, tool)` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_helpers.py#L30)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `TestGetAvailableQueriesTestMixin`
- def: [`tests/unit/mcp/_test_query_helpers.py:107`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_helpers.py#L107)
- doc: Tests for get_available_queries method.
- signature: `class TestGetAvailableQueriesTestMixin:`
- members:
  - `test_get_available_queries(self, tool)` — [`L110`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/_test_query_helpers.py#L110)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

