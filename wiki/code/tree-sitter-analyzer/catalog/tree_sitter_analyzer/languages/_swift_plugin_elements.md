---
title: 'Module: tree_sitter_analyzer/languages/_swift_plugin_elements.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/_swift_plugin_elements.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages._swift_plugin_elements`/
symbols:
  extract_swift_variable: extract_swift_variable().
  extract_swift_class: extract_swift_class().
  extract_swift_function: extract_swift_function().
  extract_swift_import: extract_swift_import().
  _swift_function: _swift_function().
  _swift_function_fields: _swift_function_fields().
  _swift_class: _swift_class().
  _swift_variable: _swift_variable().
  _parameter_names: _parameter_names().
  _swift_calculate_complexity: _swift_calculate_complexity().
  _swift_class_fields: _swift_class_fields().
  _swift_type_fields: _swift_type_fields().
  _function_name: _function_name().
  _swift_function_flags: _swift_function_flags().
  _swift_variable_fields: _swift_variable_fields().
  _swift_import_fields: _swift_import_fields().
  _parameter: _parameter().
  _return_type: _return_type().
  _safe_children: _safe_children().
  _parameter_clause: _parameter_clause().
  _split_top_level: _split_top_level().
  _parameter_name: _parameter_name().
  _param_list_end: _param_list_end().
  _import_module_path: _import_module_path().
  _has_word: _has_word().
  _SWIFT_DECISION_NODE_TYPES._SWIFT_DECISION_NODE_TYPES: _SWIFT_DECISION_NODE_TYPES._SWIFT_DECISION_NODE_TYPES.
---
# Module: [`tree_sitter_analyzer/languages/_swift_plugin_elements.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_swift_plugin_elements.py)

## Functions
- `_function_name(extractor: Any, node: tree_sitter.Node)` — [`L144`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_swift_plugin_elements.py#L144)
- `_has_word(raw_text: str, word: str)` — [`L411`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_swift_plugin_elements.py#L411)
- `_import_module_path(raw_text: str)` — [`L404`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_swift_plugin_elements.py#L404)
- `_param_list_end(raw_text: str)` — [`L387`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_swift_plugin_elements.py#L387) — Index of the parameter list's matching closing paren, or -1.
- `_parameter(parameter_text: str)` — [`L343`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_swift_plugin_elements.py#L343) — Render a Swift parameter as ``name: Type`` (mirrors Rust).
- `_parameter_clause(raw_text: str)` — [`L300`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_swift_plugin_elements.py#L300) — Return the text inside the parameter parentheses, matched with
- `_parameter_name(before_type: str)` — [`L360`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_swift_plugin_elements.py#L360)
- `_parameter_names(raw_text: str)` — [`L293`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_swift_plugin_elements.py#L293)
- `_return_type(raw_text: str)` — [`L368`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_swift_plugin_elements.py#L368) — Extract a Swift return type, including bracket/tuple-led types.
- `_safe_children(node: object)` — [`L52`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_swift_plugin_elements.py#L52) — Return children list from a tree-sitter node, empty list on any error.
- `_split_top_level(text: str)` — [`L318`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_swift_plugin_elements.py#L318) — Split on commas that sit outside any (), [], or <> nesting, so a
- `_swift_calculate_complexity(node: object)` — [`L63`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_swift_plugin_elements.py#L63) — Return cyclomatic complexity for a Swift function node.
- `_swift_class(node: tree_sitter.Node, raw_text: str, name: str, declaration_kind: str, modifiers: list[str])` — [`L193`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_swift_plugin_elements.py#L193)
- `_swift_class_fields(node: tree_sitter.Node, raw_text: str, name: str, declaration_kind: str, modifiers: list[str], inherited: list[str], parent_type: str | None)` — [`L214`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_swift_plugin_elements.py#L214)
- `_swift_function(node: tree_sitter.Node, raw_text: str, name: str, modifiers: list[str])` — [`L150`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_swift_plugin_elements.py#L150)
- `_swift_function_fields(node: tree_sitter.Node, raw_text: str, modifiers: list[str], found_visibility: str)` — [`L162`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_swift_plugin_elements.py#L162)
- `_swift_function_flags(modifiers: list[str], raw_text: str, found_visibility: str)` — [`L179`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_swift_plugin_elements.py#L179)
- `_swift_import_fields(node: tree_sitter.Node, raw_text: str, module_path: str)` — [`L275`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_swift_plugin_elements.py#L275)
- `_swift_type_fields(declaration_kind: str, modifiers: list[str], inherited: list[str], parent_type: str | None, name: str)` — [`L229`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_swift_plugin_elements.py#L229)
- `_swift_variable(node: tree_sitter.Node, raw_text: str, name: str, annotation: str | None, modifiers: list[str], binding: str)` — [`L246`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_swift_plugin_elements.py#L246)
- `_swift_variable_fields(annotation: str | None, modifiers: list[str], is_constant: bool)` — [`L260`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_swift_plugin_elements.py#L260)
- `extract_swift_class(extractor: Any, node: tree_sitter.Node)` — [`L98`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_swift_plugin_elements.py#L98) — Extract one Swift type declaration.
- `extract_swift_function(extractor: Any, node: tree_sitter.Node)` — [`L83`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_swift_plugin_elements.py#L83) — Extract one Swift function-like declaration.
- `extract_swift_import(extractor: Any, node: tree_sitter.Node)` — [`L133`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_swift_plugin_elements.py#L133) — Extract one Swift import declaration.
- `extract_swift_variable(extractor: Any, node: tree_sitter.Node)` — [`L115`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_swift_plugin_elements.py#L115) — Extract one Swift property declaration.

## Module values
- `_SWIFT_DECISION_NODE_TYPES` — [`L36`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_swift_plugin_elements.py#L36)

