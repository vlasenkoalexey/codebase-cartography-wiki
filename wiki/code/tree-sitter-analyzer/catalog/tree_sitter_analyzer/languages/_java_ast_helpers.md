---
title: 'Module: tree_sitter_analyzer/languages/_java_ast_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/_java_ast_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages._java_ast_helpers`/
symbols:
  parse_method_signature: parse_method_signature().
  _count_decision_nodes: _count_decision_nodes().
  parse_field_declaration: parse_field_declaration().
  extract_modifiers: extract_modifiers().
  calculate_complexity: calculate_complexity().
  _extract_modifier_tokens: _extract_modifier_tokens().
  _modifier_token: _modifier_token().
  _extract_formal_parameters: _extract_formal_parameters().
  _extract_variable_names: _extract_variable_names().
  _first_child_text: _first_child_text().
  _MODIFIER_KEYWORDS: _MODIFIER_KEYWORDS.
  _RETURN_TYPE_NODES: _RETURN_TYPE_NODES.
  _FIELD_TYPE_NODES: _FIELD_TYPE_NODES.
  _JAVA_DECISION_NODES: _JAVA_DECISION_NODES.
  _JAVA_LOGICAL_OPERATORS: _JAVA_LOGICAL_OPERATORS.
  _JAVA_NON_EXECUTABLE_ANCHORS: _JAVA_NON_EXECUTABLE_ANCHORS.
  _formal_parameter_texts: _formal_parameter_texts().
  _extract_throws: _extract_throws().
  _variable_declarator_names: _variable_declarator_names().
  _safe_children: _safe_children().
---
# Module: [`tree_sitter_analyzer/languages/_java_ast_helpers.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_java_ast_helpers.py)

## Functions
- `_count_decision_nodes(node: Any)` — [`L215`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_java_ast_helpers.py#L215)
- `_extract_formal_parameters(node: Any, get_node_text: Callable[..., str])` — [`L167`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_java_ast_helpers.py#L167)
- `_extract_modifier_tokens(modifiers_node: Any, get_node_text: Callable[..., str])` — [`L135`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_java_ast_helpers.py#L135)
- `_extract_throws(node: Any, get_node_text: Callable[..., str])` — [`L188`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_java_ast_helpers.py#L188)
- `_extract_variable_names(node: Any, get_node_text: Callable[..., str])` — [`L196`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_java_ast_helpers.py#L196)
- `_first_child_text(node: Any, child_types: frozenset[str] | set[str], get_node_text: Callable[..., str])` — [`L156`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_java_ast_helpers.py#L156)
- `_formal_parameter_texts(parameters_node: Any, get_node_text: Callable[..., str])` — [`L177`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_java_ast_helpers.py#L177)
- `_modifier_token(node: Any, get_node_text: Callable[..., str])` — [`L147`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_java_ast_helpers.py#L147)
- `_safe_children(node: Any)` — [`L230`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_java_ast_helpers.py#L230)
- `_variable_declarator_names(declarator_node: Any, get_node_text: Callable[..., str])` — [`L204`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_java_ast_helpers.py#L204)
- `calculate_complexity(node: Any)` — [`L130`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_java_ast_helpers.py#L130) — Calculate cyclomatic complexity.
- `extract_modifiers(node: Any, get_node_text: Callable[..., str])` — [`L77`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_java_ast_helpers.py#L77) — Extract modifiers from a declaration node.
- `parse_field_declaration(node: Any, get_node_text: Callable[..., str])` — [`L110`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_java_ast_helpers.py#L110) — Parse field declaration into (type, variable_names, modifiers).
- `parse_method_signature(node: Any, get_node_text: Callable[..., str])` — [`L87`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_java_ast_helpers.py#L87) — Parse method signature into (name, return_type, parameters, modifiers, throws).

## Module values
- `_FIELD_TYPE_NODES` — [`L36`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_java_ast_helpers.py#L36)
- `_JAVA_DECISION_NODES` — [`L53`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_java_ast_helpers.py#L53)
- `_JAVA_LOGICAL_OPERATORS` — [`L71`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_java_ast_helpers.py#L71)
- `_JAVA_NON_EXECUTABLE_ANCHORS` — [`L72`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_java_ast_helpers.py#L72)
- `_MODIFIER_KEYWORDS` — [`L9`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_java_ast_helpers.py#L9)
- `_RETURN_TYPE_NODES` — [`L23`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_java_ast_helpers.py#L23)

