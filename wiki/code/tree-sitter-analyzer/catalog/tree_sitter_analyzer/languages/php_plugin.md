---
title: 'Module: tree_sitter_analyzer/languages/php_plugin.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/php_plugin.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.php_plugin`/
symbols:
  PHPPlugin: PHPPlugin#
  PHPPlugin.create_extractor: PHPPlugin#create_extractor().
  PHPPlugin.analyze_file: PHPPlugin#analyze_file().
  TREE_SITTER_AVAILABLE: TREE_SITTER_AVAILABLE.
  PHPElementExtractor: PHPElementExtractor#
  PHPElementExtractor.extract_functions: PHPElementExtractor#extract_functions().
  PHPElementExtractor._get_node_text_optimized: PHPElementExtractor#_get_node_text_optimized().
  PHPElementExtractor.extract_classes: PHPElementExtractor#extract_classes().
  PHPElementExtractor._extract_class_element: PHPElementExtractor#_extract_class_element().
  PHPElementExtractor.extract_variables: PHPElementExtractor#extract_variables().
  PHPElementExtractor._reset_caches: PHPElementExtractor#_reset_caches().
  PHPElementExtractor._extract_method_element: PHPElementExtractor#_extract_method_element().
  PHPPlugin.get_tree_sitter_language: PHPPlugin#get_tree_sitter_language().
  PHPElementExtractor._extract_function_element: PHPElementExtractor#_extract_function_element().
  PHPElementExtractor._extract_property_elements: PHPElementExtractor#_extract_property_elements().
  PHPElementExtractor._extract_constant_elements: PHPElementExtractor#_extract_constant_elements().
  PHPElementExtractor._extract_namespace: PHPElementExtractor#_extract_namespace().
  PHPElementExtractor.extract_imports: PHPElementExtractor#extract_imports().
  PHPElementExtractor._extract_attributes: PHPElementExtractor#_extract_attributes().
  PHPElementExtractor._extract_modifiers: PHPElementExtractor#_extract_modifiers().
  PHPElementExtractor._extract_use_statement: PHPElementExtractor#_extract_use_statement().
  PHPElementExtractor._determine_visibility: PHPElementExtractor#_determine_visibility().
  PHPElementExtractor._node_text_cache: PHPElementExtractor#_node_text_cache.
  PHPPlugin._count_nodes: PHPPlugin#_count_nodes().
  PHPElementExtractor.source_code: PHPElementExtractor#source_code.
  PHPElementExtractor.current_namespace: PHPElementExtractor#current_namespace.
  PHPPlugin.extract_elements: PHPPlugin#extract_elements().
  PHPElementExtractor.content_lines: PHPElementExtractor#content_lines.
  PHPPlugin._load_file_safe: PHPPlugin#_load_file_safe().
  PHPPlugin._language_instance: PHPPlugin#_language_instance.
  PHPPlugin.get_language_name: PHPPlugin#get_language_name().
  PHPElementExtractor.__init__: PHPElementExtractor#__init__().
  PHPElementExtractor._processed_nodes: PHPElementExtractor#_processed_nodes.
  PHPElementExtractor._attribute_cache: PHPElementExtractor#_attribute_cache.
  PHPElementExtractor._element_cache: PHPElementExtractor#_element_cache.
  PHPPlugin.get_file_extensions: PHPPlugin#get_file_extensions().
---
# Module: [`tree_sitter_analyzer/languages/php_plugin.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/php_plugin.py)

## Classes
### `PHPElementExtractor`  ·  implements/extends ElementExtractor
- def: [`tree_sitter_analyzer/languages/php_plugin.py:59`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/php_plugin.py#L59)
- doc: PHP-specific element extractor.
- signature: `class PHPElementExtractor(ElementExtractor):`
- members:
  - `__init__(self)` — [`L78`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/php_plugin.py#L78) — Initialize the PHP element extractor.
  - `_determine_visibility(self, modifiers: list[str])` — [`L153`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/php_plugin.py#L153) — Determine visibility from modifiers.
  - `_extract_attributes(self, node: tree_sitter.Node)` — [`L157`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/php_plugin.py#L157) — Extract PHP 8+ attributes from a node.
  - `_extract_class_element(self, node: tree_sitter.Node)` — [`L203`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/php_plugin.py#L203) — Extract a single class, interface, trait, or enum element.
  - `_extract_constant_elements(self, node: tree_sitter.Node, parent_class: str)` — [`L351`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/php_plugin.py#L351) — Extract constant elements from a const declaration.
  - `_extract_function_element(self, node: tree_sitter.Node)` — [`L281`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/php_plugin.py#L281) — Extract a function element.
  - `_extract_method_element(self, node: tree_sitter.Node, parent_class: str)` — [`L269`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/php_plugin.py#L269) — Extract a method element.
  - `_extract_modifiers(self, node: tree_sitter.Node)` — [`L149`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/php_plugin.py#L149) — Extract modifiers from a declaration node.
  - `_extract_namespace(self, node: tree_sitter.Node)` — [`L126`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/php_plugin.py#L126) — Extract namespace from the AST and set current_namespace.
  - `_extract_property_elements(self, node: tree_sitter.Node, parent_class: str)` — [`L340`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/php_plugin.py#L340) — Extract property elements from a property declaration.
  - `_extract_use_statement(self, node: tree_sitter.Node)` — [`L394`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/php_plugin.py#L394) — Extract use statement elements.
  - `_get_node_text_optimized(self, node: tree_sitter.Node)` — [`L104`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/php_plugin.py#L104) — Get text content of a node with caching for performance.
  - `_reset_caches(self)` — [`L96`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/php_plugin.py#L96) — Reset all internal caches for a new file analysis.
  - `extract_classes(self, tree: tree_sitter.Tree, source_code: str)` — [`L163`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/php_plugin.py#L163) — Extract PHP classes, interfaces, traits, and enums.
  - `extract_functions(self, tree: tree_sitter.Tree, source_code: str)` — [`L213`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/php_plugin.py#L213) — Extract PHP methods and functions.
  - `extract_imports(self, tree: tree_sitter.Tree, source_code: str)` — [`L362`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/php_plugin.py#L362) — Extract PHP use statements.
  - `extract_variables(self, tree: tree_sitter.Tree, source_code: str)` — [`L289`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/php_plugin.py#L289) — Extract PHP properties and constants.
  - `content_lines` — [`L87`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/php_plugin.py#L87)
  - `current_namespace` — [`L88`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/php_plugin.py#L88)
  - `source_code` — [`L86`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/php_plugin.py#L86)
- protocol/private: `_attribute_cache`[`L94`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/php_plugin.py#L94), `_element_cache`[`L93`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/php_plugin.py#L93), `_node_text_cache`[`L91`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/php_plugin.py#L91), `_processed_nodes`[`L92`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/php_plugin.py#L92)
- uses (calls/refs, reference-scoped): [`Function`](../models/base.md#Function), [`Class`](../models/base.md#Class), [`Variable`](../models/base.md#Variable), [`Import`](../models/base.md#Import), [`ElementExtractor`](../plugins/base.md#ElementExtractor), [`get_node_text_safe`](../utils/tree_sitter_compat.md#get_node_text_safe), [`extract_php_method_element`](php_helpers.md#extract_php_method_element), [`extract_php_function_element`](php_helpers.md#extract_php_function_element), [`extract_php_class_element`](php_helpers.md#extract_php_class_element), [`extract_php_constant_elements`](php_helpers.md#extract_php_constant_elements), [`extract_php_property_elements`](php_helpers.md#extract_php_property_elements), [`extract_use_statement`](php_helpers.md#extract_use_statement), [`determine_visibility`](php_helpers.md#determine_visibility), [`extract_modifiers`](php_helpers.md#extract_modifiers), [`__init__`](../plugins/base.md#ElementExtractor.__init__), [`extract_attributes`](php_helpers.md#extract_attributes)
- used by: [`ElementExtractor`](../plugins/base.md#ElementExtractor), [`extract_functions`](../plugins/base.md#ElementExtractor.extract_functions), [`extract_classes`](../plugins/base.md#ElementExtractor.extract_classes), [`extract_variables`](../plugins/base.md#ElementExtractor.extract_variables), [`extract_imports`](../plugins/base.md#ElementExtractor.extract_imports), [`create_extractor`](php_plugin.md#PHPPlugin.create_extractor)  (16 test-only)

### `PHPPlugin`  ·  implements/extends LanguagePlugin
- def: [`tree_sitter_analyzer/languages/php_plugin.py:399`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/php_plugin.py#L399) — documented in [tree_sitter_analyzer-plugins-manager](../../../concepts/tree_sitter_analyzer-plugins-manager.md)
- doc: PHP language plugin.
- signature: `class PHPPlugin(LanguagePlugin):`
- members:
  - `_count_nodes(self, node: tree_sitter.Node)` — [`L524`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/php_plugin.py#L524) — Count total nodes in the AST.
  - `_load_file_safe(self, file_path: str)` — [`L540`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/php_plugin.py#L540) — Load file content with encoding detection.
  - `analyze_file(self, file_path: str, request: AnalysisRequest)` — [`L471`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/php_plugin.py#L471) — Analyze a PHP file. — documented in [tree_sitter_analyzer-models-result](../../../concepts/tree_sitter_analyzer-models-result.md)
  - `create_extractor(self)` — [`L456`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/php_plugin.py#L456) — Create a PHP element extractor. — documented in [tree_sitter_analyzer-plugins-base](../../../concepts/tree_sitter_analyzer-plugins-base.md)
  - `extract_elements(self, tree: tree_sitter.Tree, source_code: str)` — [`L465`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/php_plugin.py#L465) — Unified extraction entry point — delegates to the extractor.
  - `get_file_extensions(self)` — [`L418`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/php_plugin.py#L418) — Get supported file extensions.
  - `get_language_name(self)` — [`L409`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/php_plugin.py#L409) — Get the name of the language.
  - `get_tree_sitter_language(self)` — [`L427`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/php_plugin.py#L427) — Get the tree-sitter language instance for PHP.
- protocol/private: `_language_instance`[`L407`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/php_plugin.py#L407)
- uses (calls/refs, reference-scoped): [`AnalysisResult`](../models/result.md#AnalysisResult), [`log_error`](../utils/logging.md#log_error), [`AnalysisRequest`](../core/request.md#AnalysisRequest), [`elements`](../models/result.md#AnalysisResult.elements), [`language`](../models/result.md#AnalysisResult.language), [`LanguagePlugin`](../plugins/base.md#LanguagePlugin), [`file_path`](../models/result.md#AnalysisResult.file_path), [`success`](../models/result.md#AnalysisResult.success), [`ElementExtractor`](../plugins/base.md#ElementExtractor), [`extract_functions`](../plugins/base.md#ElementExtractor.extract_functions), [`extract_classes`](../plugins/base.md#ElementExtractor.extract_classes), [`line_count`](../models/result.md#AnalysisResult.line_count), [`extract_variables`](../plugins/base.md#ElementExtractor.extract_variables), [`error_message`](../models/result.md#AnalysisResult.error_message), [`extract_imports`](../plugins/base.md#ElementExtractor.extract_imports), [`node_count`](../models/result.md#AnalysisResult.node_count), [`TREE_SITTER_AVAILABLE`](php_plugin.md#TREE_SITTER_AVAILABLE), [`extract_elements`](../plugins/base.md#ElementExtractor.extract_elements), [`PHPElementExtractor`](php_plugin.md#PHPElementExtractor)
- used by: [`LanguagePlugin`](../plugins/base.md#LanguagePlugin), [`get_language_name`](../plugins/base.md#LanguagePlugin.get_language_name), [`analyze_file`](../plugins/base.md#LanguagePlugin.analyze_file), [`get_file_extensions`](../plugins/base.md#LanguagePlugin.get_file_extensions), [`create_extractor`](../plugins/base.md#LanguagePlugin.create_extractor), [`get_tree_sitter_language`](../plugins/base.md#LanguagePlugin.get_tree_sitter_language)  (55 test-only)

## Module values
- `TREE_SITTER_AVAILABLE` — [`L22`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/php_plugin.py#L22)

