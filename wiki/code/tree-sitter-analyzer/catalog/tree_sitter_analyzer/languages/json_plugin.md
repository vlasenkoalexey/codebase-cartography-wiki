---
title: 'Module: tree_sitter_analyzer/languages/json_plugin.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/json_plugin.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.json_plugin`/
symbols:
  JSONPlugin.analyze_file: JSONPlugin#analyze_file().
  JSONElementExtractor.extract_json_elements: JSONElementExtractor#extract_json_elements().
  JSONElementExtractor._extract_elements_by_type: JSONElementExtractor#_extract_elements_by_type().
  JSONElement: JSONElement#
  JSONElementExtractor._get_node_text: JSONElementExtractor#_get_node_text().
  JSONPlugin: JSONPlugin#
  JSONPlugin.create_extractor: JSONPlugin#create_extractor().
  JSONElementExtractor._extract_pair: JSONElementExtractor#_extract_pair().
  JSONElementExtractor._extract_boolean: JSONElementExtractor#_extract_boolean().
  JSONElementExtractor._extract_object: JSONElementExtractor#_extract_object().
  JSONElementExtractor._extract_array: JSONElementExtractor#_extract_array().
  JSONElementExtractor._extract_string: JSONElementExtractor#_extract_string().
  JSONElementExtractor._extract_number: JSONElementExtractor#_extract_number().
  JSONElementExtractor._extract_null: JSONElementExtractor#_extract_null().
  JSON_PARSER: JSON_PARSER.
  JSONElementExtractor._calculate_nesting_level: JSONElementExtractor#_calculate_nesting_level().
  _JSON_PARSER_LOCK: _JSON_PARSER_LOCK.
  JSONPlugin.get_tree_sitter_language: JSONPlugin#get_tree_sitter_language().
  JSONElementExtractor: JSONElementExtractor#
  JSONPlugin.extract_elements: JSONPlugin#extract_elements().
  JSONElementExtractor.extract_elements: JSONElementExtractor#extract_elements().
  JSONElementExtractor._traverse_nodes: JSONElementExtractor#_traverse_nodes().
  JSONElementExtractor._node_text_cache: JSONElementExtractor#_node_text_cache.
  JSONElementExtractor._extract_value_info: JSONElementExtractor#_extract_value_info().
  JSON_AVAILABLE: JSON_AVAILABLE.
  JSONElementExtractor.source_code: JSONElementExtractor#source_code.
  JSONElement.__init__: JSONElement#__init__().
  JSONElementExtractor.extract_functions: JSONElementExtractor#extract_functions().
  JSONElementExtractor.extract_classes: JSONElementExtractor#extract_classes().
  JSONElementExtractor.extract_variables: JSONElementExtractor#extract_variables().
  JSONElementExtractor.extract_imports: JSONElementExtractor#extract_imports().
  JSONPlugin.extractor: JSONPlugin#extractor.
  JSONPlugin.execute_query_strategy: JSONPlugin#execute_query_strategy().
  JSON_LANGUAGE: JSON_LANGUAGE.
  JSONElementExtractor.content_lines: JSONElementExtractor#content_lines.
  JSONPlugin.get_language_name: JSONPlugin#get_language_name().
  JSONPlugin.get_file_extensions: JSONPlugin#get_file_extensions().
  JSONPlugin.get_queries: JSONPlugin#get_queries().
  logger: logger.
  JSONElement.key: JSONElement#key.
  JSONElement.value: JSONElement#value.
  JSONElement.value_type: JSONElement#value_type.
  JSONElement.nesting_level: JSONElement#nesting_level.
  JSONElement.child_count: JSONElement#child_count.
  JSONElementExtractor.__init__: JSONElementExtractor#__init__().
  JSONPlugin.__init__: JSONPlugin#__init__().
  JSONPlugin.get_supported_element_types: JSONPlugin#get_supported_element_types().
  JSONPlugin.get_element_categories: JSONPlugin#get_element_categories().
---
# Module: [`tree_sitter_analyzer/languages/json_plugin.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/json_plugin.py)

## Classes
### `JSONElement`  ·  implements/extends CodeElement
- def: [`tree_sitter_analyzer/languages/json_plugin.py:43`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/json_plugin.py#L43)
- doc: JSON-specific code element.
- signature: `class JSONElement(CodeElement):`
- members:
  - `__init__(self, name: str, start_line: int, end_line: int, raw_text: str, language: str = "json", element_type: str = "json", key: str | None = None, value: str | None = None, value_type: str | None = None, nesting_level: int = 0, child_count: int | None = None, **kwargs: Any)` — [`L46`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/json_plugin.py#L46) — Initialize JSONElement.
  - `child_count` — [`L92`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/json_plugin.py#L92)
  - `key` — [`L88`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/json_plugin.py#L88)
  - `nesting_level` — [`L91`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/json_plugin.py#L91)
  - `value` — [`L89`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/json_plugin.py#L89)
  - `value_type` — [`L90`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/json_plugin.py#L90)
- uses (calls/refs, reference-scoped): [`CodeElement`](../models/base.md#CodeElement), [`element_type`](../models/base.md#CodeElement.element_type)
- used by: [`CodeElement`](../models/base.md#CodeElement), [`extract_json_elements`](json_plugin.md#JSONElementExtractor.extract_json_elements), [`_extract_elements_by_type`](json_plugin.md#JSONElementExtractor._extract_elements_by_type), [`_extract_pair`](json_plugin.md#JSONElementExtractor._extract_pair), [`_extract_boolean`](json_plugin.md#JSONElementExtractor._extract_boolean), [`_extract_array`](json_plugin.md#JSONElementExtractor._extract_array), [`_extract_null`](json_plugin.md#JSONElementExtractor._extract_null), [`_extract_number`](json_plugin.md#JSONElementExtractor._extract_number), [`_extract_object`](json_plugin.md#JSONElementExtractor._extract_object), [`_extract_string`](json_plugin.md#JSONElementExtractor._extract_string)

### `JSONElementExtractor`  ·  implements/extends ElementExtractor
- def: [`tree_sitter_analyzer/languages/json_plugin.py:95`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/json_plugin.py#L95)
- doc: JSON-specific element extractor using tree-sitter-json.
- signature: `class JSONElementExtractor(ElementExtractor):`
- members:
  - `__init__(self)` — [`L98`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/json_plugin.py#L98) — Initialize the JSON element extractor.
  - `_calculate_nesting_level(self, node: tree_sitter.Node)` — [`L184`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/json_plugin.py#L184) — Calculate AST-based logical nesting level.
  - `_extract_array(self, node: tree_sitter.Node, elements: list[JSONElement])` — [`L256`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/json_plugin.py#L256) — Extract JSON array.
  - `_extract_boolean(self, node: tree_sitter.Node, elements: list[JSONElement], bool_value: bool)` — [`L405`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/json_plugin.py#L405) — Extract JSON boolean.
  - `_extract_elements_by_type(self, root_node: tree_sitter.Node, elements: list[JSONElement])` — [`L203`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/json_plugin.py#L203) — Extract all JSON elements by traversing the tree.
  - `_extract_null(self, node: tree_sitter.Node, elements: list[JSONElement])` — [`L431`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/json_plugin.py#L431) — Extract JSON null.
  - `_extract_number(self, node: tree_sitter.Node, elements: list[JSONElement])` — [`L379`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/json_plugin.py#L379) — Extract JSON number.
  - `_extract_object(self, node: tree_sitter.Node, elements: list[JSONElement])` — [`L228`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/json_plugin.py#L228) — Extract JSON object.
  - `_extract_pair(self, node: tree_sitter.Node, elements: list[JSONElement])` — [`L286`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/json_plugin.py#L286) — Extract JSON key-value pair.
  - `_extract_string(self, node: tree_sitter.Node, elements: list[JSONElement])` — [`L343`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/json_plugin.py#L343) — Extract JSON string.
  - `_extract_value_info(self, node: tree_sitter.Node | None)` — [`L456`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/json_plugin.py#L456) — Extract value information from a node.
  - `_get_node_text(self, node: tree_sitter.Node)` — [`L166`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/json_plugin.py#L166) — Get text content from a tree-sitter node.
  - `_traverse_nodes(self, node: tree_sitter.Node)` — [`L196`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/json_plugin.py#L196) — Traverse all nodes in the tree.
  - `extract_classes(self, tree: tree_sitter.Tree, source_code: str)` — [`L110`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/json_plugin.py#L110) — JSON doesn't have classes, return empty list.
  - `extract_elements(self, tree: tree_sitter.Tree | None, source_code: str)` — [`L154`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/json_plugin.py#L154) — Return JSON elements grouped under the ``json_elements`` key.
  - `extract_functions(self, tree: tree_sitter.Tree, source_code: str)` — [`L104`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/json_plugin.py#L104) — JSON doesn't have functions, return empty list.
  - `extract_imports(self, tree: tree_sitter.Tree, source_code: str)` — [`L120`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/json_plugin.py#L120) — JSON doesn't have imports, return empty list.
  - `extract_json_elements(self, tree: tree_sitter.Tree | None, source_code: str)` — [`L124`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/json_plugin.py#L124) — Extract all JSON elements from the parsed tree.
  - `extract_variables(self, tree: tree_sitter.Tree, source_code: str)` — [`L114`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/json_plugin.py#L114) — JSON doesn't have variables, return empty list.
  - `content_lines` — [`L101`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/json_plugin.py#L101)
  - `source_code` — [`L100`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/json_plugin.py#L100)
- protocol/private: `_node_text_cache`[`L102`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/json_plugin.py#L102)
- uses (calls/refs, reference-scoped): [`log_debug`](../utils/logging.md#log_debug), [`Function`](../models/base.md#Function), [`log_error`](../utils/logging.md#log_error), [`Class`](../models/base.md#Class), [`Variable`](../models/base.md#Variable), [`Import`](../models/base.md#Import), [`ElementExtractor`](../plugins/base.md#ElementExtractor), [`JSONElement`](json_plugin.md#JSONElement)
- used by: [`ElementExtractor`](../plugins/base.md#ElementExtractor), [`extract_functions`](../plugins/base.md#ElementExtractor.extract_functions), [`extract_classes`](../plugins/base.md#ElementExtractor.extract_classes), [`extract_variables`](../plugins/base.md#ElementExtractor.extract_variables), [`extract_imports`](../plugins/base.md#ElementExtractor.extract_imports), [`analyze_file`](json_plugin.md#JSONPlugin.analyze_file), [`extract_elements`](../plugins/base.md#ElementExtractor.extract_elements), [`create_extractor`](json_plugin.md#JSONPlugin.create_extractor), [`extract_elements`](json_plugin.md#JSONPlugin.extract_elements), [`extractor`](json_plugin.md#JSONPlugin.extractor)  (7 test-only)

### `JSONPlugin`  ·  implements/extends LanguagePlugin
- def: [`tree_sitter_analyzer/languages/json_plugin.py:492`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/json_plugin.py#L492)
- doc: JSON language plugin using tree-sitter-json for true JSON parsing.
- signature: `class JSONPlugin(LanguagePlugin):`
- members:
  - `__init__(self)` — [`L495`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/json_plugin.py#L495) — Initialize JSON plugin with extractor.
  - `analyze_file(self, file_path: str, request: AnalysisRequest)` — [`L560`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/json_plugin.py#L560) — Analyze JSON file using tree-sitter-json parser. — documented in [tree_sitter_analyzer-models-result](../../../concepts/tree_sitter_analyzer-models-result.md)
  - `create_extractor(self)` — [`L508`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/json_plugin.py#L508) — Create and return a JSON element extractor.
  - `execute_query_strategy(self, query_key: str | None, language: str)` — [`L536`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/json_plugin.py#L536) — Execute query strategy for JSON.
  - `extract_elements(self, tree: tree_sitter.Tree, source_code: str)` — [`L554`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/json_plugin.py#L554) — Unified extraction entry point — delegates to the extractor.
  - `get_element_categories(self)` — [`L546`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/json_plugin.py#L546) — Return JSON element categories for query execution.
  - `get_file_extensions(self)` — [`L504`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/json_plugin.py#L504) — Return supported file extensions.
  - `get_language_name(self)` — [`L500`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/json_plugin.py#L500) — Return the language name.
  - `get_queries(self)` — [`L531`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/json_plugin.py#L531) — Return JSON-specific tree-sitter queries.
  - `get_supported_element_types(self)` — [`L518`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/json_plugin.py#L518) — Return supported element types.
  - `get_tree_sitter_language(self)` — [`L512`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/json_plugin.py#L512) — Get tree-sitter language object for JSON.
  - `extractor` — [`L498`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/json_plugin.py#L498)
- uses (calls/refs, reference-scoped): [`AnalysisResult`](../models/result.md#AnalysisResult), [`log_error`](../utils/logging.md#log_error), [`AnalysisRequest`](../core/request.md#AnalysisRequest), [`elements`](../models/result.md#AnalysisResult.elements), [`language`](../models/result.md#AnalysisResult.language), [`LanguagePlugin`](../plugins/base.md#LanguagePlugin), [`file_path`](../models/result.md#AnalysisResult.file_path), [`success`](../models/result.md#AnalysisResult.success), [`line_count`](../models/result.md#AnalysisResult.line_count), [`error_message`](../models/result.md#AnalysisResult.error_message), [`source_code`](../models/result.md#AnalysisResult.source_code), [`log_info`](../utils/logging.md#log_info), [`read_file_safe`](../encoding_utils.md#read_file_safe), [`node_count`](../models/result.md#AnalysisResult.node_count), [`query_results`](../models/result.md#AnalysisResult.query_results), [`extract_json_elements`](json_plugin.md#JSONElementExtractor.extract_json_elements), [`JSON_PARSER`](json_plugin.md#JSON_PARSER), [`_JSON_PARSER_LOCK`](json_plugin.md#_JSON_PARSER_LOCK), [`JSONElementExtractor`](json_plugin.md#JSONElementExtractor), [`extract_elements`](json_plugin.md#JSONElementExtractor.extract_elements), [`JSON_AVAILABLE`](json_plugin.md#JSON_AVAILABLE), [`JSON_LANGUAGE`](json_plugin.md#JSON_LANGUAGE)
- used by: [`LanguagePlugin`](../plugins/base.md#LanguagePlugin), [`get_language_name`](../plugins/base.md#LanguagePlugin.get_language_name), [`analyze_file`](../plugins/base.md#LanguagePlugin.analyze_file), [`get_file_extensions`](../plugins/base.md#LanguagePlugin.get_file_extensions), [`create_extractor`](../plugins/base.md#LanguagePlugin.create_extractor), [`get_tree_sitter_language`](../plugins/base.md#LanguagePlugin.get_tree_sitter_language), [`execute_query_strategy`](../plugins/base.md#LanguagePlugin.execute_query_strategy), [`get_queries`](../plugins/base.md#LanguagePlugin.get_queries), [`get_element_categories`](../plugins/base.md#LanguagePlugin.get_element_categories), [`get_supported_element_types`](../plugins/base.md#LanguagePlugin.get_supported_element_types)  (13 test-only)

## Module values
- `JSON_AVAILABLE` — [`L32`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/json_plugin.py#L32)
- `JSON_LANGUAGE` — [`L34`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/json_plugin.py#L34)
- `JSON_PARSER` — [`L35`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/json_plugin.py#L35)
- `_JSON_PARSER_LOCK` — [`L37`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/json_plugin.py#L37)
- `logger` — [`L25`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/json_plugin.py#L25)

