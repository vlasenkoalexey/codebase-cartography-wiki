---
title: 'Module: tree_sitter_analyzer/languages/python_plugin/extractor.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/python_plugin/extractor.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.python_plugin.extractor`/
symbols:
  PythonElementExtractor: PythonElementExtractor#
  PythonElementExtractor._extract_name_from_node: PythonElementExtractor#_extract_name_from_node.
  PythonElementExtractor._calculate_complexity: PythonElementExtractor#_calculate_complexity.
  PythonElementExtractor._extract_parameters_from_node: PythonElementExtractor#_extract_parameters_from_node.
  PythonElementExtractor._extract_decorators_from_node: PythonElementExtractor#_extract_decorators_from_node.
  PythonElementExtractor._extract_class_attribute_info: PythonElementExtractor#_extract_class_attribute_info.
  PythonElementExtractor._parse_simple_import: PythonElementExtractor#_parse_simple_import.
  PythonElementExtractor._parse_from_import: PythonElementExtractor#_parse_from_import.
  PythonElementExtractor._validate_node: PythonElementExtractor#_validate_node.
  PythonElementExtractor._extract_function_body: PythonElementExtractor#_extract_function_body.
  PythonElementExtractor._extract_superclasses_from_node: PythonElementExtractor#_extract_superclasses_from_node.
  __all__: __all__.
  PythonElementExtractor.__init__: PythonElementExtractor#__init__().
  PythonElementExtractor.current_module: PythonElementExtractor#current_module.
  PythonElementExtractor.current_file: PythonElementExtractor#current_file.
  PythonElementExtractor.source_code: PythonElementExtractor#source_code.
  PythonElementExtractor.content_lines: PythonElementExtractor#content_lines.
  PythonElementExtractor.imports: PythonElementExtractor#imports.
  PythonElementExtractor.exports: PythonElementExtractor#exports.
  PythonElementExtractor._node_text_cache: PythonElementExtractor#_node_text_cache.
  PythonElementExtractor._processed_nodes: PythonElementExtractor#_processed_nodes.
  PythonElementExtractor._element_cache: PythonElementExtractor#_element_cache.
  PythonElementExtractor._file_encoding: PythonElementExtractor#_file_encoding.
  PythonElementExtractor._docstring_cache: PythonElementExtractor#_docstring_cache.
  PythonElementExtractor._complexity_cache: PythonElementExtractor#_complexity_cache.
  PythonElementExtractor.is_module: PythonElementExtractor#is_module.
  PythonElementExtractor.framework_type: PythonElementExtractor#framework_type.
  PythonElementExtractor.python_version: PythonElementExtractor#python_version.
---
# Module: [`tree_sitter_analyzer/languages/python_plugin/extractor.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/extractor.py)

## Classes
### `PythonElementExtractor`  ·  implements/extends ElementExtractor, PythonClassExtractionMixin, PythonExtractorCoreMixin, PythonFunctionExtractionMixin, PythonImportPackageMixin
- def: [`tree_sitter_analyzer/languages/python_plugin/extractor.py:36`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/extractor.py#L36) — documented in [tree_sitter_analyzer-plugins-base](../../../../concepts/tree_sitter_analyzer-plugins-base.md)
- doc: Enhanced Python-specific element extractor with comprehensive feature support.
- signature: `class PythonElementExtractor(PythonFunctionExtractionMixin, PythonClassExtractionMixin, PythonImportPackageMixin, PythonExtractorCoreMixin, ElementExtractor):`
- members:
  - `__init__(self)` — [`L56`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/extractor.py#L56) — Initialize the Python element extractor.
  - `content_lines` — [`L61`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/extractor.py#L61)
  - `current_file` — [`L59`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/extractor.py#L59)
  - `current_module` — [`L58`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/extractor.py#L58)
  - `exports` — [`L63`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/extractor.py#L63)
  - `framework_type` — [`L73`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/extractor.py#L73)
  - `imports` — [`L62`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/extractor.py#L62)
  - `is_module` — [`L72`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/extractor.py#L72)
  - `python_version` — [`L74`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/extractor.py#L74)
  - `source_code` — [`L60`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/extractor.py#L60)
- protocol/private: `_calculate_complexity`[`L54`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/extractor.py#L54), `_complexity_cache`[`L70`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/extractor.py#L70), `_docstring_cache`[`L69`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/extractor.py#L69), `_element_cache`[`L67`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/extractor.py#L67), `_extract_class_attribute_info`[`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/extractor.py#L45), `_extract_decorators_from_node`[`L51`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/extractor.py#L51), `_extract_function_body`[`L52`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/extractor.py#L52), `_extract_name_from_node`[`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/extractor.py#L49), `_extract_parameters_from_node`[`L50`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/extractor.py#L50), `_extract_superclasses_from_node`[`L53`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/extractor.py#L53), `_file_encoding`[`L68`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/extractor.py#L68), `_node_text_cache`[`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/extractor.py#L65), `_parse_from_import`[`L47`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/extractor.py#L47), `_parse_simple_import`[`L46`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/extractor.py#L46), `_processed_nodes`[`L66`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/extractor.py#L66), `_validate_node`[`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/extractor.py#L48)
- uses (calls/refs, reference-scoped): [`ElementExtractor`](../../plugins/base.md#ElementExtractor), [`parse_simple_import`](_import_helpers.md#parse_simple_import), [`parse_from_import`](_import_helpers.md#parse_from_import), [`extract_class_attribute_info`](_element_builders.md#extract_class_attribute_info), [`extract_decorators_from_node`](_node_helpers.md#extract_decorators_from_node), [`extract_superclasses_from_node`](_node_helpers.md#extract_superclasses_from_node), [`PythonExtractorCoreMixin`](_core_extractor_mixin.md#PythonExtractorCoreMixin), [`extract_function_body`](_node_helpers.md#extract_function_body), [`extract_name_from_node`](_node_helpers.md#extract_name_from_node), [`extract_parameters_from_node`](_node_helpers.md#extract_parameters_from_node), [`PythonClassExtractionMixin`](_class_extractor_mixin.md#PythonClassExtractionMixin), [`PythonFunctionExtractionMixin`](_function_extractor_mixin.md#PythonFunctionExtractionMixin), [`PythonImportPackageMixin`](_import_package_mixin.md#PythonImportPackageMixin), [`calculate_complexity`](_node_helpers.md#calculate_complexity), [`validate_node`](_node_helpers.md#validate_node)
- used by: [`ElementExtractor`](../../plugins/base.md#ElementExtractor), [`TREE_SITTER_AVAILABLE`](plugin.md#TREE_SITTER_AVAILABLE), [`create_extractor`](plugin.md#PythonPlugin.create_extractor), [`get_extractor`](plugin.md#PythonPlugin.get_extractor), [`PythonExtractorCoreMixin`](_core_extractor_mixin.md#PythonExtractorCoreMixin), [`_extractor`](plugin.md#PythonPlugin._extractor), [`PythonClassExtractionMixin`](_class_extractor_mixin.md#PythonClassExtractionMixin), [`PythonFunctionExtractionMixin`](_function_extractor_mixin.md#PythonFunctionExtractionMixin), [`PythonImportPackageMixin`](_import_package_mixin.md#PythonImportPackageMixin)  (41 test-only)

## Module values
- `__all__` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/extractor.py#L26)

