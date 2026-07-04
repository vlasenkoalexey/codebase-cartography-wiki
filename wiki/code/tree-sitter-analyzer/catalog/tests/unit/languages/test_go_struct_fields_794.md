---
title: 'Module: tests/unit/languages/test_go_struct_fields_794.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_go_struct_fields_794.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_go_struct_fields_794`/
symbols:
  test_go_struct_field_types: test_go_struct_field_types().
  test_go_struct_field_names: test_go_struct_field_names().
  test_go_struct_field_element_type: test_go_struct_field_element_type().
  test_go_struct_fields_count: test_go_struct_fields_count().
  test_go_plain_var_still_extracted: test_go_plain_var_still_extracted().
  test_go_multiple_structs_fields_isolated: test_go_multiple_structs_fields_isolated().
  _extractor: _extractor().
  _WORKER_SRC: _WORKER_SRC.
  _make_tree: _make_tree().
---
# Module: [`tests/unit/languages/test_go_struct_fields_794.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_struct_fields_794.py)

## Functions
- `_extractor()` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_struct_fields_794.py#L26)
- `_make_tree(src: str)` — [`L17`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_struct_fields_794.py#L17)
- `test_go_multiple_structs_fields_isolated()` — [`L126`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_struct_fields_794.py#L126) — Fields from multiple structs are correctly attributed to their owners.
- `test_go_plain_var_still_extracted()` — [`L96`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_struct_fields_794.py#L96) — Package-level var declarations must still be extracted (no regression).
- `test_go_struct_field_element_type()` — [`L85`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_struct_fields_794.py#L85) — Fields must carry element_type='variable' so the formatter routes them correctly.
- `test_go_struct_field_names()` — [`L60`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_struct_fields_794.py#L60) — Field names must match the struct declaration order.
- `test_go_struct_field_types()` — [`L71`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_struct_fields_794.py#L71) — Field types must capture both qualified (sync.WaitGroup) and simple types.
- `test_go_struct_fields_count()` — [`L50`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_struct_fields_794.py#L50) — Four struct fields must be returned as Variable elements.

## Module values
- `_WORKER_SRC` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_struct_fields_794.py#L36)

