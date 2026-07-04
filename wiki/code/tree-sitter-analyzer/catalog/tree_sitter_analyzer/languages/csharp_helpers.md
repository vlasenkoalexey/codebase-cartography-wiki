---
title: 'Module: tree_sitter_analyzer/languages/csharp_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/csharp_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.csharp_helpers`/
symbols:
  extract_class_declaration: extract_class_declaration().
  extract_method_declaration: extract_method_declaration().
  extract_field_declaration: extract_field_declaration().
  extract_event_declaration: extract_event_declaration().
  extract_property_declaration: extract_property_declaration().
  extract_constructor_declaration: extract_constructor_declaration().
  extract_using_directive: extract_using_directive().
  determine_visibility: determine_visibility().
  extract_attributes: extract_attributes().
  extract_modifiers: extract_modifiers().
  calculate_complexity: calculate_complexity().
  extract_parameters: extract_parameters().
  extract_type_name: extract_type_name().
  find_owning_class_name: find_owning_class_name().
  _find_variable_declaration: _find_variable_declaration().
  _iter_variable_declarators: _iter_variable_declarators().
  _apply_interface_implicit_public: _apply_interface_implicit_public().
  _extract_declarator_name: _extract_declarator_name().
  _CSHARP_NON_EXECUTABLE_ANCHORS: _CSHARP_NON_EXECUTABLE_ANCHORS.
  _OWNING_TYPE_NODES: _OWNING_TYPE_NODES.
  _CLASS_TYPE_MAP: _CLASS_TYPE_MAP.
  _BASE_TYPE_NODES: _BASE_TYPE_NODES.
  _ACCESS_MODIFIERS: _ACCESS_MODIFIERS.
---
# Module: [`tree_sitter_analyzer/languages/csharp_helpers.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_helpers.py)

## Functions
- `_apply_interface_implicit_public(node: Any, modifiers: list[str], visibility: str)` — [`L220`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_helpers.py#L220) — C# interface members without an explicit access modifier are public.
- `_extract_declarator_name(declarator: Any, get_node_text: Callable[..., str])` — [`L452`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_helpers.py#L452)
- `_find_variable_declaration(node: Any)` — [`L437`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_helpers.py#L437)
- `_iter_variable_declarators(variable_declaration: Any | None)` — [`L444`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_helpers.py#L444)
- `calculate_complexity(node: Any, traverse_fn: Callable[..., Iterator])` — [`L97`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_helpers.py#L97) — Calculate cyclomatic complexity.
- `determine_visibility(modifiers: list[str])` — [`L45`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_helpers.py#L45) — Determine visibility from C# modifiers.
- `extract_attributes(node: Any, get_node_text: Callable[..., str], attribute_cache: dict[tuple[int, int], list[dict[str, Any]]])` — [`L124`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_helpers.py#L124) — Extract attributes (annotations) from a node's direct children.
- `extract_class_declaration(node: Any, current_namespace: str, get_node_text: Callable[..., str], extract_modifiers_fn: Callable[[Any], list[str]], extract_attributes_fn: Callable[[Any], list[dict[str, Any]]])` — [`L239`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_helpers.py#L239) — Extract a single class declaration. — documented in [tree_sitter_analyzer-languages-csharp_plugin](../../../concepts/tree_sitter_analyzer-languages-csharp_plugin.md)
- `extract_constructor_declaration(node: Any, get_node_text: Callable[..., str], extract_modifiers_fn: Callable[[Any], list[str]], extract_attributes_fn: Callable[[Any], list[dict[str, Any]]], extract_params_fn: Callable[[Any], list[str]])` — [`L353`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_helpers.py#L353) — Extract a constructor declaration.
- `extract_event_declaration(node: Any, get_node_text: Callable[..., str], extract_modifiers_fn: Callable[[Any], list[str]], extract_attributes_fn: Callable[[Any], list[dict[str, Any]]], extract_type_fn: Callable[[Any], str])` — [`L512`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_helpers.py#L512) — Extract event field declarations. — documented in [tree_sitter_analyzer-languages-csharp_plugin](../../../concepts/tree_sitter_analyzer-languages-csharp_plugin.md)
- `extract_field_declaration(node: Any, get_node_text: Callable[..., str], extract_modifiers_fn: Callable[[Any], list[str]], extract_attributes_fn: Callable[[Any], list[dict[str, Any]]], extract_type_fn: Callable[[Any], str])` — [`L463`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_helpers.py#L463) — Extract field declarations. — documented in [tree_sitter_analyzer-languages-csharp_plugin](../../../concepts/tree_sitter_analyzer-languages-csharp_plugin.md)
- `extract_method_declaration(node: Any, get_node_text: Callable[..., str], extract_modifiers_fn: Callable[[Any], list[str]], extract_attributes_fn: Callable[[Any], list[dict[str, Any]]], extract_type_fn: Callable[[Any], str], extract_params_fn: Callable[[Any], list[str]], calc_complexity_fn: Callable[[Any], int])` — [`L300`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_helpers.py#L300) — Extract a method declaration. — documented in [tree_sitter_analyzer-languages-csharp_plugin](../../../concepts/tree_sitter_analyzer-languages-csharp_plugin.md)
- `extract_modifiers(node: Any, get_node_text: Callable[..., str])` — [`L85`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_helpers.py#L85) — Extract modifiers from a declaration node.
- `extract_parameters(params_node: Any, get_node_text: Callable[..., str])` — [`L59`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_helpers.py#L59) — Extract method parameters.
- `extract_property_declaration(node: Any, get_node_text: Callable[..., str], extract_modifiers_fn: Callable[[Any], list[str]], extract_attributes_fn: Callable[[Any], list[dict[str, Any]]], extract_type_fn: Callable[[Any], str])` — [`L394`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_helpers.py#L394) — Extract a property declaration. — documented in [tree_sitter_analyzer-languages-csharp_plugin](../../../concepts/tree_sitter_analyzer-languages-csharp_plugin.md)
- `extract_type_name(type_node: Any, get_node_text: Callable[..., str])` — [`L74`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_helpers.py#L74) — Extract type name from a type node.
- `extract_using_directive(node: Any, get_node_text: Callable[..., str])` — [`L166`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_helpers.py#L166) — Extract a using directive. — documented in [tree_sitter_analyzer-languages-csharp_plugin](../../../concepts/tree_sitter_analyzer-languages-csharp_plugin.md)
- `find_owning_class_name(node: Any, get_node_text: Callable[..., str])` — [`L27`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_helpers.py#L27) — Walk up node.parent to find the enclosing class/interface/struct/record.

## Module values
- `_ACCESS_MODIFIERS` — [`L217`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_helpers.py#L217)
- `_BASE_TYPE_NODES` — [`L215`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_helpers.py#L215)
- `_CLASS_TYPE_MAP` — [`L207`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_helpers.py#L207)
- `_CSHARP_NON_EXECUTABLE_ANCHORS` — [`L12`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_helpers.py#L12)
- `_OWNING_TYPE_NODES` — [`L16`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/csharp_helpers.py#L16)

