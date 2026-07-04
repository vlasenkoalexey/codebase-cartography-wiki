---
title: 'Module: tree_sitter_analyzer/languages/yaml_plugin.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/yaml_plugin.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.yaml_plugin`/
symbols:
  YAMLPlugin: YAMLPlugin#
  YAMLElementExtractor.extract_yaml_elements: YAMLElementExtractor#extract_yaml_elements().
  YAMLPlugin.analyze_file: YAMLPlugin#analyze_file().
  YAML_AVAILABLE: YAML_AVAILABLE.
  YAMLPlugin.extractor: YAMLPlugin#extractor.
  YAMLElementExtractor: YAMLElementExtractor#
  YAMLElementExtractor._extract_mappings: YAMLElementExtractor#_extract_mappings().
  YAMLElementExtractor._extract_sequences: YAMLElementExtractor#_extract_sequences().
  YAMLElementExtractor._extract_anchors: YAMLElementExtractor#_extract_anchors().
  YAMLElementExtractor._extract_aliases: YAMLElementExtractor#_extract_aliases().
  YAMLElementExtractor._extract_documents: YAMLElementExtractor#_extract_documents().
  YAMLElementExtractor._extract_comments: YAMLElementExtractor#_extract_comments().
  YAMLElementExtractor._get_node_text: YAMLElementExtractor#_get_node_text().
  YAMLElementExtractor._get_document_index: YAMLElementExtractor#_get_document_index().
  YAMLElementExtractor._traverse_nodes: YAMLElementExtractor#_traverse_nodes().
  YAMLPlugin.get_tree_sitter_language: YAMLPlugin#get_tree_sitter_language().
  YAMLElementExtractor._calculate_nesting_level: YAMLElementExtractor#_calculate_nesting_level().
  YAML_PARSER: YAML_PARSER.
  _YAML_PARSER_LOCK: _YAML_PARSER_LOCK.
  YAMLElementExtractor._extract_value_info: YAMLElementExtractor#_extract_value_info().
  YAMLPlugin.extract_elements: YAMLPlugin#extract_elements().
  YAMLPlugin.create_extractor: YAMLPlugin#create_extractor().
  YAMLPlugin.get_queries: YAMLPlugin#get_queries().
  YAMLElementExtractor.extract_functions: YAMLElementExtractor#extract_functions().
  YAMLElementExtractor.extract_classes: YAMLElementExtractor#extract_classes().
  YAMLElementExtractor.extract_elements: YAMLElementExtractor#extract_elements().
  YAMLElementExtractor.source_code: YAMLElementExtractor#source_code.
  YAMLElementExtractor.extract_variables: YAMLElementExtractor#extract_variables().
  YAMLElementExtractor.extract_imports: YAMLElementExtractor#extract_imports().
  YAMLElementExtractor._count_document_children: YAMLElementExtractor#_count_document_children().
  YAMLElementExtractor._is_number: YAMLElementExtractor#_is_number().
  YAMLPlugin.execute_query_strategy: YAMLPlugin#execute_query_strategy().
  YAML_LANGUAGE: YAML_LANGUAGE.
  YAMLPlugin.get_file_extensions: YAMLPlugin#get_file_extensions().
  YAMLElementExtractor.content_lines: YAMLElementExtractor#content_lines.
  YAMLElementExtractor._current_document_index: YAMLElementExtractor#_current_document_index.
  YAMLPlugin.get_supported_element_types: YAMLPlugin#get_supported_element_types().
  logger: logger.
  YAMLElementExtractor.__init__: YAMLElementExtractor#__init__().
  YAMLPlugin.__init__: YAMLPlugin#__init__().
  YAMLPlugin.get_language_name: YAMLPlugin#get_language_name().
  YAMLPlugin.get_element_categories: YAMLPlugin#get_element_categories().
---
# Module: [`tree_sitter_analyzer/languages/yaml_plugin.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_plugin.py)

## Classes
### `YAMLElementExtractor`  ·  implements/extends ElementExtractor
- def: [`tree_sitter_analyzer/languages/yaml_plugin.py:93`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_plugin.py#L93)
- doc: YAML-specific element extractor using tree-sitter-yaml.
- signature: `class YAMLElementExtractor(ElementExtractor):`
- members:
  - `__init__(self)` — [`L96`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_plugin.py#L96) — Initialize the YAML element extractor.
  - `_calculate_nesting_level(self, node: tree_sitter.Node)` — [`L185`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_plugin.py#L185) — Calculate AST-based logical nesting level.
  - `_count_document_children(self, document_node: tree_sitter.Node)` — [`L197`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_plugin.py#L197) — Count meaningful children in a document (top-level mappings).
  - `_extract_aliases(self, root_node: tree_sitter.Node, elements: list[YAMLElement])` — [`L285`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_plugin.py#L285) — Extract YAML aliases (*name).
  - `_extract_anchors(self, root_node: tree_sitter.Node, elements: list[YAMLElement])` — [`L267`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_plugin.py#L267) — Extract YAML anchors (&name).
  - `_extract_comments(self, root_node: tree_sitter.Node, elements: list[YAMLElement])` — [`L303`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_plugin.py#L303) — Extract YAML comments.
  - `_extract_documents(self, root_node: tree_sitter.Node, elements: list[YAMLElement])` — [`L206`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_plugin.py#L206) — Extract YAML documents.
  - `_extract_mappings(self, root_node: tree_sitter.Node, elements: list[YAMLElement])` — [`L222`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_plugin.py#L222) — Extract YAML mappings (key-value pairs).
  - `_extract_sequences(self, root_node: tree_sitter.Node, elements: list[YAMLElement])` — [`L250`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_plugin.py#L250) — Extract YAML sequences (lists).
  - `_extract_value_info(self, node: tree_sitter.Node | None)` — [`L237`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_plugin.py#L237) — Extract value information from a node.
  - `_get_document_index(self, node: tree_sitter.Node)` — [`L189`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_plugin.py#L189) — Get document index for a node.
  - `_get_node_text(self, node: tree_sitter.Node)` — [`L173`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_plugin.py#L173) — Get text content from a tree-sitter node.
  - `_is_number(self, text: str)` — [`L243`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_plugin.py#L243) — Check if text represents a number.
  - `_traverse_nodes(self, node: tree_sitter.Node)` — [`L193`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_plugin.py#L193) — Traverse all nodes in the tree.
  - `extract_classes(self, tree: tree_sitter.Tree, source_code: str)` — [`L110`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_plugin.py#L110) — YAML doesn't have classes, return empty list.
  - `extract_elements(self, tree: tree_sitter.Tree | None, source_code: str)` — [`L167`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_plugin.py#L167)
  - `extract_functions(self, tree: tree_sitter.Tree, source_code: str)` — [`L103`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_plugin.py#L103) — YAML doesn't have functions, return empty list.
  - `extract_imports(self, tree: tree_sitter.Tree, source_code: str)` — [`L122`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_plugin.py#L122) — YAML doesn't have imports, return empty list.
  - `extract_variables(self, tree: tree_sitter.Tree, source_code: str)` — [`L115`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_plugin.py#L115) — YAML doesn't have variables, return empty list.
  - `extract_yaml_elements(self, tree: tree_sitter.Tree | None, source_code: str)` — [`L127`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_plugin.py#L127) — Extract all YAML elements from the parsed tree. — documented in [tree_sitter_analyzer-utils-logging](../../../concepts/tree_sitter_analyzer-utils-logging.md)
  - `content_lines` — [`L99`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_plugin.py#L99)
  - `source_code` — [`L98`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_plugin.py#L98)
- protocol/private: `_current_document_index`[`L100`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_plugin.py#L100)
- uses (calls/refs, reference-scoped): [`log_debug`](../utils/logging.md#log_debug), [`Function`](../models/base.md#Function), [`log_error`](../utils/logging.md#log_error), [`Class`](../models/base.md#Class), [`Variable`](../models/base.md#Variable), [`Import`](../models/base.md#Import), [`ElementExtractor`](../plugins/base.md#ElementExtractor), [`YAMLElement`](yaml_helpers.md#YAMLElement), [`extract_value_info`](yaml_helpers.md#extract_value_info), [`append_mapping_element`](yaml_helpers.md#append_mapping_element), [`append_alias_element`](yaml_helpers.md#append_alias_element), [`append_anchor_element`](yaml_helpers.md#append_anchor_element), [`append_comment_element`](yaml_helpers.md#append_comment_element), [`append_document_element`](yaml_helpers.md#append_document_element), [`append_sequence_element`](yaml_helpers.md#append_sequence_element), [`count_document_children`](yaml_helpers.md#count_document_children), [`traverse_nodes`](yaml_helpers.md#traverse_nodes), [`iter_nodes_by_type`](yaml_helpers.md#iter_nodes_by_type), [`calculate_nesting_level`](yaml_helpers.md#calculate_nesting_level), [`get_document_index`](yaml_helpers.md#get_document_index), [`iter_document_nodes`](yaml_helpers.md#iter_document_nodes), [`iter_mapping_nodes`](yaml_helpers.md#iter_mapping_nodes), [`iter_sequence_nodes`](yaml_helpers.md#iter_sequence_nodes), [`is_number`](yaml_helpers.md#is_number)
- used by: [`ElementExtractor`](../plugins/base.md#ElementExtractor), [`extract_functions`](../plugins/base.md#ElementExtractor.extract_functions), [`extract_classes`](../plugins/base.md#ElementExtractor.extract_classes), [`extract_variables`](../plugins/base.md#ElementExtractor.extract_variables), [`extract_imports`](../plugins/base.md#ElementExtractor.extract_imports), [`extractor`](yaml_plugin.md#YAMLPlugin.extractor), [`extract_elements`](../plugins/base.md#ElementExtractor.extract_elements), [`extract_elements`](yaml_plugin.md#YAMLPlugin.extract_elements), [`create_extractor`](yaml_plugin.md#YAMLPlugin.create_extractor)  (44 test-only)

### `YAMLPlugin`  ·  implements/extends LanguagePlugin
- def: [`tree_sitter_analyzer/languages/yaml_plugin.py:320`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_plugin.py#L320) — documented in [tree_sitter_analyzer-plugins-base](../../../concepts/tree_sitter_analyzer-plugins-base.md)
- doc: YAML language plugin using tree-sitter-yaml for true YAML parsing.
- signature: `class YAMLPlugin(LanguagePlugin):`
- members:
  - `__init__(self)` — [`L323`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_plugin.py#L323) — Initialize YAML plugin with extractor.
  - `analyze_file(self, file_path: str, request: AnalysisRequest)` — [`L399`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_plugin.py#L399) — Analyze YAML file using tree-sitter-yaml parser. — documented in [tree_sitter_analyzer-models-result](../../../concepts/tree_sitter_analyzer-models-result.md)
  - `create_extractor(self)` — [`L337`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_plugin.py#L337) — Create and return a YAML element extractor.
  - `execute_query_strategy(self, query_key: str | None, language: str)` — [`L366`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_plugin.py#L366) — Execute query strategy for YAML.
  - `extract_elements(self, tree: tree_sitter.Tree, source_code: str)` — [`L393`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_plugin.py#L393) — Unified extraction entry point — delegates to the extractor.
  - `get_element_categories(self)` — [`L376`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_plugin.py#L376) — Return YAML element categories for query execution.
  - `get_file_extensions(self)` — [`L332`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_plugin.py#L332) — Return supported file extensions.
  - `get_language_name(self)` — [`L328`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_plugin.py#L328) — Return the language name.
  - `get_queries(self)` — [`L359`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_plugin.py#L359) — Return YAML-specific tree-sitter queries.
  - `get_supported_element_types(self)` — [`L347`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_plugin.py#L347) — Return supported element types.
  - `get_tree_sitter_language(self)` — [`L341`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_plugin.py#L341) — Get tree-sitter language object for YAML.
  - `extractor` — [`L326`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_plugin.py#L326)
- uses (calls/refs, reference-scoped): [`AnalysisResult`](../models/result.md#AnalysisResult), [`AnalysisRequest`](../core/request.md#AnalysisRequest), [`LanguagePlugin`](../plugins/base.md#LanguagePlugin), [`YAML_AVAILABLE`](yaml_plugin.md#YAML_AVAILABLE), [`YAML_QUERIES`](../queries/yaml.md#YAML_QUERIES.YAML_QUERIES), [`YAMLElementExtractor`](yaml_plugin.md#YAMLElementExtractor), [`analyze_yaml_file`](yaml_helpers.md#analyze_yaml_file), [`extract_elements`](yaml_plugin.md#YAMLElementExtractor.extract_elements), [`YAML_LANGUAGE`](yaml_plugin.md#YAML_LANGUAGE)
- used by: [`LanguagePlugin`](../plugins/base.md#LanguagePlugin), [`get_language_name`](../plugins/base.md#LanguagePlugin.get_language_name), [`analyze_file`](../plugins/base.md#LanguagePlugin.analyze_file), [`get_file_extensions`](../plugins/base.md#LanguagePlugin.get_file_extensions), [`create_extractor`](../plugins/base.md#LanguagePlugin.create_extractor), [`get_tree_sitter_language`](../plugins/base.md#LanguagePlugin.get_tree_sitter_language), [`execute_query_strategy`](../plugins/base.md#LanguagePlugin.execute_query_strategy), [`get_queries`](../plugins/base.md#LanguagePlugin.get_queries), [`get_element_categories`](../plugins/base.md#LanguagePlugin.get_element_categories), [`get_supported_element_types`](../plugins/base.md#LanguagePlugin.get_supported_element_types)  (67 test-only)

## Module values
- `YAML_AVAILABLE` — [`L81`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_plugin.py#L81)
- `YAML_LANGUAGE` — [`L84`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_plugin.py#L84)
- `YAML_PARSER` — [`L85`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_plugin.py#L85)
- `_YAML_PARSER_LOCK` — [`L87`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_plugin.py#L87)
- `logger` — [`L74`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/yaml_plugin.py#L74)

