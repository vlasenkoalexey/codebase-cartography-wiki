---
title: 'Module: tests/unit/languages/test_plugins_base_core.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_plugins_base_core.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_plugins_base_core`/Test
symbols:
  TestDefaultExtractorIntegration.test_full_extraction_workflow: DefaultExtractorIntegration#test_full_extraction_workflow().
  TestLanguagePlugin.test_default_language_plugin_initialization: LanguagePlugin#test_default_language_plugin_initialization().
  TestLanguagePlugin.test_default_language_plugin_create_extractor: LanguagePlugin#test_default_language_plugin_create_extractor().
  TestLanguagePlugin.test_get_supported_element_types: LanguagePlugin#test_get_supported_element_types().
  TestLanguagePlugin.test_get_queries: LanguagePlugin#test_get_queries().
  TestLanguagePlugin.test_execute_query_strategy: LanguagePlugin#test_execute_query_strategy().
  TestLanguagePlugin.test_get_formatter_map: LanguagePlugin#test_get_formatter_map().
  TestLanguagePlugin.test_get_element_categories: LanguagePlugin#test_get_element_categories().
  TestElementExtractor.test_default_extractor_initialization: ElementExtractor#test_default_extractor_initialization().
  TestElementExtractor.test_extract_functions: ElementExtractor#test_extract_functions().
  TestElementExtractor.test_extract_classes: ElementExtractor#test_extract_classes().
  TestElementExtractor.test_extract_variables: ElementExtractor#test_extract_variables().
  TestElementExtractor.test_extract_imports: ElementExtractor#test_extract_imports().
  TestElementExtractor.test_extract_all_elements: ElementExtractor#test_extract_all_elements().
  TestElementExtractor.test_extract_all_elements_with_exception: ElementExtractor#test_extract_all_elements_with_exception().
  TestElementExtractor.test_is_function_node: ElementExtractor#test_is_function_node().
  TestElementExtractor.test_is_class_node: ElementExtractor#test_is_class_node().
  TestElementExtractor.test_is_variable_node: ElementExtractor#test_is_variable_node().
  TestElementExtractor.test_is_import_node: ElementExtractor#test_is_import_node().
  TestElementExtractor.test_extract_node_text: ElementExtractor#test_extract_node_text().
  TestElementExtractor.test_extract_node_text_with_unicode: ElementExtractor#test_extract_node_text_with_unicode().
  TestElementExtractor.test_extract_node_text_error_handling: ElementExtractor#test_extract_node_text_error_handling().
  TestElementExtractor.test_extract_node_name: ElementExtractor#test_extract_node_name().
  TestElementExtractor.test_extract_node_name_no_identifier: ElementExtractor#test_extract_node_name_no_identifier().
  TestElementExtractor.test_extract_node_name_error_handling: ElementExtractor#test_extract_node_name_error_handling().
  TestElementExtractor.test_get_language_hint: ElementExtractor#test_get_language_hint().
  TestDefaultExtractorTraversalDirect.test_traverse_for_functions: DefaultExtractorTraversalDirect#test_traverse_for_functions().
  TestDefaultExtractorTraversalDirect.test_traverse_for_functions_with_children: DefaultExtractorTraversalDirect#test_traverse_for_functions_with_children().
  TestDefaultExtractorTraversalDirect.test_traverse_error_handling: DefaultExtractorTraversalDirect#test_traverse_error_handling().
  TestDefaultExtractorIntegration.test_extraction_with_no_tree: DefaultExtractorIntegration#test_extraction_with_no_tree().
  TestElementExtractor.extractor: ElementExtractor#extractor().
  TestDefaultExtractorTraversalDirect.extractor: DefaultExtractorTraversalDirect#extractor().
  TestLanguagePlugin: LanguagePlugin#
  TestElementExtractor: ElementExtractor#
  TestElementExtractor.mock_tree: ElementExtractor#mock_tree().
  TestDefaultExtractorTraversalDirect: DefaultExtractorTraversalDirect#
  TestDefaultExtractorIntegration: DefaultExtractorIntegration#
---
# Module: [`tests/unit/languages/test_plugins_base_core.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_base_core.py)

## Classes
### `TestDefaultExtractorIntegration`
- def: [`tests/unit/languages/test_plugins_base_core.py:402`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_base_core.py#L402)
- doc: Integration tests for DefaultExtractor
- signature: `class TestDefaultExtractorIntegration:`
- members:
  - `test_extraction_with_no_tree(self)` — [`L430`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_base_core.py#L430) — Test extraction with invalid tree
  - `test_full_extraction_workflow(self)` — [`L405`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_base_core.py#L405) — Test complete extraction workflow
- uses (calls/refs, reference-scoped): [`DefaultExtractor`](../../../tree_sitter_analyzer/plugins/base.md#DefaultExtractor), [`extract_all_elements`](../../../tree_sitter_analyzer/plugins/base.md#ElementExtractor.extract_all_elements), [`extract_functions`](../../../tree_sitter_analyzer/plugins/base.md#DefaultExtractor.extract_functions), [`extract_classes`](../../../tree_sitter_analyzer/plugins/base.md#DefaultExtractor.extract_classes), [`extract_imports`](../../../tree_sitter_analyzer/plugins/base.md#DefaultExtractor.extract_imports), [`extract_variables`](../../../tree_sitter_analyzer/plugins/base.md#DefaultExtractor.extract_variables)

### `TestDefaultExtractorTraversalDirect`
- def: [`tests/unit/languages/test_plugins_base_core.py:325`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_base_core.py#L325)
- doc: Test DefaultExtractor traversal methods
- signature: `class TestDefaultExtractorTraversalDirect:`
- members:
  - `extractor(self)` — [`L329`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_base_core.py#L329) — Create a DefaultExtractor instance
  - `test_traverse_error_handling(self, extractor: DefaultExtractor)` — [`L382`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_base_core.py#L382) — Test traversal error handling
  - `test_traverse_for_functions(self, extractor: DefaultExtractor)` — [`L333`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_base_core.py#L333) — Test _traverse_for_functions method
  - `test_traverse_for_functions_with_children(self, extractor: DefaultExtractor)` — [`L355`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_base_core.py#L355) — Test _traverse_for_functions with child nodes
- uses (calls/refs, reference-scoped): [`DefaultExtractor`](../../../tree_sitter_analyzer/plugins/base.md#DefaultExtractor), [`_traverse_for_functions`](../../../tree_sitter_analyzer/plugins/_base_traverse_mixin.md#DefaultTraverseMixin._traverse_for_functions)

### `TestElementExtractor`
- def: [`tests/unit/languages/test_plugins_base_core.py:86`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_base_core.py#L86)
- doc: Test ElementExtractor abstract base class
- signature: `class TestElementExtractor:`
- members:
  - `extractor(self)` — [`L97`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_base_core.py#L97) — Create a DefaultExtractor instance
  - `mock_tree(self)` — [`L90`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_base_core.py#L90) — Create a mock tree-sitter tree
  - `test_default_extractor_initialization(self, extractor: DefaultExtractor)` — [`L101`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_base_core.py#L101) — Test DefaultExtractor initialization
  - `test_extract_all_elements(self, extractor: DefaultExtractor, mock_tree: Mock)` — [`L189`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_base_core.py#L189) — Test extract_all_elements method
  - `test_extract_all_elements_with_exception(self, extractor: DefaultExtractor, mock_tree: Mock)` — [`L200`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_base_core.py#L200) — Test extract_all_elements with exception handling
  - `test_extract_classes(self, extractor: DefaultExtractor, mock_tree: Mock)` — [`L129`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_base_core.py#L129) — Test extract_classes method
  - `test_extract_functions(self, extractor: DefaultExtractor, mock_tree: Mock)` — [`L107`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_base_core.py#L107) — Test extract_functions method
  - `test_extract_imports(self, extractor: DefaultExtractor, mock_tree: Mock)` — [`L169`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_base_core.py#L169) — Test extract_imports method
  - `test_extract_node_name(self, extractor: DefaultExtractor)` — [`L278`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_base_core.py#L278) — Test _extract_node_name method
  - `test_extract_node_name_error_handling(self, extractor: DefaultExtractor)` — [`L308`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_base_core.py#L308) — Test _extract_node_name error handling
  - `test_extract_node_name_no_identifier(self, extractor: DefaultExtractor)` — [`L297`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_base_core.py#L297) — Test _extract_node_name without identifier child
  - `test_extract_node_text(self, extractor: DefaultExtractor)` — [`L244`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_base_core.py#L244) — Test _extract_node_text method
  - `test_extract_node_text_error_handling(self, extractor: DefaultExtractor)` — [`L267`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_base_core.py#L267) — Test _extract_node_text error handling
  - `test_extract_node_text_with_unicode(self, extractor: DefaultExtractor)` — [`L255`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_base_core.py#L255) — Test _extract_node_text with unicode characters
  - `test_extract_variables(self, extractor: DefaultExtractor, mock_tree: Mock)` — [`L149`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_base_core.py#L149) — Test extract_variables method
  - `test_get_language_hint(self, extractor: DefaultExtractor)` — [`L319`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_base_core.py#L319) — Test _get_language_hint method
  - `test_is_class_node(self, extractor: DefaultExtractor)` — [`L220`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_base_core.py#L220) — Test _is_class_node method
  - `test_is_function_node(self, extractor: DefaultExtractor)` — [`L212`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_base_core.py#L212) — Test _is_function_node method
  - `test_is_import_node(self, extractor: DefaultExtractor)` — [`L236`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_base_core.py#L236) — Test _is_import_node method
  - `test_is_variable_node(self, extractor: DefaultExtractor)` — [`L228`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_base_core.py#L228) — Test _is_variable_node method
- uses (calls/refs, reference-scoped): [`ElementExtractor`](../../../tree_sitter_analyzer/plugins/base.md#ElementExtractor), [`DefaultExtractor`](../../../tree_sitter_analyzer/plugins/base.md#DefaultExtractor), [`extract_all_elements`](../../../tree_sitter_analyzer/plugins/base.md#ElementExtractor.extract_all_elements), [`_is_class_node`](../../../tree_sitter_analyzer/plugins/_base_traverse_mixin.md#DefaultNodeMixin._is_class_node), [`_is_function_node`](../../../tree_sitter_analyzer/plugins/_base_traverse_mixin.md#DefaultNodeMixin._is_function_node), [`_is_import_node`](../../../tree_sitter_analyzer/plugins/_base_traverse_mixin.md#DefaultNodeMixin._is_import_node), [`_is_variable_node`](../../../tree_sitter_analyzer/plugins/_base_traverse_mixin.md#DefaultNodeMixin._is_variable_node), [`_extract_node_name`](../../../tree_sitter_analyzer/plugins/_base_traverse_mixin.md#DefaultNodeMixin._extract_node_name), [`extract_functions`](../../../tree_sitter_analyzer/plugins/base.md#DefaultExtractor.extract_functions), [`extract_classes`](../../../tree_sitter_analyzer/plugins/base.md#DefaultExtractor.extract_classes), [`extract_imports`](../../../tree_sitter_analyzer/plugins/base.md#DefaultExtractor.extract_imports), [`extract_variables`](../../../tree_sitter_analyzer/plugins/base.md#DefaultExtractor.extract_variables), [`_extract_node_text`](../../../tree_sitter_analyzer/plugins/_base_traverse_mixin.md#DefaultNodeMixin._extract_node_text), [`_get_language_hint`](../../../tree_sitter_analyzer/plugins/_base_traverse_mixin.md#DefaultNodeMixin._get_language_hint)

### `TestLanguagePlugin`
- def: [`tests/unit/languages/test_plugins_base_core.py:19`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_base_core.py#L19)
- doc: Test LanguagePlugin abstract base class
- signature: `class TestLanguagePlugin:`
- members:
  - `test_default_language_plugin_create_extractor(self)` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_base_core.py#L29) — Test DefaultLanguagePlugin create_extractor method
  - `test_default_language_plugin_initialization(self)` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_base_core.py#L22) — Test DefaultLanguagePlugin initialization
  - `test_execute_query_strategy(self)` — [`L56`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_base_core.py#L56) — Test execute_query_strategy method
  - `test_get_element_categories(self)` — [`L76`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_base_core.py#L76) — Test get_element_categories method
  - `test_get_formatter_map(self)` — [`L67`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_base_core.py#L67) — Test get_formatter_map method
  - `test_get_queries(self)` — [`L47`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_base_core.py#L47) — Test get_queries method
  - `test_get_supported_element_types(self)` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugins_base_core.py#L36) — Test get_supported_element_types method
- uses (calls/refs, reference-scoped): [`DefaultExtractor`](../../../tree_sitter_analyzer/plugins/base.md#DefaultExtractor), [`DefaultLanguagePlugin`](../../../tree_sitter_analyzer/plugins/base.md#DefaultLanguagePlugin), [`execute_query_strategy`](../../../tree_sitter_analyzer/plugins/base.md#LanguagePlugin.execute_query_strategy), [`get_queries`](../../../tree_sitter_analyzer/plugins/base.md#LanguagePlugin.get_queries), [`get_element_categories`](../../../tree_sitter_analyzer/plugins/base.md#LanguagePlugin.get_element_categories), [`get_supported_element_types`](../../../tree_sitter_analyzer/plugins/base.md#LanguagePlugin.get_supported_element_types), [`create_extractor`](../../../tree_sitter_analyzer/plugins/base.md#DefaultLanguagePlugin.create_extractor), [`get_file_extensions`](../../../tree_sitter_analyzer/plugins/base.md#DefaultLanguagePlugin.get_file_extensions), [`get_language_name`](../../../tree_sitter_analyzer/plugins/base.md#DefaultLanguagePlugin.get_language_name), [`get_formatter_map`](../../../tree_sitter_analyzer/plugins/base.md#LanguagePlugin.get_formatter_map)

