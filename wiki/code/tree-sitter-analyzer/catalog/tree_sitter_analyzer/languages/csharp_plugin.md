---
title: 'Module: tree_sitter_analyzer/languages/csharp_plugin.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/csharp_plugin.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.csharp_plugin`/
symbols:
  CSharpPlugin: CSharpPlugin#
  CSharpPlugin.extractor: CSharpPlugin#extractor.
  CSharpElementExtractor.extract_classes: CSharpElementExtractor#extract_classes().
  TREE_SITTER_AVAILABLE: TREE_SITTER_AVAILABLE.
  CSharpElementExtractor.extract_functions: CSharpElementExtractor#extract_functions().
  CSharpPlugin.analyze_file: CSharpPlugin#analyze_file().
  CSharpElementExtractor.extract_packages: CSharpElementExtractor#extract_packages().
  CSharpElementExtractor.extract_variables: CSharpElementExtractor#extract_variables().
  CSharpElementExtractor._get_node_text_optimized: CSharpElementExtractor#_get_node_text_optimized().
  CSharpElementExtractor._extract_method: CSharpElementExtractor#_extract_method().
  CSharpElementExtractor.extract_imports: CSharpElementExtractor#extract_imports().
  CSharpElementExtractor: CSharpElementExtractor#
  CSharpElementExtractor._reset_caches: CSharpElementExtractor#_reset_caches().
  CSharpPlugin.get_tree_sitter_language: CSharpPlugin#get_tree_sitter_language().
  CSharpElementExtractor._extract_class_declaration: CSharpElementExtractor#_extract_class_declaration().
  CSharpElementExtractor._extract_constructor: CSharpElementExtractor#_extract_constructor().
  CSharpElementExtractor._extract_property: CSharpElementExtractor#_extract_property().
  CSharpElementExtractor._extract_field: CSharpElementExtractor#_extract_field().
  CSharpElementExtractor._extract_event: CSharpElementExtractor#_extract_event().
  CSharpElementExtractor._extract_attributes: CSharpElementExtractor#_extract_attributes().
  CSharpElementExtractor.source_code: CSharpElementExtractor#source_code.
  CSharpElementExtractor.extract_elements: CSharpElementExtractor#extract_elements().
  CSharpElementExtractor._extract_modifiers: CSharpElementExtractor#_extract_modifiers().
  CSharpElementExtractor._extract_namespace: CSharpElementExtractor#_extract_namespace().
  CSharpElementExtractor._traverse_iterative: CSharpElementExtractor#_traverse_iterative().
  CSharpElementExtractor._extract_type_name: CSharpElementExtractor#_extract_type_name().
  CSharpPlugin.create_extractor: CSharpPlugin#create_extractor().
  CSharpElementExtractor._extract_using_directive: CSharpElementExtractor#_extract_using_directive().
  CSharpElementExtractor._extract_parameters: CSharpElementExtractor#_extract_parameters().
  CSharpPlugin.execute_query_strategy: CSharpPlugin#execute_query_strategy().
  CSharpElementExtractor._enclosing_namespace: CSharpElementExtractor#_enclosing_namespace().
  CSharpElementExtractor._calculate_complexity: CSharpElementExtractor#_calculate_complexity().
  CSharpPlugin.extract_elements: CSharpPlugin#extract_elements().
  CSharpElementExtractor.content_lines: CSharpElementExtractor#content_lines.
  CSharpPlugin._cached_language: CSharpPlugin#_cached_language.
  CSharpPlugin.get_queries: CSharpPlugin#get_queries().
  CSharpElementExtractor._node_text_cache: CSharpElementExtractor#_node_text_cache.
  CSharpElementExtractor._file_scoped_namespace: CSharpElementExtractor#_file_scoped_namespace().
  CSharpElementExtractor.current_namespace: CSharpElementExtractor#current_namespace.
  CSharpElementExtractor.__init__: CSharpElementExtractor#__init__().
  CSharpElementExtractor._determine_visibility: CSharpElementExtractor#_determine_visibility().
  _traverse_nodes: _traverse_nodes().
  CSharpElementExtractor._attribute_cache: CSharpElementExtractor#_attribute_cache.
  CSharpElementExtractor._processed_nodes: CSharpElementExtractor#_processed_nodes.
  CSharpElementExtractor._element_cache: CSharpElementExtractor#_element_cache.
  CSharpPlugin.get_language_name: CSharpPlugin#get_language_name().
  CSharpPlugin.get_file_extensions: CSharpPlugin#get_file_extensions().
  CSharpPlugin.get_element_categories: CSharpPlugin#get_element_categories().
  CSharpPlugin.__init__: CSharpPlugin#__init__().
  CSharpPlugin.language: CSharpPlugin#language.
  CSharpPlugin.supported_extensions: CSharpPlugin#supported_extensions.
---
# Module: [`tree_sitter_analyzer/languages/csharp_plugin.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_plugin.py)

## Classes
### `CSharpElementExtractor`  ·  implements/extends ElementExtractor
- def: [`tree_sitter_analyzer/languages/csharp_plugin.py:83`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_plugin.py#L83)
- doc: C#-specific element extractor.
- signature: `class CSharpElementExtractor(ElementExtractor):`
- members:
  - `__init__(self)` — [`L102`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_plugin.py#L102) — Initialize the C# element extractor.
  - `_calculate_complexity(self, node: tree_sitter.Node)` — [`L396`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_plugin.py#L396) — Calculate cyclomatic complexity of a method.
  - `_determine_visibility(self, modifiers: list[str])` — [`L180`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_plugin.py#L180) — Determine visibility from modifiers.
  - `_enclosing_namespace(self, node: tree_sitter.Node)` — [`L246`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_plugin.py#L246) — Compute a node's fully-qualified enclosing namespace.
  - `_extract_attributes(self, node: tree_sitter.Node)` — [`L184`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_plugin.py#L184) — Extract attributes (annotations) from a node.
  - `_extract_class_declaration(self, node: tree_sitter.Node)` — [`L300`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_plugin.py#L300) — Extract a single class declaration.
  - `_extract_constructor(self, node: tree_sitter.Node)` — [`L376`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_plugin.py#L376) — Extract a constructor declaration.
  - `_extract_event(self, node: tree_sitter.Node)` — [`L446`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_plugin.py#L446) — Extract event field declarations.
  - `_extract_field(self, node: tree_sitter.Node)` — [`L436`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_plugin.py#L436) — Extract field declarations.
  - `_extract_method(self, node: tree_sitter.Node)` — [`L364`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_plugin.py#L364) — Extract a method declaration.
  - `_extract_modifiers(self, node: tree_sitter.Node)` — [`L176`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_plugin.py#L176) — Extract modifiers from a declaration node.
  - `_extract_namespace(self, node: tree_sitter.Node)` — [`L150`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_plugin.py#L150) — Extract namespace from the AST and set current_namespace.
  - `_extract_parameters(self, params_node: tree_sitter.Node | None)` — [`L194`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_plugin.py#L194) — Extract method parameters.
  - `_extract_property(self, node: tree_sitter.Node)` — [`L386`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_plugin.py#L386) — Extract a property declaration.
  - `_extract_type_name(self, type_node: tree_sitter.Node | None)` — [`L190`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_plugin.py#L190) — Extract type name from a type node.
  - `_extract_using_directive(self, node: tree_sitter.Node)` — [`L489`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_plugin.py#L489) — Extract a using directive.
  - `_file_scoped_namespace(self, node: tree_sitter.Node)` — [`L276`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_plugin.py#L276) — Return the file-scoped namespace name in effect for ``node``, if any.
  - `_get_node_text_optimized(self, node: tree_sitter.Node)` — [`L128`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_plugin.py#L128) — Get text content of a node with caching for performance.
  - `_reset_caches(self)` — [`L120`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_plugin.py#L120) — Reset all internal caches for a new file analysis.
  - `extract_classes(self, tree: tree_sitter.Tree | None, source_code: str)` — [`L203`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_plugin.py#L203) — Extract classes, interfaces, records, enums, and structs. — documented in [tree_sitter_analyzer-languages-csharp_plugin](../../../concepts/tree_sitter_analyzer-languages-csharp_plugin.md)
  - `extract_elements(self, tree: tree_sitter.Tree, source_code: str)` — [`L541`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_plugin.py#L541) — Extract grouped C# elements, including namespace packages.
  - `extract_functions(self, tree: tree_sitter.Tree | None, source_code: str)` — [`L310`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_plugin.py#L310) — Extract methods, constructors, and properties. — documented in [tree_sitter_analyzer-plugins-base](../../../concepts/tree_sitter_analyzer-plugins-base.md)
  - `extract_imports(self, tree: tree_sitter.Tree | None, source_code: str)` — [`L456`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_plugin.py#L456) — Extract using directives.
  - `extract_packages(self, tree: tree_sitter.Tree | None, source_code: str)` — [`L493`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_plugin.py#L493) — Extract the C# namespace declaration as a Package element.
  - `extract_variables(self, tree: tree_sitter.Tree | None, source_code: str)` — [`L400`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_plugin.py#L400) — Extract fields, constants, and events.
  - `content_lines` — [`L111`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_plugin.py#L111)
  - `current_namespace` — [`L112`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_plugin.py#L112)
  - `source_code` — [`L110`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_plugin.py#L110)
- protocol/private: `_attribute_cache`[`L118`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_plugin.py#L118), `_element_cache`[`L117`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_plugin.py#L117), `_node_text_cache`[`L115`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_plugin.py#L115), `_processed_nodes`[`L116`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_plugin.py#L116), `_traverse_iterative`[`L198`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_plugin.py#L198)
- uses (calls/refs, reference-scoped): [`name`](../models/base.md#CodeElement.name), [`start_line`](../models/base.md#CodeElement.start_line), [`end_line`](../models/base.md#CodeElement.end_line), [`language`](../models/base.md#CodeElement.language), [`Function`](../models/base.md#Function), [`raw_text`](../models/base.md#CodeElement.raw_text), [`Class`](../models/base.md#Class), [`Variable`](../models/base.md#Variable), [`Import`](../models/base.md#Import), [`ElementExtractor`](../plugins/base.md#ElementExtractor), [`get_node_text_safe`](../utils/tree_sitter_compat.md#get_node_text_safe), [`receiver_type`](../models/base.md#Function.receiver_type), [`Package`](../models/base.md#Package), [`extract_class_declaration`](csharp_helpers.md#extract_class_declaration), [`extract_field_declaration`](csharp_helpers.md#extract_field_declaration), [`extract_method_declaration`](csharp_helpers.md#extract_method_declaration), [`extract_event_declaration`](csharp_helpers.md#extract_event_declaration), [`extract_property_declaration`](csharp_helpers.md#extract_property_declaration), [`extract_constructor_declaration`](csharp_helpers.md#extract_constructor_declaration), [`extract_using_directive`](csharp_helpers.md#extract_using_directive), [`determine_visibility`](csharp_helpers.md#determine_visibility), [`extract_attributes`](csharp_helpers.md#extract_attributes), [`extract_modifiers`](csharp_helpers.md#extract_modifiers), [`calculate_complexity`](csharp_helpers.md#calculate_complexity), [`extract_parameters`](csharp_helpers.md#extract_parameters), [`extract_type_name`](csharp_helpers.md#extract_type_name), [`find_owning_class_name`](csharp_helpers.md#find_owning_class_name), [`__init__`](../plugins/base.md#ElementExtractor.__init__), [`_traverse_nodes`](csharp_plugin.md#_traverse_nodes)
- used by: [`ElementExtractor`](../plugins/base.md#ElementExtractor), [`extract_functions`](../plugins/base.md#ElementExtractor.extract_functions), [`extract_classes`](../plugins/base.md#ElementExtractor.extract_classes), [`extractor`](csharp_plugin.md#CSharpPlugin.extractor), [`extract_variables`](../plugins/base.md#ElementExtractor.extract_variables), [`extract_imports`](../plugins/base.md#ElementExtractor.extract_imports), [`extract_elements`](../plugins/base.md#ElementExtractor.extract_elements), [`extract_packages`](../plugins/base.md#ElementExtractor.extract_packages), [`create_extractor`](csharp_plugin.md#CSharpPlugin.create_extractor)  (110 test-only)

### `CSharpPlugin`  ·  implements/extends LanguagePlugin
- def: [`tree_sitter_analyzer/languages/csharp_plugin.py:554`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_plugin.py#L554) — documented in [tree_sitter_analyzer-languages-csharp_plugin](../../../concepts/tree_sitter_analyzer-languages-csharp_plugin.md)
- doc: C# language plugin implementation.
- signature: `class CSharpPlugin(LanguagePlugin):`
- members:
  - `__init__(self)` — [`L563`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_plugin.py#L563) — Initialize the C# plugin.
  - `analyze_file(self, file_path: str, request: AnalysisRequest)` — [`L692`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_plugin.py#L692) — Analyze a C# file and extract all elements. — documented in [tree_sitter_analyzer-models-result](../../../concepts/tree_sitter_analyzer-models-result.md)
  - `create_extractor(self)` — [`L589`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_plugin.py#L589) — Create a new C# element extractor instance.
  - `execute_query_strategy(self, query_key: str | None, language: str)` — [`L609`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_plugin.py#L609) — Execute query strategy for C#.
  - `extract_elements(self, tree: tree_sitter.Tree, source_code: str)` — [`L686`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_plugin.py#L686) — Unified extraction entry point — delegates to the extractor.
  - `get_element_categories(self)` — [`L628`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_plugin.py#L628) — Return C# element categories for query execution.
  - `get_file_extensions(self)` — [`L580`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_plugin.py#L580) — Get supported file extensions.
  - `get_language_name(self)` — [`L571`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_plugin.py#L571) — Get the language name.
  - `get_queries(self)` — [`L598`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_plugin.py#L598) — Return C#-specific tree-sitter queries.
  - `get_tree_sitter_language(self)` — [`L654`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_plugin.py#L654) — Load tree-sitter-c-sharp language.
  - `extractor` — [`L566`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_plugin.py#L566) — documented in [tree_sitter_analyzer-languages-csharp_plugin](../../../concepts/tree_sitter_analyzer-languages-csharp_plugin.md)
  - `language` — [`L567`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_plugin.py#L567)
  - `supported_extensions` — [`L568`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_plugin.py#L568)
- protocol/private: `_cached_language`[`L569`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_plugin.py#L569)
- uses (calls/refs, reference-scoped): [`log_debug`](../utils/logging.md#log_debug), [`AnalysisResult`](../models/result.md#AnalysisResult), [`log_error`](../utils/logging.md#log_error), [`AnalysisRequest`](../core/request.md#AnalysisRequest), [`elements`](../models/result.md#AnalysisResult.elements), [`language`](../models/result.md#AnalysisResult.language), [`LanguagePlugin`](../plugins/base.md#LanguagePlugin), [`file_path`](../models/result.md#AnalysisResult.file_path), [`success`](../models/result.md#AnalysisResult.success), [`ElementExtractor`](../plugins/base.md#ElementExtractor), [`extract_functions`](../plugins/base.md#ElementExtractor.extract_functions), [`extract_classes`](../plugins/base.md#ElementExtractor.extract_classes), [`line_count`](../models/result.md#AnalysisResult.line_count), [`extract_variables`](../plugins/base.md#ElementExtractor.extract_variables), [`error_message`](../models/result.md#AnalysisResult.error_message), [`extract_imports`](../plugins/base.md#ElementExtractor.extract_imports), [`source_code`](../models/result.md#AnalysisResult.source_code), [`read_file_safe`](../encoding_utils.md#read_file_safe), [`node_count`](../models/result.md#AnalysisResult.node_count), [`extract_elements`](../plugins/base.md#ElementExtractor.extract_elements), [`extract_packages`](../plugins/base.md#ElementExtractor.extract_packages), [`CSharpElementExtractor`](csharp_plugin.md#CSharpElementExtractor), [`CSHARP_QUERIES`](../queries/csharp.md#CSHARP_QUERIES.CSHARP_QUERIES), [`_traverse_nodes`](csharp_plugin.md#_traverse_nodes)
- used by: [`LanguagePlugin`](../plugins/base.md#LanguagePlugin), [`get_language_name`](../plugins/base.md#LanguagePlugin.get_language_name), [`analyze_file`](../plugins/base.md#LanguagePlugin.analyze_file), [`get_file_extensions`](../plugins/base.md#LanguagePlugin.get_file_extensions), [`create_extractor`](../plugins/base.md#LanguagePlugin.create_extractor), [`get_tree_sitter_language`](../plugins/base.md#LanguagePlugin.get_tree_sitter_language), [`execute_query_strategy`](../plugins/base.md#LanguagePlugin.execute_query_strategy), [`get_queries`](../plugins/base.md#LanguagePlugin.get_queries), [`get_element_categories`](../plugins/base.md#LanguagePlugin.get_element_categories)  (126 test-only)

## Functions
- `_traverse_nodes(root_node: tree_sitter.Node)` — [`L75`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_plugin.py#L75)

## Module values
- `TREE_SITTER_AVAILABLE` — [`L23`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_plugin.py#L23) — documented in [tree_sitter_analyzer-plugins-base](../../../concepts/tree_sitter_analyzer-plugins-base.md)

