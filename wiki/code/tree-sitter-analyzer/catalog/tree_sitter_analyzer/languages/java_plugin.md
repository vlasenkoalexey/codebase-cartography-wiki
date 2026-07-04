---
title: 'Module: tree_sitter_analyzer/languages/java_plugin.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/java_plugin.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.java_plugin`/Java
symbols:
  JavaElementExtractor: ElementExtractor#
  JavaPlugin.analyze_file: Plugin#analyze_file().
  JavaPlugin: Plugin#
  JavaElementExtractor.extract_classes: ElementExtractor#extract_classes().
  JavaElementExtractor._extract_class_optimized: ElementExtractor#_extract_class_optimized().
  JavaElementExtractor._get_node_text_optimized: ElementExtractor#_get_node_text_optimized().
  JavaElementExtractor._extract_method_optimized: ElementExtractor#_extract_method_optimized().
  JavaElementExtractor.extract_variables: ElementExtractor#extract_variables().
  JavaElementExtractor.extract_annotations: ElementExtractor#extract_annotations().
  JavaElementExtractor.extract_functions: ElementExtractor#extract_functions().
  JavaPlugin._analyze_sync: Plugin#_analyze_sync().
  JavaElementExtractor._extract_field_optimized: ElementExtractor#_extract_field_optimized().
  JavaPlugin.extract_elements: Plugin#extract_elements().
  JavaElementExtractor._reset_caches: ElementExtractor#_reset_caches().
  JavaElementExtractor.extract_packages: ElementExtractor#extract_packages().
  JavaElementExtractor.extract_imports: ElementExtractor#extract_imports().
  JavaElementExtractor.content_lines: ElementExtractor#content_lines.
  JavaPlugin.create_extractor: Plugin#create_extractor().
  JavaElementExtractor._traverse_and_extract_iterative: ElementExtractor#_traverse_and_extract_iterative().
  JavaPlugin.get_tree_sitter_language: Plugin#get_tree_sitter_language().
  JavaElementExtractor._extract_package_info: ElementExtractor#_extract_package_info().
  JavaElementExtractor._extract_import_info: ElementExtractor#_extract_import_info().
  JavaElementExtractor._find_annotations_for_line_cached: ElementExtractor#_find_annotations_for_line_cached().
  JavaElementExtractor._process_field_batch: ElementExtractor#_process_field_batch().
  JavaElementExtractor._extract_package_element: ElementExtractor#_extract_package_element().
  JavaElementExtractor.source_code: ElementExtractor#source_code.
  JavaElementExtractor._extract_annotation_optimized: ElementExtractor#_extract_annotation_optimized().
  JavaElementExtractor._extract_javadoc_for_line: ElementExtractor#_extract_javadoc_for_line().
  JavaElementExtractor._extract_class_name: ElementExtractor#_extract_class_name().
  JavaElementExtractor.current_package: ElementExtractor#current_package.
  JavaElementExtractor._parse_method_signature_optimized: ElementExtractor#_parse_method_signature_optimized().
  JavaElementExtractor._parse_field_declaration_optimized: ElementExtractor#_parse_field_declaration_optimized().
  JavaElementExtractor._extract_modifiers_optimized: ElementExtractor#_extract_modifiers_optimized().
  JavaElementExtractor._find_parent_class: ElementExtractor#_find_parent_class().
  JavaElementExtractor._determine_visibility: ElementExtractor#_determine_visibility().
  JavaElementExtractor._calculate_complexity_optimized: ElementExtractor#_calculate_complexity_optimized().
  JavaElementExtractor.annotations: ElementExtractor#annotations.
  JavaElementExtractor._annotation_cache: ElementExtractor#_annotation_cache.
  JavaElementExtractor._node_text_cache: ElementExtractor#_node_text_cache.
  JavaElementExtractor._extract_imports_fallback: ElementExtractor#_extract_imports_fallback().
  JavaPlugin._cached_language: Plugin#_cached_language.
  JavaElementExtractor._file_encoding: ElementExtractor#_file_encoding.
  JavaElementExtractor._extract_package_from_tree: ElementExtractor#_extract_package_from_tree().
  JavaElementExtractor._is_nested_class: ElementExtractor#_is_nested_class().
  JavaElementExtractor._processed_nodes: ElementExtractor#_processed_nodes.
  JavaElementExtractor._element_cache: ElementExtractor#_element_cache.
  JavaPlugin.get_language_name: Plugin#get_language_name().
  JavaPlugin.get_file_extensions: Plugin#get_file_extensions().
  JavaPlugin.extractor: Plugin#extractor.
  JavaPlugin.supported_extensions: Plugin#supported_extensions.
  JavaPlugin._count_tree_nodes: Plugin#_count_tree_nodes().
  JavaElementExtractor.current_file: ElementExtractor#current_file.
  JavaElementExtractor.imports: ElementExtractor#imports.
  JavaElementExtractor._signature_cache: ElementExtractor#_signature_cache.
  JavaElementExtractor.__init__: ElementExtractor#__init__().
  JavaPlugin.__init__: Plugin#__init__().
  JavaPlugin.language: Plugin#language.
---
# Module: [`tree_sitter_analyzer/languages/java_plugin.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/java_plugin.py)

## Classes
### `JavaElementExtractor`  ·  implements/extends ElementExtractor
- def: [`tree_sitter_analyzer/languages/java_plugin.py:75`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/java_plugin.py#L75) — documented in [tree_sitter_analyzer-plugins-base](../../../concepts/tree_sitter_analyzer-plugins-base.md)
- doc: Java-specific element extractor with AdvancedAnalyzer implementation
- signature: `class JavaElementExtractor(ElementExtractor):`
- members:
  - `__init__(self)` — [`L78`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/java_plugin.py#L78) — Initialize the Java element extractor.
  - `_calculate_complexity_optimized(self, node: tree_sitter.Node)` — [`L458`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/java_plugin.py#L458) — Calculate cyclomatic complexity optimized
  - `_determine_visibility(self, modifiers: list[str])` — [`L430`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/java_plugin.py#L430) — Determine visibility from modifiers
  - `_extract_annotation_optimized(self, node: tree_sitter.Node)` — [`L424`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/java_plugin.py#L424) — Extract annotation information optimized
  - `_extract_class_name(self, node: tree_sitter.Node)` — [`L468`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/java_plugin.py#L468) — Extract class name from a class declaration node.
  - `_extract_class_optimized(self, node: tree_sitter.Node)` — [`L329`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/java_plugin.py#L329) — Extract class information optimized
  - `_extract_field_optimized(self, node: tree_sitter.Node)` — [`L358`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/java_plugin.py#L358) — Extract field information optimized
  - `_extract_import_info(self, node: tree_sitter.Node, source_code: str)` — [`L415`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/java_plugin.py#L415) — Extract import information from import declaration node
  - `_extract_imports_fallback(self, source_code: str)` — [`L221`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/java_plugin.py#L221) — Fallback import extraction using regex when tree-sitter fails
  - `_extract_javadoc_for_line(self, line: int)` — [`L463`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/java_plugin.py#L463) — Extract JavaDoc comment for a specific line
  - `_extract_method_optimized(self, node: tree_sitter.Node)` — [`L344`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/java_plugin.py#L344) — Extract method information optimized
  - `_extract_modifiers_optimized(self, node: tree_sitter.Node)` — [`L385`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/java_plugin.py#L385) — Extract modifiers efficiently (from AdvancedAnalyzer)
  - `_extract_package_element(self, node: tree_sitter.Node)` — [`L399`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/java_plugin.py#L399) — Extract package element for inclusion in results
  - `_extract_package_from_tree(self, tree: tree_sitter.Tree)` — [`L406`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/java_plugin.py#L406) — Extract package information from tree when needed
  - `_extract_package_info(self, node: tree_sitter.Node)` — [`L390`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/java_plugin.py#L390) — Extract package information
  - `_find_annotations_for_line_cached(self, line: int)` — [`L435`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/java_plugin.py#L435) — Find annotations for a specific line with caching
  - `_find_parent_class(self, node: tree_sitter.Node)` — [`L454`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/java_plugin.py#L454) — Find parent class name for nested classes
  - `_get_node_text_optimized(self, node: tree_sitter.Node)` — [`L279`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/java_plugin.py#L279) — Get node text with optimized caching using position-based keys
  - `_is_nested_class(self, node: tree_sitter.Node)` — [`L449`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/java_plugin.py#L449) — Check if this is a nested class
  - `_parse_field_declaration_optimized(self, node: tree_sitter.Node)` — [`L378`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/java_plugin.py#L378) — Parse field declaration optimized (from AdvancedAnalyzer)
  - `_parse_method_signature_optimized(self, node: tree_sitter.Node)` — [`L371`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/java_plugin.py#L371) — Parse method signature optimized (from AdvancedAnalyzer)
  - `_process_field_batch(self, batch: list[tree_sitter.Node], extractors: dict, results: list[Any])` — [`L269`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/java_plugin.py#L269) — Process field nodes with caching — delegated to helper.
  - `_reset_caches(self)` — [`L239`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/java_plugin.py#L239) — Reset performance caches
  - `_traverse_and_extract_iterative(self, root_node: tree_sitter.Node | None, extractors: dict[str, Any], results: list[Any], element_type: str)` — [`L251`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/java_plugin.py#L251) — Iterative node traversal and extraction with batch processing
  - `extract_annotations(self, tree: tree_sitter.Tree, source_code: str)` — [`L98`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/java_plugin.py#L98) — Extract Java annotations using AdvancedAnalyzer implementation
  - `extract_classes(self, tree: tree_sitter.Tree, source_code: str)` — [`L149`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/java_plugin.py#L149) — Extract Java class definitions using AdvancedAnalyzer implementation
  - `extract_functions(self, tree: tree_sitter.Tree, source_code: str)` — [`L125`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/java_plugin.py#L125) — Extract Java method definitions using AdvancedAnalyzer implementation
  - `extract_imports(self, tree: tree_sitter.Tree, source_code: str)` — [`L208`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/java_plugin.py#L208) — Extract Java import statements with enhanced robustness
  - `extract_packages(self, tree: tree_sitter.Tree, source_code: str)` — [`L228`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/java_plugin.py#L228) — Extract Java package declarations
  - `extract_variables(self, tree: tree_sitter.Tree, source_code: str)` — [`L182`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/java_plugin.py#L182) — Extract Java field definitions using AdvancedAnalyzer implementation
  - `annotations` — [`L95`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/java_plugin.py#L95)
  - `content_lines` — [`L83`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/java_plugin.py#L83)
  - `current_file` — [`L81`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/java_plugin.py#L81)
  - `current_package` — [`L80`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/java_plugin.py#L80)
  - `imports` — [`L84`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/java_plugin.py#L84)
  - `source_code` — [`L82`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/java_plugin.py#L82)
- protocol/private: `_annotation_cache`[`L91`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/java_plugin.py#L91), `_element_cache`[`L89`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/java_plugin.py#L89), `_file_encoding`[`L90`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/java_plugin.py#L90), `_node_text_cache`[`L87`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/java_plugin.py#L87), `_processed_nodes`[`L88`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/java_plugin.py#L88), `_signature_cache`[`L92`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/java_plugin.py#L92)
- uses (calls/refs, reference-scoped): [`name`](../models/base.md#CodeElement.name), [`log_debug`](../utils/logging.md#log_debug), [`Function`](../models/base.md#Function), [`log_error`](../utils/logging.md#log_error), [`Class`](../models/base.md#Class), [`Variable`](../models/base.md#Variable), [`Import`](../models/base.md#Import), [`ElementExtractor`](../plugins/base.md#ElementExtractor), [`Package`](../models/base.md#Package), [`variable_type`](../models/base.md#Variable.variable_type), [`safe_encode`](../encoding_utils.md#safe_encode), [`extract_text_slice`](../encoding_utils.md#extract_text_slice), [`_extract_package_element`](_java_import_helpers.md#_extract_package_element), [`extract_java_imports`](_java_import_helpers.md#extract_java_imports), [`parse_method_signature`](_java_ast_helpers.md#parse_method_signature), [`parse_field_declaration`](_java_ast_helpers.md#parse_field_declaration), [`extract_java_class`](java_helpers.md#extract_java_class), [`extract_java_field`](java_helpers.md#extract_java_field), [`extract_java_method`](java_helpers.md#extract_java_method), [`_extract_import_info`](_java_import_helpers.md#_extract_import_info), [`extract_java_packages`](_java_import_helpers.md#extract_java_packages), [`java_traverse_and_extract`](java_helpers.md#java_traverse_and_extract), [`_extract_imports_fallback`](_java_import_helpers.md#_extract_imports_fallback), [`_extract_package_name`](_java_import_helpers.md#_extract_package_name), [`determine_visibility`](java_helpers.md#determine_visibility), [`extract_modifiers`](_java_ast_helpers.md#extract_modifiers), [`extract_class_name`](java_helpers.md#extract_class_name), [`extract_javadoc_for_line`](java_helpers.md#extract_javadoc_for_line), [`find_parent_class`](java_helpers.md#find_parent_class), [`_process_field_batch`](_java_traversal_helpers.md#_process_field_batch), [`calculate_complexity`](_java_ast_helpers.md#calculate_complexity), [`extract_annotation`](java_helpers.md#extract_annotation), [`is_nested_class`](java_helpers.md#is_nested_class)  (1 test-only)
- used by: [`ElementExtractor`](../plugins/base.md#ElementExtractor), [`extract_functions`](../plugins/base.md#ElementExtractor.extract_functions), [`extract_classes`](../plugins/base.md#ElementExtractor.extract_classes), [`extract_variables`](../plugins/base.md#ElementExtractor.extract_variables), [`extract_imports`](../plugins/base.md#ElementExtractor.extract_imports), [`extract_packages`](../plugins/base.md#ElementExtractor.extract_packages), [`create_extractor`](java_plugin.md#JavaPlugin.create_extractor), [`extract_annotations`](../plugins/base.md#ElementExtractor.extract_annotations), [`extractor`](java_plugin.md#JavaPlugin.extractor)  (44 test-only)

### `JavaPlugin`  ·  implements/extends LanguagePlugin
- def: [`tree_sitter_analyzer/languages/java_plugin.py:473`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/java_plugin.py#L473) — documented in [tree_sitter_analyzer-plugins-manager](../../../concepts/tree_sitter_analyzer-plugins-manager.md)
- doc: Java language plugin implementation
- signature: `class JavaPlugin(LanguagePlugin):`
- members:
  - `__init__(self)` — [`L476`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/java_plugin.py#L476) — Initialize the Java language plugin.
  - `_count_tree_nodes(self, node: Any)` — [`L595`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/java_plugin.py#L595) — Recursively count nodes in the AST tree (Deprecated: use iterative version).
  - `analyze_file(self, file_path: str, request: AnalysisRequest)` — [`L500`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/java_plugin.py#L500) — Analyze Java code and return structured results. — documented in [tree_sitter_analyzer-models-result](../../../concepts/tree_sitter_analyzer-models-result.md)
  - `create_extractor(self)` — [`L495`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/java_plugin.py#L495) — Create a new element extractor instance.
  - `extract_elements(self, tree: Any | None, source_code: str)` — [`L639`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/java_plugin.py#L639) — Extract all elements from Java code for test compatibility.
  - `get_file_extensions(self)` — [`L490`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/java_plugin.py#L490) — Get supported file extensions.
  - `get_language_name(self)` — [`L486`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/java_plugin.py#L486) — Get the language name.
  - `get_tree_sitter_language(self)` — [`L603`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/java_plugin.py#L603) — Get the tree-sitter language for Java.
  - `extractor` — [`L479`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/java_plugin.py#L479)
  - `language` — [`L480`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/java_plugin.py#L480)
  - `supported_extensions` — [`L481`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/java_plugin.py#L481)
- protocol/private: `_analyze_sync`[`L528`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/java_plugin.py#L528), `_cached_language`[`L484`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/java_plugin.py#L484)
- uses (calls/refs, reference-scoped): [`AnalysisResult`](../models/result.md#AnalysisResult), [`log_error`](../utils/logging.md#log_error), [`AnalysisRequest`](../core/request.md#AnalysisRequest), [`elements`](../models/result.md#AnalysisResult.elements), [`language`](../models/result.md#AnalysisResult.language), [`LanguagePlugin`](../plugins/base.md#LanguagePlugin), [`file_path`](../models/result.md#AnalysisResult.file_path), [`success`](../models/result.md#AnalysisResult.success), [`ElementExtractor`](../plugins/base.md#ElementExtractor), [`extract_functions`](../plugins/base.md#ElementExtractor.extract_functions), [`extract_classes`](../plugins/base.md#ElementExtractor.extract_classes), [`line_count`](../models/result.md#AnalysisResult.line_count), [`extract_variables`](../plugins/base.md#ElementExtractor.extract_variables), [`error_message`](../models/result.md#AnalysisResult.error_message), [`extract_imports`](../plugins/base.md#ElementExtractor.extract_imports), [`JavaElementExtractor`](java_plugin.md#JavaElementExtractor), [`source_code`](../models/result.md#AnalysisResult.source_code), [`node_count`](../models/result.md#AnalysisResult.node_count), [`extract_packages`](../plugins/base.md#ElementExtractor.extract_packages), [`read_file_safe_async`](../encoding_utils.md#read_file_safe_async), [`package`](../models/result.md#AnalysisResult.package), [`count_nodes_iterative`](../utils/tree_sitter_compat.md#count_nodes_iterative), [`extract_annotations`](../plugins/base.md#ElementExtractor.extract_annotations), [`set_file_encoding`](../plugins/base.md#ElementExtractor.set_file_encoding)
- used by: [`LanguagePlugin`](../plugins/base.md#LanguagePlugin), [`get_language_name`](../plugins/base.md#LanguagePlugin.get_language_name), [`analyze_file`](../plugins/base.md#LanguagePlugin.analyze_file), [`get_file_extensions`](../plugins/base.md#LanguagePlugin.get_file_extensions), [`create_extractor`](../plugins/base.md#LanguagePlugin.create_extractor), [`get_tree_sitter_language`](../plugins/base.md#LanguagePlugin.get_tree_sitter_language)  (26 test-only)

