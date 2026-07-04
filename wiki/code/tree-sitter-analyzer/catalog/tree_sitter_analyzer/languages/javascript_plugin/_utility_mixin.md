---
title: 'Module: tree_sitter_analyzer/languages/javascript_plugin/_utility_mixin.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/javascript_plugin/_utility_mixin.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.javascript_plugin._utility_mixin`/JavaScriptUtilityMixin#
symbols:
  JavaScriptUtilityMixin._extract_jsdoc_for_line: _extract_jsdoc_for_line().
  JavaScriptUtilityMixin._infer_type_from_value: _infer_type_from_value().
  JavaScriptUtilityMixin._calculate_complexity_optimized: _calculate_complexity_optimized().
  JavaScriptUtilityMixin: ''
  JavaScriptUtilityMixin._clean_jsdoc: _clean_jsdoc().
  JavaScriptUtilityMixin._is_react_component: _is_react_component().
  JavaScriptUtilityMixin._is_exported_class: _is_exported_class().
  JavaScriptUtilityMixin._find_parent_class_name: _find_parent_class_name().
  JavaScriptUtilityMixin._get_variable_kind: _get_variable_kind().
---
# Module: [`tree_sitter_analyzer/languages/javascript_plugin/_utility_mixin.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_utility_mixin.py)

## Classes
### `JavaScriptUtilityMixin`
- def: [`tree_sitter_analyzer/languages/javascript_plugin/_utility_mixin.py:16`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_utility_mixin.py#L16)
- doc: Small compatibility methods shared by JavaScript extraction helpers.
- signature: `class JavaScriptUtilityMixin:`
- members:
  - `_calculate_complexity_optimized(self, node: tree_sitter.Node)` — [`L82`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_utility_mixin.py#L82) — Calculate cyclomatic complexity efficiently.
  - `_clean_jsdoc(self, jsdoc_text: str)` — [`L78`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_utility_mixin.py#L78) — Clean JSDoc text by removing comment markers.
  - `_extract_jsdoc_for_line(self, target_line: int)` — [`L69`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_utility_mixin.py#L69) — Extract JSDoc comment immediately before the specified line.
  - `_find_parent_class_name(self, node: tree_sitter.Node)` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_utility_mixin.py#L20) — Find parent class name for methods/properties.
  - `_get_variable_kind(self, var_data: dict | str)` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_utility_mixin.py#L49) — Get variable declaration kind from variable data or raw text.
  - `_infer_type_from_value(self, value: str | None)` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_utility_mixin.py#L45) — Infer JavaScript type from value.
  - `_is_exported_class(self, class_name: str)` — [`L41`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_utility_mixin.py#L41) — Check if class is exported.
  - `_is_react_component(self, node: tree_sitter.Node, class_name: str)` — [`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_utility_mixin.py#L31) — Check if class is a React component.
- uses (calls/refs, reference-scoped): [`log_debug`](../../utils/logging.md#log_debug), [`JavaScriptElementExtractor`](extractor.md#JavaScriptElementExtractor), [`extract_jsdoc_for_line`](_jsdoc_helpers.md#extract_jsdoc_for_line), [`count_decision_complexity`](../_complexity_decisions.md#count_decision_complexity), [`clean_jsdoc`](_jsdoc_helpers.md#clean_jsdoc), [`infer_type_from_value`](_variable_helpers.md#infer_type_from_value)
- used by: [`JavaScriptElementExtractor`](extractor.md#JavaScriptElementExtractor), [`TREE_SITTER_AVAILABLE`](extractor.md#TREE_SITTER_AVAILABLE), [`_extract_field_definition_optimized`](extractor.md#JavaScriptElementExtractor._extract_field_definition_optimized), [`_extract_property_optimized`](extractor.md#JavaScriptElementExtractor._extract_property_optimized), [`_extract_class_optimized`](extractor.md#JavaScriptElementExtractor._extract_class_optimized), [`_parse_variable_declarator`](extractor.md#JavaScriptElementExtractor._parse_variable_declarator)

