---
title: 'Module: tree_sitter_analyzer/languages/python_plugin/_node_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/python_plugin/_node_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.python_plugin._node_helpers`/
symbols:
  extract_decorators_from_node: extract_decorators_from_node().
  extract_superclasses_from_node: extract_superclasses_from_node().
  _extract_parameter_children: _extract_parameter_children().
  extract_name_from_node: extract_name_from_node().
  extract_parameters_from_node: extract_parameters_from_node().
  extract_function_body: extract_function_body().
  _extract_superclass_arguments: _extract_superclass_arguments().
  _source_text: _source_text().
  validate_node: validate_node().
  calculate_complexity: calculate_complexity().
  _PARAMETER_NODE_TYPES: _PARAMETER_NODE_TYPES.
  _normalize_decorator_text: _normalize_decorator_text().
---
# Module: [`tree_sitter_analyzer/languages/python_plugin/_node_helpers.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_node_helpers.py)

## Functions
- `_extract_parameter_children(parameters_node: Any, source_code: str)` — [`L44`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_node_helpers.py#L44)
- `_extract_superclass_arguments(argument_list_node: Any, source_code: str)` — [`L83`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_node_helpers.py#L83)
- `_normalize_decorator_text(decorator_text: str)` — [`L103`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_node_helpers.py#L103)
- `_source_text(node: Any, source_code: str)` — [`L109`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_node_helpers.py#L109)
- `calculate_complexity(body: str)` — [`L94`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_node_helpers.py#L94) — Calculate simplified cyclomatic complexity.
- `extract_decorators_from_node(node: Any, source_code: str)` — [`L53`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_node_helpers.py#L53) — Extract decorators from a node.
- `extract_function_body(node: Any, source_code: str)` — [`L66`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_node_helpers.py#L66) — Extract a function body from a function node.
- `extract_name_from_node(node: Any, source_code: str)` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_node_helpers.py#L27) — Extract a node identifier name.
- `extract_parameters_from_node(node: Any, source_code: str)` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_node_helpers.py#L35) — Extract function parameters from a node.
- `extract_superclasses_from_node(node: Any, source_code: str)` — [`L74`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_node_helpers.py#L74) — Extract superclass names from a class node.
- `validate_node(node: Any)` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_node_helpers.py#L18) — Validate that a node has required attributes.

## Module values
- `_PARAMETER_NODE_TYPES` — [`L9`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_node_helpers.py#L9)

