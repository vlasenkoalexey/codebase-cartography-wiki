---
title: 'Module: tree_sitter_analyzer/languages/sql_plugin/plugin.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/sql_plugin/plugin.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.sql_plugin.plugin`/
symbols:
  SQLPlugin.analyze_file: SQLPlugin#analyze_file().
  SQLPlugin: SQLPlugin#
  SQLPlugin.platform_info: SQLPlugin#platform_info.
  TREE_SITTER_AVAILABLE: TREE_SITTER_AVAILABLE.
  SQLPlugin.create_extractor: SQLPlugin#create_extractor().
  SQLPlugin.adapter: SQLPlugin#adapter.
  SQLPlugin.extractor: SQLPlugin#extractor.
  SQLPlugin.extract_elements: SQLPlugin#extract_elements().
  SQLPlugin._cached_language: SQLPlugin#_cached_language.
  SQLPlugin.diagnostic_mode: SQLPlugin#diagnostic_mode.
  SQLPlugin.get_tree_sitter_language: SQLPlugin#get_tree_sitter_language().
  SQLPlugin.supported_extensions: SQLPlugin#supported_extensions.
  SQLPlugin.language: SQLPlugin#language.
  SQLPlugin.get_language_name: SQLPlugin#get_language_name().
  SQLPlugin.get_file_extensions: SQLPlugin#get_file_extensions().
  SQLPlugin.__init__: SQLPlugin#__init__().
---
# Module: [`tree_sitter_analyzer/languages/sql_plugin/plugin.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/plugin.py)

## Classes
### `SQLPlugin`  ·  implements/extends LanguagePlugin
- def: [`tree_sitter_analyzer/languages/sql_plugin/plugin.py:30`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/plugin.py#L30) — documented in [tree_sitter_analyzer-plugins-manager](../../../../concepts/tree_sitter_analyzer-plugins-manager.md)
- doc: SQL language plugin implementation.
- signature: `class SQLPlugin(LanguagePlugin):`
- members:
  - `__init__(self, diagnostic_mode: bool = False)` — [`L43`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/plugin.py#L43) — Initialize the SQL language plugin.
  - `analyze_file(self, file_path: str, request: AnalysisRequest)` — [`L174`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/plugin.py#L174) — Analyze SQL file and return structured results. — documented in [tree_sitter_analyzer-models-result](../../../../concepts/tree_sitter_analyzer-models-result.md)
  - `create_extractor(self)` — [`L132`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/plugin.py#L132) — Create a new element extractor instance.
  - `extract_elements(self, tree: Any, source_code: str)` — [`L141`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/plugin.py#L141) — Legacy method for extracting elements.
  - `get_file_extensions(self)` — [`L128`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/plugin.py#L128) — Get supported file extensions.
  - `get_language_name(self)` — [`L124`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/plugin.py#L124) — Get the language name.
  - `get_tree_sitter_language(self)` — [`L100`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/plugin.py#L100) — Get the tree-sitter language object for SQL.
  - `adapter` — [`L93`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/plugin.py#L93)
  - `diagnostic_mode` — [`L51`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/plugin.py#L51)
  - `extractor` — [`L52`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/plugin.py#L52)
  - `language` — [`L53`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/plugin.py#L53)
  - `platform_info` — [`L58`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/plugin.py#L58)
  - `supported_extensions` — [`L54`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/plugin.py#L54)
- protocol/private: `_cached_language`[`L55`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/plugin.py#L55)
- uses (calls/refs, reference-scoped): [`log_debug`](../../utils/logging.md#log_debug), [`AnalysisResult`](../../models/result.md#AnalysisResult), [`log_error`](../../utils/logging.md#log_error), [`AnalysisRequest`](../../core/request.md#AnalysisRequest), [`elements`](../../models/result.md#AnalysisResult.elements), [`language`](../../models/result.md#AnalysisResult.language), [`LanguagePlugin`](../../plugins/base.md#LanguagePlugin), [`file_path`](../../models/result.md#AnalysisResult.file_path), [`success`](../../models/result.md#AnalysisResult.success), [`Parser`](../../core/parser.md#Parser), [`ElementExtractor`](../../plugins/base.md#ElementExtractor), [`tree`](../../core/parser.md#ParseResult.tree), [`line_count`](../../models/result.md#AnalysisResult.line_count), [`error_message`](../../models/result.md#AnalysisResult.error_message), [`parse_code`](../../core/parser.md#Parser.parse_code), [`source_code`](../../models/result.md#AnalysisResult.source_code), [`success`](../../core/parser.md#ParseResult.success), [`BehaviorProfile`](../../platform_compat/profiles.md#BehaviorProfile), [`node_count`](../../models/result.md#AnalysisResult.node_count), [`SQLElementExtractor`](extractor.md#SQLElementExtractor), [`query_results`](../../models/result.md#AnalysisResult.query_results), [`error_message`](../../core/parser.md#ParseResult.error_message), [`detect`](../../platform_compat/detector.md#PlatformDetector.detect), [`load`](../../platform_compat/profiles.md#BehaviorProfile.load), [`adaptation_rules`](../../platform_compat/profiles.md#BehaviorProfile.adaptation_rules), [`PlatformDetector`](../../platform_compat/detector.md#PlatformDetector), [`CompatibilityAdapter`](../../platform_compat/adapter.md#CompatibilityAdapter), [`set_adapter`](extractor.md#SQLElementExtractor.set_adapter), [`platform_key`](../../platform_compat/detector.md#PlatformInfo.platform_key), [`platform_info`](../../plugins/base.md#ElementExtractor.platform_info)
- used by: [`LanguagePlugin`](../../plugins/base.md#LanguagePlugin), [`get_language_name`](../../plugins/base.md#LanguagePlugin.get_language_name), [`analyze_file`](../../plugins/base.md#LanguagePlugin.analyze_file), [`get_file_extensions`](../../plugins/base.md#LanguagePlugin.get_file_extensions), [`create_extractor`](../../plugins/base.md#LanguagePlugin.create_extractor), [`get_tree_sitter_language`](../../plugins/base.md#LanguagePlugin.get_tree_sitter_language)  (35 test-only)

## Module values
- `TREE_SITTER_AVAILABLE` — [`L17`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/plugin.py#L17)

