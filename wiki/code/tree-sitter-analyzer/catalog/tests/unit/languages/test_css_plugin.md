---
title: 'Module: tests/unit/languages/test_css_plugin.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_css_plugin.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_css_plugin`/
symbols:
  TestCssIntegration.test_style_element_summary: TestCssIntegration#test_style_element_summary().
  MockRequest.query_filters: MockRequest#query_filters.
  TestCssIntegration.test_style_element_creation: TestCssIntegration#test_style_element_creation().
  TestCssIntegration.test_media_query_element: TestCssIntegration#test_media_query_element().
  TestCssIntegration.test_keyframes_element: TestCssIntegration#test_keyframes_element().
  TestCssIntegration.test_complex_selector_element: TestCssIntegration#test_complex_selector_element().
  TestCssElementExtractor.extractor: TestCssElementExtractor#extractor.
  TestCssExtractorErrorPaths.extractor: TestCssExtractorErrorPaths#extractor.
  TestScssVariableExtraction.test_scss_variables_extracted_from_file.MockRequest.query_filters: TestScssVariableExtraction#test_scss_variables_extracted_from_file().MockRequest#query_filters.
  TestScssVariableExtraction.test_scss_variables_have_correct_line_numbers.MockRequest.query_filters: TestScssVariableExtraction#test_scss_variables_have_correct_line_numbers().MockRequest#query_filters.
  TestCssExtractAtRuleName.extractor: TestCssExtractAtRuleName#extractor.
  TestCssExtractAtRuleName._get_parser: TestCssExtractAtRuleName#_get_parser().
  TestCssPluginAnalyzeFallback.test_analyze_file_import_error_fallback.MockRequest.query_filters: TestCssPluginAnalyzeFallback#test_analyze_file_import_error_fallback().MockRequest#query_filters.
  TestCssPluginAnalyzeFallback.test_analyze_file_read_error.MockRequest.query_filters: TestCssPluginAnalyzeFallback#test_analyze_file_read_error().MockRequest#query_filters.
  TestScssVariableExtraction.test_scss_no_variables_returns_css_rules_only.MockRequest.query_filters: TestScssVariableExtraction#test_scss_no_variables_returns_css_rules_only().MockRequest#query_filters.
  TestScssVariableExtraction.test_plain_css_file_unaffected_by_scss_extraction.MockRequest.query_filters: TestScssVariableExtraction#test_plain_css_file_unaffected_by_scss_extraction().MockRequest#query_filters.
  TestCssPlugin.plugin: TestCssPlugin#plugin.
  TestCssExtractAtRuleName.test_extract_keyframes_name_with_animation_name: TestCssExtractAtRuleName#test_extract_keyframes_name_with_animation_name().
  TestCssExtractAtRuleName.test_extract_media_query_with_full_condition: TestCssExtractAtRuleName#test_extract_media_query_with_full_condition().
  TestCssExtractAtRuleName.test_extract_media_query_with_screen_and_condition: TestCssExtractAtRuleName#test_extract_media_query_with_screen_and_condition().
  TestCssExtractAtRuleName.test_extract_media_query_with_complex_condition: TestCssExtractAtRuleName#test_extract_media_query_with_complex_condition().
  TestCssExtractAtRuleName.test_extract_media_query_prefers_color_scheme: TestCssExtractAtRuleName#test_extract_media_query_prefers_color_scheme().
  TestCssExtractAtRuleName.test_extract_media_query_print: TestCssExtractAtRuleName#test_extract_media_query_print().
  TestCssExtractAtRuleName.test_extract_multiple_keyframes: TestCssExtractAtRuleName#test_extract_multiple_keyframes().
  TestCssExtractAtRuleName.test_extract_supports_rule: TestCssExtractAtRuleName#test_extract_supports_rule().
  TestCssExtractorErrorPaths.test_extract_css_rules_exception_during_traversal.BadTree.root_node: TestCssExtractorErrorPaths#test_extract_css_rules_exception_during_traversal().BadTree#root_node.
  TestCssExtractorErrorPaths.test_extract_node_text_exception.BadNode.end_byte: TestCssExtractorErrorPaths#test_extract_node_text_exception().BadNode#end_byte.
  TestCssExtractorErrorPaths.test_extract_selector_no_selectors_child_with_brace.FakeNode.end_byte: TestCssExtractorErrorPaths#test_extract_selector_no_selectors_child_with_brace().FakeNode#end_byte.
  TestCssExtractorErrorPaths.test_extract_selector_no_brace_returns_unknown.FakeNode.end_byte: TestCssExtractorErrorPaths#test_extract_selector_no_brace_returns_unknown().FakeNode#end_byte.
  TestCssExtractorErrorPaths.test_extract_selector_exception_returns_unknown.BadNode.children: TestCssExtractorErrorPaths#test_extract_selector_exception_returns_unknown().BadNode#children.
  TestCssExtractorErrorPaths.test_extract_properties_no_block_child.FakeNode.children: TestCssExtractorErrorPaths#test_extract_properties_no_block_child().FakeNode#children.
  TestCssExtractorErrorPaths.test_extract_properties_exception.BadNode.children: TestCssExtractorErrorPaths#test_extract_properties_exception().BadNode#children.
  TestCssExtractorErrorPaths.test_parse_declaration_no_children.FakeDecl.end_byte: TestCssExtractorErrorPaths#test_parse_declaration_no_children().FakeDecl#end_byte.
  TestCssExtractorErrorPaths.test_parse_declaration_empty_children.FakeDecl.end_byte: TestCssExtractorErrorPaths#test_parse_declaration_empty_children().FakeDecl#end_byte.
  TestCssExtractorErrorPaths.test_parse_declaration_exception.BadDecl.children: TestCssExtractorErrorPaths#test_parse_declaration_exception().BadDecl#children.
  TestCssExtractorErrorPaths.test_create_style_element_exception.BadNode.type: TestCssExtractorErrorPaths#test_create_style_element_exception().BadNode#type.
  TestCssExtractorErrorPaths.test_extract_at_rule_name_non_standard.FakeNode.end_byte: TestCssExtractorErrorPaths#test_extract_at_rule_name_non_standard().FakeNode#end_byte.
  TestCssExtractorErrorPaths.test_extract_at_rule_name_no_at_sign.FakeNode.end_byte: TestCssExtractorErrorPaths#test_extract_at_rule_name_no_at_sign().FakeNode#end_byte.
  TestCssExtractorErrorPaths.test_extract_at_rule_name_exception.BadNode.end_byte: TestCssExtractorErrorPaths#test_extract_at_rule_name_exception().BadNode#end_byte.
  TestScssVariableExtraction.test_extract_scss_variables_unit: TestScssVariableExtraction#test_extract_scss_variables_unit().
  TestScssVariableExtraction.test_extract_scss_variables_deduplicates_on_first_occurrence: TestScssVariableExtraction#test_extract_scss_variables_deduplicates_on_first_occurrence().
  TestCssElementExtractor.test_property_categories: TestCssElementExtractor#test_property_categories().
  TestCssElementExtractor.test_classify_rule: TestCssElementExtractor#test_classify_rule().
  TestCssElementExtractor.test_extract_functions_returns_empty: TestCssElementExtractor#test_extract_functions_returns_empty().
  TestCssElementExtractor.test_extract_classes_returns_empty: TestCssElementExtractor#test_extract_classes_returns_empty().
  TestCssElementExtractor.test_extract_variables_returns_empty: TestCssElementExtractor#test_extract_variables_returns_empty().
  TestCssElementExtractor.test_extract_imports_returns_empty: TestCssElementExtractor#test_extract_imports_returns_empty().
  TestCssPlugin.test_get_supported_element_types: TestCssPlugin#test_get_supported_element_types().
  TestCssPlugin.test_get_queries: TestCssPlugin#test_get_queries().
  TestCssPlugin.test_execute_query_strategy: TestCssPlugin#test_execute_query_strategy().
  TestCssPlugin.test_get_element_categories: TestCssPlugin#test_get_element_categories().
  TestCssExtractorErrorPaths.test_extract_css_rules_no_root_node: TestCssExtractorErrorPaths#test_extract_css_rules_no_root_node().
  TestCssPluginAnalyzeFallback.test_execute_query_strategy_none_key: TestCssPluginAnalyzeFallback#test_execute_query_strategy_none_key().
  TestCssPluginAnalyzeFallback.test_execute_query_strategy_unknown_key: TestCssPluginAnalyzeFallback#test_execute_query_strategy_unknown_key().
  TestScssVariableExtraction.test_scss_variables_extracted_from_file: TestScssVariableExtraction#test_scss_variables_extracted_from_file().
  TestScssVariableExtraction.test_scss_variables_have_correct_line_numbers: TestScssVariableExtraction#test_scss_variables_have_correct_line_numbers().
  TestScssVariableExtraction.test_scss_no_variables_returns_css_rules_only: TestScssVariableExtraction#test_scss_no_variables_returns_css_rules_only().
  TestScssVariableExtraction.test_plain_css_file_unaffected_by_scss_extraction: TestScssVariableExtraction#test_plain_css_file_unaffected_by_scss_extraction().
  TestScssVariableExtraction.test_extract_scss_variables_skips_block_comments: TestScssVariableExtraction#test_extract_scss_variables_skips_block_comments().
  TestScssVariableExtraction.test_extract_scss_variables_skips_inline_block_comment: TestScssVariableExtraction#test_extract_scss_variables_skips_inline_block_comment().
  TestScssVariableExtraction.test_extract_scss_variables_literal_slash_star_in_string: TestScssVariableExtraction#test_extract_scss_variables_literal_slash_star_in_string().
  TestScssVariableExtraction.test_extract_scss_variables_single_quoted_slash_star: TestScssVariableExtraction#test_extract_scss_variables_single_quoted_slash_star().
  TestCssExtractAtRuleName.plugin: TestCssExtractAtRuleName#plugin.
  TestCssExtractorErrorPaths.setup_method: TestCssExtractorErrorPaths#setup_method().
  TestCssExtractorErrorPaths.test_parse_declaration_empty_children.FakeDecl.children: TestCssExtractorErrorPaths#test_parse_declaration_empty_children().FakeDecl#children.
  TestCssPluginAnalyzeFallback.test_analyze_file_import_error_fallback: TestCssPluginAnalyzeFallback#test_analyze_file_import_error_fallback().
  TestCssPluginAnalyzeFallback.test_analyze_file_read_error: TestCssPluginAnalyzeFallback#test_analyze_file_read_error().
  TestCssPlugin.test_analyze_file_fallback.MockRequest: TestCssPlugin#test_analyze_file_fallback().MockRequest#
  TestCssExtractorErrorPaths.test_extract_css_rules_exception_during_traversal.BadTree: TestCssExtractorErrorPaths#test_extract_css_rules_exception_during_traversal().BadTree#
  TestCssExtractorErrorPaths.test_extract_node_text_exception.BadNode: TestCssExtractorErrorPaths#test_extract_node_text_exception().BadNode#
  TestCssExtractorErrorPaths.test_extract_selector_no_selectors_child_with_brace.FakeNode: TestCssExtractorErrorPaths#test_extract_selector_no_selectors_child_with_brace().FakeNode#
  TestCssExtractorErrorPaths.test_extract_selector_no_brace_returns_unknown.FakeNode: TestCssExtractorErrorPaths#test_extract_selector_no_brace_returns_unknown().FakeNode#
  TestCssExtractorErrorPaths.test_extract_selector_exception_returns_unknown.BadNode: TestCssExtractorErrorPaths#test_extract_selector_exception_returns_unknown().BadNode#
  TestCssExtractorErrorPaths.test_extract_properties_no_block_child.FakeNode: TestCssExtractorErrorPaths#test_extract_properties_no_block_child().FakeNode#
  TestCssExtractorErrorPaths.test_extract_properties_exception.BadNode: TestCssExtractorErrorPaths#test_extract_properties_exception().BadNode#
  TestCssExtractorErrorPaths.test_parse_declaration_no_children.FakeDecl: TestCssExtractorErrorPaths#test_parse_declaration_no_children().FakeDecl#
  TestCssExtractorErrorPaths.test_parse_declaration_empty_children.FakeChild: TestCssExtractorErrorPaths#test_parse_declaration_empty_children().FakeChild#
  TestCssExtractorErrorPaths.test_parse_declaration_empty_children.FakeDecl: TestCssExtractorErrorPaths#test_parse_declaration_empty_children().FakeDecl#
  TestCssExtractorErrorPaths.test_parse_declaration_exception.BadDecl: TestCssExtractorErrorPaths#test_parse_declaration_exception().BadDecl#
  TestCssExtractorErrorPaths.test_create_style_element_exception.BadNode: TestCssExtractorErrorPaths#test_create_style_element_exception().BadNode#
  TestCssExtractorErrorPaths.test_extract_at_rule_name_non_standard.FakeNode: TestCssExtractorErrorPaths#test_extract_at_rule_name_non_standard().FakeNode#
  TestCssExtractorErrorPaths.test_extract_at_rule_name_no_at_sign.FakeNode: TestCssExtractorErrorPaths#test_extract_at_rule_name_no_at_sign().FakeNode#
  TestCssExtractorErrorPaths.test_extract_at_rule_name_exception.BadNode: TestCssExtractorErrorPaths#test_extract_at_rule_name_exception().BadNode#
  TestCssPluginAnalyzeFallback.test_analyze_file_import_error_fallback.MockRequest: TestCssPluginAnalyzeFallback#test_analyze_file_import_error_fallback().MockRequest#
  TestCssPluginAnalyzeFallback.test_analyze_file_read_error.MockRequest: TestCssPluginAnalyzeFallback#test_analyze_file_read_error().MockRequest#
  TestScssVariableExtraction.test_scss_variables_extracted_from_file.MockRequest: TestScssVariableExtraction#test_scss_variables_extracted_from_file().MockRequest#
  TestScssVariableExtraction.test_scss_variables_have_correct_line_numbers.MockRequest: TestScssVariableExtraction#test_scss_variables_have_correct_line_numbers().MockRequest#
  TestScssVariableExtraction.test_scss_no_variables_returns_css_rules_only.MockRequest: TestScssVariableExtraction#test_scss_no_variables_returns_css_rules_only().MockRequest#
  TestScssVariableExtraction.test_plain_css_file_unaffected_by_scss_extraction.MockRequest: TestScssVariableExtraction#test_plain_css_file_unaffected_by_scss_extraction().MockRequest#
  TestCssElementExtractor: TestCssElementExtractor#
  TestCssElementExtractor.setup_method: TestCssElementExtractor#setup_method().
  TestCssPlugin: TestCssPlugin#
  TestCssPlugin.setup_method: TestCssPlugin#setup_method().
  TestCssPlugin.test_analyze_file_fallback: TestCssPlugin#test_analyze_file_fallback().
  TestCssPlugin.test_analyze_file_fallback.MockRequest.__init__: TestCssPlugin#test_analyze_file_fallback().MockRequest#__init__().
  MockRequest.include_source: MockRequest#include_source.
  TestCssExtractAtRuleName: TestCssExtractAtRuleName#
  TestCssExtractAtRuleName.setup_method: TestCssExtractAtRuleName#setup_method().
  TestCssExtractorErrorPaths: TestCssExtractorErrorPaths#
  TestCssExtractorErrorPaths.test_extract_css_rules_exception_during_traversal: TestCssExtractorErrorPaths#test_extract_css_rules_exception_during_traversal().
  TestCssExtractorErrorPaths.test_extract_node_text_exception: TestCssExtractorErrorPaths#test_extract_node_text_exception().
  TestCssExtractorErrorPaths.test_extract_node_text_exception.BadNode.start_byte: TestCssExtractorErrorPaths#test_extract_node_text_exception().BadNode#start_byte.
  TestCssExtractorErrorPaths.test_extract_selector_no_selectors_child_with_brace: TestCssExtractorErrorPaths#test_extract_selector_no_selectors_child_with_brace().
  TestCssExtractorErrorPaths.test_extract_selector_no_selectors_child_with_brace.FakeNode.type: TestCssExtractorErrorPaths#test_extract_selector_no_selectors_child_with_brace().FakeNode#type.
  TestCssExtractorErrorPaths.test_extract_selector_no_selectors_child_with_brace.FakeNode.children: TestCssExtractorErrorPaths#test_extract_selector_no_selectors_child_with_brace().FakeNode#children.
  TestCssExtractorErrorPaths.test_extract_selector_no_selectors_child_with_brace.FakeNode.start_byte: TestCssExtractorErrorPaths#test_extract_selector_no_selectors_child_with_brace().FakeNode#start_byte.
  TestCssExtractorErrorPaths.test_extract_selector_no_brace_returns_unknown: TestCssExtractorErrorPaths#test_extract_selector_no_brace_returns_unknown().
  TestCssExtractorErrorPaths.test_extract_selector_no_brace_returns_unknown.FakeNode.type: TestCssExtractorErrorPaths#test_extract_selector_no_brace_returns_unknown().FakeNode#type.
  TestCssExtractorErrorPaths.test_extract_selector_no_brace_returns_unknown.FakeNode.children: TestCssExtractorErrorPaths#test_extract_selector_no_brace_returns_unknown().FakeNode#children.
  TestCssExtractorErrorPaths.test_extract_selector_no_brace_returns_unknown.FakeNode.start_byte: TestCssExtractorErrorPaths#test_extract_selector_no_brace_returns_unknown().FakeNode#start_byte.
  TestCssExtractorErrorPaths.test_extract_selector_exception_returns_unknown: TestCssExtractorErrorPaths#test_extract_selector_exception_returns_unknown().
  TestCssExtractorErrorPaths.test_extract_properties_no_block_child: TestCssExtractorErrorPaths#test_extract_properties_no_block_child().
  TestCssExtractorErrorPaths.test_extract_properties_exception: TestCssExtractorErrorPaths#test_extract_properties_exception().
  TestCssExtractorErrorPaths.test_parse_declaration_no_children: TestCssExtractorErrorPaths#test_parse_declaration_no_children().
  TestCssExtractorErrorPaths.test_parse_declaration_no_children.FakeDecl.start_byte: TestCssExtractorErrorPaths#test_parse_declaration_no_children().FakeDecl#start_byte.
  TestCssExtractorErrorPaths.test_parse_declaration_empty_children: TestCssExtractorErrorPaths#test_parse_declaration_empty_children().
  TestCssExtractorErrorPaths.test_parse_declaration_empty_children.FakeChild.type: TestCssExtractorErrorPaths#test_parse_declaration_empty_children().FakeChild#type.
  TestCssExtractorErrorPaths.test_parse_declaration_empty_children.FakeChild.start_byte: TestCssExtractorErrorPaths#test_parse_declaration_empty_children().FakeChild#start_byte.
  TestCssExtractorErrorPaths.test_parse_declaration_empty_children.FakeChild.end_byte: TestCssExtractorErrorPaths#test_parse_declaration_empty_children().FakeChild#end_byte.
  TestCssExtractorErrorPaths.test_parse_declaration_empty_children.FakeDecl.start_byte: TestCssExtractorErrorPaths#test_parse_declaration_empty_children().FakeDecl#start_byte.
  TestCssExtractorErrorPaths.test_parse_declaration_exception: TestCssExtractorErrorPaths#test_parse_declaration_exception().
  TestCssExtractorErrorPaths.test_create_style_element_exception: TestCssExtractorErrorPaths#test_create_style_element_exception().
  TestCssExtractorErrorPaths.test_extract_at_rule_name_non_standard: TestCssExtractorErrorPaths#test_extract_at_rule_name_non_standard().
  TestCssExtractorErrorPaths.test_extract_at_rule_name_non_standard.FakeNode.start_byte: TestCssExtractorErrorPaths#test_extract_at_rule_name_non_standard().FakeNode#start_byte.
  TestCssExtractorErrorPaths.test_extract_at_rule_name_no_at_sign: TestCssExtractorErrorPaths#test_extract_at_rule_name_no_at_sign().
  TestCssExtractorErrorPaths.test_extract_at_rule_name_no_at_sign.FakeNode.start_byte: TestCssExtractorErrorPaths#test_extract_at_rule_name_no_at_sign().FakeNode#start_byte.
  TestCssExtractorErrorPaths.test_extract_at_rule_name_exception: TestCssExtractorErrorPaths#test_extract_at_rule_name_exception().
  TestCssExtractorErrorPaths.test_extract_at_rule_name_exception.BadNode.start_byte: TestCssExtractorErrorPaths#test_extract_at_rule_name_exception().BadNode#start_byte.
  TestCssPluginAnalyzeFallback: TestCssPluginAnalyzeFallback#
  TestCssPluginAnalyzeFallback.test_analyze_file_import_error_fallback.MockRequest.include_source: TestCssPluginAnalyzeFallback#test_analyze_file_import_error_fallback().MockRequest#include_source.
  TestCssPluginAnalyzeFallback.test_analyze_file_read_error.MockRequest.include_source: TestCssPluginAnalyzeFallback#test_analyze_file_read_error().MockRequest#include_source.
  TestCssIntegration: TestCssIntegration#
  TestScssVariableExtraction: TestScssVariableExtraction#
  TestScssVariableExtraction.test_scss_variables_extracted_from_file.MockRequest.include_source: TestScssVariableExtraction#test_scss_variables_extracted_from_file().MockRequest#include_source.
  TestScssVariableExtraction.test_scss_variables_have_correct_line_numbers.MockRequest.include_source: TestScssVariableExtraction#test_scss_variables_have_correct_line_numbers().MockRequest#include_source.
  TestScssVariableExtraction.test_scss_no_variables_returns_css_rules_only.MockRequest.include_source: TestScssVariableExtraction#test_scss_no_variables_returns_css_rules_only().MockRequest#include_source.
  TestScssVariableExtraction.test_plain_css_file_unaffected_by_scss_extraction.MockRequest.include_source: TestScssVariableExtraction#test_plain_css_file_unaffected_by_scss_extraction().MockRequest#include_source.
---
# Module: [`tests/unit/languages/test_css_plugin.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py)

## Classes
### `BadDecl`
- def: [`tests/unit/languages/test_css_plugin.py:461`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L461)
- signature: `class BadDecl:`
- members:
  - `children` — [`L462`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L462)
- uses (calls/refs, reference-scoped): [`_parse_declaration`](../../../tree_sitter_analyzer/languages/css_plugin.md#CssElementExtractor._parse_declaration)  (1 test-only)

### `BadNode`
- def: [`tests/unit/languages/test_css_plugin.py:500`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L500)
- signature: `class BadNode:`
- members:
  - `children` — [`L407`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L407)
  - `children` — [`L425`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L425)
  - `end_byte` — [`L375`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L375)
  - `end_byte` — [`L502`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L502)
  - `start_byte` — [`L372`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L372)
  - `start_byte` — [`L501`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L501)
  - `type` — [`L472`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L472)
- uses (calls/refs, reference-scoped): [`_create_style_element`](../../../tree_sitter_analyzer/languages/css_plugin.md#CssElementExtractor._create_style_element), [`_extract_node_text`](../../../tree_sitter_analyzer/languages/css_plugin.md#CssElementExtractor._extract_node_text), [`_extract_at_rule_name`](../../../tree_sitter_analyzer/languages/css_plugin.md#CssElementExtractor._extract_at_rule_name), [`_extract_selector`](../../../tree_sitter_analyzer/languages/css_plugin.md#CssElementExtractor._extract_selector), [`_extract_properties`](../../../tree_sitter_analyzer/languages/css_plugin.md#CssElementExtractor._extract_properties)  (5 test-only)

### `BadTree`
- def: [`tests/unit/languages/test_css_plugin.py:360`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L360)
- signature: `class BadTree:`
- members:
  - `root_node` — [`L361`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L361)
- uses (calls/refs, reference-scoped): [`extract_css_rules`](../../../tree_sitter_analyzer/languages/css_plugin.md#CssElementExtractor.extract_css_rules)  (1 test-only)

### `FakeChild`
- def: [`tests/unit/languages/test_css_plugin.py:444`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L444)
- signature: `class FakeChild:`
- members:
  - `end_byte` — [`L447`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L447)
  - `start_byte` — [`L446`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L446)
  - `type` — [`L445`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L445)
- used by: (1 test-only callers)

### `FakeDecl`
- def: [`tests/unit/languages/test_css_plugin.py:449`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L449)
- signature: `class FakeDecl:`
- members:
  - `children` — [`L450`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L450)
  - `end_byte` — [`L435`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L435)
  - `end_byte` — [`L452`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L452)
  - `start_byte` — [`L434`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L434)
  - `start_byte` — [`L451`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L451)
- uses (calls/refs, reference-scoped): [`_parse_declaration`](../../../tree_sitter_analyzer/languages/css_plugin.md#CssElementExtractor._parse_declaration)  (3 test-only)

### `FakeNode`
- def: [`tests/unit/languages/test_css_plugin.py:490`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L490)
- signature: `class FakeNode:`
- members:
  - `children` — [`L384`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L384)
  - `children` — [`L396`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L396)
  - `children` — [`L416`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L416)
  - `end_byte` — [`L386`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L386)
  - `end_byte` — [`L398`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L398)
  - `end_byte` — [`L482`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L482)
  - `end_byte` — [`L492`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L492)
  - `start_byte` — [`L385`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L385)
  - `start_byte` — [`L397`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L397)
  - `start_byte` — [`L481`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L481)
  - `start_byte` — [`L491`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L491)
  - `type` — [`L383`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L383)
  - `type` — [`L395`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L395)
- uses (calls/refs, reference-scoped): [`_extract_at_rule_name`](../../../tree_sitter_analyzer/languages/css_plugin.md#CssElementExtractor._extract_at_rule_name), [`_extract_selector`](../../../tree_sitter_analyzer/languages/css_plugin.md#CssElementExtractor._extract_selector), [`_extract_properties`](../../../tree_sitter_analyzer/languages/css_plugin.md#CssElementExtractor._extract_properties)  (5 test-only)

### `MockRequest`
- def: [`tests/unit/languages/test_css_plugin.py:775`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L775)
- signature: `class MockRequest:`
- members:
  - `include_source` — [`L162`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L162)
  - `include_source` — [`L520`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L520)
  - `include_source` — [`L552`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L552)
  - `include_source` — [`L687`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L687)
  - `include_source` — [`L721`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L721)
  - `include_source` — [`L750`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L750)
  - `include_source` — [`L776`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L776)
  - `query_filters` — [`L163`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L163)
  - `query_filters` — [`L521`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L521)
  - `query_filters` — [`L553`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L553)
  - `query_filters` — [`L688`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L688)
  - `query_filters` — [`L722`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L722)
  - `query_filters` — [`L751`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L751)
  - `query_filters` — [`L777`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L777)
- protocol/private: `__init__`[`L161`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L161)
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`start_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`Variable`](../../../tree_sitter_analyzer/models/base.md#Variable), [`elements`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.elements), [`language`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.language), [`success`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.success), [`line_count`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.line_count), [`error_message`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.error_message), [`StyleElement`](../../../tree_sitter_analyzer/models/markup_models.md#StyleElement), [`source_code`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.source_code), [`analyze_file`](../../../tree_sitter_analyzer/languages/css_plugin.md#CssPlugin.analyze_file)  (7 test-only)

### `TestCssElementExtractor`
- def: [`tests/unit/languages/test_css_plugin.py:16`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L16)
- doc: Test CSS element extraction functionality
- signature: `class TestCssElementExtractor:`
- members:
  - `setup_method(self)` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L19) — Set up test fixtures
  - `test_classify_rule(self)` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L33) — Test CSS rule classification
  - `test_extract_classes_returns_empty(self)` — [`L63`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L63) — Test that CSS extractor returns empty list for classes
  - `test_extract_functions_returns_empty(self)` — [`L58`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L58) — Test that CSS extractor returns empty list for functions
  - `test_extract_imports_returns_empty(self)` — [`L73`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L73) — Test that CSS extractor returns empty list for imports
  - `test_extract_variables_returns_empty(self)` — [`L68`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L68) — Test that CSS extractor returns empty list for variables
  - `test_property_categories(self)` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L23) — Test CSS property categorization
  - `extractor` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L21)
- uses (calls/refs, reference-scoped): [`_classify_rule`](../../../tree_sitter_analyzer/languages/css_plugin.md#CssElementExtractor._classify_rule), [`property_categories`](../../../tree_sitter_analyzer/languages/css_plugin.md#CssElementExtractor.property_categories), [`CssElementExtractor`](../../../tree_sitter_analyzer/languages/css_plugin.md#CssElementExtractor), [`extract_classes`](../../../tree_sitter_analyzer/languages/css_plugin.md#CssElementExtractor.extract_classes), [`extract_functions`](../../../tree_sitter_analyzer/languages/css_plugin.md#CssElementExtractor.extract_functions), [`extract_imports`](../../../tree_sitter_analyzer/languages/css_plugin.md#CssElementExtractor.extract_imports), [`extract_variables`](../../../tree_sitter_analyzer/languages/css_plugin.md#CssElementExtractor.extract_variables)

### `TestCssExtractAtRuleName`
- def: [`tests/unit/languages/test_css_plugin.py:195`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L195)
- doc: Test _extract_at_rule_name method for CSS at-rules.
- signature: `class TestCssExtractAtRuleName:`
- members:
  - `_get_parser(self)` — [`L203`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L203) — Get a configured tree-sitter parser for CSS.
  - `setup_method(self)` — [`L198`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L198) — Set up test fixtures
  - `test_extract_keyframes_name_with_animation_name(self)` — [`L217`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L217) — Test that @keyframes extracts the full name including animation name.
  - `test_extract_media_query_prefers_color_scheme(self)` — [`L274`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L274) — Test that @media prefers-color-scheme extracts correctly.
  - `test_extract_media_query_print(self)` — [`L288`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L288) — Test that @media print extracts correctly.
  - `test_extract_media_query_with_complex_condition(self)` — [`L260`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L260) — Test that @media with combined conditions extracts correctly.
  - `test_extract_media_query_with_full_condition(self)` — [`L232`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L232) — Test that @media extracts the full condition.
  - `test_extract_media_query_with_screen_and_condition(self)` — [`L246`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L246) — Test that @media screen and condition extracts correctly.
  - `test_extract_multiple_keyframes(self)` — [`L301`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L301) — Test that multiple @keyframes are extracted with distinct names.
  - `test_extract_supports_rule(self)` — [`L330`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L330) — Test that @supports extracts the full condition.
  - `extractor` — [`L201`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L201)
  - `plugin` — [`L200`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L200)
- uses (calls/refs, reference-scoped): [`CssPlugin`](../../../tree_sitter_analyzer/languages/css_plugin.md#CssPlugin), [`extract_css_rules`](../../../tree_sitter_analyzer/plugins/base.md#ElementExtractor.extract_css_rules), [`create_extractor`](../../../tree_sitter_analyzer/languages/css_plugin.md#CssPlugin.create_extractor), [`get_tree_sitter_language`](../../../tree_sitter_analyzer/languages/css_plugin.md#CssPlugin.get_tree_sitter_language)

### `TestCssExtractorErrorPaths`
- def: [`tests/unit/languages/test_css_plugin.py:346`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L346)
- doc: Cover error-handling and fallback branches in CssElementExtractor.
- signature: `class TestCssExtractorErrorPaths:`
- members:
  - `setup_method(self)` — [`L349`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L349)
  - `test_create_style_element_exception(self)` — [`L468`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L468) — _create_style_element returns None on exception.
  - `test_extract_at_rule_name_exception(self)` — [`L497`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L497) — _extract_at_rule_name returns empty string when _extract_node_text swallows error.
  - `test_extract_at_rule_name_no_at_sign(self)` — [`L487`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L487) — _extract_at_rule_name for text not starting with @.
  - `test_extract_at_rule_name_non_standard(self)` — [`L477`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L477) — _extract_at_rule_name for @charset / @namespace returns truncated text.
  - `test_extract_css_rules_exception_during_traversal(self)` — [`L357`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L357) — extract_css_rules handles exception from traversal.
  - `test_extract_css_rules_no_root_node(self)` — [`L352`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L352) — extract_css_rules with tree lacking root_node returns empty.
  - `test_extract_node_text_exception(self)` — [`L368`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L368) — _extract_node_text returns empty string on exception.
  - `test_extract_properties_exception(self)` — [`L421`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L421) — _extract_properties handles exception gracefully.
  - `test_extract_properties_no_block_child(self)` — [`L412`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L412) — _extract_properties returns empty dict when no block child.
  - `test_extract_selector_exception_returns_unknown(self)` — [`L403`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L403) — _extract_selector returns 'unknown' on exception.
  - `test_extract_selector_no_brace_returns_unknown(self)` — [`L391`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L391) — _extract_selector returns 'unknown' when text has no opening brace.
  - `test_extract_selector_no_selectors_child_with_brace(self)` — [`L379`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L379) — _extract_selector fallback when no selectors child but has brace.
  - `test_parse_declaration_empty_children(self)` — [`L441`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L441) — _parse_declaration fallback when children don't match types.
  - `test_parse_declaration_exception(self)` — [`L458`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L458) — _parse_declaration returns empty tuple on exception.
  - `test_parse_declaration_no_children(self)` — [`L430`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L430) — _parse_declaration fallback when node has no children.
  - `extractor` — [`L350`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L350)
- uses (calls/refs, reference-scoped): [`extract_css_rules`](../../../tree_sitter_analyzer/languages/css_plugin.md#CssElementExtractor.extract_css_rules), [`CssElementExtractor`](../../../tree_sitter_analyzer/languages/css_plugin.md#CssElementExtractor)
- used by: (14 test-only callers)

### `TestCssIntegration`
- def: [`tests/unit/languages/test_css_plugin.py:572`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L572)
- doc: Integration tests for CSS plugin
- signature: `class TestCssIntegration:`
- members:
  - `test_complex_selector_element(self)` — [`L650`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L650) — Test complex selector StyleElement
  - `test_keyframes_element(self)` — [`L633`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L633) — Test keyframes StyleElement
  - `test_media_query_element(self)` — [`L616`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L616) — Test media query StyleElement
  - `test_style_element_creation(self)` — [`L575`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L575) — Test StyleElement creation
  - `test_style_element_summary(self)` — [`L595`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L595) — Test StyleElement summary generation
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`start_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`end_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.end_line), [`language`](../../../tree_sitter_analyzer/models/base.md#CodeElement.language), [`raw_text`](../../../tree_sitter_analyzer/models/base.md#CodeElement.raw_text), [`StyleElement`](../../../tree_sitter_analyzer/models/markup_models.md#StyleElement), [`selector`](../../../tree_sitter_analyzer/models/markup_models.md#StyleElement.selector), [`element_class`](../../../tree_sitter_analyzer/models/markup_models.md#StyleElement.element_class), [`properties`](../../../tree_sitter_analyzer/models/markup_models.md#StyleElement.properties), [`to_summary_item`](../../../tree_sitter_analyzer/models/markup_models.md#StyleElement.to_summary_item)

### `TestCssPlugin`
- def: [`tests/unit/languages/test_css_plugin.py:79`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L79)
- doc: Test CSS plugin functionality
- signature: `class TestCssPlugin:`
- members:
  - `setup_method(self)` — [`L82`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L82) — Set up test fixtures
  - `test_analyze_file_fallback(self)` — [`L121`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L121) — Test CSS file analysis with fallback parsing
  - `test_execute_query_strategy(self)` — [`L100`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L100) — Test query strategy execution
  - `test_get_element_categories(self)` — [`L111`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L111) — Test element categories
  - `test_get_queries(self)` — [`L91`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L91) — Test query retrieval
  - `test_get_supported_element_types(self)` — [`L86`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L86) — Test supported element types
  - `plugin` — [`L84`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L84)
- uses (calls/refs, reference-scoped): [`CssPlugin`](../../../tree_sitter_analyzer/languages/css_plugin.md#CssPlugin), [`execute_query_strategy`](../../../tree_sitter_analyzer/languages/css_plugin.md#CssPlugin.execute_query_strategy), [`get_queries`](../../../tree_sitter_analyzer/languages/css_plugin.md#CssPlugin.get_queries), [`get_element_categories`](../../../tree_sitter_analyzer/languages/css_plugin.md#CssPlugin.get_element_categories), [`get_supported_element_types`](../../../tree_sitter_analyzer/languages/css_plugin.md#CssPlugin.get_supported_element_types)
- used by: (1 test-only callers)

### `TestCssPluginAnalyzeFallback`
- def: [`tests/unit/languages/test_css_plugin.py:508`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L508)
- doc: Cover analyze_file ImportError fallback path.
- signature: `class TestCssPluginAnalyzeFallback:`
- members:
  - `test_analyze_file_import_error_fallback(self)` — [`L512`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L512) — analyze_file falls back gracefully when tree_sitter_css is missing.
  - `test_analyze_file_read_error(self)` — [`L547`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L547) — analyze_file returns error result when file reading fails.
  - `test_execute_query_strategy_none_key(self)` — [`L559`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L559) — execute_query_strategy returns None when query_key is None.
  - `test_execute_query_strategy_unknown_key(self)` — [`L565`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L565) — execute_query_strategy returns None for unknown query key.
- uses (calls/refs, reference-scoped): [`CssPlugin`](../../../tree_sitter_analyzer/languages/css_plugin.md#CssPlugin), [`execute_query_strategy`](../../../tree_sitter_analyzer/languages/css_plugin.md#CssPlugin.execute_query_strategy)

### `TestScssVariableExtraction`
- def: [`tests/unit/languages/test_css_plugin.py:668`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L668)
- doc: Tests for SCSS `$variable` extraction (Bug #807).
- signature: `class TestScssVariableExtraction:`
- members:
  - `test_extract_scss_variables_deduplicates_on_first_occurrence(self)` — [`L809`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L809) — Reassignment of ``$var`` in nested scope → only first occurrence kept.
  - `test_extract_scss_variables_literal_slash_star_in_string(self)` — [`L841`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L841) — Bug #967: a literal ``/*`` inside a quoted value must NOT open a comment.
  - `test_extract_scss_variables_single_quoted_slash_star(self)` — [`L855`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L855) — A single-quoted ``'a/*b'`` literal also must not open a block comment.
  - `test_extract_scss_variables_skips_block_comments(self)` — [`L819`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L819) — Bug #790: ``$var`` inside a ``/* ... */`` block comment is skipped.
  - `test_extract_scss_variables_skips_inline_block_comment(self)` — [`L832`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L832) — A single-line ``/* $old: red; */`` block comment yields no Variable.
  - `test_extract_scss_variables_unit(self)` — [`L792`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L792) — Unit test for ``_extract_scss_variables`` helper directly.
  - `test_plain_css_file_unaffected_by_scss_extraction(self)` — [`L767`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L767) — Plain ``.css`` file: no Variable elements, only CSS rules.
  - `test_scss_no_variables_returns_css_rules_only(self)` — [`L741`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L741) — SCSS file with no ``$var`` declarations → 0 Variable elements.
  - `test_scss_variables_extracted_from_file(self)` — [`L678`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L678) — 3 SCSS ``$variable`` declarations → 3 Variable elements.
  - `test_scss_variables_have_correct_line_numbers(self)` — [`L712`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_css_plugin.py#L712) — Each Variable element's start_line matches its source line.
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`start_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`Variable`](../../../tree_sitter_analyzer/models/base.md#Variable), [`CssPlugin`](../../../tree_sitter_analyzer/languages/css_plugin.md#CssPlugin), [`_extract_scss_variables`](../../../tree_sitter_analyzer/languages/css_plugin.md#_extract_scss_variables)

