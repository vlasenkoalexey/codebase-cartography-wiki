---
title: 'Module: tree_sitter_analyzer/languages/html_plugin.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/html_plugin.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.html_plugin`/
symbols:
  HtmlPlugin: HtmlPlugin#
  HtmlPlugin.create_extractor: HtmlPlugin#create_extractor().
  _analyze_html_fallback: _analyze_html_fallback().
  HtmlPlugin._analyze_with_tree_sitter: HtmlPlugin#_analyze_with_tree_sitter().
  _html_error_result: _html_error_result().
  HtmlPlugin.analyze_file: HtmlPlugin#analyze_file().
  HtmlElementExtractor._traverse_for_html_elements: HtmlElementExtractor#_traverse_for_html_elements().
  HtmlElementExtractor._classify_element: HtmlElementExtractor#_classify_element().
  HtmlElementExtractor._try_create_html_element: HtmlElementExtractor#_try_create_html_element().
  HtmlElementExtractor._create_markup_element: HtmlElementExtractor#_create_markup_element().
  HtmlElementExtractor: HtmlElementExtractor#
  HtmlElementExtractor.extract_html_elements: HtmlElementExtractor#extract_html_elements().
  HtmlElementExtractor._extract_node_text: HtmlElementExtractor#_extract_node_text().
  HtmlElementExtractor.element_categories: HtmlElementExtractor#element_categories.
  HtmlElementExtractor._extract_tag_name: HtmlElementExtractor#_extract_tag_name().
  HtmlElementExtractor._extract_attributes: HtmlElementExtractor#_extract_attributes().
  HtmlElementExtractor._parse_attribute: HtmlElementExtractor#_parse_attribute().
  HtmlPlugin.extract_elements: HtmlPlugin#extract_elements().
  HtmlPlugin.get_queries: HtmlPlugin#get_queries().
  HtmlPlugin.execute_query_strategy: HtmlPlugin#execute_query_strategy().
  HtmlPlugin.get_tree_sitter_language: HtmlPlugin#get_tree_sitter_language().
  HtmlElementExtractor.extract_functions: HtmlElementExtractor#extract_functions().
  HtmlElementExtractor.extract_classes: HtmlElementExtractor#extract_classes().
  HtmlElementExtractor.extract_variables: HtmlElementExtractor#extract_variables().
  HtmlElementExtractor.extract_imports: HtmlElementExtractor#extract_imports().
  HtmlElementExtractor._is_html_element_node: HtmlElementExtractor#_is_html_element_node().
  HtmlPlugin.get_supported_element_types: HtmlPlugin#get_supported_element_types().
  HtmlPlugin.get_element_categories: HtmlPlugin#get_element_categories().
  logger: logger.
  HtmlElementExtractor.__init__: HtmlElementExtractor#__init__().
  HtmlPlugin.get_language_name: HtmlPlugin#get_language_name().
  HtmlPlugin.get_file_extensions: HtmlPlugin#get_file_extensions().
---
# Module: [`tree_sitter_analyzer/languages/html_plugin.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/html_plugin.py)

## Classes
### `HtmlElementExtractor`  ·  implements/extends ElementExtractor
- def: [`tree_sitter_analyzer/languages/html_plugin.py:82`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/html_plugin.py#L82)
- doc: HTML-specific element extractor using tree-sitter-html
- signature: `class HtmlElementExtractor(ElementExtractor):`
- members:
  - `_classify_element(self, tag_name: str)` — [`L278`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/html_plugin.py#L278) — Classify HTML element based on tag name
  - `_create_markup_element(self, node: tree_sitter.Node, source_code: str, parent: MarkupElement | None)` — [`L264`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/html_plugin.py#L264) — Create MarkupElement from tree-sitter node using tree-sitter-html grammar
  - `_extract_attributes(self, node: tree_sitter.Node, source_code: str)` — [`L290`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/html_plugin.py#L290) — Extract attributes from HTML element node
  - `_extract_node_text(self, node: tree_sitter.Node, source_code: str)` — [`L310`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/html_plugin.py#L310) — Extract text content from a tree-sitter node
  - `_extract_tag_name(self, node: tree_sitter.Node, source_code: str)` — [`L282`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/html_plugin.py#L282) — Extract tag name from HTML element node
  - `_is_html_element_node(self, node_type: str)` — [`L251`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/html_plugin.py#L251) — Check if a node type represents an HTML element in tree-sitter-html grammar
  - `_parse_attribute(self, attr_node: tree_sitter.Node, source_code: str)` — [`L300`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/html_plugin.py#L300) — Parse individual attribute node
  - `_traverse_for_html_elements(self, node: tree_sitter.Node, elements: list[MarkupElement], source_code: str, parent: MarkupElement | None)` — [`L196`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/html_plugin.py#L196) — Traverse tree to find HTML elements using tree-sitter-html grammar.
  - `_try_create_html_element(self, node: tree_sitter.Node, elements: list[MarkupElement], source_code: str, parent: MarkupElement | None)` — [`L218`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/html_plugin.py#L218) — Create a MarkupElement for ``node`` and recurse with it as parent.
  - `extract_classes(self, tree: tree_sitter.Tree, source_code: str)` — [`L168`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/html_plugin.py#L168) — HTML doesn't have classes in the traditional sense, return empty list
  - `extract_functions(self, tree: tree_sitter.Tree, source_code: str)` — [`L164`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/html_plugin.py#L164) — HTML doesn't have functions, return empty list
  - `extract_html_elements(self, tree: tree_sitter.Tree, source_code: str)` — [`L180`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/html_plugin.py#L180) — Extract HTML elements using tree-sitter-html parser
  - `extract_imports(self, tree: tree_sitter.Tree, source_code: str)` — [`L176`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/html_plugin.py#L176) — HTML doesn't have imports, return empty list
  - `extract_variables(self, tree: tree_sitter.Tree, source_code: str)` — [`L172`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/html_plugin.py#L172) — HTML doesn't have variables, return empty list
  - `element_categories` — [`L86`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/html_plugin.py#L86)
- protocol/private: `__init__`[`L85`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/html_plugin.py#L85)
- uses (calls/refs, reference-scoped): [`log_debug`](../utils/logging.md#log_debug), [`log_error`](../utils/logging.md#log_error), [`ElementExtractor`](../plugins/base.md#ElementExtractor), [`MarkupElement`](../models/markup_models.md#MarkupElement), [`create_markup_element`](html_helpers.md#create_markup_element), [`extract_html_tag_name`](html_helpers.md#extract_html_tag_name), [`parse_attribute`](html_helpers.md#parse_attribute), [`extract_html_attributes`](html_helpers.md#extract_html_attributes), [`classify_element`](html_helpers.md#classify_element)
- used by: [`ElementExtractor`](../plugins/base.md#ElementExtractor), [`extract_functions`](../plugins/base.md#ElementExtractor.extract_functions), [`extract_classes`](../plugins/base.md#ElementExtractor.extract_classes), [`extract_variables`](../plugins/base.md#ElementExtractor.extract_variables), [`create_extractor`](html_plugin.md#HtmlPlugin.create_extractor), [`extract_imports`](../plugins/base.md#ElementExtractor.extract_imports), [`extract_html_elements`](../plugins/base.md#ElementExtractor.extract_html_elements)  (9 test-only)

### `HtmlPlugin`  ·  implements/extends LanguagePlugin
- def: [`tree_sitter_analyzer/languages/html_plugin.py:323`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/html_plugin.py#L323) — documented in [tree_sitter_analyzer-plugins-base](../../../concepts/tree_sitter_analyzer-plugins-base.md)
- doc: HTML language plugin using tree-sitter-html for true HTML parsing
- signature: `class HtmlPlugin(LanguagePlugin):`
- members:
  - `_analyze_with_tree_sitter(self, file_path: str, content: str)` — [`L407`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/html_plugin.py#L407) — Parse via ``tree-sitter-html``; may raise ``ImportError`` if missing. — documented in [tree_sitter_analyzer-models-result](../../../concepts/tree_sitter_analyzer-models-result.md)
  - `analyze_file(self, file_path: str, request: AnalysisRequest)` — [`L380`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/html_plugin.py#L380) — Analyze HTML file using tree-sitter-html parser.
  - `create_extractor(self)` — [`L332`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/html_plugin.py#L332) — documented in [tree_sitter_analyzer-plugins-base](../../../concepts/tree_sitter_analyzer-plugins-base.md)
  - `execute_query_strategy(self, query_key: str | None, language: str)` — [`L351`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/html_plugin.py#L351) — Execute query strategy for HTML
  - `extract_elements(self, tree: tree_sitter.Tree, source_code: str)` — [`L374`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/html_plugin.py#L374) — Unified extraction entry point — delegates to the extractor.
  - `get_element_categories(self)` — [`L361`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/html_plugin.py#L361) — Return HTML element categories for query execution
  - `get_file_extensions(self)` — [`L329`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/html_plugin.py#L329)
  - `get_language_name(self)` — [`L326`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/html_plugin.py#L326)
  - `get_queries(self)` — [`L345`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/html_plugin.py#L345) — Return HTML-specific tree-sitter queries
  - `get_supported_element_types(self)` — [`L342`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/html_plugin.py#L342)
  - `get_tree_sitter_language(self)` — [`L335`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/html_plugin.py#L335) — Get tree-sitter language object for HTML.
- uses (calls/refs, reference-scoped): [`AnalysisResult`](../models/result.md#AnalysisResult), [`log_error`](../utils/logging.md#log_error), [`AnalysisRequest`](../core/request.md#AnalysisRequest), [`elements`](../models/result.md#AnalysisResult.elements), [`language`](../models/result.md#AnalysisResult.language), [`LanguagePlugin`](../plugins/base.md#LanguagePlugin), [`file_path`](../models/result.md#AnalysisResult.file_path), [`success`](../models/result.md#AnalysisResult.success), [`ElementExtractor`](../plugins/base.md#ElementExtractor), [`line_count`](../models/result.md#AnalysisResult.line_count), [`error_message`](../models/result.md#AnalysisResult.error_message), [`extract_html_elements`](../plugins/base.md#ElementExtractor.extract_html_elements), [`HTML_QUERIES`](../queries/html.md#HTML_QUERIES.HTML_QUERIES), [`source_code`](../models/result.md#AnalysisResult.source_code), [`log_info`](../utils/logging.md#log_info), [`read_file_safe`](../encoding_utils.md#read_file_safe), [`node_count`](../models/result.md#AnalysisResult.node_count), [`_analyze_html_fallback`](html_plugin.md#_analyze_html_fallback), [`extract_elements`](../plugins/base.md#ElementExtractor.extract_elements), [`query_results`](../models/result.md#AnalysisResult.query_results), [`_html_error_result`](html_plugin.md#_html_error_result), [`HtmlElementExtractor`](html_plugin.md#HtmlElementExtractor)
- used by: [`LanguagePlugin`](../plugins/base.md#LanguagePlugin), [`get_language_name`](../plugins/base.md#LanguagePlugin.get_language_name), [`analyze_file`](../plugins/base.md#LanguagePlugin.analyze_file), [`get_file_extensions`](../plugins/base.md#LanguagePlugin.get_file_extensions), [`create_extractor`](../plugins/base.md#LanguagePlugin.create_extractor), [`get_tree_sitter_language`](../plugins/base.md#LanguagePlugin.get_tree_sitter_language), [`execute_query_strategy`](../plugins/base.md#LanguagePlugin.execute_query_strategy), [`get_queries`](../plugins/base.md#LanguagePlugin.get_queries), [`get_element_categories`](../plugins/base.md#LanguagePlugin.get_element_categories), [`get_supported_element_types`](../plugins/base.md#LanguagePlugin.get_supported_element_types)  (100 test-only)

## Functions
- `_analyze_html_fallback(file_path: str, content: str)` — [`L48`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/html_plugin.py#L48) — Best-effort fallback when ``tree-sitter-html`` is not installed. — documented in [tree_sitter_analyzer-models-base](../../../concepts/tree_sitter_analyzer-models-base.md)
- `_html_error_result(file_path: str, exc: Exception)` — [`L33`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/html_plugin.py#L33) — Build the canonical failure ``AnalysisResult`` for HTML parse errors.

## Module values
- `logger` — [`L30`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/html_plugin.py#L30)

