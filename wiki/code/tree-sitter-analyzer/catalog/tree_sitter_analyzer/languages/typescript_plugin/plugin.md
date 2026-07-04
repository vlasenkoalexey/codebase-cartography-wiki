---
title: 'Module: tree_sitter_analyzer/languages/typescript_plugin/plugin.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/typescript_plugin/plugin.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.typescript_plugin.plugin`/T
symbols:
  TypeScriptPlugin.analyze_file: ypeScriptPlugin#analyze_file().
  TypeScriptPlugin: ypeScriptPlugin#
  TREE_SITTER_AVAILABLE: REE_SITTER_AVAILABLE.
  TypeScriptPlugin.extract_elements: ypeScriptPlugin#extract_elements().
  TypeScriptPlugin.get_tree_sitter_language: ypeScriptPlugin#get_tree_sitter_language().
  TypeScriptPlugin.is_applicable: ypeScriptPlugin#is_applicable().
  TypeScriptPlugin.get_plugin_info: ypeScriptPlugin#get_plugin_info().
  TypeScriptPlugin.create_extractor: ypeScriptPlugin#create_extractor().
  TypeScriptPlugin.get_language_name: ypeScriptPlugin#get_language_name().
  TypeScriptPlugin.get_file_extensions: ypeScriptPlugin#get_file_extensions().
  TypeScriptPlugin.get_extractor: ypeScriptPlugin#get_extractor().
  TypeScriptPlugin.count_nodes: ypeScriptPlugin#count_nodes().
  TypeScriptPlugin._extractor: ypeScriptPlugin#_extractor.
  TypeScriptPlugin._language: ypeScriptPlugin#_language.
  TypeScriptPlugin.execute_query_strategy: ypeScriptPlugin#execute_query_strategy().
  TypeScriptPlugin.get_supported_queries: ypeScriptPlugin#get_supported_queries().
  TypeScriptPlugin.get_element_categories: ypeScriptPlugin#get_element_categories().
  TypeScriptPlugin.__init__: ypeScriptPlugin#__init__().
---
# Module: [`tree_sitter_analyzer/languages/typescript_plugin/plugin.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/plugin.py)

## Classes
### `TypeScriptPlugin`  ·  implements/extends LanguagePlugin
- def: [`tree_sitter_analyzer/languages/typescript_plugin/plugin.py:28`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/plugin.py#L28) — documented in [tree_sitter_analyzer-plugins-manager](../../../../concepts/tree_sitter_analyzer-plugins-manager.md)
- doc: Enhanced TypeScript language plugin with comprehensive feature support
- signature: `class TypeScriptPlugin(LanguagePlugin):`
- members:
  - `analyze_file(self, file_path: str, request: AnalysisRequest)` — [`L124`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/plugin.py#L124) — Analyze a TypeScript file and return the analysis results. — documented in [tree_sitter_analyzer-models-result](../../../../concepts/tree_sitter_analyzer-models-result.md)
  - `count_nodes(node: tree_sitter.Node)` — [`L170`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/plugin.py#L170)
  - `create_extractor(self)` — [`L43`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/plugin.py#L43) — Create and return an element extractor for this language
  - `execute_query_strategy(self, query_key: str | None, language: str)` — [`L215`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/plugin.py#L215) — Execute query strategy for TypeScript language
  - `extract_elements(self, tree: tree_sitter.Tree, source_code: str)` — [`L193`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/plugin.py#L193)
  - `get_element_categories(self)` — [`L222`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/plugin.py#L222) — Get TypeScript element categories mapping query_key to node_types
  - `get_extractor(self)` — [`L47`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/plugin.py#L47)
  - `get_file_extensions(self)` — [`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/plugin.py#L39) — Return list of file extensions this plugin supports
  - `get_language_name(self)` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/plugin.py#L35) — Return the name of the programming language this plugin supports
  - `get_plugin_info(self)` — [`L92`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/plugin.py#L92) — Get information about this plugin
  - `get_supported_queries(self)` — [`L62`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/plugin.py#L62) — Get list of supported query names for this language
  - `get_tree_sitter_language(self)` — [`L50`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/plugin.py#L50) — Load and return TypeScript tree-sitter language
  - `is_applicable(self, file_path: str)` — [`L85`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/plugin.py#L85) — Check if this plugin is applicable for the given file
- protocol/private: `__init__`[`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/plugin.py#L31), `_extractor`[`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/plugin.py#L32), `_language`[`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/plugin.py#L33)
- uses (calls/refs, reference-scoped): [`log_debug`](../../utils/logging.md#log_debug), [`AnalysisResult`](../../models/result.md#AnalysisResult), [`log_error`](../../utils/logging.md#log_error), [`AnalysisRequest`](../../core/request.md#AnalysisRequest), [`elements`](../../models/result.md#AnalysisResult.elements), [`language`](../../models/result.md#AnalysisResult.language), [`CodeElement`](../../models/base.md#CodeElement), [`LanguagePlugin`](../../plugins/base.md#LanguagePlugin), [`file_path`](../../models/result.md#AnalysisResult.file_path), [`success`](../../models/result.md#AnalysisResult.success), [`ElementExtractor`](../../plugins/base.md#ElementExtractor), [`extract_functions`](../../plugins/base.md#ElementExtractor.extract_functions), [`extract_classes`](../../plugins/base.md#ElementExtractor.extract_classes), [`line_count`](../../models/result.md#AnalysisResult.line_count), [`extract_variables`](../../plugins/base.md#ElementExtractor.extract_variables), [`error_message`](../../models/result.md#AnalysisResult.error_message), [`extract_imports`](../../plugins/base.md#ElementExtractor.extract_imports), [`read_file_safe`](../../encoding_utils.md#read_file_safe), [`loader`](../../language_loader.md#loader), [`node_count`](../../models/result.md#AnalysisResult.node_count), [`load_language`](../../language_loader.md#LanguageLoader.load_language), [`TypeScriptElementExtractor`](extractor.md#TypeScriptElementExtractor), [`get_queries`](../../plugins/base.md#LanguagePlugin.get_queries), [`TREE_SITTER_AVAILABLE`](plugin.md#TREE_SITTER_AVAILABLE), [`current_file`](../../plugins/base.md#ElementExtractor.current_file)
- used by: [`LanguagePlugin`](../../plugins/base.md#LanguagePlugin), [`get_language_name`](../../plugins/base.md#LanguagePlugin.get_language_name), [`analyze_file`](../../plugins/base.md#LanguagePlugin.analyze_file), [`get_file_extensions`](../../plugins/base.md#LanguagePlugin.get_file_extensions), [`create_extractor`](../../plugins/base.md#LanguagePlugin.create_extractor), [`get_tree_sitter_language`](../../plugins/base.md#LanguagePlugin.get_tree_sitter_language), [`is_applicable`](../../plugins/base.md#LanguagePlugin.is_applicable), [`execute_query_strategy`](../../plugins/base.md#LanguagePlugin.execute_query_strategy), [`get_plugin_info`](../../plugins/base.md#LanguagePlugin.get_plugin_info), [`get_element_categories`](../../plugins/base.md#LanguagePlugin.get_element_categories)  (16 test-only)

## Module values
- `TREE_SITTER_AVAILABLE` — [`L17`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/plugin.py#L17)

