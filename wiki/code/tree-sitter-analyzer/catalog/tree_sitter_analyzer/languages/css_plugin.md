---
title: 'Module: tree_sitter_analyzer/languages/css_plugin.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/css_plugin.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.css_plugin`/
symbols:
  CssPlugin: CssPlugin#
  CssPlugin.create_extractor: CssPlugin#create_extractor().
  _analyze_css_fallback: _analyze_css_fallback().
  _extract_scss_variables: _extract_scss_variables().
  CssPlugin._analyze_with_tree_sitter: CssPlugin#_analyze_with_tree_sitter().
  _css_error_result: _css_error_result().
  CssPlugin.analyze_file: CssPlugin#analyze_file().
  CssElementExtractor._traverse_for_css_rules: CssElementExtractor#_traverse_for_css_rules().
  CssElementExtractor._create_style_element: CssElementExtractor#_create_style_element().
  CssElementExtractor._classify_rule: CssElementExtractor#_classify_rule().
  CssElementExtractor.extract_css_rules: CssElementExtractor#extract_css_rules().
  CssElementExtractor.property_categories: CssElementExtractor#property_categories.
  CssElementExtractor._extract_node_text: CssElementExtractor#_extract_node_text().
  CssElementExtractor._extract_selector: CssElementExtractor#_extract_selector().
  CssElementExtractor._parse_declaration: CssElementExtractor#_parse_declaration().
  CssElementExtractor._extract_at_rule_name: CssElementExtractor#_extract_at_rule_name().
  CssElementExtractor: CssElementExtractor#
  CssElementExtractor._extract_properties: CssElementExtractor#_extract_properties().
  CssPlugin.execute_query_strategy: CssPlugin#execute_query_strategy().
  CssPlugin.extract_elements: CssPlugin#extract_elements().
  CssPlugin.get_queries: CssPlugin#get_queries().
  CssPlugin.get_tree_sitter_language: CssPlugin#get_tree_sitter_language().
  CssPlugin.extractor: CssPlugin#extractor.
  _SCSS_VAR_RE: _SCSS_VAR_RE.
  _blank_quoted_ranges: _blank_quoted_ranges().
  CssElementExtractor.extract_functions: CssElementExtractor#extract_functions().
  CssElementExtractor.extract_classes: CssElementExtractor#extract_classes().
  CssElementExtractor.extract_variables: CssElementExtractor#extract_variables().
  CssElementExtractor.extract_imports: CssElementExtractor#extract_imports().
  CssElementExtractor._is_css_rule_node: CssElementExtractor#_is_css_rule_node().
  CssPlugin.get_supported_element_types: CssPlugin#get_supported_element_types().
  CssPlugin.get_element_categories: CssPlugin#get_element_categories().
  logger: logger.
  CssElementExtractor.__init__: CssElementExtractor#__init__().
  CssPlugin.__init__: CssPlugin#__init__().
  CssPlugin.get_language_name: CssPlugin#get_language_name().
  CssPlugin.get_file_extensions: CssPlugin#get_file_extensions().
---
# Module: [`tree_sitter_analyzer/languages/css_plugin.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/css_plugin.py)

## Classes
### `CssElementExtractor`  ·  implements/extends ElementExtractor
- def: [`tree_sitter_analyzer/languages/css_plugin.py:170`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/css_plugin.py#L170)
- doc: CSS-specific element extractor using tree-sitter-css
- signature: `class CssElementExtractor(ElementExtractor):`
- members:
  - `_classify_rule(self, properties: dict[str, str])` — [`L301`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/css_plugin.py#L301) — Classify CSS rule based on properties
  - `_create_style_element(self, node: tree_sitter.Node, source_code: str)` — [`L291`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/css_plugin.py#L291) — Create StyleElement from tree-sitter node using tree-sitter-css grammar
  - `_extract_at_rule_name(self, node: tree_sitter.Node, source_code: str)` — [`L333`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/css_plugin.py#L333) — Extract at-rule name from CSS at-rule node
  - `_extract_node_text(self, node: tree_sitter.Node, source_code: str)` — [`L341`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/css_plugin.py#L341) — Extract text content from a tree-sitter node
  - `_extract_properties(self, node: tree_sitter.Node, source_code: str)` — [`L313`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/css_plugin.py#L313) — Extract properties from CSS rule_set node
  - `_extract_selector(self, node: tree_sitter.Node, source_code: str)` — [`L305`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/css_plugin.py#L305) — Extract selector from CSS rule_set node
  - `_is_css_rule_node(self, node_type: str)` — [`L275`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/css_plugin.py#L275) — Check if a node type represents a CSS rule in tree-sitter-css grammar
  - `_parse_declaration(self, decl_node: tree_sitter.Node, source_code: str)` — [`L323`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/css_plugin.py#L323) — Parse individual CSS declaration
  - `_traverse_for_css_rules(self, node: tree_sitter.Node, elements: list[StyleElement], source_code: str)` — [`L258`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/css_plugin.py#L258) — Traverse tree to find CSS rules using tree-sitter-css grammar
  - `extract_classes(self, tree: tree_sitter.Tree, source_code: str)` — [`L232`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/css_plugin.py#L232) — CSS doesn't have classes in the traditional sense, return empty list
  - `extract_css_rules(self, tree: tree_sitter.Tree, source_code: str)` — [`L244`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/css_plugin.py#L244) — Extract CSS rules using tree-sitter-css parser
  - `extract_functions(self, tree: tree_sitter.Tree, source_code: str)` — [`L228`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/css_plugin.py#L228) — CSS doesn't have functions in the traditional sense, return empty list
  - `extract_imports(self, tree: tree_sitter.Tree, source_code: str)` — [`L240`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/css_plugin.py#L240) — CSS doesn't have imports in the traditional sense, return empty list
  - `extract_variables(self, tree: tree_sitter.Tree, source_code: str)` — [`L236`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/css_plugin.py#L236) — CSS doesn't have variables (except custom properties), return empty list
  - `property_categories` — [`L174`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/css_plugin.py#L174)
- protocol/private: `__init__`[`L173`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/css_plugin.py#L173)
- uses (calls/refs, reference-scoped): [`log_debug`](../utils/logging.md#log_debug), [`log_error`](../utils/logging.md#log_error), [`ElementExtractor`](../plugins/base.md#ElementExtractor), [`StyleElement`](../models/markup_models.md#StyleElement), [`create_style_element`](css_helpers.md#create_style_element), [`extract_css_properties`](css_helpers.md#extract_css_properties), [`classify_rule`](css_helpers.md#classify_rule), [`extract_at_rule_name`](css_helpers.md#extract_at_rule_name), [`extract_css_selector`](css_helpers.md#extract_css_selector), [`parse_declaration`](css_helpers.md#parse_declaration)
- used by: [`ElementExtractor`](../plugins/base.md#ElementExtractor), [`extract_functions`](../plugins/base.md#ElementExtractor.extract_functions), [`extract_classes`](../plugins/base.md#ElementExtractor.extract_classes), [`extract_variables`](../plugins/base.md#ElementExtractor.extract_variables), [`extract_imports`](../plugins/base.md#ElementExtractor.extract_imports), [`extract_css_rules`](../plugins/base.md#ElementExtractor.extract_css_rules), [`create_extractor`](css_plugin.md#CssPlugin.create_extractor), [`extractor`](css_plugin.md#CssPlugin.extractor)  (23 test-only)

### `CssPlugin`  ·  implements/extends LanguagePlugin
- def: [`tree_sitter_analyzer/languages/css_plugin.py:354`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/css_plugin.py#L354) — documented in [tree_sitter_analyzer-plugins-base](../../../concepts/tree_sitter_analyzer-plugins-base.md)
- doc: CSS language plugin using tree-sitter-css for true CSS parsing
- signature: `class CssPlugin(LanguagePlugin):`
- members:
  - `__init__(self)` — [`L357`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/css_plugin.py#L357) — Initialize CSS plugin with extractor.
  - `_analyze_with_tree_sitter(self, file_path: str, content: str)` — [`L445`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/css_plugin.py#L445) — Parse via ``tree-sitter-css``; may raise ``ImportError`` if missing. — documented in [tree_sitter_analyzer-models-result](../../../concepts/tree_sitter_analyzer-models-result.md)
  - `analyze_file(self, file_path: str, request: AnalysisRequest)` — [`L418`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/css_plugin.py#L418) — Analyze CSS file using tree-sitter-css parser.
  - `create_extractor(self)` — [`L368`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/css_plugin.py#L368) — documented in [tree_sitter_analyzer-plugins-base](../../../concepts/tree_sitter_analyzer-plugins-base.md)
  - `execute_query_strategy(self, query_key: str | None, language: str)` — [`L387`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/css_plugin.py#L387) — Execute query strategy for CSS
  - `extract_elements(self, tree: tree_sitter.Tree, source_code: str)` — [`L412`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/css_plugin.py#L412) — Unified extraction entry point — delegates to the extractor.
  - `get_element_categories(self)` — [`L397`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/css_plugin.py#L397) — Return CSS element categories for query execution
  - `get_file_extensions(self)` — [`L365`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/css_plugin.py#L365)
  - `get_language_name(self)` — [`L362`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/css_plugin.py#L362)
  - `get_queries(self)` — [`L381`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/css_plugin.py#L381) — Return CSS-specific tree-sitter queries
  - `get_supported_element_types(self)` — [`L378`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/css_plugin.py#L378)
  - `get_tree_sitter_language(self)` — [`L371`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/css_plugin.py#L371) — Get tree-sitter language object for CSS.
  - `extractor` — [`L360`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/css_plugin.py#L360)
- uses (calls/refs, reference-scoped): [`AnalysisResult`](../models/result.md#AnalysisResult), [`log_error`](../utils/logging.md#log_error), [`AnalysisRequest`](../core/request.md#AnalysisRequest), [`elements`](../models/result.md#AnalysisResult.elements), [`language`](../models/result.md#AnalysisResult.language), [`LanguagePlugin`](../plugins/base.md#LanguagePlugin), [`file_path`](../models/result.md#AnalysisResult.file_path), [`success`](../models/result.md#AnalysisResult.success), [`ElementExtractor`](../plugins/base.md#ElementExtractor), [`CSS_QUERIES`](../queries/css.md#CSS_QUERIES.CSS_QUERIES), [`line_count`](../models/result.md#AnalysisResult.line_count), [`error_message`](../models/result.md#AnalysisResult.error_message), [`source_code`](../models/result.md#AnalysisResult.source_code), [`log_info`](../utils/logging.md#log_info), [`extract_css_rules`](../plugins/base.md#ElementExtractor.extract_css_rules), [`read_file_safe`](../encoding_utils.md#read_file_safe), [`node_count`](../models/result.md#AnalysisResult.node_count), [`_analyze_css_fallback`](css_plugin.md#_analyze_css_fallback), [`_extract_scss_variables`](css_plugin.md#_extract_scss_variables), [`extract_elements`](../plugins/base.md#ElementExtractor.extract_elements), [`query_results`](../models/result.md#AnalysisResult.query_results), [`_css_error_result`](css_plugin.md#_css_error_result), [`CssElementExtractor`](css_plugin.md#CssElementExtractor)
- used by: [`LanguagePlugin`](../plugins/base.md#LanguagePlugin), [`get_language_name`](../plugins/base.md#LanguagePlugin.get_language_name), [`analyze_file`](../plugins/base.md#LanguagePlugin.analyze_file), [`get_file_extensions`](../plugins/base.md#LanguagePlugin.get_file_extensions), [`create_extractor`](../plugins/base.md#LanguagePlugin.create_extractor), [`get_tree_sitter_language`](../plugins/base.md#LanguagePlugin.get_tree_sitter_language), [`execute_query_strategy`](../plugins/base.md#LanguagePlugin.execute_query_strategy), [`get_queries`](../plugins/base.md#LanguagePlugin.get_queries), [`get_element_categories`](../plugins/base.md#LanguagePlugin.get_element_categories), [`get_supported_element_types`](../plugins/base.md#LanguagePlugin.get_supported_element_types)  (79 test-only)

## Functions
- `_analyze_css_fallback(file_path: str, content: str)` — [`L138`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/css_plugin.py#L138) — Best-effort fallback when ``tree-sitter-css`` is not installed. — documented in [tree_sitter_analyzer-models-base](../../../concepts/tree_sitter_analyzer-models-base.md)
- `_blank_quoted_ranges(line: str)` — [`L39`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/css_plugin.py#L39) — Replace the contents of quoted strings with spaces (markers excluded).
- `_css_error_result(file_path: str, exc: Exception)` — [`L123`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/css_plugin.py#L123) — Build the canonical failure ``AnalysisResult`` for CSS parse errors.
- `_extract_scss_variables(file_path: str, content: str)` — [`L67`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/css_plugin.py#L67) — Return a ``Variable`` element for every SCSS ``$variable`` declaration.

## Module values
- `_SCSS_VAR_RE` — [`L36`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/css_plugin.py#L36)
- `logger` — [`L32`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/css_plugin.py#L32)

