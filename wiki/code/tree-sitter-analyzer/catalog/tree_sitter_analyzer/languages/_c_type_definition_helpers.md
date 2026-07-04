---
title: 'Module: tree_sitter_analyzer/languages/_c_type_definition_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/_c_type_definition_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages._c_type_definition_helpers`/
symbols:
  _extract_type_definition: _extract_type_definition().
  extract_enum_definition: extract_enum_definition().
  extract_struct_definition: extract_struct_definition().
  _type_name_and_range: _type_name_and_range().
  _direct_type_name: _direct_type_name().
  _typedef_type_name: _typedef_type_name().
  _raw_text: _raw_text().
  _is_anonymous_nested_member: _is_anonymous_nested_member().
  _node_line_range: _node_line_range().
  _has_body: _has_body().
---
# Module: [`tree_sitter_analyzer/languages/_c_type_definition_helpers.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_c_type_definition_helpers.py)

## Functions
- `_direct_type_name(node: Any, get_node_text: Callable[..., str])` — [`L133`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_c_type_definition_helpers.py#L133)
- `_extract_type_definition(node: Any, get_node_text: Callable[..., str], content_lines: list[str], class_type: str, anonymous_prefix: str, error_label: str)` — [`L69`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_c_type_definition_helpers.py#L69)
- `_has_body(node: Any)` — [`L54`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_c_type_definition_helpers.py#L54) — Return True when ``node`` (struct/union/enum specifier) has a definition
- `_is_anonymous_nested_member(node: Any, get_node_text: Callable[..., str])` — [`L33`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_c_type_definition_helpers.py#L33) — Return True when ``node`` is an anonymous container (struct/union/enum
- `_node_line_range(node: Any)` — [`L149`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_c_type_definition_helpers.py#L149)
- `_raw_text(content_lines: list[str], start_line: int, end_line: int)` — [`L153`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_c_type_definition_helpers.py#L153)
- `_type_name_and_range(node: Any, get_node_text: Callable[..., str], start_line: int, end_line: int, anonymous_prefix: str)` — [`L114`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_c_type_definition_helpers.py#L114)
- `_typedef_type_name(node: Any, get_node_text: Callable[..., str])` — [`L140`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_c_type_definition_helpers.py#L140)
- `extract_enum_definition(node: Any, get_node_text: Callable[..., str], content_lines: list[str])` — [`L22`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_c_type_definition_helpers.py#L22) — Extract enum definition.
- `extract_struct_definition(node: Any, get_node_text: Callable[..., str], content_lines: list[str])` — [`L11`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_c_type_definition_helpers.py#L11) — Extract struct definition.

