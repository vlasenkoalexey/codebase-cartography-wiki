---
title: 'Module: tree_sitter_analyzer/languages/java_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/java_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.java_helpers`/
symbols:
  extract_java_class: extract_java_class().
  extract_java_method: extract_java_method().
  extract_java_field: extract_java_field().
  java_traverse_and_extract: java_traverse_and_extract().
  determine_visibility: determine_visibility().
  find_parent_class: find_parent_class().
  extract_class_name: extract_class_name().
  extract_javadoc_for_line: extract_javadoc_for_line().
  is_nested_class: is_nested_class().
  _find_parent_class_node: _find_parent_class_node().
  extract_annotation: extract_annotation().
  _first_child_text: _first_child_text().
  _CLASS_DECLARATION_NODES: _CLASS_DECLARATION_NODES.
  __all__: __all__.
---
# Module: [`tree_sitter_analyzer/languages/java_helpers.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/java_helpers.py)

## Functions
- `_find_parent_class_node(node: Any)` — [`L103`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/java_helpers.py#L103)
- `_first_child_text(node: Any, child_types: frozenset[str] | set[str], get_node_text: Callable[..., str])` — [`L125`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/java_helpers.py#L125)
- `determine_visibility(modifiers: list[str])` — [`L75`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/java_helpers.py#L75) — Determine visibility from Java modifiers.
- `extract_annotation(node: Any, get_node_text: Callable[..., str])` — [`L137`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/java_helpers.py#L137) — Extract annotation information from annotation node.
- `extract_class_name(node: Any, get_node_text: Callable[..., str])` — [`L113`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/java_helpers.py#L113) — Extract class name from a class declaration node.
- `extract_java_class(node: Any, get_node_text: Callable[..., str], content_lines: list[str], current_package: str, extract_modifiers: Callable, determine_visibility: Callable, find_annotations_for_line: Callable, is_nested_class: Callable, find_parent_class: Callable)` — [`L203`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/java_helpers.py#L203) — Extract Java class/interface/enum information.
- `extract_java_field(node: Any, get_node_text: Callable[..., str], content_lines: list[str], parse_field_declaration: Callable, determine_visibility: Callable, find_annotations_for_line: Callable, extract_javadoc: Callable)` — [`L257`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/java_helpers.py#L257) — Extract Java field declarations.
- `extract_java_method(node: Any, get_node_text: Callable[..., str], content_lines: list[str], parse_method_signature: Callable, determine_visibility: Callable, find_annotations_for_line: Callable, calculate_complexity: Callable, extract_javadoc: Callable)` — [`L231`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/java_helpers.py#L231) — Extract Java method/constructor information.
- `extract_javadoc_for_line(line: int, content_lines: list[str])` — [`L171`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/java_helpers.py#L171) — Extract JavaDoc comment for a specific line.
- `find_parent_class(node: Any, get_node_text: Callable[..., str])` — [`L92`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/java_helpers.py#L92) — Find parent class name for nested classes.
- `is_nested_class(node: Any)` — [`L86`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/java_helpers.py#L86) — Check if a node is inside a class/interface/enum declaration.
- `java_traverse_and_extract(root_node: Any, extractors: dict[str, Any], results: list[Any], element_type: str, processed_nodes: set[int], element_cache: dict[tuple[int, str], Any])` — [`L181`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/java_helpers.py#L181) — Iterative node traversal and extraction with batch field processing.

## Module values
- `_CLASS_DECLARATION_NODES` — [`L66`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/java_helpers.py#L66)
- `__all__` — [`L42`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/java_helpers.py#L42)

