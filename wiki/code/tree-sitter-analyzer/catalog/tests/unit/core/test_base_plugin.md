---
title: 'Module: tests/unit/core/test_base_plugin.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_base_plugin.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_base_plugin`/Test
symbols:
  TestDefaultLanguagePluginAnalyze.test_analyze_file_handles_error: DefaultLanguagePluginAnalyze#test_analyze_file_handles_error().
  TestDefaultLanguagePlugin.test_create_extractor: DefaultLanguagePlugin#test_create_extractor().
  TestDefaultExtractorInit.test_init_sets_current_file: DefaultExtractorInit#test_init_sets_current_file().
  TestDefaultExtractorNodeTypeChecks.test_is_function_node_true_cases: DefaultExtractorNodeTypeChecks#test_is_function_node_true_cases().
  TestDefaultExtractorNodeTypeChecks.test_is_function_node_false_cases: DefaultExtractorNodeTypeChecks#test_is_function_node_false_cases().
  TestDefaultExtractorNodeTypeChecks.test_is_class_node_true_cases: DefaultExtractorNodeTypeChecks#test_is_class_node_true_cases().
  TestDefaultExtractorNodeTypeChecks.test_is_class_node_false_cases: DefaultExtractorNodeTypeChecks#test_is_class_node_false_cases().
  TestDefaultExtractorNodeTypeChecks.test_is_variable_node_true_cases: DefaultExtractorNodeTypeChecks#test_is_variable_node_true_cases().
  TestDefaultExtractorNodeTypeChecks.test_is_variable_node_false_cases: DefaultExtractorNodeTypeChecks#test_is_variable_node_false_cases().
  TestDefaultExtractorNodeTypeChecks.test_is_import_node_true_cases: DefaultExtractorNodeTypeChecks#test_is_import_node_true_cases().
  TestDefaultExtractorNodeTypeChecks.test_is_import_node_false_cases: DefaultExtractorNodeTypeChecks#test_is_import_node_false_cases().
  TestDefaultExtractorNodeText.test_extract_node_text_with_bytes: DefaultExtractorNodeText#test_extract_node_text_with_bytes().
  TestDefaultExtractorNodeText.test_extract_node_text_without_attributes: DefaultExtractorNodeText#test_extract_node_text_without_attributes().
  TestDefaultExtractorNodeText.test_extract_node_text_with_unicode: DefaultExtractorNodeText#test_extract_node_text_with_unicode().
  TestDefaultExtractorNodeName.test_extract_node_name_with_identifier_child: DefaultExtractorNodeName#test_extract_node_name_with_identifier_child().
  TestDefaultExtractorNodeName.test_extract_node_name_fallback: DefaultExtractorNodeName#test_extract_node_name_fallback().
  TestDefaultExtractorExtraction.test_extract_functions_empty_tree: DefaultExtractorExtraction#test_extract_functions_empty_tree().
  TestDefaultExtractorExtraction.test_extract_functions_with_tree: DefaultExtractorExtraction#test_extract_functions_with_tree().
  TestDefaultExtractorExtraction.test_extract_classes_empty_tree: DefaultExtractorExtraction#test_extract_classes_empty_tree().
  TestDefaultExtractorExtraction.test_extract_variables_empty_tree: DefaultExtractorExtraction#test_extract_variables_empty_tree().
  TestDefaultExtractorExtraction.test_extract_imports_empty_tree: DefaultExtractorExtraction#test_extract_imports_empty_tree().
  TestDefaultExtractorDefaultMethods.test_extract_packages_returns_empty: DefaultExtractorDefaultMethods#test_extract_packages_returns_empty().
  TestDefaultExtractorDefaultMethods.test_extract_annotations_returns_empty: DefaultExtractorDefaultMethods#test_extract_annotations_returns_empty().
  TestDefaultExtractorDefaultMethods.test_extract_html_elements_returns_empty: DefaultExtractorDefaultMethods#test_extract_html_elements_returns_empty().
  TestDefaultExtractorDefaultMethods.test_extract_css_rules_returns_empty: DefaultExtractorDefaultMethods#test_extract_css_rules_returns_empty().
  TestDefaultExtractorDefaultMethods.test_get_language_hint_returns_unknown: DefaultExtractorDefaultMethods#test_get_language_hint_returns_unknown().
  TestDefaultExtractorAllElements.test_extract_all_elements_aggregates_all: DefaultExtractorAllElements#test_extract_all_elements_aggregates_all().
  TestDefaultLanguagePlugin.test_get_language_name: DefaultLanguagePlugin#test_get_language_name().
  TestDefaultLanguagePlugin.test_get_file_extensions: DefaultLanguagePlugin#test_get_file_extensions().
  TestDefaultLanguagePlugin.test_get_supported_element_types: DefaultLanguagePlugin#test_get_supported_element_types().
  TestDefaultLanguagePlugin.test_get_queries_returns_empty: DefaultLanguagePlugin#test_get_queries_returns_empty().
  TestDefaultLanguagePlugin.test_get_formatter_map_returns_empty: DefaultLanguagePlugin#test_get_formatter_map_returns_empty().
  TestDefaultLanguagePlugin.test_get_element_categories_returns_empty: DefaultLanguagePlugin#test_get_element_categories_returns_empty().
  TestDefaultLanguagePlugin.test_is_applicable_for_txt: DefaultLanguagePlugin#test_is_applicable_for_txt().
  TestDefaultLanguagePlugin.test_is_applicable_for_md: DefaultLanguagePlugin#test_is_applicable_for_md().
  TestDefaultLanguagePlugin.test_is_applicable_false_for_other: DefaultLanguagePlugin#test_is_applicable_false_for_other().
  TestDefaultLanguagePlugin.test_is_applicable_case_insensitive: DefaultLanguagePlugin#test_is_applicable_case_insensitive().
  TestDefaultLanguagePlugin.test_get_plugin_info: DefaultLanguagePlugin#test_get_plugin_info().
  TestDefaultLanguagePlugin.test_execute_query_strategy_none_key: DefaultLanguagePlugin#test_execute_query_strategy_none_key().
  TestDefaultLanguagePlugin.test_execute_query_strategy_unknown_key: DefaultLanguagePlugin#test_execute_query_strategy_unknown_key().
  TestDefaultLanguagePluginAnalyze.test_analyze_file_returns_result: DefaultLanguagePluginAnalyze#test_analyze_file_returns_result().
  TestElementExtractorAbstract.test_cannot_instantiate_directly: ElementExtractorAbstract#test_cannot_instantiate_directly().
  TestElementExtractorAbstract.test_has_required_abstract_methods: ElementExtractorAbstract#test_has_required_abstract_methods().
  TestLanguagePluginAbstract.test_cannot_instantiate_directly: LanguagePluginAbstract#test_cannot_instantiate_directly().
  TestLanguagePluginAbstract.test_has_required_abstract_methods: LanguagePluginAbstract#test_has_required_abstract_methods().
  TestDefaultExtractorInit.test_init_creates_instance: DefaultExtractorInit#test_init_creates_instance().
  TestElementExtractorAbstract: ElementExtractorAbstract#
  TestLanguagePluginAbstract: LanguagePluginAbstract#
  TestDefaultExtractorInit: DefaultExtractorInit#
  TestDefaultExtractorNodeTypeChecks: DefaultExtractorNodeTypeChecks#
  TestDefaultExtractorNodeText: DefaultExtractorNodeText#
  TestDefaultExtractorNodeName: DefaultExtractorNodeName#
  TestDefaultExtractorExtraction: DefaultExtractorExtraction#
  TestDefaultExtractorDefaultMethods: DefaultExtractorDefaultMethods#
  TestDefaultExtractorAllElements: DefaultExtractorAllElements#
  TestDefaultLanguagePlugin: DefaultLanguagePlugin#
  TestDefaultLanguagePluginAnalyze: DefaultLanguagePluginAnalyze#
---
# Module: [`tests/unit/core/test_base_plugin.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_base_plugin.py)

## Classes
### `TestDefaultExtractorAllElements`
- def: [`tests/unit/core/test_base_plugin.py:306`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_base_plugin.py#L306)
- doc: Tests for extract_all_elements method.
- signature: `class TestDefaultExtractorAllElements:`
- members:
  - `test_extract_all_elements_aggregates_all(self)` — [`L309`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_base_plugin.py#L309) — extract_all_elements should combine all element types.
- uses (calls/refs, reference-scoped): [`DefaultExtractor`](../../../tree_sitter_analyzer/plugins/base.md#DefaultExtractor), [`extract_all_elements`](../../../tree_sitter_analyzer/plugins/base.md#ElementExtractor.extract_all_elements)

### `TestDefaultExtractorDefaultMethods`
- def: [`tests/unit/core/test_base_plugin.py:263`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_base_plugin.py#L263)
- doc: Tests for DefaultExtractor default method implementations.
- signature: `class TestDefaultExtractorDefaultMethods:`
- members:
  - `test_extract_annotations_returns_empty(self)` — [`L274`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_base_plugin.py#L274) — extract_annotations should return empty list by default.
  - `test_extract_css_rules_returns_empty(self)` — [`L290`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_base_plugin.py#L290) — extract_css_rules should return empty list by default.
  - `test_extract_html_elements_returns_empty(self)` — [`L282`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_base_plugin.py#L282) — extract_html_elements should return empty list by default.
  - `test_extract_packages_returns_empty(self)` — [`L266`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_base_plugin.py#L266) — extract_packages should return empty list by default.
  - `test_get_language_hint_returns_unknown(self)` — [`L298`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_base_plugin.py#L298) — _get_language_hint should return 'unknown' by default.
- uses (calls/refs, reference-scoped): [`extract_html_elements`](../../../tree_sitter_analyzer/plugins/base.md#ElementExtractor.extract_html_elements), [`DefaultExtractor`](../../../tree_sitter_analyzer/plugins/base.md#DefaultExtractor), [`extract_css_rules`](../../../tree_sitter_analyzer/plugins/base.md#ElementExtractor.extract_css_rules), [`extract_packages`](../../../tree_sitter_analyzer/plugins/base.md#ElementExtractor.extract_packages), [`extract_annotations`](../../../tree_sitter_analyzer/plugins/base.md#ElementExtractor.extract_annotations), [`_get_language_hint`](../../../tree_sitter_analyzer/plugins/_base_traverse_mixin.md#DefaultNodeMixin._get_language_hint)

### `TestDefaultExtractorExtraction`
- def: [`tests/unit/core/test_base_plugin.py:203`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_base_plugin.py#L203)
- doc: Tests for DefaultExtractor extraction methods.
- signature: `class TestDefaultExtractorExtraction:`
- members:
  - `test_extract_classes_empty_tree(self)` — [`L238`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_base_plugin.py#L238) — extract_classes should return empty list for empty tree.
  - `test_extract_functions_empty_tree(self)` — [`L206`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_base_plugin.py#L206) — extract_functions should return empty list for empty tree.
  - `test_extract_functions_with_tree(self)` — [`L214`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_base_plugin.py#L214) — extract_functions should extract functions from tree.
  - `test_extract_imports_empty_tree(self)` — [`L254`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_base_plugin.py#L254) — extract_imports should return empty list for empty tree.
  - `test_extract_variables_empty_tree(self)` — [`L246`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_base_plugin.py#L246) — extract_variables should return empty list for empty tree.
- uses (calls/refs, reference-scoped): [`DefaultExtractor`](../../../tree_sitter_analyzer/plugins/base.md#DefaultExtractor), [`extract_functions`](../../../tree_sitter_analyzer/plugins/base.md#DefaultExtractor.extract_functions), [`extract_classes`](../../../tree_sitter_analyzer/plugins/base.md#DefaultExtractor.extract_classes), [`extract_imports`](../../../tree_sitter_analyzer/plugins/base.md#DefaultExtractor.extract_imports), [`extract_variables`](../../../tree_sitter_analyzer/plugins/base.md#DefaultExtractor.extract_variables)

### `TestDefaultExtractorInit`
- def: [`tests/unit/core/test_base_plugin.py:47`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_base_plugin.py#L47)
- doc: Tests for DefaultExtractor initialization.
- signature: `class TestDefaultExtractorInit:`
- members:
  - `test_init_creates_instance(self)` — [`L50`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_base_plugin.py#L50) — DefaultExtractor should be instantiable.
  - `test_init_sets_current_file(self)` — [`L55`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_base_plugin.py#L55) — DefaultExtractor should initialize current_file as empty string.
- uses (calls/refs, reference-scoped): [`DefaultExtractor`](../../../tree_sitter_analyzer/plugins/base.md#DefaultExtractor), [`current_file`](../../../tree_sitter_analyzer/plugins/base.md#ElementExtractor.current_file)

### `TestDefaultExtractorNodeName`
- def: [`tests/unit/core/test_base_plugin.py:168`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_base_plugin.py#L168)
- doc: Tests for DefaultExtractor node name extraction.
- signature: `class TestDefaultExtractorNodeName:`
- members:
  - `test_extract_node_name_fallback(self)` — [`L190`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_base_plugin.py#L190) — _extract_node_name should use fallback when no identifier found.
  - `test_extract_node_name_with_identifier_child(self)` — [`L171`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_base_plugin.py#L171) — _extract_node_name should find identifier in children.
- uses (calls/refs, reference-scoped): [`DefaultExtractor`](../../../tree_sitter_analyzer/plugins/base.md#DefaultExtractor), [`_extract_node_name`](../../../tree_sitter_analyzer/plugins/_base_traverse_mixin.md#DefaultNodeMixin._extract_node_name)

### `TestDefaultExtractorNodeText`
- def: [`tests/unit/core/test_base_plugin.py:127`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_base_plugin.py#L127)
- doc: Tests for DefaultExtractor node text extraction.
- signature: `class TestDefaultExtractorNodeText:`
- members:
  - `test_extract_node_text_with_bytes(self)` — [`L130`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_base_plugin.py#L130) — _extract_node_text should extract text using byte positions.
  - `test_extract_node_text_with_unicode(self)` — [`L151`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_base_plugin.py#L151) — _extract_node_text should handle unicode characters.
  - `test_extract_node_text_without_attributes(self)` — [`L143`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_base_plugin.py#L143) — _extract_node_text should return empty string if no byte attributes.
- uses (calls/refs, reference-scoped): [`DefaultExtractor`](../../../tree_sitter_analyzer/plugins/base.md#DefaultExtractor), [`_extract_node_text`](../../../tree_sitter_analyzer/plugins/_base_traverse_mixin.md#DefaultNodeMixin._extract_node_text)

### `TestDefaultExtractorNodeTypeChecks`
- def: [`tests/unit/core/test_base_plugin.py:61`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_base_plugin.py#L61)
- doc: Tests for DefaultExtractor node type checking methods.
- signature: `class TestDefaultExtractorNodeTypeChecks:`
- members:
  - `test_is_class_node_false_cases(self)` — [`L89`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_base_plugin.py#L89) — _is_class_node should return False for non-class types.
  - `test_is_class_node_true_cases(self)` — [`L80`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_base_plugin.py#L80) — _is_class_node should return True for class types.
  - `test_is_function_node_false_cases(self)` — [`L73`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_base_plugin.py#L73) — _is_function_node should return False for non-function types.
  - `test_is_function_node_true_cases(self)` — [`L64`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_base_plugin.py#L64) — _is_function_node should return True for function types.
  - `test_is_import_node_false_cases(self)` — [`L119`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_base_plugin.py#L119) — _is_import_node should return False for non-import types.
  - `test_is_import_node_true_cases(self)` — [`L111`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_base_plugin.py#L111) — _is_import_node should return True for import types.
  - `test_is_variable_node_false_cases(self)` — [`L104`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_base_plugin.py#L104) — _is_variable_node should return False for non-variable types.
  - `test_is_variable_node_true_cases(self)` — [`L96`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_base_plugin.py#L96) — _is_variable_node should return True for variable types.
- uses (calls/refs, reference-scoped): [`DefaultExtractor`](../../../tree_sitter_analyzer/plugins/base.md#DefaultExtractor), [`_is_class_node`](../../../tree_sitter_analyzer/plugins/_base_traverse_mixin.md#DefaultNodeMixin._is_class_node), [`_is_function_node`](../../../tree_sitter_analyzer/plugins/_base_traverse_mixin.md#DefaultNodeMixin._is_function_node), [`_is_import_node`](../../../tree_sitter_analyzer/plugins/_base_traverse_mixin.md#DefaultNodeMixin._is_import_node), [`_is_variable_node`](../../../tree_sitter_analyzer/plugins/_base_traverse_mixin.md#DefaultNodeMixin._is_variable_node)

### `TestDefaultLanguagePlugin`
- def: [`tests/unit/core/test_base_plugin.py:318`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_base_plugin.py#L318)
- doc: Tests for DefaultLanguagePlugin class.
- signature: `class TestDefaultLanguagePlugin:`
- members:
  - `test_create_extractor(self)` — [`L333`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_base_plugin.py#L333) — create_extractor should return DefaultExtractor instance.
  - `test_execute_query_strategy_none_key(self)` — [`L401`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_base_plugin.py#L401) — execute_query_strategy should return None for None key.
  - `test_execute_query_strategy_unknown_key(self)` — [`L407`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_base_plugin.py#L407) — execute_query_strategy should return None for unknown key.
  - `test_get_element_categories_returns_empty(self)` — [`L360`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_base_plugin.py#L360) — get_element_categories should return empty dict by default.
  - `test_get_file_extensions(self)` — [`L326`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_base_plugin.py#L326) — get_file_extensions should return txt and md.
  - `test_get_formatter_map_returns_empty(self)` — [`L354`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_base_plugin.py#L354) — get_formatter_map should return empty dict by default.
  - `test_get_language_name(self)` — [`L321`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_base_plugin.py#L321) — get_language_name should return 'generic'.
  - `test_get_plugin_info(self)` — [`L390`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_base_plugin.py#L390) — get_plugin_info should return plugin information.
  - `test_get_queries_returns_empty(self)` — [`L348`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_base_plugin.py#L348) — get_queries should return empty dict by default.
  - `test_get_supported_element_types(self)` — [`L339`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_base_plugin.py#L339) — get_supported_element_types should return standard types.
  - `test_is_applicable_case_insensitive(self)` — [`L384`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_base_plugin.py#L384) — is_applicable should be case insensitive.
  - `test_is_applicable_false_for_other(self)` — [`L378`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_base_plugin.py#L378) — is_applicable should return False for non-supported extensions.
  - `test_is_applicable_for_md(self)` — [`L372`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_base_plugin.py#L372) — is_applicable should return True for .md files.
  - `test_is_applicable_for_txt(self)` — [`L366`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_base_plugin.py#L366) — is_applicable should return True for .txt files.
- uses (calls/refs, reference-scoped): [`DefaultExtractor`](../../../tree_sitter_analyzer/plugins/base.md#DefaultExtractor), [`is_applicable`](../../../tree_sitter_analyzer/plugins/base.md#LanguagePlugin.is_applicable), [`DefaultLanguagePlugin`](../../../tree_sitter_analyzer/plugins/base.md#DefaultLanguagePlugin), [`execute_query_strategy`](../../../tree_sitter_analyzer/plugins/base.md#LanguagePlugin.execute_query_strategy), [`get_plugin_info`](../../../tree_sitter_analyzer/plugins/base.md#LanguagePlugin.get_plugin_info), [`get_queries`](../../../tree_sitter_analyzer/plugins/base.md#LanguagePlugin.get_queries), [`get_element_categories`](../../../tree_sitter_analyzer/plugins/base.md#LanguagePlugin.get_element_categories), [`get_supported_element_types`](../../../tree_sitter_analyzer/plugins/base.md#LanguagePlugin.get_supported_element_types), [`create_extractor`](../../../tree_sitter_analyzer/plugins/base.md#DefaultLanguagePlugin.create_extractor), [`get_file_extensions`](../../../tree_sitter_analyzer/plugins/base.md#DefaultLanguagePlugin.get_file_extensions), [`get_language_name`](../../../tree_sitter_analyzer/plugins/base.md#DefaultLanguagePlugin.get_language_name), [`get_formatter_map`](../../../tree_sitter_analyzer/plugins/base.md#LanguagePlugin.get_formatter_map)

### `TestDefaultLanguagePluginAnalyze`
- def: [`tests/unit/core/test_base_plugin.py:414`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_base_plugin.py#L414)
- doc: Tests for DefaultLanguagePlugin analyze_file method.
- signature: `class TestDefaultLanguagePluginAnalyze:`
- members:
  - `test_analyze_file_handles_error(self)` — [`L432`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_base_plugin.py#L432) — analyze_file should handle errors gracefully.
  - `test_analyze_file_returns_result(self, tmp_path)` — [`L418`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_base_plugin.py#L418) — analyze_file should return AnalysisResult.
- uses (calls/refs, reference-scoped): [`success`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.success), [`error_message`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.error_message), [`analyze_file`](../../../tree_sitter_analyzer/plugins/base.md#DefaultLanguagePlugin.analyze_file), [`DefaultLanguagePlugin`](../../../tree_sitter_analyzer/plugins/base.md#DefaultLanguagePlugin)

### `TestElementExtractorAbstract`
- def: [`tests/unit/core/test_base_plugin.py:15`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_base_plugin.py#L15)
- doc: Tests for ElementExtractor abstract class.
- signature: `class TestElementExtractorAbstract:`
- members:
  - `test_cannot_instantiate_directly(self)` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_base_plugin.py#L18) — ElementExtractor should not be instantiable directly.
  - `test_has_required_abstract_methods(self)` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_base_plugin.py#L23) — ElementExtractor should define required abstract methods.
- uses (calls/refs, reference-scoped): [`ElementExtractor`](../../../tree_sitter_analyzer/plugins/base.md#ElementExtractor)

### `TestLanguagePluginAbstract`
- def: [`tests/unit/core/test_base_plugin.py:31`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_base_plugin.py#L31)
- doc: Tests for LanguagePlugin abstract class.
- signature: `class TestLanguagePluginAbstract:`
- members:
  - `test_cannot_instantiate_directly(self)` — [`L34`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_base_plugin.py#L34) — LanguagePlugin should not be instantiable directly.
  - `test_has_required_abstract_methods(self)` — [`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_base_plugin.py#L39) — LanguagePlugin should define required abstract methods.
- uses (calls/refs, reference-scoped): [`LanguagePlugin`](../../../tree_sitter_analyzer/plugins/base.md#LanguagePlugin)

