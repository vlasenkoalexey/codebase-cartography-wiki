---
title: 'Module: tree_sitter_analyzer/languages/_go_type_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/_go_type_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages._go_type_helpers`/
symbols:
  _build_go_class: _build_go_class().
  extract_type_declaration: extract_type_declaration().
  extract_go_type_spec: extract_go_type_spec().
  extract_embedded_types: extract_embedded_types().
  _go_struct_interfaces: _go_struct_interfaces().
  _go_class_type: _go_class_type().
  _GO_TYPE_NODE_TO_CLASS_TYPE: _GO_TYPE_NODE_TO_CLASS_TYPE.
  _iter_struct_fields: _iter_struct_fields().
  _extract_embedded_type: _extract_embedded_type().
  _go_type_name_and_node: _go_type_name_and_node().
  _go_interface_embedded: _go_interface_embedded().
  _iter_type_specs: _iter_type_specs().
---
# Module: [`tree_sitter_analyzer/languages/_go_type_helpers.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_go_type_helpers.py)

## Functions
- `_build_go_class(name: str, type_node: Any | None, node: Any, get_node_text: Callable[..., str], content_lines: list[str])` — [`L80`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_go_type_helpers.py#L80)
- `_extract_embedded_type(field: Any, get_node_text: Callable[..., str])` — [`L39`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_go_type_helpers.py#L39)
- `_go_class_type(type_node: Any | None)` — [`L100`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_go_type_helpers.py#L100)
- `_go_interface_embedded(interface_node: Any, get_node_text: Callable[..., str])` — [`L119`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_go_type_helpers.py#L119) — Extract embedded interface names from an interface_type node.
- `_go_struct_interfaces(type_node: Any | None, get_node_text: Callable[..., str])` — [`L106`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_go_type_helpers.py#L106)
- `_go_type_name_and_node(node: Any, get_node_text: Callable[..., str])` — [`L69`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_go_type_helpers.py#L69)
- `_iter_struct_fields(struct_node: Any)` — [`L28`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_go_type_helpers.py#L28)
- `_iter_type_specs(node: Any)` — [`L153`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_go_type_helpers.py#L153)
- `extract_embedded_types(struct_node: Any, get_node_text: Callable[..., str])` — [`L16`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_go_type_helpers.py#L16) — Extract embedded types from struct.
- `extract_go_type_spec(node: Any, get_node_text: Callable[..., str], content_lines: list[str])` — [`L52`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_go_type_helpers.py#L52) — Extract single Go type spec (struct, interface, type alias).
- `extract_type_declaration(node: Any, get_node_text: Callable[..., str], content_lines: list[str])` — [`L136`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_go_type_helpers.py#L136) — Extract type declaration (struct, interface, type alias).

## Module values
- `_GO_TYPE_NODE_TO_CLASS_TYPE` — [`L10`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_go_type_helpers.py#L10)

