---
title: 'Module: tree_sitter_analyzer/languages/_java_element_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/_java_element_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages._java_element_helpers`/
symbols:
  extract_java_method: extract_java_method().
  _build_java_class: _build_java_class().
  _build_java_field: _build_java_field().
  extract_java_class: extract_java_class().
  extract_java_field: extract_java_field().
  _split_respecting_generics: _split_respecting_generics().
  _extract_class_relationships: _extract_class_relationships().
  _build_java_fields: _build_java_fields().
  extract_javadoc_for_line: extract_javadoc_for_line().
  _extract_node_annotations: _extract_node_annotations().
  _node_line_span: _node_line_span().
  _raw_text_for_span: _raw_text_for_span().
  _CLASS_TYPE_MAP: _CLASS_TYPE_MAP.
  _collect_javadoc: _collect_javadoc().
  _ANNOTATION_NODE_TYPES: _ANNOTATION_NODE_TYPES.
  _extract_identifier: _extract_identifier().
  _extract_superclass: _extract_superclass().
  _qualified_class_name: _qualified_class_name().
---
# Module: [`tree_sitter_analyzer/languages/_java_element_helpers.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_java_element_helpers.py)

## Functions
- `_build_java_class(node: Any, class_name: str, start_line: int, end_line: int, raw_text: str, full_qualified_name: str, package_name: str, extends_class: str | None, implements_interfaces: list[str], modifiers: list[str], visibility: str, annotations: list[dict[str, Any]], is_nested: bool, parent_class: str | None)` — [`L332`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_java_element_helpers.py#L332)
- `_build_java_field(var_name: str, start_line: int, end_line: int, raw_text: str, field_type: str, modifiers: list[str], visibility: str, annotations: list[dict[str, Any]], javadoc: str | None)` — [`L396`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_java_element_helpers.py#L396)
- `_build_java_fields(variable_names: list[str], start_line: int, end_line: int, raw_text: str, field_type: str, modifiers: list[str], visibility: str, annotations: list[dict[str, Any]], javadoc: str | None)` — [`L369`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_java_element_helpers.py#L369)
- `_collect_javadoc(content_lines: list[str], start_index: int, end_index: int)` — [`L186`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_java_element_helpers.py#L186)
- `_extract_class_relationships(node: Any, get_node_text: Callable[..., str])` — [`L289`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_java_element_helpers.py#L289)
- `_extract_identifier(node: Any, get_node_text: Callable[..., str])` — [`L248`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_java_element_helpers.py#L248)
- `_extract_node_annotations(node: Any, get_node_text: Callable[..., str])` — [`L207`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_java_element_helpers.py#L207) — Extract annotations directly from a node's modifiers subtree.
- `_extract_superclass(node: Any, get_node_text: Callable[..., str])` — [`L313`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_java_element_helpers.py#L313)
- `_node_line_span(node: Any)` — [`L200`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_java_element_helpers.py#L200)
- `_qualified_class_name(package_name: str, class_name: str)` — [`L318`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_java_element_helpers.py#L318)
- `_raw_text_for_span(content_lines: list[str], start_line: int, end_line: int)` — [`L322`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_java_element_helpers.py#L322)
- `_split_respecting_generics(text: str)` — [`L255`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_java_element_helpers.py#L255) — Split a comma-separated interface list while preserving generic type arguments.
- `extract_java_class(node: Any, get_node_text: Callable[..., str], content_lines: list[str], current_package: str, extract_modifiers: Callable, determine_visibility: Callable, find_annotations_for_line: Callable, is_nested_class: Callable, find_parent_class: Callable, *, log_debug_func: Callable[[str], None], log_error_func: Callable[[str], None])` — [`L37`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_java_element_helpers.py#L37) — Extract Java class/interface/enum information.
- `extract_java_field(node: Any, get_node_text: Callable[..., str], content_lines: list[str], parse_field_declaration: Callable, determine_visibility: Callable, find_annotations_for_line: Callable, extract_javadoc: Callable, *, log_debug_func: Callable[[str], None], log_error_func: Callable[[str], None])` — [`L139`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_java_element_helpers.py#L139) — Extract Java field declarations.
- `extract_java_method(node: Any, get_node_text: Callable[..., str], content_lines: list[str], parse_method_signature: Callable, determine_visibility: Callable, find_annotations_for_line: Callable, calculate_complexity: Callable, extract_javadoc: Callable, *, log_debug_func: Callable[[str], None], log_error_func: Callable[[str], None])` — [`L87`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_java_element_helpers.py#L87) — Extract Java method/constructor information. — documented in [tree_sitter_analyzer-models-base](../../../concepts/tree_sitter_analyzer-models-base.md)
- `extract_javadoc_for_line(line: int, content_lines: list[str], *, log_debug_func: Callable[[str], None])` — [`L19`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_java_element_helpers.py#L19) — Extract JavaDoc comment for a specific line.

## Module values
- `_ANNOTATION_NODE_TYPES` — [`L204`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_java_element_helpers.py#L204)
- `_CLASS_TYPE_MAP` — [`L9`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_java_element_helpers.py#L9)

