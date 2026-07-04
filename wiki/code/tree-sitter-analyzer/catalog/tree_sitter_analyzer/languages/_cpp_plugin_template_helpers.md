---
title: 'Module: tree_sitter_analyzer/languages/_cpp_plugin_template_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/_cpp_plugin_template_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages._cpp_plugin_template_helpers`/
symbols:
  extract_template_function: extract_template_function().
  extract_template_class: extract_template_class().
  _with_template_modifier: _with_template_modifier().
  _template_class_extractor: _template_class_extractor().
  _first_child_of_type: _first_child_of_type().
---
# Module: [`tree_sitter_analyzer/languages/_cpp_plugin_template_helpers.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_plugin_template_helpers.py)

## Functions
- `_first_child_of_type(node: Any, node_types: set[str])` — [`L41`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_plugin_template_helpers.py#L41)
- `_template_class_extractor(node_type: str, extract_class: Callable[[Any], Class | None], extract_struct: Callable[[Any], Class | None])` — [`L48`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_plugin_template_helpers.py#L48)
- `_with_template_modifier(element: Class | Function | None)` — [`L60`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_plugin_template_helpers.py#L60)
- `extract_template_class(node: Any, processed_nodes: set[int], extract_class: Callable[[Any], Class | None], extract_struct: Callable[[Any], Class | None])` — [`L23`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_plugin_template_helpers.py#L23) — Extract the class or struct definition inside a template declaration.
- `extract_template_function(node: Any, processed_nodes: set[int], extract_function: Callable[[Any], Function | None])` — [`L9`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_plugin_template_helpers.py#L9) — Extract the function definition inside a template declaration.

