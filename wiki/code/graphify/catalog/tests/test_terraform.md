---
title: 'Module: tests/test_terraform.py'
type: catalog
provenance: extracted
module: tests/test_terraform.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_terraform`/
symbols:
  _write: _write().
  test_no_error_and_all_block_types_become_nodes: test_no_error_and_all_block_types_become_nodes().
  test_reference_edges: test_reference_edges().
  test_depends_on_edge: test_depends_on_edge().
  test_file_contains_blocks: test_file_contains_blocks().
  test_meta_heads_not_emitted: test_meta_heads_not_emitted().
  test_cross_file_references_resolve_after_merge: test_cross_file_references_resolve_after_merge().
  test_empty_and_commentonly_files_are_safe: test_empty_and_commentonly_files_are_safe().
  test_tfvars_key_value_is_safe: test_tfvars_key_value_is_safe().
  _rel_pairs: _rel_pairs().
  SAMPLE: SAMPLE.
  _labels: _labels().
---
# Module: [`tests/test_terraform.py`](../../../../../raw/code/graphify/tests/test_terraform.py)

## Functions
- `_labels(r)` — [`L16`](../../../../../raw/code/graphify/tests/test_terraform.py#L16)
- `_rel_pairs(r, relation: str)` — [`L20`](../../../../../raw/code/graphify/tests/test_terraform.py#L20)
- `_write(tmp_path: Path, name: str, body: str)` — [`L10`](../../../../../raw/code/graphify/tests/test_terraform.py#L10)
- `test_cross_file_references_resolve_after_merge(tmp_path)` — [`L115`](../../../../../raw/code/graphify/tests/test_terraform.py#L115)
- `test_depends_on_edge(tmp_path)` — [`L88`](../../../../../raw/code/graphify/tests/test_terraform.py#L88)
- `test_empty_and_commentonly_files_are_safe(tmp_path)` — [`L145`](../../../../../raw/code/graphify/tests/test_terraform.py#L145)
- `test_file_contains_blocks(tmp_path)` — [`L93`](../../../../../raw/code/graphify/tests/test_terraform.py#L93)
- `test_meta_heads_not_emitted(tmp_path)` — [`L100`](../../../../../raw/code/graphify/tests/test_terraform.py#L100)
- `test_no_error_and_all_block_types_become_nodes(tmp_path)` — [`L60`](../../../../../raw/code/graphify/tests/test_terraform.py#L60)
- `test_reference_edges(tmp_path)` — [`L78`](../../../../../raw/code/graphify/tests/test_terraform.py#L78)
- `test_tfvars_key_value_is_safe(tmp_path)` — [`L152`](../../../../../raw/code/graphify/tests/test_terraform.py#L152)

## Module values
- `SAMPLE` — [`L29`](../../../../../raw/code/graphify/tests/test_terraform.py#L29)

