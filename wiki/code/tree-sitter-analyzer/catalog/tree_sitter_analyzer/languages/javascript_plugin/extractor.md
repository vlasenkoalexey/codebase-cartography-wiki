---
title: 'Module: tree_sitter_analyzer/languages/javascript_plugin/extractor.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/javascript_plugin/extractor.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.javascript_plugin.extractor`/
symbols:
  JavaScriptElementExtractor: JavaScriptElementExtractor#
  TREE_SITTER_AVAILABLE: TREE_SITTER_AVAILABLE.
  JavaScriptElementExtractor._extract_field_definition_optimized: JavaScriptElementExtractor#_extract_field_definition_optimized().
  JavaScriptElementExtractor._extract_property_optimized: JavaScriptElementExtractor#_extract_property_optimized().
  JavaScriptElementExtractor._get_node_text_optimized: JavaScriptElementExtractor#_get_node_text_optimized().
  JavaScriptElementExtractor._extract_class_optimized: JavaScriptElementExtractor#_extract_class_optimized().
  JavaScriptElementExtractor._parse_variable_declarator: JavaScriptElementExtractor#_parse_variable_declarator().
  JavaScriptElementExtractor._reset_caches: JavaScriptElementExtractor#_reset_caches().
  JavaScriptElementExtractor._detect_file_characteristics: JavaScriptElementExtractor#_detect_file_characteristics().
  JavaScriptElementExtractor._extract_variables_from_declaration: JavaScriptElementExtractor#_extract_variables_from_declaration().
  JavaScriptElementExtractor._traverse_and_extract_iterative: JavaScriptElementExtractor#_traverse_and_extract_iterative().
  JavaScriptElementExtractor._extract_lexical_variable_optimized: JavaScriptElementExtractor#_extract_lexical_variable_optimized().
  JavaScriptElementExtractor.source_code: JavaScriptElementExtractor#source_code.
  JavaScriptElementExtractor._extract_variable_optimized: JavaScriptElementExtractor#_extract_variable_optimized().
  JavaScriptElementExtractor.framework_type: JavaScriptElementExtractor#framework_type.
  JavaScriptElementExtractor.current_file: JavaScriptElementExtractor#current_file.
  JavaScriptElementExtractor._file_encoding: JavaScriptElementExtractor#_file_encoding.
  JavaScriptElementExtractor._node_text_cache: JavaScriptElementExtractor#_node_text_cache.
  JavaScriptElementExtractor._processed_nodes: JavaScriptElementExtractor#_processed_nodes.
  JavaScriptElementExtractor._element_cache: JavaScriptElementExtractor#_element_cache.
  JavaScriptElementExtractor.content_lines: JavaScriptElementExtractor#content_lines.
  JavaScriptElementExtractor._jsdoc_cache: JavaScriptElementExtractor#_jsdoc_cache.
  JavaScriptElementExtractor._complexity_cache: JavaScriptElementExtractor#_complexity_cache.
  JavaScriptElementExtractor.is_module: JavaScriptElementExtractor#is_module.
  JavaScriptElementExtractor.is_jsx: JavaScriptElementExtractor#is_jsx.
  JavaScriptElementExtractor.__init__: JavaScriptElementExtractor#__init__().
  JavaScriptElementExtractor.imports: JavaScriptElementExtractor#imports.
  JavaScriptElementExtractor.exports: JavaScriptElementExtractor#exports.
---
# Module: [`tree_sitter_analyzer/languages/javascript_plugin/extractor.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/extractor.py)

## Classes
### `JavaScriptElementExtractor`  ·  implements/extends ElementExtractor, JavaScriptFunctionExtractionMixin, JavaScriptImportExportMixin, JavaScriptPublicExtractionMixin, JavaScriptUtilityMixin
- def: [`tree_sitter_analyzer/languages/javascript_plugin/extractor.py:37`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/extractor.py#L37)
- doc: Enhanced JavaScript-specific element extractor with comprehensive feature support
- signature: `class JavaScriptElementExtractor(JavaScriptPublicExtractionMixin, JavaScriptImportExportMixin, JavaScriptUtilityMixin, JavaScriptFunctionExtractionMixin, ElementExtractor):`
- members:
  - `__init__(self)` — [`L46`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/extractor.py#L46) — Initialize the JavaScript element extractor.
  - `_detect_file_characteristics(self)` — [`L75`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/extractor.py#L75) — Detect JavaScript file characteristics
  - `_extract_class_optimized(self, node: tree_sitter.Node)` — [`L119`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/extractor.py#L119) — Extract class information with detailed metadata
  - `_extract_field_definition_optimized(self, node: tree_sitter.Node)` — [`L190`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/extractor.py#L190) — Extract class field declaration (public and private, not arrow methods).
  - `_extract_lexical_variable_optimized(self, node: tree_sitter.Node)` — [`L134`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/extractor.py#L134) — Extract let/const declaration variables
  - `_extract_property_optimized(self, node: tree_sitter.Node)` — [`L143`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/extractor.py#L143) — Extract class property definition
  - `_extract_variable_optimized(self, node: tree_sitter.Node)` — [`L130`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/extractor.py#L130) — Extract var declaration variables
  - `_extract_variables_from_declaration(self, node: tree_sitter.Node, kind: str)` — [`L267`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/extractor.py#L267) — Extract variables from declaration node
  - `_get_node_text_optimized(self, node: tree_sitter.Node)` — [`L108`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/extractor.py#L108) — Get node text with optimized caching using position-based keys
  - `_parse_variable_declarator(self, node: tree_sitter.Node, kind: str, start_line: int, end_line: int)` — [`L291`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/extractor.py#L291) — Parse individual variable declarator
  - `_reset_caches(self)` — [`L67`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/extractor.py#L67) — Reset performance caches
  - `_traverse_and_extract_iterative(self, root_node: Optional[tree_sitter.Node], extractors: dict[str, Any], results: list[Any], element_type: str)` — [`L91`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/extractor.py#L91) — Iterative node traversal and extraction with caching
  - `content_lines` — [`L50`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/extractor.py#L50)
  - `current_file` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/extractor.py#L48)
  - `exports` — [`L52`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/extractor.py#L52)
  - `framework_type` — [`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/extractor.py#L65)
  - `imports` — [`L51`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/extractor.py#L51)
  - `is_jsx` — [`L64`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/extractor.py#L64)
  - `is_module` — [`L63`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/extractor.py#L63)
  - `source_code` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/extractor.py#L49)
- protocol/private: `_complexity_cache`[`L60`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/extractor.py#L60), `_element_cache`[`L57`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/extractor.py#L57), `_file_encoding`[`L58`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/extractor.py#L58), `_jsdoc_cache`[`L59`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/extractor.py#L59), `_node_text_cache`[`L55`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/extractor.py#L55), `_processed_nodes`[`L56`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/extractor.py#L56)
- uses (calls/refs, reference-scoped): [`name`](../../models/base.md#CodeElement.name), [`start_line`](../../models/base.md#CodeElement.start_line), [`end_line`](../../models/base.md#CodeElement.end_line), [`log_debug`](../../utils/logging.md#log_debug), [`language`](../../models/base.md#CodeElement.language), [`raw_text`](../../models/base.md#CodeElement.raw_text), [`Class`](../../models/base.md#Class), [`Variable`](../../models/base.md#Variable), [`ElementExtractor`](../../plugins/base.md#ElementExtractor), [`parse_variable_declarator`](_variable_helpers.md#parse_variable_declarator), [`extract_class`](_class_helpers.md#extract_class), [`variable_type`](../../models/base.md#Variable.variable_type), [`safe_encode`](../../encoding_utils.md#safe_encode), [`extract_text_slice`](../../encoding_utils.md#extract_text_slice), [`visibility`](../../models/base.md#Variable.visibility), [`is_constant`](../../models/base.md#Variable.is_constant), [`traverse_and_extract_iterative`](_traversal_helpers.md#traverse_and_extract_iterative), [`get_node_text_optimized`](_text_helpers.md#get_node_text_optimized), [`JavaScriptFunctionExtractionMixin`](_function_mixin.md#JavaScriptFunctionExtractionMixin), [`is_static`](../../models/base.md#Variable.is_static), [`_extract_jsdoc_for_line`](_utility_mixin.md#JavaScriptUtilityMixin._extract_jsdoc_for_line), [`initializer`](../../models/base.md#Variable.initializer), [`_infer_type_from_value`](_utility_mixin.md#JavaScriptUtilityMixin._infer_type_from_value), [`JavaScriptImportExportMixin`](_import_export_mixin.md#JavaScriptImportExportMixin), [`JavaScriptPublicExtractionMixin`](_public_extraction_mixin.md#JavaScriptPublicExtractionMixin), [`JavaScriptUtilityMixin`](_utility_mixin.md#JavaScriptUtilityMixin), [`_is_exported_class`](_utility_mixin.md#JavaScriptUtilityMixin._is_exported_class), [`_is_react_component`](_utility_mixin.md#JavaScriptUtilityMixin._is_react_component)
- used by: [`ElementExtractor`](../../plugins/base.md#ElementExtractor), [`TREE_SITTER_AVAILABLE`](plugin.md#TREE_SITTER_AVAILABLE), [`JavaScriptFunctionExtractionMixin`](_function_mixin.md#JavaScriptFunctionExtractionMixin), [`create_extractor`](plugin.md#JavaScriptPlugin.create_extractor), [`JavaScriptImportExportMixin`](_import_export_mixin.md#JavaScriptImportExportMixin), [`JavaScriptPublicExtractionMixin`](_public_extraction_mixin.md#JavaScriptPublicExtractionMixin), [`JavaScriptUtilityMixin`](_utility_mixin.md#JavaScriptUtilityMixin), [`_extractor`](plugin.md#JavaScriptPlugin._extractor)  (21 test-only)

## Module values
- `TREE_SITTER_AVAILABLE` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/extractor.py#L19)

