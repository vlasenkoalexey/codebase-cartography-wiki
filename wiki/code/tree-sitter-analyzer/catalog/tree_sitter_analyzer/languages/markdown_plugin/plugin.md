---
title: 'Module: tree_sitter_analyzer/languages/markdown_plugin/plugin.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/markdown_plugin/plugin.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.markdown_plugin.plugin`/
symbols:
  MarkdownPlugin.analyze_file: MarkdownPlugin#analyze_file().
  MarkdownPlugin.extract_elements: MarkdownPlugin#extract_elements().
  MarkdownPlugin._collect_markdown_elements: MarkdownPlugin#_collect_markdown_elements().
  MarkdownPlugin: MarkdownPlugin#
  MarkdownPlugin._check_markdown_runtime: MarkdownPlugin#_check_markdown_runtime().
  TREE_SITTER_AVAILABLE: TREE_SITTER_AVAILABLE.
  MarkdownPlugin.get_tree_sitter_language: MarkdownPlugin#get_tree_sitter_language().
  MarkdownPlugin.execute_query_strategy: MarkdownPlugin#execute_query_strategy().
  MarkdownPlugin.get_plugin_info: MarkdownPlugin#get_plugin_info().
  MarkdownPlugin.create_extractor: MarkdownPlugin#create_extractor().
  MarkdownPlugin._language_cache: MarkdownPlugin#_language_cache.
  MarkdownPlugin.get_extractor: MarkdownPlugin#get_extractor().
  MarkdownPlugin._extractor: MarkdownPlugin#_extractor.
  MarkdownPlugin.get_language_name: MarkdownPlugin#get_language_name().
  _count_markdown_nodes: _count_markdown_nodes().
  MarkdownPlugin.get_element_categories: MarkdownPlugin#get_element_categories().
  MarkdownPlugin.get_supported_queries: MarkdownPlugin#get_supported_queries().
  MarkdownPlugin.extractor: MarkdownPlugin#extractor.
  MarkdownPlugin.is_applicable: MarkdownPlugin#is_applicable().
  MarkdownPlugin.get_file_extensions: MarkdownPlugin#get_file_extensions().
  MarkdownPlugin.language: MarkdownPlugin#language.
  _MARKDOWN_ELEMENT_CATEGORIES._MARKDOWN_ELEMENT_CATEGORIES: _MARKDOWN_ELEMENT_CATEGORIES._MARKDOWN_ELEMENT_CATEGORIES.
  MarkdownPlugin.__init__: MarkdownPlugin#__init__().
---
# Module: [`tree_sitter_analyzer/languages/markdown_plugin/plugin.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/plugin.py)

## Classes
### `MarkdownPlugin`  ·  implements/extends LanguagePlugin
- def: [`tree_sitter_analyzer/languages/markdown_plugin/plugin.py:108`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/plugin.py#L108)
- doc: Markdown language plugin for the tree-sitter analyzer
- signature: `class MarkdownPlugin(LanguagePlugin):`
- members:
  - `__init__(self)` — [`L111`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/plugin.py#L111) — Initialize the Markdown plugin
  - `_check_markdown_runtime(self, file_path: str)` — [`L279`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/plugin.py#L279) — Return a failure result when tree-sitter / language is unavailable.
  - `_collect_markdown_elements(extractor: Any, tree: tree_sitter.Tree, source_code: str)` — [`L303`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/plugin.py#L303) — Run every markdown-specific extractor and concatenate results.
  - `analyze_file(self, file_path: str, request: AnalysisRequest)` — [`L223`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/plugin.py#L223) — Analyze a Markdown file and return the analysis results. — documented in [tree_sitter_analyzer-models-result](../../../../concepts/tree_sitter_analyzer-models-result.md)
  - `create_extractor(self)` — [`L129`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/plugin.py#L129) — Create and return a NEW element extractor for this language (avoid state pollution)
  - `execute_query_strategy(self, query_key: str | None, language: str)` — [`L367`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/plugin.py#L367) — Execute query strategy for Markdown language
  - `extract_elements(self, tree: tree_sitter.Tree, source_code: str)` — [`L333`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/plugin.py#L333)
  - `get_element_categories(self)` — [`L387`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/plugin.py#L387) — Get Markdown element categories mapping query_key to node_types.
  - `get_extractor(self)` — [`L133`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/plugin.py#L133) — Get the cached extractor instance, creating it if necessary
  - `get_file_extensions(self)` — [`L125`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/plugin.py#L125) — Return list of file extensions this plugin supports
  - `get_language_name(self)` — [`L121`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/plugin.py#L121) — Return the name of the programming language this plugin supports
  - `get_plugin_info(self)` — [`L187`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/plugin.py#L187) — Get information about this plugin
  - `get_supported_queries(self)` — [`L158`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/plugin.py#L158) — Get list of supported query names for this language
  - `get_tree_sitter_language(self)` — [`L137`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/plugin.py#L137) — Get the Tree-sitter language object for Markdown
  - `is_applicable(self, file_path: str)` — [`L180`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/plugin.py#L180) — Check if this plugin is applicable for the given file
  - `extractor` — [`L119`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/plugin.py#L119)
  - `language` — [`L118`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/plugin.py#L118)
- protocol/private: `_extractor`[`L115`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/plugin.py#L115), `_language_cache`[`L114`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/plugin.py#L114)
- uses (calls/refs, reference-scoped): [`AnalysisResult`](../../models/result.md#AnalysisResult), [`log_error`](../../utils/logging.md#log_error), [`AnalysisRequest`](../../core/request.md#AnalysisRequest), [`elements`](../../models/result.md#AnalysisResult.elements), [`language`](../../models/result.md#AnalysisResult.language), [`CodeElement`](../../models/base.md#CodeElement), [`LanguagePlugin`](../../plugins/base.md#LanguagePlugin), [`file_path`](../../models/result.md#AnalysisResult.file_path), [`success`](../../models/result.md#AnalysisResult.success), [`ElementExtractor`](../../plugins/base.md#ElementExtractor), [`line_count`](../../models/result.md#AnalysisResult.line_count), [`error_message`](../../models/result.md#AnalysisResult.error_message), [`source_code`](../../models/result.md#AnalysisResult.source_code), [`read_file_safe`](../../encoding_utils.md#read_file_safe), [`MarkdownElementExtractor`](extractor.md#MarkdownElementExtractor), [`node_count`](../../models/result.md#AnalysisResult.node_count), [`query_results`](../../models/result.md#AnalysisResult.query_results), [`get_queries`](../../plugins/base.md#LanguagePlugin.get_queries), [`extract_images`](public_extraction.md#MarkdownInlineExtractionMixin.extract_images), [`extract_links`](public_extraction.md#MarkdownInlineExtractionMixin.extract_links), [`TREE_SITTER_AVAILABLE`](plugin.md#TREE_SITTER_AVAILABLE), [`extract_blockquotes`](public_extraction.md#MarkdownBlockExtractionMixin.extract_blockquotes), [`extract_references`](public_extraction.md#MarkdownInlineExtractionMixin.extract_references), [`extract_footnotes`](public_extraction.md#MarkdownInlineExtractionMixin.extract_footnotes), [`extract_headers`](public_extraction.md#MarkdownBlockExtractionMixin.extract_headers), [`extract_horizontal_rules`](public_extraction.md#MarkdownBlockExtractionMixin.extract_horizontal_rules), [`extract_html_elements`](public_extraction.md#MarkdownBlockExtractionMixin.extract_html_elements), [`extract_text_formatting`](public_extraction.md#MarkdownInlineExtractionMixin.extract_text_formatting), [`extract_code_blocks`](public_extraction.md#MarkdownBlockExtractionMixin.extract_code_blocks), [`extract_lists`](public_extraction.md#MarkdownBlockExtractionMixin.extract_lists), [`extract_tables`](public_extraction.md#MarkdownBlockExtractionMixin.extract_tables), [`current_file`](../../plugins/base.md#ElementExtractor.current_file), [`_count_markdown_nodes`](plugin.md#_count_markdown_nodes), [`_MARKDOWN_ELEMENT_CATEGORIES`](plugin.md#_MARKDOWN_ELEMENT_CATEGORIES._MARKDOWN_ELEMENT_CATEGORIES)
- used by: [`LanguagePlugin`](../../plugins/base.md#LanguagePlugin), [`get_language_name`](../../plugins/base.md#LanguagePlugin.get_language_name), [`analyze_file`](../../plugins/base.md#LanguagePlugin.analyze_file), [`get_file_extensions`](../../plugins/base.md#LanguagePlugin.get_file_extensions), [`create_extractor`](../../plugins/base.md#LanguagePlugin.create_extractor), [`get_tree_sitter_language`](../../plugins/base.md#LanguagePlugin.get_tree_sitter_language), [`is_applicable`](../../plugins/base.md#LanguagePlugin.is_applicable), [`execute_query_strategy`](../../plugins/base.md#LanguagePlugin.execute_query_strategy), [`get_plugin_info`](../../plugins/base.md#LanguagePlugin.get_plugin_info), [`get_element_categories`](../../plugins/base.md#LanguagePlugin.get_element_categories)  (31 test-only)

## Functions
- `_count_markdown_nodes(node: tree_sitter.Node)` — [`L397`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/plugin.py#L397) — Return the total number of AST nodes under ``node`` (inclusive).

## Module values
- `TREE_SITTER_AVAILABLE` — [`L17`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/plugin.py#L17)
- `_MARKDOWN_ELEMENT_CATEGORIES` — [`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/plugin.py#L39)

