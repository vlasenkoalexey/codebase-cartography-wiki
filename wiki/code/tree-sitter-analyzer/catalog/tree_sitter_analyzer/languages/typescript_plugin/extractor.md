---
title: 'Module: tree_sitter_analyzer/languages/typescript_plugin/extractor.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/typescript_plugin/extractor.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.typescript_plugin.extractor`/T
symbols:
  TREE_SITTER_AVAILABLE: REE_SITTER_AVAILABLE.
  TypeScriptElementExtractor._get_node_text_optimized: ypeScriptElementExtractor#_get_node_text_optimized().
  TypeScriptElementExtractor: ypeScriptElementExtractor#
  TypeScriptElementExtractor.extract_functions: ypeScriptElementExtractor#extract_functions().
  TypeScriptElementExtractor.extract_classes: ypeScriptElementExtractor#extract_classes().
  TypeScriptElementExtractor.extract_variables: ypeScriptElementExtractor#extract_variables().
  TypeScriptElementExtractor._extract_tsdoc_for_line: ypeScriptElementExtractor#_extract_tsdoc_for_line().
  TypeScriptElementExtractor._extract_class_optimized: ypeScriptElementExtractor#_extract_class_optimized().
  TypeScriptElementExtractor._extract_function_optimized: ypeScriptElementExtractor#_extract_function_optimized().
  TypeScriptElementExtractor.source_code: ypeScriptElementExtractor#source_code.
  TypeScriptElementExtractor._extract_arrow_function_optimized: ypeScriptElementExtractor#_extract_arrow_function_optimized().
  TypeScriptElementExtractor._extract_method_optimized: ypeScriptElementExtractor#_extract_method_optimized().
  TypeScriptElementExtractor._extract_generator_function_optimized: ypeScriptElementExtractor#_extract_generator_function_optimized().
  TypeScriptElementExtractor._extract_interface_optimized: ypeScriptElementExtractor#_extract_interface_optimized().
  TypeScriptElementExtractor._extract_type_alias_optimized: ypeScriptElementExtractor#_extract_type_alias_optimized().
  TypeScriptElementExtractor.framework_type: ypeScriptElementExtractor#framework_type.
  TypeScriptElementExtractor._extract_namespace_optimized: ypeScriptElementExtractor#_extract_namespace_optimized().
  TypeScriptElementExtractor._detect_file_characteristics: ypeScriptElementExtractor#_detect_file_characteristics().
  TypeScriptElementExtractor._extract_method_signature_optimized: ypeScriptElementExtractor#_extract_method_signature_optimized().
  TypeScriptElementExtractor._extract_abstract_method_signature_optimized: ypeScriptElementExtractor#_extract_abstract_method_signature_optimized().
  TypeScriptElementExtractor._extract_enum_optimized: ypeScriptElementExtractor#_extract_enum_optimized().
  TypeScriptElementExtractor._reset_caches: ypeScriptElementExtractor#_reset_caches().
  TypeScriptElementExtractor._extract_variables_from_declaration: ypeScriptElementExtractor#_extract_variables_from_declaration().
  TypeScriptElementExtractor.extract_imports: ypeScriptElementExtractor#extract_imports().
  TypeScriptElementExtractor._parse_variable_declarator: ypeScriptElementExtractor#_parse_variable_declarator().
  TypeScriptElementExtractor._parse_method_signature_optimized: ypeScriptElementExtractor#_parse_method_signature_optimized().
  TypeScriptElementExtractor.extract_elements: ypeScriptElementExtractor#extract_elements().
  TypeScriptElementExtractor._parse_function_signature_optimized: ypeScriptElementExtractor#_parse_function_signature_optimized().
  TypeScriptElementExtractor._infer_type_from_value: ypeScriptElementExtractor#_infer_type_from_value().
  TypeScriptElementExtractor._calculate_complexity_optimized: ypeScriptElementExtractor#_calculate_complexity_optimized().
  TypeScriptElementExtractor._extract_lexical_variable_optimized: ypeScriptElementExtractor#_extract_lexical_variable_optimized().
  TypeScriptElementExtractor._is_framework_component: ypeScriptElementExtractor#_is_framework_component().
  TypeScriptElementExtractor._traverse_and_extract_iterative: ypeScriptElementExtractor#_traverse_and_extract_iterative().
  TypeScriptElementExtractor._extract_import_info_simple: ypeScriptElementExtractor#_extract_import_info_simple().
  TypeScriptElementExtractor._is_exported_class: ypeScriptElementExtractor#_is_exported_class().
  TypeScriptElementExtractor._extract_variable_optimized: ypeScriptElementExtractor#_extract_variable_optimized().
  TypeScriptElementExtractor._extract_public_field_optimized: ypeScriptElementExtractor#_extract_public_field_optimized().
  TypeScriptElementExtractor._extract_property_optimized: ypeScriptElementExtractor#_extract_property_optimized().
  TypeScriptElementExtractor._extract_property_signature_optimized: ypeScriptElementExtractor#_extract_property_signature_optimized().
  TypeScriptElementExtractor._extract_import_names: ypeScriptElementExtractor#_extract_import_names().
  TypeScriptElementExtractor.content_lines: ypeScriptElementExtractor#content_lines.
  TypeScriptElementExtractor._extract_parameters_with_types: ypeScriptElementExtractor#_extract_parameters_with_types().
  TypeScriptElementExtractor._extract_generics: ypeScriptElementExtractor#_extract_generics().
  TypeScriptElementExtractor._extract_dynamic_import: ypeScriptElementExtractor#_extract_dynamic_import().
  TypeScriptElementExtractor._extract_commonjs_requires: ypeScriptElementExtractor#_extract_commonjs_requires().
  TypeScriptElementExtractor._clean_tsdoc: ypeScriptElementExtractor#_clean_tsdoc().
  TypeScriptElementExtractor.is_module: ypeScriptElementExtractor#is_module.
  TypeScriptElementExtractor.current_file: ypeScriptElementExtractor#current_file.
  TypeScriptElementExtractor.is_tsx: ypeScriptElementExtractor#is_tsx.
  TypeScriptElementExtractor._node_text_cache: ypeScriptElementExtractor#_node_text_cache.
  TypeScriptElementExtractor._processed_nodes: ypeScriptElementExtractor#_processed_nodes.
  TypeScriptElementExtractor._element_cache: ypeScriptElementExtractor#_element_cache.
  TypeScriptElementExtractor._tsdoc_cache: ypeScriptElementExtractor#_tsdoc_cache.
  TypeScriptElementExtractor._complexity_cache: ypeScriptElementExtractor#_complexity_cache.
  TypeScriptElementExtractor._is_inside_function_body: ypeScriptElementExtractor#_is_inside_function_body().
  TypeScriptElementExtractor.imports: ypeScriptElementExtractor#imports.
  TypeScriptElementExtractor.exports: ypeScriptElementExtractor#exports.
  TypeScriptElementExtractor._file_encoding: ypeScriptElementExtractor#_file_encoding.
  TypeScriptElementExtractor.__init__: ypeScriptElementExtractor#__init__().
  TypeScriptElementExtractor.typescript_version: ypeScriptElementExtractor#typescript_version.
---
# Module: [`tree_sitter_analyzer/languages/typescript_plugin/extractor.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/extractor.py)

## Classes
### `TypeScriptElementExtractor`  ·  implements/extends ElementExtractor
- def: [`tree_sitter_analyzer/languages/typescript_plugin/extractor.py:75`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/extractor.py#L75)
- doc: Enhanced TypeScript-specific element extractor with comprehensive feature support
- signature: `class TypeScriptElementExtractor(ElementExtractor):`
- members:
  - `__init__(self)` — [`L78`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/extractor.py#L78) — Initialize the TypeScript element extractor.
  - `_calculate_complexity_optimized(self, node: tree_sitter.Node)` — [`L565`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/extractor.py#L565) — Calculate cyclomatic complexity efficiently
  - `_clean_tsdoc(self, tsdoc_text: str)` — [`L561`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/extractor.py#L561) — Clean TSDoc text by removing comment markers
  - `_detect_file_characteristics(self)` — [`L210`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/extractor.py#L210) — Detect TypeScript file characteristics
  - `_extract_abstract_method_signature_optimized(self, node: tree_sitter.Node)` — [`L303`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/extractor.py#L303) — Extract abstract method signature from an abstract class (preserves visibility).
  - `_extract_arrow_function_optimized(self, node: tree_sitter.Node)` — [`L267`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/extractor.py#L267) — Extract arrow function information
  - `_extract_class_optimized(self, node: tree_sitter.Node)` — [`L328`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/extractor.py#L328) — Extract class information with detailed metadata
  - `_extract_enum_optimized(self, node: tree_sitter.Node)` — [`L362`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/extractor.py#L362) — Extract enum information
  - `_extract_function_optimized(self, node: tree_sitter.Node)` — [`L256`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/extractor.py#L256) — Extract regular function information with detailed metadata
  - `_extract_generator_function_optimized(self, node: tree_sitter.Node)` — [`L315`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/extractor.py#L315) — Extract generator function information
  - `_extract_generics(self, type_params_node: tree_sitter.Node)` — [`L500`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/extractor.py#L500) — Extract generic type parameters
  - `_extract_import_info_simple(self, node: tree_sitter.Node)` — [`L511`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/extractor.py#L511) — Extract import information from an import_statement node.
  - `_extract_interface_optimized(self, node: tree_sitter.Node)` — [`L340`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/extractor.py#L340) — Extract interface information
  - `_extract_lexical_variable_optimized(self, node: tree_sitter.Node)` — [`L399`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/extractor.py#L399) — Extract let/const declaration variables (top-level / class-body only).
  - `_extract_method_optimized(self, node: tree_sitter.Node)` — [`L280`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/extractor.py#L280) — Extract method information from class
  - `_extract_method_signature_optimized(self, node: tree_sitter.Node)` — [`L291`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/extractor.py#L291) — Extract method signature information from interfaces
  - `_extract_namespace_optimized(self, node: tree_sitter.Node)` — [`L372`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/extractor.py#L372) — Extract namespace/module container information
  - `_extract_parameters_with_types(self, params_node: tree_sitter.Node)` — [`L494`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/extractor.py#L494) — Extract function parameters with TypeScript type annotations
  - `_extract_property_optimized(self, node: tree_sitter.Node)` — [`L422`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/extractor.py#L422) — Extract class property definition
  - `_extract_property_signature_optimized(self, node: tree_sitter.Node)` — [`L426`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/extractor.py#L426) — Extract property signature from interface
  - `_extract_public_field_optimized(self, node: tree_sitter.Node)` — [`L410`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/extractor.py#L410) — Extract a class member declaration (public_field_definition node).
  - `_extract_tsdoc_for_line(self, target_line: int)` — [`L552`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/extractor.py#L552) — Extract TSDoc comment immediately before the specified line
  - `_extract_type_alias_optimized(self, node: tree_sitter.Node)` — [`L351`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/extractor.py#L351) — Extract type alias information
  - `_extract_variable_optimized(self, node: tree_sitter.Node)` — [`L393`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/extractor.py#L393) — Extract var declaration variables (top-level / class-body only).
  - `_extract_variables_from_declaration(self, node: tree_sitter.Node, kind: str)` — [`L432`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/extractor.py#L432) — Extract variables from declaration node
  - `_get_node_text_optimized(self, node: tree_sitter.Node)` — [`L245`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/extractor.py#L245) — Get node text with optimized caching using position-based keys
  - `_infer_type_from_value(self, value: str | None)` — [`L548`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/extractor.py#L548) — Infer TypeScript type from value
  - `_is_exported_class(self, class_name: str)` — [`L544`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/extractor.py#L544) — Check if class is exported
  - `_is_framework_component(self, node: tree_sitter.Node, class_name: str)` — [`L536`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/extractor.py#L536) — Check if class is a framework component
  - `_is_inside_function_body(node: tree_sitter.Node)` — [`L383`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/extractor.py#L383) — Return True when node is a direct child of a function/method body.
  - `_parse_function_signature_optimized(self, node: tree_sitter.Node)` — [`L458`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/extractor.py#L458) — Parse function signature for TypeScript functions
  - `_parse_method_signature_optimized(self, node: tree_sitter.Node)` — [`L469`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/extractor.py#L469) — Parse method signature for TypeScript class methods
  - `_parse_variable_declarator(self, node: tree_sitter.Node, kind: str, start_line: int, end_line: int)` — [`L444`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/extractor.py#L444) — Parse individual variable declarator with TypeScript type annotations
  - `_reset_caches(self)` — [`L202`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/extractor.py#L202) — Reset performance caches
  - `_traverse_and_extract_iterative(self, root_node: Optional[tree_sitter.Node], extractors: dict[str, Any], results: list[Any], element_type: str)` — [`L228`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/extractor.py#L228) — Iterative node traversal and extraction with caching
  - `extract_classes(self, tree: tree_sitter.Tree, source_code: str)` — [`L132`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/extractor.py#L132) — Extract TypeScript class and interface definitions with detailed information
  - `extract_elements(self, tree: tree_sitter.Tree, source_code: str)` — [`L571`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/extractor.py#L571) — Legacy method for backward compatibility with tests
  - `extract_functions(self, tree: tree_sitter.Tree, source_code: str)` — [`L100`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/extractor.py#L100) — Extract TypeScript function definitions with comprehensive details
  - `extract_imports(self, tree: tree_sitter.Tree, source_code: str)` — [`L192`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/extractor.py#L192) — Extract TypeScript import statements with ES6+ and type import support
  - `extract_variables(self, tree: tree_sitter.Tree, source_code: str)` — [`L162`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/extractor.py#L162) — Extract TypeScript variable definitions with type annotations
  - `content_lines` — [`L82`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/extractor.py#L82)
  - `current_file` — [`L80`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/extractor.py#L80)
  - `exports` — [`L84`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/extractor.py#L84)
  - `framework_type` — [`L97`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/extractor.py#L97)
  - `imports` — [`L83`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/extractor.py#L83)
  - `is_module` — [`L95`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/extractor.py#L95)
  - `is_tsx` — [`L96`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/extractor.py#L96)
  - `source_code` — [`L81`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/extractor.py#L81)
  - `typescript_version` — [`L98`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/extractor.py#L98)
- protocol/private: `_complexity_cache`[`L92`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/extractor.py#L92), `_element_cache`[`L89`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/extractor.py#L89), `_extract_commonjs_requires`[`L529`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/extractor.py#L529), `_extract_dynamic_import`[`L526`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/extractor.py#L526), `_extract_import_names`[`L519`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/extractor.py#L519), `_file_encoding`[`L90`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/extractor.py#L90), `_node_text_cache`[`L87`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/extractor.py#L87), `_processed_nodes`[`L88`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/extractor.py#L88), `_tsdoc_cache`[`L91`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/extractor.py#L91)
- uses (calls/refs, reference-scoped): [`log_debug`](../../utils/logging.md#log_debug), [`Function`](../../models/base.md#Function), [`Class`](../../models/base.md#Class), [`Variable`](../../models/base.md#Variable), [`Import`](../../models/base.md#Import), [`CodeElement`](../../models/base.md#CodeElement), [`ElementExtractor`](../../plugins/base.md#ElementExtractor), [`extract_class`](_class_helpers.md#extract_class), [`extract_method`](_function_helpers.md#extract_method), [`extract_arrow_function`](_function_helpers.md#extract_arrow_function), [`extract_abstract_method_signature`](_function_helpers.md#extract_abstract_method_signature), [`extract_generator_function`](_function_helpers.md#extract_generator_function), [`extract_function`](_function_helpers.md#extract_function), [`extract_method_signature`](_function_helpers.md#extract_method_signature), [`extract_property`](_variable_helpers.md#extract_property), [`parse_variable_declarator`](_variable_helpers.md#parse_variable_declarator), [`extract_interface`](_class_helpers.md#extract_interface), [`parse_method_signature`](_signature_helpers.md#parse_method_signature), [`safe_encode`](../../encoding_utils.md#safe_encode), [`extract_namespace`](_class_helpers.md#extract_namespace), [`extract_text_slice`](../../encoding_utils.md#extract_text_slice), [`extract_type_alias`](_class_helpers.md#extract_type_alias), [`extract_enum`](_class_helpers.md#extract_enum), [`extract_import_info_simple`](_import_info_helpers.md#extract_import_info_simple), [`_extract_dynamic_import`](import_extractor.md#_extract_dynamic_import), [`extract_property_signature`](_variable_helpers.md#extract_property_signature), [`parse_function_signature`](_signature_helpers.md#parse_function_signature), [`traverse_and_extract_iterative`](_traversal_helpers.md#traverse_and_extract_iterative), [`extract_ts_imports`](import_extractor.md#extract_ts_imports), [`extract_tsdoc_for_line`](_tsdoc_helpers.md#extract_tsdoc_for_line), [`get_node_text_optimized`](_text_helpers.md#get_node_text_optimized), [`_extract_commonjs_requires`](import_extractor.md#_extract_commonjs_requires), [`extract_variables_from_declaration`](_variable_helpers.md#extract_variables_from_declaration), [`_extract_import_names`](import_extractor.md#_extract_import_names), [`is_exported_class`](_variable_helpers.md#is_exported_class), [`calculate_complexity`](_text_helpers.md#calculate_complexity), [`extract_parameters_with_types`](_parameter_helpers.md#extract_parameters_with_types), [`clean_tsdoc`](_tsdoc_helpers.md#clean_tsdoc), [`is_framework_component`](_variable_helpers.md#is_framework_component), [`infer_type_from_value`](_variable_helpers.md#infer_type_from_value)
- used by: [`ElementExtractor`](../../plugins/base.md#ElementExtractor), [`extract_functions`](../../plugins/base.md#ElementExtractor.extract_functions), [`extract_classes`](../../plugins/base.md#ElementExtractor.extract_classes), [`extract_variables`](../../plugins/base.md#ElementExtractor.extract_variables), [`extract_imports`](../../plugins/base.md#ElementExtractor.extract_imports), [`extract_elements`](../../plugins/base.md#ElementExtractor.extract_elements), [`TREE_SITTER_AVAILABLE`](plugin.md#TREE_SITTER_AVAILABLE), [`create_extractor`](plugin.md#TypeScriptPlugin.create_extractor), [`_extractor`](plugin.md#TypeScriptPlugin._extractor)  (21 test-only)

## Module values
- `TREE_SITTER_AVAILABLE` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/extractor.py#L19) — documented in [tree_sitter_analyzer-plugins-base](../../../../concepts/tree_sitter_analyzer-plugins-base.md)

