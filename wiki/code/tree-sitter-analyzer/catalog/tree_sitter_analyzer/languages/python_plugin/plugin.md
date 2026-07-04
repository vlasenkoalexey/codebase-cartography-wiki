---
title: 'Module: tree_sitter_analyzer/languages/python_plugin/plugin.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/python_plugin/plugin.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.python_plugin.plugin`/
symbols:
  PythonPlugin: PythonPlugin#
  PythonPlugin.analyze_file: PythonPlugin#analyze_file().
  TREE_SITTER_AVAILABLE: TREE_SITTER_AVAILABLE.
  PythonPlugin._analyze_sync: PythonPlugin#_analyze_sync().
  PythonPlugin.create_extractor: PythonPlugin#create_extractor().
  PythonPlugin.extract_elements: PythonPlugin#extract_elements().
  PythonPlugin.get_extractor: PythonPlugin#get_extractor().
  PythonPlugin.get_tree_sitter_language: PythonPlugin#get_tree_sitter_language().
  PythonPlugin.get_plugin_info: PythonPlugin#get_plugin_info().
  PythonPlugin._get_node_type_for_element: PythonPlugin#_get_node_type_for_element().
  PythonPlugin.get_language_name: PythonPlugin#get_language_name().
  PythonPlugin.extractor: PythonPlugin#extractor.
  PythonPlugin._extractor: PythonPlugin#_extractor.
  PythonPlugin.is_applicable: PythonPlugin#is_applicable().
  PythonPlugin._language_cache: PythonPlugin#_language_cache.
  PythonPlugin.get_file_extensions: PythonPlugin#get_file_extensions().
  PythonPlugin.execute_query_strategy: PythonPlugin#execute_query_strategy().
  PythonPlugin.get_supported_queries: PythonPlugin#get_supported_queries().
  PythonPlugin.__init__: PythonPlugin#__init__().
  PythonPlugin.language: PythonPlugin#language.
  PythonPlugin.get_element_categories: PythonPlugin#get_element_categories().
---
# Module: [`tree_sitter_analyzer/languages/python_plugin/plugin.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/plugin.py)

## Classes
### `PythonPlugin`  ·  implements/extends LanguagePlugin
- def: [`tree_sitter_analyzer/languages/python_plugin/plugin.py:27`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/plugin.py#L27) — documented in [tree_sitter_analyzer-plugins-manager](../../../../concepts/tree_sitter_analyzer-plugins-manager.md)
- doc: Python language plugin for the new architecture
- signature: `class PythonPlugin(LanguagePlugin):`
- members:
  - `__init__(self)` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/plugin.py#L30) — Initialize the Python plugin
  - `analyze_file(self, file_path: str, request: AnalysisRequest)` — [`L207`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/plugin.py#L207) — documented in [tree_sitter_analyzer-models-result](../../../../concepts/tree_sitter_analyzer-models-result.md)
  - `create_extractor(self)` — [`L46`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/plugin.py#L46)
  - `execute_query_strategy(self, query_key: str | None, language: str)` — [`L123`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/plugin.py#L123)
  - `extract_elements(self, tree: tree_sitter.Tree, source_code: str)` — [`L274`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/plugin.py#L274)
  - `get_element_categories(self)` — [`L140`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/plugin.py#L140)
  - `get_extractor(self)` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/plugin.py#L49)
  - `get_file_extensions(self)` — [`L43`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/plugin.py#L43)
  - `get_language_name(self)` — [`L40`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/plugin.py#L40)
  - `get_plugin_info(self)` — [`L96`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/plugin.py#L96)
  - `get_supported_queries(self)` — [`L70`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/plugin.py#L70)
  - `get_tree_sitter_language(self)` — [`L54`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/plugin.py#L54)
  - `is_applicable(self, file_path: str)` — [`L90`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/plugin.py#L90)
  - `extractor` — [`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/plugin.py#L38)
  - `language` — [`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/plugin.py#L37)
- protocol/private: `_analyze_sync`[`L233`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/plugin.py#L233), `_extractor`[`L34`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/plugin.py#L34), `_get_node_type_for_element`[`L129`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/plugin.py#L129), `_language_cache`[`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/plugin.py#L33)
- uses (calls/refs, reference-scoped): [`AnalysisResult`](../../models/result.md#AnalysisResult), [`Function`](../../models/base.md#Function), [`log_error`](../../utils/logging.md#log_error), [`Class`](../../models/base.md#Class), [`Variable`](../../models/base.md#Variable), [`AnalysisRequest`](../../core/request.md#AnalysisRequest), [`elements`](../../models/result.md#AnalysisResult.elements), [`Import`](../../models/base.md#Import), [`language`](../../models/result.md#AnalysisResult.language), [`CodeElement`](../../models/base.md#CodeElement), [`LanguagePlugin`](../../plugins/base.md#LanguagePlugin), [`file_path`](../../models/result.md#AnalysisResult.file_path), [`success`](../../models/result.md#AnalysisResult.success), [`ElementExtractor`](../../plugins/base.md#ElementExtractor), [`extract_functions`](../../plugins/base.md#ElementExtractor.extract_functions), [`extract_classes`](../../plugins/base.md#ElementExtractor.extract_classes), [`line_count`](../../models/result.md#AnalysisResult.line_count), [`extract_variables`](../../plugins/base.md#ElementExtractor.extract_variables), [`error_message`](../../models/result.md#AnalysisResult.error_message), [`extract_imports`](../../plugins/base.md#ElementExtractor.extract_imports), [`PythonElementExtractor`](extractor.md#PythonElementExtractor), [`node_count`](../../models/result.md#AnalysisResult.node_count), [`TREE_SITTER_AVAILABLE`](plugin.md#TREE_SITTER_AVAILABLE), [`get_queries`](../../plugins/base.md#LanguagePlugin.get_queries), [`read_file_safe_async`](../../encoding_utils.md#read_file_safe_async), [`count_nodes_iterative`](../../utils/tree_sitter_compat.md#count_nodes_iterative), [`current_file`](../../plugins/base.md#ElementExtractor.current_file)
- used by: [`LanguagePlugin`](../../plugins/base.md#LanguagePlugin), [`get_language_name`](../../plugins/base.md#LanguagePlugin.get_language_name), [`analyze_file`](../../plugins/base.md#LanguagePlugin.analyze_file), [`get_file_extensions`](../../plugins/base.md#LanguagePlugin.get_file_extensions), [`create_extractor`](../../plugins/base.md#LanguagePlugin.create_extractor), [`get_tree_sitter_language`](../../plugins/base.md#LanguagePlugin.get_tree_sitter_language), [`is_applicable`](../../plugins/base.md#LanguagePlugin.is_applicable), [`execute_query_strategy`](../../plugins/base.md#LanguagePlugin.execute_query_strategy), [`get_plugin_info`](../../plugins/base.md#LanguagePlugin.get_plugin_info), [`get_element_categories`](../../plugins/base.md#LanguagePlugin.get_element_categories)  (42 test-only)

## Module values
- `TREE_SITTER_AVAILABLE` — [`L16`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/plugin.py#L16)

