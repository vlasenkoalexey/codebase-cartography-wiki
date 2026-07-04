---
title: 'Module: tree_sitter_analyzer/languages/php_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/php_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.php_helpers`/
symbols:
  extract_php_method_element: extract_php_method_element().
  extract_php_function_element: extract_php_function_element().
  extract_php_class_element: extract_php_class_element().
  _build_php_property_variable: _build_php_property_variable().
  _build_php_constant_variable: _build_php_constant_variable().
  _build_use_clause_import: _build_use_clause_import().
  extract_php_property_elements: extract_php_property_elements().
  extract_php_constant_elements: extract_php_constant_elements().
  extract_use_statement: extract_use_statement().
  calculate_php_complexity: calculate_php_complexity().
  determine_visibility: determine_visibility().
  extract_modifiers: extract_modifiers().
  extract_attributes: extract_attributes().
  _safe_children: _safe_children().
  _collect_php_attribute_list: _collect_php_attribute_list().
  _collect_php_class_bases: _collect_php_class_bases().
  _PHP_DECISION_TYPES._PHP_DECISION_TYPES: _PHP_DECISION_TYPES._PHP_DECISION_TYPES.
  _PHP_LOGIC_OP_TOKENS._PHP_LOGIC_OP_TOKENS: _PHP_LOGIC_OP_TOKENS._PHP_LOGIC_OP_TOKENS.
---
# Module: [`tree_sitter_analyzer/languages/php_helpers.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/php_helpers.py)

## Functions
- `_build_php_constant_variable(const_node: Any, element_node: Any, parent_class: str, get_node_text: Callable[..., str], modifiers: list[str], visibility: str)` — [`L516`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/php_helpers.py#L516) — Build a ``Variable`` from one ``const_element`` AST child.
- `_build_php_property_variable(property_node: Any, element_node: Any, parent_class: str, get_node_text: Callable[..., str], modifiers: list[str], visibility: str, var_type: str)` — [`L459`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/php_helpers.py#L459) — Build a ``Variable`` from one ``property_element`` AST child.
- `_build_use_clause_import(use_node: Any, clause_node: Any, get_node_text: Callable[..., str], prefix: str = "")` — [`L181`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/php_helpers.py#L181) — Build one ``Import`` from a ``namespace_use_clause`` node.
- `_collect_php_attribute_list(attribute_list_node: Any, get_node_text: Callable[..., str], attributes: list[dict[str, Any]])` — [`L114`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/php_helpers.py#L114) — Walk one ``attribute_list`` node, appending each attribute name.
- `_collect_php_class_bases(node: Any, get_node_text: Callable[..., str])` — [`L221`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/php_helpers.py#L221) — Return ``(base_classes, interfaces)`` from a PHP class declaration.
- `_safe_children(node: Any)` — [`L30`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/php_helpers.py#L30) — Return children list from a tree-sitter node, empty list on any error.
- `calculate_php_complexity(node: Any)` — [`L41`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/php_helpers.py#L41) — Return cyclomatic complexity for a PHP function or method node.
- `determine_visibility(modifiers: list[str])` — [`L64`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/php_helpers.py#L64) — Determine visibility from PHP modifiers.
- `extract_attributes(node: Any, get_node_text: Callable[..., str], attribute_cache: dict[tuple[int, int], list[dict[str, Any]]])` — [`L95`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/php_helpers.py#L95) — Extract PHP 8+ attributes from a node.
- `extract_modifiers(node: Any, get_node_text: Callable[..., str])` — [`L76`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/php_helpers.py#L76) — Extract modifiers from a PHP declaration node.
- `extract_php_class_element(node: Any, current_namespace: str, get_node_text: Callable[..., str], extract_modifiers_fn: Callable[[Any], list[str]], extract_attributes_fn: Callable[[Any], list[dict[str, Any]]])` — [`L256`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/php_helpers.py#L256) — Extract a single PHP class, interface, trait, or enum element.
- `extract_php_constant_elements(node: Any, parent_class: str, get_node_text: Callable[..., str], extract_modifiers_fn: Callable[[Any], list[str]])` — [`L491`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/php_helpers.py#L491) — Extract PHP constant elements.
- `extract_php_function_element(node: Any, current_namespace: str, get_node_text: Callable[..., str])` — [`L374`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/php_helpers.py#L374) — Extract a PHP function element.
- `extract_php_method_element(node: Any, parent_class: str, get_node_text: Callable[..., str], extract_modifiers_fn: Callable[[Any], list[str]], extract_attributes_fn: Callable[[Any], list[dict[str, Any]]])` — [`L318`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/php_helpers.py#L318) — Extract a PHP method element.
- `extract_php_property_elements(node: Any, parent_class: str, get_node_text: Callable[..., str], extract_modifiers_fn: Callable[[Any], list[str]])` — [`L425`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/php_helpers.py#L425) — Extract PHP property elements.
- `extract_use_statement(node: Any, get_node_text: Callable[..., str])` — [`L138`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/php_helpers.py#L138) — Extract use statement elements from a ``namespace_use_declaration``.

## Module values
- `_PHP_DECISION_TYPES` — [`L13`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/php_helpers.py#L13)
- `_PHP_LOGIC_OP_TOKENS` — [`L27`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/php_helpers.py#L27)

