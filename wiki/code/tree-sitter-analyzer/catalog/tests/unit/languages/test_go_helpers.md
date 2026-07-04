---
title: 'Module: tests/unit/languages/test_go_helpers.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_go_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_go_helpers`/
symbols:
  FakeNode: FakeNode#
  test_extract_import_spec_handles_named_alias: test_extract_import_spec_handles_named_alias().
  test_extract_go_type_spec_includes_embedded_struct_types: test_extract_go_type_spec_includes_embedded_struct_types().
  test_extract_import_declaration_flattens_grouped_imports: test_extract_import_declaration_flattens_grouped_imports().
  test_extract_embedded_types_ignores_named_fields: test_extract_embedded_types_ignores_named_fields().
  FakeNode.children: FakeNode#children.
  test_extract_docstring_collects_contiguous_go_comments: test_extract_docstring_collects_contiguous_go_comments().
  FakeNode.child_by_field_name: FakeNode#child_by_field_name().
  FakeNode.fields: FakeNode#fields.
  get_node_text: get_node_text().
  FakeNode.start_point: FakeNode#start_point.
  FakeNode.end_point: FakeNode#end_point.
  FakeNode.text: FakeNode#text.
---
# Module: [`tests/unit/languages/test_go_helpers.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_helpers.py)

## Classes
### `FakeNode`
- def: [`tests/unit/languages/test_go_helpers.py:18`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_helpers.py#L18)
- signature: `class FakeNode:`
- members:
  - `child_by_field_name(self, name: str)` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_helpers.py#L26)
  - `children` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_helpers.py#L21)
  - `end_point` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_helpers.py#L24)
  - `fields` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_helpers.py#L22)
  - `start_point` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_helpers.py#L23)
  - `text` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_helpers.py#L20)
- used by: (5 test-only callers)

## Functions
- `get_node_text(node: Any)` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_helpers.py#L30)
- `test_extract_docstring_collects_contiguous_go_comments()` — [`L141`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_helpers.py#L141)
- `test_extract_embedded_types_ignores_named_fields()` — [`L81`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_helpers.py#L81)
- `test_extract_go_type_spec_includes_embedded_struct_types()` — [`L108`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_helpers.py#L108)
- `test_extract_import_declaration_flattens_grouped_imports()` — [`L55`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_helpers.py#L55)
- `test_extract_import_spec_handles_named_alias()` — [`L34`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_helpers.py#L34)

