---
title: 'Module: tests/unit/languages/test_scala_plugin.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_scala_plugin.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_scala_plugin`/
symbols:
  _node: _node().
  TestScalaElementExtractorInit.test_initial_state: TestScalaElementExtractorInit#test_initial_state().
  _tree: _tree().
  TestScalaPlugin.test_scala_analysis_result_builds_result: TestScalaPlugin#test_scala_analysis_result_builds_result().
  TestScalaPlugin.test_analyze_file_returns_empty_when_no_language: TestScalaPlugin#test_analyze_file_returns_empty_when_no_language().
  TestScalaPlugin.test_analyze_file_returns_error_on_read_failure: TestScalaPlugin#test_analyze_file_returns_error_on_read_failure().
  TestScalaElementExtractorInit.test_reset_caches_clears_cache: TestScalaElementExtractorInit#test_reset_caches_clears_cache().
  TestScalaElementExtractorInit.test_reset_caches_clears_package_when_no_source: TestScalaElementExtractorInit#test_reset_caches_clears_package_when_no_source().
  TestScalaElementExtractorInit.test_reset_caches_preserves_package_when_has_source: TestScalaElementExtractorInit#test_reset_caches_preserves_package_when_has_source().
  TestGetNodeText.test_returns_cached_value: TestGetNodeText#test_returns_cached_value().
  TestGetNodeText.test_extracts_text_from_source: TestGetNodeText#test_extracts_text_from_source().
  TestScalaFunctionName.test_uses_name_field_when_present: TestScalaFunctionName#test_uses_name_field_when_present().
  TestScalaFunctionName.test_falls_back_to_identifier_child: TestScalaFunctionName#test_falls_back_to_identifier_child().
  TestScalaFunctionName.test_returns_anonymous_when_no_name: TestScalaFunctionName#test_returns_anonymous_when_no_name().
  TestScalaClassLikeName.test_uses_name_field_when_present: TestScalaClassLikeName#test_uses_name_field_when_present().
  TestScalaClassLikeName.test_falls_back_to_type_identifier_child: TestScalaClassLikeName#test_falls_back_to_type_identifier_child().
  TestScalaClassLikeName.test_returns_anonymous_when_no_name: TestScalaClassLikeName#test_returns_anonymous_when_no_name().
  TestScalaTypeAfterColon.test_returns_type_after_colon: TestScalaTypeAfterColon#test_returns_type_after_colon().
  TestScalaTypeAfterColon.test_returns_default_when_no_colon: TestScalaTypeAfterColon#test_returns_default_when_no_colon().
  TestScalaTypeAfterColon.test_returns_default_when_colon_is_last_child: TestScalaTypeAfterColon#test_returns_default_when_colon_is_last_child().
  TestScalaVisibility.test_private_visibility: TestScalaVisibility#test_private_visibility().
  TestScalaVisibility.test_protected_visibility: TestScalaVisibility#test_protected_visibility().
  TestScalaVisibility.test_public_by_default: TestScalaVisibility#test_public_by_default().
  TestScalaVisibility.test_public_when_modifiers_has_no_keyword: TestScalaVisibility#test_public_when_modifiers_has_no_keyword().
  TestExtractParameters.test_empty_param_node: TestExtractParameters#test_empty_param_node().
  TestExtractParameters.test_parameter_with_name_and_type: TestExtractParameters#test_parameter_with_name_and_type().
  TestExtractFunctionsWithEmptyTree.test_returns_empty_when_non_function_nodes: TestExtractFunctionsWithEmptyTree#test_returns_empty_when_non_function_nodes().
  TestScalaPackageNameFromClause.test_finds_package_identifier: TestScalaPackageNameFromClause#test_finds_package_identifier().
  TestScalaPackageNameFromClause.test_finds_plain_identifier: TestScalaPackageNameFromClause#test_finds_plain_identifier().
  TestScalaPackageNameFromClause.test_returns_none_when_no_identifier: TestScalaPackageNameFromClause#test_returns_none_when_no_identifier().
  TestScalaPlugin.test_get_tree_sitter_language_cached: TestScalaPlugin#test_get_tree_sitter_language_cached().
  TestScalaPlugin.test_extract_elements_exception_returns_empty: TestScalaPlugin#test_extract_elements_exception_returns_empty().
  TestScalaPlugin.test_extract_elements_with_mock_extractor: TestScalaPlugin#test_extract_elements_with_mock_extractor().
  TestScalaPlugin.test_scala_analysis_result_with_package: TestScalaPlugin#test_scala_analysis_result_with_package().
  TestGetNodeText.test_returns_empty_on_exception: TestGetNodeText#test_returns_empty_on_exception().
  TestTraverseAndExtract.test_empty_tree_produces_no_results: TestTraverseAndExtract#test_empty_tree_produces_no_results().
  TestTraverseAndExtract.test_matching_node_calls_extractor: TestTraverseAndExtract#test_matching_node_calls_extractor().
  TestTraverseAndExtract.test_extractor_returning_none_not_appended: TestTraverseAndExtract#test_extractor_returning_none_not_appended().
  TestTraverseAndExtract.test_nested_nodes_traversed: TestTraverseAndExtract#test_nested_nodes_traversed().
  TestExtractFunctionsWithEmptyTree.test_returns_empty_when_no_function_nodes: TestExtractFunctionsWithEmptyTree#test_returns_empty_when_no_function_nodes().
  TestExtractClassesWithEmptyTree.test_returns_empty_for_empty_tree: TestExtractClassesWithEmptyTree#test_returns_empty_for_empty_tree().
  TestExtractVariablesWithEmptyTree.test_returns_empty_for_empty_tree: TestExtractVariablesWithEmptyTree#test_returns_empty_for_empty_tree().
  TestExtractImportsWithEmptyTree.test_returns_empty_for_empty_tree: TestExtractImportsWithEmptyTree#test_returns_empty_for_empty_tree().
  TestExtractPackagesWithEmptyTree.test_returns_empty_for_empty_tree: TestExtractPackagesWithEmptyTree#test_returns_empty_for_empty_tree().
  TestExtractCommentsAnnotations.test_comments_empty_tree: TestExtractCommentsAnnotations#test_comments_empty_tree().
  TestExtractCommentsAnnotations.test_annotations_empty_tree: TestExtractCommentsAnnotations#test_annotations_empty_tree().
  TestLastNearbyBlockComment.test_returns_none_when_no_parent: TestLastNearbyBlockComment#test_returns_none_when_no_parent().
  TestLastNearbyBlockComment.test_returns_none_when_no_block_comment: TestLastNearbyBlockComment#test_returns_none_when_no_block_comment().
  TestLastNearbyBlockComment.test_returns_close_block_comment: TestLastNearbyBlockComment#test_returns_close_block_comment().
  TestScalaEmptyResult.test_line_count_uses_splitlines: TestScalaEmptyResult#test_line_count_uses_splitlines().
  TestScalaEmptyResult.test_language_is_scala: TestScalaEmptyResult#test_language_is_scala().
  TestScalaEmptyResult.test_elements_empty: TestScalaEmptyResult#test_elements_empty().
  TestScalaEmptyResult.test_file_path_preserved: TestScalaEmptyResult#test_file_path_preserved().
  TestScalaErrorResult.test_success_false: TestScalaErrorResult#test_success_false().
  TestScalaErrorResult.test_error_message_captured: TestScalaErrorResult#test_error_message_captured().
  TestScalaErrorResult.test_line_count_zero: TestScalaErrorResult#test_line_count_zero().
  TestScalaPlugin.test_count_tree_nodes_none: TestScalaPlugin#test_count_tree_nodes_none().
  TestScalaPlugin.test_count_tree_nodes_single: TestScalaPlugin#test_count_tree_nodes_single().
  TestScalaPlugin.test_count_tree_nodes_nested: TestScalaPlugin#test_count_tree_nodes_nested().
  TestScalaPlugin.test_get_tree_sitter_language_import_error: TestScalaPlugin#test_get_tree_sitter_language_import_error().
  TestScalaPlugin.test_extract_elements_none_tree: TestScalaPlugin#test_extract_elements_none_tree().
  TestParseScaladocText.test_valid_scaladoc_single_line: TestParseScaladocText#test_valid_scaladoc_single_line().
  TestParseScaladocText.test_valid_scaladoc_multiline: TestParseScaladocText#test_valid_scaladoc_multiline().
  TestParseScaladocText.test_not_scaladoc_returns_none_for_regular_comment: TestParseScaladocText#test_not_scaladoc_returns_none_for_regular_comment().
  TestParseScaladocText.test_triple_star_returns_none: TestParseScaladocText#test_triple_star_returns_none().
  TestParseScaladocText.test_empty_content_returns_none: TestParseScaladocText#test_empty_content_returns_none().
  TestParseScaladocText.test_strips_leading_asterisk_per_line: TestParseScaladocText#test_strips_leading_asterisk_per_line().
  TestParseScaladocText.test_returns_none_for_empty_string: TestParseScaladocText#test_returns_none_for_empty_string().
  TestFlattenScalaElements.test_returns_all_elements_in_canonical_order: TestFlattenScalaElements#test_returns_all_elements_in_canonical_order().
  TestFlattenScalaElements.test_missing_keys_silently_skipped: TestFlattenScalaElements#test_missing_keys_silently_skipped().
  TestFlattenScalaElements.test_empty_dict_returns_empty: TestFlattenScalaElements#test_empty_dict_returns_empty().
  TestMakeScalaParser.test_uses_set_language_when_available: TestMakeScalaParser#test_uses_set_language_when_available().
  TestMakeScalaParser.test_uses_language_property_when_no_set_language: TestMakeScalaParser#test_uses_language_property_when_no_set_language().
  TestMakeScalaParser.test_falls_back_to_constructor_when_neither_attr: TestMakeScalaParser#test_falls_back_to_constructor_when_neither_attr().
  TestScalaPlugin.plugin: TestScalaPlugin#plugin().
  TestParseScaladocText: TestParseScaladocText#
  TestFlattenScalaElements: TestFlattenScalaElements#
  TestScalaEmptyResult: TestScalaEmptyResult#
  TestScalaErrorResult: TestScalaErrorResult#
  TestMakeScalaParser: TestMakeScalaParser#
  TestScalaPlugin: TestScalaPlugin#
  TestScalaElementExtractorInit: TestScalaElementExtractorInit#
  TestGetNodeText: TestGetNodeText#
  TestTraverseAndExtract: TestTraverseAndExtract#
  TestScalaFunctionName: TestScalaFunctionName#
  TestScalaClassLikeName: TestScalaClassLikeName#
  TestScalaTypeAfterColon: TestScalaTypeAfterColon#
  TestScalaVisibility: TestScalaVisibility#
  TestExtractParameters: TestExtractParameters#
  TestExtractFunctionsWithEmptyTree: TestExtractFunctionsWithEmptyTree#
  TestExtractClassesWithEmptyTree: TestExtractClassesWithEmptyTree#
  TestExtractVariablesWithEmptyTree: TestExtractVariablesWithEmptyTree#
  TestExtractImportsWithEmptyTree: TestExtractImportsWithEmptyTree#
  TestExtractPackagesWithEmptyTree: TestExtractPackagesWithEmptyTree#
  TestExtractCommentsAnnotations: TestExtractCommentsAnnotations#
  TestScalaPackageNameFromClause: TestScalaPackageNameFromClause#
  TestLastNearbyBlockComment: TestLastNearbyBlockComment#
---
# Module: [`tests/unit/languages/test_scala_plugin.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py)

## Classes
### `TestExtractClassesWithEmptyTree`
- def: [`tests/unit/languages/test_scala_plugin.py:582`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L582)
- signature: `class TestExtractClassesWithEmptyTree:`
- members:
  - `test_returns_empty_for_empty_tree(self)` — [`L583`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L583)
- uses (calls/refs, reference-scoped): [`ScalaElementExtractor`](../../../tree_sitter_analyzer/languages/scala_plugin.md#ScalaElementExtractor), [`extract_classes`](../../../tree_sitter_analyzer/languages/scala_plugin.md#ScalaElementExtractor.extract_classes)  (1 test-only)

### `TestExtractCommentsAnnotations`
- def: [`tests/unit/languages/test_scala_plugin.py:610`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L610)
- signature: `class TestExtractCommentsAnnotations:`
- members:
  - `test_annotations_empty_tree(self)` — [`L616`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L616)
  - `test_comments_empty_tree(self)` — [`L611`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L611)
- uses (calls/refs, reference-scoped): [`ScalaElementExtractor`](../../../tree_sitter_analyzer/languages/scala_plugin.md#ScalaElementExtractor), [`extract_annotations`](../../../tree_sitter_analyzer/languages/scala_plugin.md#ScalaElementExtractor.extract_annotations), [`extract_comments`](../../../tree_sitter_analyzer/languages/scala_plugin.md#ScalaElementExtractor.extract_comments)  (1 test-only)

### `TestExtractFunctionsWithEmptyTree`
- def: [`tests/unit/languages/test_scala_plugin.py:568`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L568)
- signature: `class TestExtractFunctionsWithEmptyTree:`
- members:
  - `test_returns_empty_when_no_function_nodes(self)` — [`L569`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L569)
  - `test_returns_empty_when_non_function_nodes(self)` — [`L575`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L575)
- uses (calls/refs, reference-scoped): [`ScalaElementExtractor`](../../../tree_sitter_analyzer/languages/scala_plugin.md#ScalaElementExtractor), [`extract_functions`](../../../tree_sitter_analyzer/languages/scala_plugin.md#ScalaElementExtractor.extract_functions)  (2 test-only)

### `TestExtractImportsWithEmptyTree`
- def: [`tests/unit/languages/test_scala_plugin.py:596`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L596)
- signature: `class TestExtractImportsWithEmptyTree:`
- members:
  - `test_returns_empty_for_empty_tree(self)` — [`L597`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L597)
- uses (calls/refs, reference-scoped): [`ScalaElementExtractor`](../../../tree_sitter_analyzer/languages/scala_plugin.md#ScalaElementExtractor), [`extract_imports`](../../../tree_sitter_analyzer/languages/scala_plugin.md#ScalaElementExtractor.extract_imports)  (1 test-only)

### `TestExtractPackagesWithEmptyTree`
- def: [`tests/unit/languages/test_scala_plugin.py:603`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L603)
- signature: `class TestExtractPackagesWithEmptyTree:`
- members:
  - `test_returns_empty_for_empty_tree(self)` — [`L604`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L604)
- uses (calls/refs, reference-scoped): [`ScalaElementExtractor`](../../../tree_sitter_analyzer/languages/scala_plugin.md#ScalaElementExtractor), [`extract_packages`](../../../tree_sitter_analyzer/languages/scala_plugin.md#ScalaElementExtractor.extract_packages)  (1 test-only)

### `TestExtractParameters`
- def: [`tests/unit/languages/test_scala_plugin.py:548`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L548)
- signature: `class TestExtractParameters:`
- members:
  - `test_empty_param_node(self)` — [`L549`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L549)
  - `test_parameter_with_name_and_type(self)` — [`L555`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L555)
- uses (calls/refs, reference-scoped): [`ScalaElementExtractor`](../../../tree_sitter_analyzer/languages/scala_plugin.md#ScalaElementExtractor), [`content_lines`](../../../tree_sitter_analyzer/languages/scala_plugin.md#ScalaElementExtractor.content_lines), [`_extract_parameters`](../../../tree_sitter_analyzer/languages/scala_plugin.md#ScalaElementExtractor._extract_parameters)  (1 test-only)

### `TestExtractVariablesWithEmptyTree`
- def: [`tests/unit/languages/test_scala_plugin.py:589`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L589)
- signature: `class TestExtractVariablesWithEmptyTree:`
- members:
  - `test_returns_empty_for_empty_tree(self)` — [`L590`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L590)
- uses (calls/refs, reference-scoped): [`ScalaElementExtractor`](../../../tree_sitter_analyzer/languages/scala_plugin.md#ScalaElementExtractor), [`extract_variables`](../../../tree_sitter_analyzer/languages/scala_plugin.md#ScalaElementExtractor.extract_variables)  (1 test-only)

### `TestFlattenScalaElements`
- def: [`tests/unit/languages/test_scala_plugin.py:103`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L103)
- signature: `class TestFlattenScalaElements:`
- members:
  - `test_empty_dict_returns_empty(self)` — [`L127`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L127)
  - `test_missing_keys_silently_skipped(self)` — [`L123`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L123)
  - `test_returns_all_elements_in_canonical_order(self)` — [`L104`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L104)
- uses (calls/refs, reference-scoped): [`_flatten_scala_elements`](../../../tree_sitter_analyzer/languages/scala_plugin.md#_flatten_scala_elements)

### `TestGetNodeText`
- def: [`tests/unit/languages/test_scala_plugin.py:373`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L373)
- signature: `class TestGetNodeText:`
- members:
  - `test_extracts_text_from_source(self)` — [`L380`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L380)
  - `test_returns_cached_value(self)` — [`L374`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L374)
  - `test_returns_empty_on_exception(self)` — [`L387`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L387)
- uses (calls/refs, reference-scoped): [`ScalaElementExtractor`](../../../tree_sitter_analyzer/languages/scala_plugin.md#ScalaElementExtractor), [`_get_node_text`](../../../tree_sitter_analyzer/languages/scala_plugin.md#ScalaElementExtractor._get_node_text), [`content_lines`](../../../tree_sitter_analyzer/languages/scala_plugin.md#ScalaElementExtractor.content_lines), [`_node_text_cache`](../../../tree_sitter_analyzer/languages/scala_plugin.md#ScalaElementExtractor._node_text_cache)  (1 test-only)

### `TestLastNearbyBlockComment`
- def: [`tests/unit/languages/test_scala_plugin.py:646`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L646)
- signature: `class TestLastNearbyBlockComment:`
- members:
  - `test_returns_close_block_comment(self)` — [`L659`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L659)
  - `test_returns_none_when_no_block_comment(self)` — [`L652`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L652)
  - `test_returns_none_when_no_parent(self)` — [`L647`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L647)
- uses (calls/refs, reference-scoped): [`ScalaElementExtractor`](../../../tree_sitter_analyzer/languages/scala_plugin.md#ScalaElementExtractor), [`_last_nearby_block_comment`](../../../tree_sitter_analyzer/languages/scala_plugin.md#ScalaElementExtractor._last_nearby_block_comment)  (1 test-only)

### `TestMakeScalaParser`
- def: [`tests/unit/languages/test_scala_plugin.py:173`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L173)
- signature: `class TestMakeScalaParser:`
- members:
  - `test_falls_back_to_constructor_when_neither_attr(self)` — [`L193`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L193)
  - `test_uses_language_property_when_no_set_language(self)` — [`L183`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L183)
  - `test_uses_set_language_when_available(self)` — [`L174`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L174)
- uses (calls/refs, reference-scoped): [`_make_scala_parser`](../../../tree_sitter_analyzer/languages/scala_plugin.md#_make_scala_parser)

### `TestParseScaladocText`
- def: [`tests/unit/languages/test_scala_plugin.py:66`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L66)
- signature: `class TestParseScaladocText:`
- members:
  - `test_empty_content_returns_none(self)` — [`L84`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L84)
  - `test_not_scaladoc_returns_none_for_regular_comment(self)` — [`L78`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L78)
  - `test_returns_none_for_empty_string(self)` — [`L94`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L94)
  - `test_strips_leading_asterisk_per_line(self)` — [`L88`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L88)
  - `test_triple_star_returns_none(self)` — [`L81`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L81)
  - `test_valid_scaladoc_multiline(self)` — [`L72`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L72)
  - `test_valid_scaladoc_single_line(self)` — [`L67`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L67)
- uses (calls/refs, reference-scoped): [`_parse_scaladoc_text`](../../../tree_sitter_analyzer/languages/scala_plugin.md#_parse_scaladoc_text)

### `TestScalaClassLikeName`
- def: [`tests/unit/languages/test_scala_plugin.py:468`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L468)
- signature: `class TestScalaClassLikeName:`
- members:
  - `test_falls_back_to_type_identifier_child(self)` — [`L478`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L478)
  - `test_returns_anonymous_when_no_name(self)` — [`L486`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L486)
  - `test_uses_name_field_when_present(self)` — [`L469`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L469)
- uses (calls/refs, reference-scoped): [`ScalaElementExtractor`](../../../tree_sitter_analyzer/languages/scala_plugin.md#ScalaElementExtractor), [`content_lines`](../../../tree_sitter_analyzer/languages/scala_plugin.md#ScalaElementExtractor.content_lines), [`_scala_class_like_name`](../../../tree_sitter_analyzer/languages/scala_plugin.md#ScalaElementExtractor._scala_class_like_name)  (1 test-only)

### `TestScalaElementExtractorInit`
- def: [`tests/unit/languages/test_scala_plugin.py:342`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L342)
- signature: `class TestScalaElementExtractorInit:`
- members:
  - `test_initial_state(self)` — [`L343`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L343)
  - `test_reset_caches_clears_cache(self)` — [`L351`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L351)
  - `test_reset_caches_clears_package_when_no_source(self)` — [`L358`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L358)
  - `test_reset_caches_preserves_package_when_has_source(self)` — [`L365`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L365)
- uses (calls/refs, reference-scoped): [`ScalaElementExtractor`](../../../tree_sitter_analyzer/languages/scala_plugin.md#ScalaElementExtractor), [`content_lines`](../../../tree_sitter_analyzer/languages/scala_plugin.md#ScalaElementExtractor.content_lines), [`_reset_caches`](../../../tree_sitter_analyzer/languages/scala_plugin.md#ScalaElementExtractor._reset_caches), [`current_package`](../../../tree_sitter_analyzer/languages/scala_plugin.md#ScalaElementExtractor.current_package), [`source_code`](../../../tree_sitter_analyzer/languages/scala_plugin.md#ScalaElementExtractor.source_code), [`_node_text_cache`](../../../tree_sitter_analyzer/languages/scala_plugin.md#ScalaElementExtractor._node_text_cache), [`current_file`](../../../tree_sitter_analyzer/languages/scala_plugin.md#ScalaElementExtractor.current_file)

### `TestScalaEmptyResult`
- def: [`tests/unit/languages/test_scala_plugin.py:136`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L136)
- signature: `class TestScalaEmptyResult:`
- members:
  - `test_elements_empty(self)` — [`L145`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L145)
  - `test_file_path_preserved(self)` — [`L149`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L149)
  - `test_language_is_scala(self)` — [`L141`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L141)
  - `test_line_count_uses_splitlines(self)` — [`L137`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L137)
- uses (calls/refs, reference-scoped): [`elements`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.elements), [`language`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.language), [`file_path`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.file_path), [`line_count`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.line_count), [`_scala_empty_result`](../../../tree_sitter_analyzer/languages/scala_plugin.md#_scala_empty_result)

### `TestScalaErrorResult`
- def: [`tests/unit/languages/test_scala_plugin.py:154`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L154)
- signature: `class TestScalaErrorResult:`
- members:
  - `test_error_message_captured(self)` — [`L159`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L159)
  - `test_line_count_zero(self)` — [`L163`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L163)
  - `test_success_false(self)` — [`L155`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L155)
- uses (calls/refs, reference-scoped): [`success`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.success), [`line_count`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.line_count), [`error_message`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.error_message), [`_scala_error_result`](../../../tree_sitter_analyzer/languages/scala_plugin.md#_scala_error_result)

### `TestScalaFunctionName`
- def: [`tests/unit/languages/test_scala_plugin.py:440`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L440)
- signature: `class TestScalaFunctionName:`
- members:
  - `test_falls_back_to_identifier_child(self)` — [`L450`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L450)
  - `test_returns_anonymous_when_no_name(self)` — [`L459`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L459)
  - `test_uses_name_field_when_present(self)` — [`L441`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L441)
- uses (calls/refs, reference-scoped): [`ScalaElementExtractor`](../../../tree_sitter_analyzer/languages/scala_plugin.md#ScalaElementExtractor), [`content_lines`](../../../tree_sitter_analyzer/languages/scala_plugin.md#ScalaElementExtractor.content_lines), [`_scala_function_name`](../../../tree_sitter_analyzer/languages/scala_plugin.md#ScalaElementExtractor._scala_function_name)  (1 test-only)

### `TestScalaPackageNameFromClause`
- def: [`tests/unit/languages/test_scala_plugin.py:622`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L622)
- signature: `class TestScalaPackageNameFromClause:`
- members:
  - `test_finds_package_identifier(self)` — [`L623`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L623)
  - `test_finds_plain_identifier(self)` — [`L631`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L631)
  - `test_returns_none_when_no_identifier(self)` — [`L639`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L639)
- uses (calls/refs, reference-scoped): [`ScalaElementExtractor`](../../../tree_sitter_analyzer/languages/scala_plugin.md#ScalaElementExtractor), [`content_lines`](../../../tree_sitter_analyzer/languages/scala_plugin.md#ScalaElementExtractor.content_lines), [`_scala_package_name_from_clause`](../../../tree_sitter_analyzer/languages/scala_plugin.md#ScalaElementExtractor._scala_package_name_from_clause)  (1 test-only)

### `TestScalaPlugin`
- def: [`tests/unit/languages/test_scala_plugin.py:211`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L211)
- signature: `class TestScalaPlugin:`
- members:
  - `plugin(self)` — [`L213`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L213)
  - `test_analyze_file_returns_empty_when_no_language(self, plugin: ScalaPlugin, tmp_path: Any)` — [`L314`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L314)
  - `test_analyze_file_returns_error_on_read_failure(self, plugin: ScalaPlugin)` — [`L325`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L325)
  - `test_count_tree_nodes_nested(self, plugin: ScalaPlugin)` — [`L224`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L224)
  - `test_count_tree_nodes_none(self, plugin: ScalaPlugin)` — [`L216`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L216)
  - `test_count_tree_nodes_single(self, plugin: ScalaPlugin)` — [`L219`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L219)
  - `test_extract_elements_exception_returns_empty(self, plugin: ScalaPlugin)` — [`L249`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L249)
  - `test_extract_elements_none_tree(self, plugin: ScalaPlugin)` — [`L243`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L243)
  - `test_extract_elements_with_mock_extractor(self, plugin: ScalaPlugin)` — [`L258`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L258)
  - `test_get_tree_sitter_language_cached(self, plugin: ScalaPlugin)` — [`L238`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L238)
  - `test_get_tree_sitter_language_import_error(self, plugin: ScalaPlugin)` — [`L233`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L233)
  - `test_scala_analysis_result_builds_result(self, plugin: ScalaPlugin)` — [`L271`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L271)
  - `test_scala_analysis_result_with_package(self, plugin: ScalaPlugin)` — [`L295`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L295)
- uses (calls/refs, reference-scoped): [`elements`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.elements), [`language`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.language), [`file_path`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.file_path), [`success`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.success), [`line_count`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.line_count), [`error_message`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.error_message), [`_scala_analysis_result`](../../../tree_sitter_analyzer/languages/scala_plugin.md#ScalaPlugin._scala_analysis_result), [`ScalaPlugin`](../../../tree_sitter_analyzer/languages/scala_plugin.md#ScalaPlugin), [`analyze_file`](../../../tree_sitter_analyzer/languages/scala_plugin.md#ScalaPlugin.analyze_file), [`extract_elements`](../../../tree_sitter_analyzer/languages/scala_plugin.md#ScalaPlugin.extract_elements), [`package`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.package), [`get_tree_sitter_language`](../../../tree_sitter_analyzer/languages/scala_plugin.md#ScalaPlugin.get_tree_sitter_language), [`_count_tree_nodes`](../../../tree_sitter_analyzer/languages/scala_plugin.md#ScalaPlugin._count_tree_nodes), [`_cached_language`](../../../tree_sitter_analyzer/languages/scala_plugin.md#ScalaPlugin._cached_language)  (1 test-only)

### `TestScalaTypeAfterColon`
- def: [`tests/unit/languages/test_scala_plugin.py:494`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L494)
- signature: `class TestScalaTypeAfterColon:`
- members:
  - `test_returns_default_when_colon_is_last_child(self)` — [`L511`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L511)
  - `test_returns_default_when_no_colon(self)` — [`L505`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L505)
  - `test_returns_type_after_colon(self)` — [`L495`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L495)
- uses (calls/refs, reference-scoped): [`ScalaElementExtractor`](../../../tree_sitter_analyzer/languages/scala_plugin.md#ScalaElementExtractor), [`content_lines`](../../../tree_sitter_analyzer/languages/scala_plugin.md#ScalaElementExtractor.content_lines), [`_scala_type_after_colon`](../../../tree_sitter_analyzer/languages/scala_plugin.md#ScalaElementExtractor._scala_type_after_colon)  (1 test-only)

### `TestScalaVisibility`
- def: [`tests/unit/languages/test_scala_plugin.py:519`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L519)
- signature: `class TestScalaVisibility:`
- members:
  - `test_private_visibility(self)` — [`L520`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L520)
  - `test_protected_visibility(self)` — [`L527`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L527)
  - `test_public_by_default(self)` — [`L534`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L534)
  - `test_public_when_modifiers_has_no_keyword(self)` — [`L540`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L540)
- uses (calls/refs, reference-scoped): [`ScalaElementExtractor`](../../../tree_sitter_analyzer/languages/scala_plugin.md#ScalaElementExtractor), [`content_lines`](../../../tree_sitter_analyzer/languages/scala_plugin.md#ScalaElementExtractor.content_lines), [`_scala_visibility`](../../../tree_sitter_analyzer/languages/scala_plugin.md#ScalaElementExtractor._scala_visibility)  (1 test-only)

### `TestTraverseAndExtract`
- def: [`tests/unit/languages/test_scala_plugin.py:404`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L404)
- signature: `class TestTraverseAndExtract:`
- members:
  - `test_empty_tree_produces_no_results(self)` — [`L405`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L405)
  - `test_extractor_returning_none_not_appended(self)` — [`L422`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L422)
  - `test_matching_node_calls_extractor(self)` — [`L412`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L412)
  - `test_nested_nodes_traversed(self)` — [`L430`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L430)
- uses (calls/refs, reference-scoped): [`ScalaElementExtractor`](../../../tree_sitter_analyzer/languages/scala_plugin.md#ScalaElementExtractor), [`_traverse_and_extract`](../../../tree_sitter_analyzer/languages/scala_plugin.md#ScalaElementExtractor._traverse_and_extract)  (1 test-only)

## Functions
- `_node(type_: str = "identifier", text: str = "x", children: list | None = None, start_point: tuple = (0, 0), end_point: tuple = (0, 1), start_byte: int = 0, end_byte: int = 1, parent: Any = None)` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L29) — Build a minimal mock tree-sitter node.
- `_tree(root_children: list | None = None)` — [`L53`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_scala_plugin.py#L53) — Build a minimal mock tree-sitter tree.

