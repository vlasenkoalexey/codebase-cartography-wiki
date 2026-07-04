---
title: 'Module: tree_sitter_analyzer/languages/cpp_plugin.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/cpp_plugin.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.cpp_plugin`/Cpp
symbols:
  CppPlugin.analyze_file: Plugin#analyze_file().
  CppElementExtractor: ElementExtractor#
  CppElementExtractor.extract_classes: ElementExtractor#extract_classes().
  CppElementExtractor._extract_function_optimized: ElementExtractor#_extract_function_optimized().
  CppElementExtractor._extract_class_optimized: ElementExtractor#_extract_class_optimized().
  CppElementExtractor._extract_function_from_field_declaration: ElementExtractor#_extract_function_from_field_declaration().
  CppElementExtractor.extract_functions: ElementExtractor#extract_functions().
  CppPlugin: Plugin#
  CppElementExtractor._get_node_text_optimized: ElementExtractor#_get_node_text_optimized().
  CppElementExtractor._traverse_and_extract_iterative: ElementExtractor#_traverse_and_extract_iterative().
  CppElementExtractor.extract_variables: ElementExtractor#extract_variables().
  CppElementExtractor._reset_caches: ElementExtractor#_reset_caches().
  CppPlugin.extract_elements: Plugin#extract_elements().
  CppElementExtractor._extract_template_class: ElementExtractor#_extract_template_class().
  CppElementExtractor.extract_imports: ElementExtractor#extract_imports().
  CppElementExtractor._extract_field_optimized: ElementExtractor#_extract_field_optimized().
  CppElementExtractor._extract_template_function: ElementExtractor#_extract_template_function().
  CppElementExtractor._extract_variable_declaration: ElementExtractor#_extract_variable_declaration().
  CppElementExtractor._extract_struct_optimized: ElementExtractor#_extract_struct_optimized().
  CppElementExtractor._extract_enum_optimized: ElementExtractor#_extract_enum_optimized().
  CppPlugin.create_extractor: Plugin#create_extractor().
  CppElementExtractor._extract_function_declaration: ElementExtractor#_extract_function_declaration().
  CppElementExtractor._extract_union_optimized: ElementExtractor#_extract_union_optimized().
  CppPlugin.get_tree_sitter_language: Plugin#get_tree_sitter_language().
  CppElementExtractor.extract_packages: ElementExtractor#extract_packages().
  CppElementExtractor.content_lines: ElementExtractor#content_lines.
  CppElementExtractor._determine_visibility: ElementExtractor#_determine_visibility().
  CppElementExtractor._parse_function_signature: ElementExtractor#_parse_function_signature().
  CppElementExtractor._extract_parameters: ElementExtractor#_extract_parameters().
  CppElementExtractor._extract_comment_for_line: ElementExtractor#_extract_comment_for_line().
  CppElementExtractor._extract_include_info: ElementExtractor#_extract_include_info().
  CppElementExtractor._extract_namespace_info: ElementExtractor#_extract_namespace_info().
  CppElementExtractor._is_global_scope: ElementExtractor#_is_global_scope().
  CppElementExtractor._extract_base_classes: ElementExtractor#_extract_base_classes().
  CppElementExtractor._calculate_complexity_optimized: ElementExtractor#_calculate_complexity_optimized().
  CppElementExtractor.source_code: ElementExtractor#source_code.
  CppElementExtractor._extract_includes_fallback: ElementExtractor#_extract_includes_fallback().
  CppElementExtractor._get_access_specifier: ElementExtractor#_get_access_specifier().
  CppPlugin._count_tree_nodes: Plugin#_count_tree_nodes().
  CppElementExtractor._processed_nodes: ElementExtractor#_processed_nodes.
  CppPlugin._cached_language: Plugin#_cached_language.
  CppElementExtractor.current_namespace: ElementExtractor#current_namespace.
  CppPlugin.extractor: Plugin#extractor.
  CppPlugin.supported_extensions: Plugin#supported_extensions.
  CppElementExtractor._node_text_cache: ElementExtractor#_node_text_cache.
  CppElementExtractor._element_cache: ElementExtractor#_element_cache.
  CppPlugin.get_file_extensions: Plugin#get_file_extensions().
  CppElementExtractor._file_encoding: ElementExtractor#_file_encoding.
  CppElementExtractor._comment_cache: ElementExtractor#_comment_cache.
  CppElementExtractor._complexity_cache: ElementExtractor#_complexity_cache.
  CppPlugin.get_language_name: Plugin#get_language_name().
  CppElementExtractor.__init__: ElementExtractor#__init__().
  CppElementExtractor.current_file: ElementExtractor#current_file.
  CppElementExtractor.includes: ElementExtractor#includes.
  CppPlugin.__init__: Plugin#__init__().
  CppPlugin.language: Plugin#language.
---
# Module: [`tree_sitter_analyzer/languages/cpp_plugin.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/cpp_plugin.py)

## Classes
### `CppElementExtractor`  ·  implements/extends ElementExtractor
- def: [`tree_sitter_analyzer/languages/cpp_plugin.py:102`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/cpp_plugin.py#L102)
- doc: C++ specific element extractor with advanced analysis support
- signature: `class CppElementExtractor(ElementExtractor):`
- members:
  - `__init__(self)` — [`L105`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/cpp_plugin.py#L105) — Initialize the C++ element extractor.
  - `_extract_base_classes(self, node: tree_sitter.Node)` — [`L394`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/cpp_plugin.py#L394) — Extract base class names from base_class_clause
  - `_extract_class_optimized(self, node: tree_sitter.Node)` — [`L324`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/cpp_plugin.py#L324) — Extract class information optimized
  - `_extract_enum_optimized(self, node: tree_sitter.Node)` — [`L362`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/cpp_plugin.py#L362) — Extract enum / scoped enum-class information optimized.
  - `_extract_field_optimized(self, node: tree_sitter.Node)` — [`L399`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/cpp_plugin.py#L399) — Extract field declaration
  - `_extract_function_declaration(self, node: tree_sitter.Node)` — [`L288`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/cpp_plugin.py#L288) — Extract function declaration (prototype)
  - `_extract_function_from_field_declaration(self, node: tree_sitter.Node)` — [`L272`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/cpp_plugin.py#L272) — Extract function from field_declaration (pure virtual, deleted, etc).
  - `_extract_function_optimized(self, node: tree_sitter.Node)` — [`L257`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/cpp_plugin.py#L257) — Extract function information optimized
  - `_extract_parameters(self, params_node: tree_sitter.Node)` — [`L319`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/cpp_plugin.py#L319) — Extract function parameters
  - `_extract_struct_optimized(self, node: tree_sitter.Node)` — [`L338`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/cpp_plugin.py#L338) — Extract struct information optimized
  - `_extract_template_class(self, node: tree_sitter.Node)` — [`L380`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/cpp_plugin.py#L380) — Extract template class definition
  - `_extract_template_function(self, node: tree_sitter.Node)` — [`L297`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/cpp_plugin.py#L297) — Extract template function definition
  - `_extract_union_optimized(self, node: tree_sitter.Node)` — [`L350`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/cpp_plugin.py#L350) — Extract union information optimized
  - `_extract_variable_declaration(self, node: tree_sitter.Node)` — [`L409`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/cpp_plugin.py#L409) — Extract variable declarations (not class members)
  - `_get_node_text_optimized(self, node: tree_sitter.Node)` — [`L245`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/cpp_plugin.py#L245) — Get node text with optimized caching using position-based keys
  - `_parse_function_signature(self, node: tree_sitter.Node)` — [`L310`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/cpp_plugin.py#L310) — Parse C++ function signature
  - `_reset_caches(self)` — [`L216`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/cpp_plugin.py#L216) — Reset performance caches
  - `_traverse_and_extract_iterative(self, root_node: tree_sitter.Node | None, extractors: dict[str, Any], results: list[Any], element_type: str)` — [`L226`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/cpp_plugin.py#L226) — Iterative node traversal and extraction with caching
  - `extract_classes(self, tree: tree_sitter.Tree, source_code: str)` — [`L148`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/cpp_plugin.py#L148) — Extract C++ class/struct definitions with detailed information
  - `extract_functions(self, tree: tree_sitter.Tree, source_code: str)` — [`L122`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/cpp_plugin.py#L122) — Extract C++ function definitions with comprehensive details
  - `extract_imports(self, tree: tree_sitter.Tree, source_code: str)` — [`L199`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/cpp_plugin.py#L199) — Extract C++ include directives
  - `extract_packages(self, tree: tree_sitter.Tree, source_code: str)` — [`L209`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/cpp_plugin.py#L209) — Extract C++ namespace declarations
  - `extract_variables(self, tree: tree_sitter.Tree, source_code: str)` — [`L175`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/cpp_plugin.py#L175) — Extract C++ variable/field declarations
  - `content_lines` — [`L110`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/cpp_plugin.py#L110)
  - `current_file` — [`L108`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/cpp_plugin.py#L108)
  - `current_namespace` — [`L107`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/cpp_plugin.py#L107)
  - `includes` — [`L111`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/cpp_plugin.py#L111)
  - `source_code` — [`L109`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/cpp_plugin.py#L109)
- protocol/private: `_calculate_complexity_optimized`[`L457`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/cpp_plugin.py#L457), `_comment_cache`[`L118`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/cpp_plugin.py#L118), `_complexity_cache`[`L119`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/cpp_plugin.py#L119), `_determine_visibility`[`L447`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/cpp_plugin.py#L447), `_element_cache`[`L116`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/cpp_plugin.py#L116), `_extract_comment_for_line`[`L461`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/cpp_plugin.py#L461), `_extract_include_info`[`L419`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/cpp_plugin.py#L419), `_extract_includes_fallback`[`L427`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/cpp_plugin.py#L427), `_extract_namespace_info`[`L433`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/cpp_plugin.py#L433), `_file_encoding`[`L117`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/cpp_plugin.py#L117), `_get_access_specifier`[`L444`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/cpp_plugin.py#L444), `_is_global_scope`[`L441`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/cpp_plugin.py#L441), `_node_text_cache`[`L114`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/cpp_plugin.py#L114), `_processed_nodes`[`L115`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/cpp_plugin.py#L115)
- uses (calls/refs, reference-scoped): [`log_debug`](../utils/logging.md#log_debug), [`Function`](../models/base.md#Function), [`Class`](../models/base.md#Class), [`Variable`](../models/base.md#Variable), [`Import`](../models/base.md#Import), [`ElementExtractor`](../plugins/base.md#ElementExtractor), [`class_type`](../models/base.md#Class.class_type), [`extract_cpp_function`](_cpp_element_helpers.md#extract_cpp_function), [`extract_function_from_field_declaration`](_cpp_field_function_helpers.md#extract_function_from_field_declaration), [`extract_cpp_class`](_cpp_element_helpers.md#extract_cpp_class), [`safe_encode`](../encoding_utils.md#safe_encode), [`extract_text_slice`](../encoding_utils.md#extract_text_slice), [`extract_function_declaration`](_cpp_field_function_helpers.md#extract_function_declaration), [`_extract_namespace_info`](_cpp_import_namespace_helpers.md#_extract_namespace_info), [`traverse_and_extract_iterative`](_cpp_traversal_helpers.md#traverse_and_extract_iterative), [`parse_function_signature`](_cpp_signature_helpers.md#parse_function_signature), [`get_node_text_optimized`](_cpp_plugin_text_helpers.md#get_node_text_optimized), [`extract_cpp_field_declaration`](_cpp_variable_helpers.md#extract_cpp_field_declaration), [`extract_cpp_variable_declaration`](_cpp_variable_helpers.md#extract_cpp_variable_declaration), [`extract_cpp_imports`](_cpp_import_namespace_helpers.md#extract_cpp_imports), [`_extract_include_info`](_cpp_import_namespace_helpers.md#_extract_include_info), [`extract_base_classes`](_cpp_variable_helpers.md#extract_base_classes), [`extract_template_class`](_cpp_plugin_template_helpers.md#extract_template_class), [`extract_template_function`](_cpp_plugin_template_helpers.md#extract_template_function), [`CppTraversalState`](_cpp_traversal_helpers.md#CppTraversalState), [`_extract_includes_fallback`](_cpp_import_namespace_helpers.md#_extract_includes_fallback), [`extract_parameters`](_cpp_signature_helpers.md#extract_parameters), [`CppClassExtractionContext`](_cpp_element_helpers.md#CppClassExtractionContext), [`CppFieldFunctionExtractionContext`](_cpp_field_function_helpers.md#CppFieldFunctionExtractionContext), [`CppFunctionExtractionContext`](_cpp_element_helpers.md#CppFunctionExtractionContext), [`calculate_complexity`](_cpp_complexity_helpers.md#calculate_complexity), [`extract_comment_for_line`](_cpp_signature_helpers.md#extract_comment_for_line), [`extract_cpp_namespaces`](_cpp_import_namespace_helpers.md#extract_cpp_namespaces), [`get_access_specifier`](cpp_helpers.md#get_access_specifier), [`determine_visibility`](cpp_helpers.md#determine_visibility), [`current_namespace`](_cpp_element_helpers.md#CppClassExtractionContext.current_namespace), [`element_cache`](_cpp_traversal_helpers.md#CppTraversalState.element_cache), [`processed_nodes`](_cpp_traversal_helpers.md#CppTraversalState.processed_nodes), [`extractors`](_cpp_traversal_helpers.md#CppTraversalState.extractors), [`get_node_text`](_cpp_field_function_helpers.md#CppFieldFunctionExtractionContext.get_node_text)  (+17 more)
- used by: [`ElementExtractor`](../plugins/base.md#ElementExtractor), [`extract_functions`](../plugins/base.md#ElementExtractor.extract_functions), [`extract_classes`](../plugins/base.md#ElementExtractor.extract_classes), [`extract_variables`](../plugins/base.md#ElementExtractor.extract_variables), [`extract_imports`](../plugins/base.md#ElementExtractor.extract_imports), [`extract_packages`](../plugins/base.md#ElementExtractor.extract_packages), [`create_extractor`](cpp_plugin.md#CppPlugin.create_extractor), [`extractor`](cpp_plugin.md#CppPlugin.extractor)  (32 test-only)

### `CppPlugin`  ·  implements/extends LanguagePlugin
- def: [`tree_sitter_analyzer/languages/cpp_plugin.py:465`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/cpp_plugin.py#L465)
- doc: C++ language plugin implementation
- signature: `class CppPlugin(LanguagePlugin):`
- members:
  - `__init__(self)` — [`L468`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/cpp_plugin.py#L468) — Initialize the C++ language plugin.
  - `_count_tree_nodes(self, node: Any)` — [`L534`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/cpp_plugin.py#L534) — Recursively count nodes in the AST tree.
  - `analyze_file(self, file_path: str, request: AnalysisRequest)` — [`L490`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/cpp_plugin.py#L490) — Analyze C++ code and return structured results. — documented in [tree_sitter_analyzer-core-request](../../../concepts/tree_sitter_analyzer-core-request.md)
  - `create_extractor(self)` — [`L485`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/cpp_plugin.py#L485) — Create a new element extractor instance.
  - `extract_elements(self, tree: Any | None, source_code: str)` — [`L555`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/cpp_plugin.py#L555) — Extract all elements from C++ code.
  - `get_file_extensions(self)` — [`L480`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/cpp_plugin.py#L480) — Get supported file extensions.
  - `get_language_name(self)` — [`L476`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/cpp_plugin.py#L476) — Get the language name.
  - `get_tree_sitter_language(self)` — [`L546`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/cpp_plugin.py#L546) — Get the tree-sitter language for C++.
  - `extractor` — [`L471`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/cpp_plugin.py#L471)
  - `language` — [`L472`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/cpp_plugin.py#L472)
  - `supported_extensions` — [`L473`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/cpp_plugin.py#L473)
- protocol/private: `_cached_language`[`L474`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/cpp_plugin.py#L474)
- uses (calls/refs, reference-scoped): [`AnalysisResult`](../models/result.md#AnalysisResult), [`log_error`](../utils/logging.md#log_error), [`AnalysisRequest`](../core/request.md#AnalysisRequest), [`elements`](../models/result.md#AnalysisResult.elements), [`language`](../models/result.md#AnalysisResult.language), [`LanguagePlugin`](../plugins/base.md#LanguagePlugin), [`file_path`](../models/result.md#AnalysisResult.file_path), [`ElementExtractor`](../plugins/base.md#ElementExtractor), [`extract_functions`](../plugins/base.md#ElementExtractor.extract_functions), [`extract_classes`](../plugins/base.md#ElementExtractor.extract_classes), [`line_count`](../models/result.md#AnalysisResult.line_count), [`extract_variables`](../plugins/base.md#ElementExtractor.extract_variables), [`extract_imports`](../plugins/base.md#ElementExtractor.extract_imports), [`source_code`](../models/result.md#AnalysisResult.source_code), [`read_file_safe`](../encoding_utils.md#read_file_safe), [`node_count`](../models/result.md#AnalysisResult.node_count), [`CppElementExtractor`](cpp_plugin.md#CppElementExtractor), [`extract_packages`](../plugins/base.md#ElementExtractor.extract_packages), [`cpp_analysis_error_result`](_cpp_plugin_analysis_helpers.md#cpp_analysis_error_result), [`empty_cpp_analysis_result`](_cpp_plugin_analysis_helpers.md#empty_cpp_analysis_result), [`create_cpp_parser`](_cpp_plugin_analysis_helpers.md#create_cpp_parser), [`load_cpp_tree_sitter_language`](_cpp_plugin_analysis_helpers.md#load_cpp_tree_sitter_language)
- used by: [`LanguagePlugin`](../plugins/base.md#LanguagePlugin), [`get_language_name`](../plugins/base.md#LanguagePlugin.get_language_name), [`analyze_file`](../plugins/base.md#LanguagePlugin.analyze_file), [`get_file_extensions`](../plugins/base.md#LanguagePlugin.get_file_extensions), [`create_extractor`](../plugins/base.md#LanguagePlugin.create_extractor), [`get_tree_sitter_language`](../plugins/base.md#LanguagePlugin.get_tree_sitter_language)  (19 test-only)

