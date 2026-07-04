---
title: 'Module: tree_sitter_analyzer/languages/kotlin_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/kotlin_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.kotlin_helpers`/
symbols:
  extract_kotlin_function: extract_kotlin_function().
  extract_kotlin_property: extract_kotlin_property().
  extract_kotlin_primary_constructor: extract_kotlin_primary_constructor().
  extract_kotlin_class_or_object: extract_kotlin_class_or_object().
  extract_import: extract_import().
  _kotlin_owning_type: _kotlin_owning_type().
  extract_kotlin_parameters: extract_kotlin_parameters().
  calculate_kotlin_complexity: calculate_kotlin_complexity().
  _extract_kotlin_property_modifiers: _extract_kotlin_property_modifiers().
  _kotlin_primary_ctor_class_name: _kotlin_primary_ctor_class_name().
  _refine_kotlin_class_kind: _refine_kotlin_class_kind().
  _kotlin_expression_body_type: _kotlin_expression_body_type().
  determine_visibility: determine_visibility().
  _kotlin_parameter_pair: _kotlin_parameter_pair().
  _kotlin_extension_receiver: _kotlin_extension_receiver().
  _safe_children: _safe_children().
  _KOTLIN_CLASS_KIND_MODIFIERS: _KOTLIN_CLASS_KIND_MODIFIERS.
  _extract_kotlin_delegation: _extract_kotlin_delegation().
  _extract_kotlin_property_name: _extract_kotlin_property_name().
  _KOTLIN_PROPERTY_VISIBILITY_MODIFIERS: _KOTLIN_PROPERTY_VISIBILITY_MODIFIERS.
  _KOTLIN_PROPERTY_OTHER_MODIFIERS: _KOTLIN_PROPERTY_OTHER_MODIFIERS.
  _KOTLIN_DECISION_TYPES._KOTLIN_DECISION_TYPES: _KOTLIN_DECISION_TYPES._KOTLIN_DECISION_TYPES.
  _KOTLIN_LOGIC_OP_TOKENS._KOTLIN_LOGIC_OP_TOKENS: _KOTLIN_LOGIC_OP_TOKENS._KOTLIN_LOGIC_OP_TOKENS.
---
# Module: [`tree_sitter_analyzer/languages/kotlin_helpers.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/kotlin_helpers.py)

## Functions
- `_extract_kotlin_delegation(node: Any, get_node_text: Callable[..., str])` — [`L536`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/kotlin_helpers.py#L536) — Return ``(superclass, interfaces)`` from a ``class_declaration`` node.
- `_extract_kotlin_property_modifiers(node: Any, get_node_text: Callable[..., str])` — [`L686`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/kotlin_helpers.py#L686) — Return ``(visibility, modifiers_list)`` from a property_declaration node.
- `_extract_kotlin_property_name(node: Any, get_node_text: Callable[..., str])` — [`L650`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/kotlin_helpers.py#L650) — Return the property name (val/var binding) for a Kotlin property node.
- `_kotlin_expression_body_type(node: Any, get_node_text: Callable[..., str])` — [`L238`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/kotlin_helpers.py#L238) — Infer the return type of an expression-body function (issue #591).
- `_kotlin_extension_receiver(node: Any, get_node_text: Callable[..., str])` — [`L151`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/kotlin_helpers.py#L151) — Return the extension receiver type name, or None.
- `_kotlin_owning_type(node: Any)` — [`L181`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/kotlin_helpers.py#L181) — Walk the parent chain and return ``(owner_name, is_companion)``.
- `_kotlin_parameter_pair(parameter_node: Any, get_node_text: Callable[..., str])` — [`L125`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/kotlin_helpers.py#L125) — Return ``(name, type)`` from a Kotlin ``parameter`` AST node.
- `_kotlin_primary_ctor_class_name(node: Any, get_node_text: Callable[..., str])` — [`L432`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/kotlin_helpers.py#L432) — Return the enclosing class name for a ``primary_constructor`` node.
- `_refine_kotlin_class_kind(node: Any, get_node_text: Callable[..., str])` — [`L520`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/kotlin_helpers.py#L520) — Return the declaration kind from the class_modifier, if any.
- `_safe_children(node: Any)` — [`L295`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/kotlin_helpers.py#L295) — Return children list from a tree-sitter node, empty list on any error.
- `calculate_kotlin_complexity(node: Any)` — [`L306`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/kotlin_helpers.py#L306) — Return cyclomatic complexity for a Kotlin function node.
- `determine_visibility(modifiers_text: str)` — [`L73`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/kotlin_helpers.py#L73) — Determine visibility from Kotlin modifiers text.
- `extract_import(node: Any, get_node_text: Callable[..., str])` — [`L10`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/kotlin_helpers.py#L10) — Extract a Kotlin import statement.
- `extract_kotlin_class_or_object(node: Any, kind: str, get_node_text: Callable[..., str], current_package: str)` — [`L583`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/kotlin_helpers.py#L583) — Extract Kotlin class/object/interface declaration.
- `extract_kotlin_function(node: Any, get_node_text: Callable[..., str], current_package: str)` — [`L328`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/kotlin_helpers.py#L328) — Extract Kotlin function declaration. — documented in [tree_sitter_analyzer-models-base](../../../concepts/tree_sitter_analyzer-models-base.md)
- `extract_kotlin_parameters(node: Any, get_node_text: Callable[..., str])` — [`L84`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/kotlin_helpers.py#L84) — Extract Kotlin function parameters.
- `extract_kotlin_primary_constructor(node: Any, get_node_text: Callable[..., str], current_package: str)` — [`L455`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/kotlin_helpers.py#L455) — Extract a Kotlin ``primary_constructor`` as a Function(is_constructor=True).
- `extract_kotlin_property(node: Any, get_node_text: Callable[..., str])` — [`L720`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/kotlin_helpers.py#L720) — Extract Kotlin property declaration.

## Module values
- `_KOTLIN_CLASS_KIND_MODIFIERS` — [`L517`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/kotlin_helpers.py#L517)
- `_KOTLIN_DECISION_TYPES` — [`L281`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/kotlin_helpers.py#L281)
- `_KOTLIN_LOGIC_OP_TOKENS` — [`L292`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/kotlin_helpers.py#L292)
- `_KOTLIN_PROPERTY_OTHER_MODIFIERS` — [`L681`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/kotlin_helpers.py#L681)
- `_KOTLIN_PROPERTY_VISIBILITY_MODIFIERS` — [`L678`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/kotlin_helpers.py#L678)

