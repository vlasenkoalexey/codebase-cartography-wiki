---
title: 'Module: tree_sitter_analyzer/languages/swift_plugin.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/swift_plugin.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.swift_plugin`/
symbols:
  SwiftPlugin: SwiftPlugin#
  SwiftPlugin.analyze_file: SwiftPlugin#analyze_file().
  SwiftPlugin.create_extractor: SwiftPlugin#create_extractor().
  _analysis_result: _analysis_result().
  _analysis_error_result: _analysis_error_result().
  SwiftPlugin.extract_elements: SwiftPlugin#extract_elements().
  _empty_analysis_result: _empty_analysis_result().
  SwiftPlugin.get_tree_sitter_language: SwiftPlugin#get_tree_sitter_language().
  _count_tree_nodes: _count_tree_nodes().
  SwiftPlugin._cached_language: SwiftPlugin#_cached_language.
  _flatten_elements: _flatten_elements().
  _empty_elements: _empty_elements().
  _parse_swift_source: _parse_swift_source().
  SwiftPlugin.supported_extensions: SwiftPlugin#supported_extensions.
  SwiftPlugin.get_file_extensions: SwiftPlugin#get_file_extensions().
  SwiftPlugin.__init__: SwiftPlugin#__init__().
  SwiftPlugin.language: SwiftPlugin#language.
  SwiftPlugin.get_language_name: SwiftPlugin#get_language_name().
---
# Module: [`tree_sitter_analyzer/languages/swift_plugin.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/swift_plugin.py)

## Classes
### `SwiftPlugin`  ·  implements/extends LanguagePlugin
- def: [`tree_sitter_analyzer/languages/swift_plugin.py:24`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/swift_plugin.py#L24) — documented in [tree_sitter_analyzer-plugins-manager](../../../concepts/tree_sitter_analyzer-plugins-manager.md)
- doc: Swift language plugin implementation.
- signature: `class SwiftPlugin(LanguagePlugin):`
- members:
  - `__init__(self)` — [`L27`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/swift_plugin.py#L27) — Initialize the Swift language plugin.
  - `analyze_file(self, file_path: str, request: AnalysisRequest)` — [`L51`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/swift_plugin.py#L51) — documented in [tree_sitter_analyzer-core-request](../../../concepts/tree_sitter_analyzer-core-request.md)
  - `create_extractor(self)` — [`L47`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/swift_plugin.py#L47) — Create a new element extractor instance.
  - `extract_elements(self, tree: Any | None, source_code: str)` — [`L103`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/swift_plugin.py#L103) — Extract all supported Swift elements.
  - `get_file_extensions(self)` — [`L38`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/swift_plugin.py#L38) — Get supported file extensions.
  - `get_language_name(self)` — [`L34`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/swift_plugin.py#L34) — Get the language name.
  - `get_tree_sitter_language(self)` — [`L81`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/swift_plugin.py#L81) — Get the tree-sitter language for Swift.
  - `language` — [`L30`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/swift_plugin.py#L30)
  - `supported_extensions` — [`L31`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/swift_plugin.py#L31)
- protocol/private: `_cached_language`[`L32`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/swift_plugin.py#L32)
- uses (calls/refs, reference-scoped): [`AnalysisResult`](../models/result.md#AnalysisResult), [`log_error`](../utils/logging.md#log_error), [`AnalysisRequest`](../core/request.md#AnalysisRequest), [`elements`](../models/result.md#AnalysisResult.elements), [`language`](../models/result.md#AnalysisResult.language), [`LanguagePlugin`](../plugins/base.md#LanguagePlugin), [`file_path`](../models/result.md#AnalysisResult.file_path), [`ElementExtractor`](../plugins/base.md#ElementExtractor), [`extract_functions`](../plugins/base.md#ElementExtractor.extract_functions), [`extract_classes`](../plugins/base.md#ElementExtractor.extract_classes), [`line_count`](../models/result.md#AnalysisResult.line_count), [`extract_variables`](../plugins/base.md#ElementExtractor.extract_variables), [`extract_imports`](../plugins/base.md#ElementExtractor.extract_imports), [`source_code`](../models/result.md#AnalysisResult.source_code), [`read_file_safe`](../encoding_utils.md#read_file_safe), [`node_count`](../models/result.md#AnalysisResult.node_count), [`_analysis_error_result`](swift_plugin.md#_analysis_error_result), [`_empty_analysis_result`](swift_plugin.md#_empty_analysis_result), [`_count_tree_nodes`](swift_plugin.md#_count_tree_nodes), [`SwiftElementExtractor`](_swift_plugin_extractor.md#SwiftElementExtractor), [`_empty_elements`](swift_plugin.md#_empty_elements), [`_parse_swift_source`](swift_plugin.md#_parse_swift_source)
- used by: [`LanguagePlugin`](../plugins/base.md#LanguagePlugin), [`get_language_name`](../plugins/base.md#LanguagePlugin.get_language_name), [`analyze_file`](../plugins/base.md#LanguagePlugin.analyze_file), [`get_file_extensions`](../plugins/base.md#LanguagePlugin.get_file_extensions), [`create_extractor`](../plugins/base.md#LanguagePlugin.create_extractor), [`get_tree_sitter_language`](../plugins/base.md#LanguagePlugin.get_tree_sitter_language)  (53 test-only)

## Functions
- `_analysis_error_result(file_path: str, message: str)` — [`L174`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/swift_plugin.py#L174)
- `_analysis_result(file_path: str, file_content: str, tree: Any, elements_dict: dict[str, list[Any]])` — [`L156`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/swift_plugin.py#L156)
- `_count_tree_nodes(node: Any)` — [`L188`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/swift_plugin.py#L188)
- `_empty_analysis_result(file_path: str, file_content: str)` — [`L131`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/swift_plugin.py#L131)
- `_empty_elements()` — [`L120`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/swift_plugin.py#L120)
- `_flatten_elements(elements: dict[str, list[Any]])` — [`L124`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/swift_plugin.py#L124)
- `_parse_swift_source(language: Any, file_content: str)` — [`L143`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/swift_plugin.py#L143)

