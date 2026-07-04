---
title: 'Module: tree_sitter_analyzer/languages/javascript_plugin/plugin.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/javascript_plugin/plugin.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.javascript_plugin.plugin`/
symbols:
  JavaScriptPlugin.analyze_file: JavaScriptPlugin#analyze_file().
  JavaScriptPlugin: JavaScriptPlugin#
  TREE_SITTER_AVAILABLE: TREE_SITTER_AVAILABLE.
  JavaScriptPlugin._analyze_sync: JavaScriptPlugin#_analyze_sync().
  JavaScriptPlugin.extract_elements: JavaScriptPlugin#extract_elements().
  JavaScriptPlugin._get_node_type_for_element: JavaScriptPlugin#_get_node_type_for_element().
  JavaScriptPlugin.get_tree_sitter_language: JavaScriptPlugin#get_tree_sitter_language().
  JavaScriptPlugin.get_plugin_info: JavaScriptPlugin#get_plugin_info().
  JavaScriptPlugin.get_extractor: JavaScriptPlugin#get_extractor().
  JavaScriptPlugin.get_language_name: JavaScriptPlugin#get_language_name().
  JavaScriptPlugin.create_extractor: JavaScriptPlugin#create_extractor().
  JavaScriptPlugin.get_file_extensions: JavaScriptPlugin#get_file_extensions().
  JavaScriptPlugin._extractor: JavaScriptPlugin#_extractor.
  JavaScriptPlugin.extractor: JavaScriptPlugin#extractor.
  JavaScriptPlugin._language: JavaScriptPlugin#_language.
  JavaScriptPlugin.supported_extensions: JavaScriptPlugin#supported_extensions.
  JavaScriptPlugin.is_applicable: JavaScriptPlugin#is_applicable().
  JavaScriptPlugin.execute_query_strategy: JavaScriptPlugin#execute_query_strategy().
  _JS_EXTENSIONS: _JS_EXTENSIONS.
  JavaScriptPlugin.get_supported_queries: JavaScriptPlugin#get_supported_queries().
  JavaScriptPlugin.__init__: JavaScriptPlugin#__init__().
  JavaScriptPlugin.language: JavaScriptPlugin#language.
  JavaScriptPlugin.get_element_categories: JavaScriptPlugin#get_element_categories().
---
# Module: [`tree_sitter_analyzer/languages/javascript_plugin/plugin.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/plugin.py)

## Classes
### `JavaScriptPlugin`  ·  implements/extends LanguagePlugin
- def: [`tree_sitter_analyzer/languages/javascript_plugin/plugin.py:32`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/plugin.py#L32) — documented in [tree_sitter_analyzer-plugins-manager](../../../../concepts/tree_sitter_analyzer-plugins-manager.md)
- doc: Enhanced JavaScript language plugin with comprehensive feature support
- signature: `class JavaScriptPlugin(LanguagePlugin):`
- members:
  - `_get_node_type_for_element(self, element: Any)` — [`L120`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/plugin.py#L120) — Get appropriate node type for element
  - `analyze_file(self, file_path: str, request: AnalysisRequest)` — [`L204`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/plugin.py#L204) — Analyze a JavaScript file and return the analysis results. — documented in [tree_sitter_analyzer-models-result](../../../../concepts/tree_sitter_analyzer-models-result.md)
  - `create_extractor(self)` — [`L52`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/plugin.py#L52) — Create and return an element extractor for this language
  - `execute_query_strategy(self, query_key: str | None, language: str)` — [`L113`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/plugin.py#L113) — Execute query strategy for JavaScript language
  - `extract_elements(self, tree: tree_sitter.Tree, source_code: str)` — [`L275`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/plugin.py#L275) — Extract elements from source code using tree-sitter AST
  - `get_element_categories(self)` — [`L140`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/plugin.py#L140) — Get element categories mapping query keys to node types
  - `get_extractor(self)` — [`L56`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/plugin.py#L56)
  - `get_file_extensions(self)` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/plugin.py#L48) — Return list of file extensions this plugin supports
  - `get_language_name(self)` — [`L44`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/plugin.py#L44) — Return the name of the programming language this plugin supports
  - `get_plugin_info(self)` — [`L89`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/plugin.py#L89) — Get information about this plugin
  - `get_supported_queries(self)` — [`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/plugin.py#L65) — Get list of supported query names for this language
  - `get_tree_sitter_language(self)` — [`L59`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/plugin.py#L59) — Load and return JavaScript tree-sitter language
  - `is_applicable(self, file_path: str)` — [`L82`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/plugin.py#L82) — Check if this plugin is applicable for the given file
  - `extractor` — [`L41`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/plugin.py#L41)
  - `language` — [`L40`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/plugin.py#L40)
  - `supported_extensions` — [`L42`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/plugin.py#L42)
- protocol/private: `__init__`[`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/plugin.py#L35), `_analyze_sync`[`L232`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/plugin.py#L232), `_extractor`[`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/plugin.py#L36), `_language`[`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/plugin.py#L37)
- uses (calls/refs, reference-scoped): [`AnalysisResult`](../../models/result.md#AnalysisResult), [`Function`](../../models/base.md#Function), [`log_error`](../../utils/logging.md#log_error), [`Class`](../../models/base.md#Class), [`Variable`](../../models/base.md#Variable), [`AnalysisRequest`](../../core/request.md#AnalysisRequest), [`elements`](../../models/result.md#AnalysisResult.elements), [`Import`](../../models/base.md#Import), [`language`](../../models/result.md#AnalysisResult.language), [`CodeElement`](../../models/base.md#CodeElement), [`LanguagePlugin`](../../plugins/base.md#LanguagePlugin), [`file_path`](../../models/result.md#AnalysisResult.file_path), [`success`](../../models/result.md#AnalysisResult.success), [`ElementExtractor`](../../plugins/base.md#ElementExtractor), [`extract_functions`](../../plugins/base.md#ElementExtractor.extract_functions), [`extract_classes`](../../plugins/base.md#ElementExtractor.extract_classes), [`line_count`](../../models/result.md#AnalysisResult.line_count), [`extract_variables`](../../plugins/base.md#ElementExtractor.extract_variables), [`error_message`](../../models/result.md#AnalysisResult.error_message), [`extract_imports`](../../plugins/base.md#ElementExtractor.extract_imports), [`loader`](../../language_loader.md#loader), [`node_count`](../../models/result.md#AnalysisResult.node_count), [`load_language`](../../language_loader.md#LanguageLoader.load_language), [`JavaScriptElementExtractor`](extractor.md#JavaScriptElementExtractor), [`is_method`](../../models/base.md#Function.is_method), [`get_queries`](../../plugins/base.md#LanguagePlugin.get_queries), [`TREE_SITTER_AVAILABLE`](plugin.md#TREE_SITTER_AVAILABLE), [`extract_classes`](_public_extraction_mixin.md#JavaScriptPublicExtractionMixin.extract_classes), [`read_file_safe_async`](../../encoding_utils.md#read_file_safe_async), [`is_arrow`](../../models/base.md#Function.is_arrow), [`extract_imports`](_public_extraction_mixin.md#JavaScriptPublicExtractionMixin.extract_imports), [`extract_variables`](_public_extraction_mixin.md#JavaScriptPublicExtractionMixin.extract_variables), [`count_nodes_iterative`](../../utils/tree_sitter_compat.md#count_nodes_iterative), [`extract_functions`](_public_extraction_mixin.md#JavaScriptPublicExtractionMixin.extract_functions), [`extract_exports`](_public_extraction_mixin.md#JavaScriptPublicExtractionMixin.extract_exports), [`current_file`](../../plugins/base.md#ElementExtractor.current_file), [`_JS_EXTENSIONS`](plugin.md#_JS_EXTENSIONS)
- used by: [`LanguagePlugin`](../../plugins/base.md#LanguagePlugin), [`get_language_name`](../../plugins/base.md#LanguagePlugin.get_language_name), [`analyze_file`](../../plugins/base.md#LanguagePlugin.analyze_file), [`get_file_extensions`](../../plugins/base.md#LanguagePlugin.get_file_extensions), [`create_extractor`](../../plugins/base.md#LanguagePlugin.create_extractor), [`get_tree_sitter_language`](../../plugins/base.md#LanguagePlugin.get_tree_sitter_language), [`is_applicable`](../../plugins/base.md#LanguagePlugin.is_applicable), [`execute_query_strategy`](../../plugins/base.md#LanguagePlugin.execute_query_strategy), [`get_plugin_info`](../../plugins/base.md#LanguagePlugin.get_plugin_info), [`get_element_categories`](../../plugins/base.md#LanguagePlugin.get_element_categories)  (17 test-only)

## Module values
- `TREE_SITTER_AVAILABLE` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/plugin.py#L19)
- `_JS_EXTENSIONS` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/plugin.py#L29)

