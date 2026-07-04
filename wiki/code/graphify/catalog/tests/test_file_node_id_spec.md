---
title: 'Module: tests/test_file_node_id_spec.py'
type: catalog
provenance: extracted
module: tests/test_file_node_id_spec.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_file_node_id_spec`/
symbols:
  test_file_node_id_uses_parent_dir_and_stem_no_extension: test_file_node_id_uses_parent_dir_and_stem_no_extension().
  test_top_level_file_node_id_is_bare_stem: test_top_level_file_node_id_is_bare_stem().
  test_top_level_file_SYMBOL_ids_use_bare_stem: test_top_level_file_SYMBOL_ids_use_bare_stem().
  test_nested_file_symbol_ids_unchanged: test_nested_file_symbol_ids_unchanged().
  test_symbol_and_file_ids_share_the_same_stem: test_symbol_and_file_ids_share_the_same_stem().
  test_cross_file_import_edges_stay_connected: test_cross_file_import_edges_stay_connected().
  _file_nodes: _file_nodes().
---
# Module: [`tests/test_file_node_id_spec.py`](../../../../../raw/code/graphify/tests/test_file_node_id_spec.py)

## Functions
- `_file_nodes(extraction: dict)` — [`L18`](../../../../../raw/code/graphify/tests/test_file_node_id_spec.py#L18)
- `test_cross_file_import_edges_stay_connected(tmp_path)` — [`L122`](../../../../../raw/code/graphify/tests/test_file_node_id_spec.py#L122) — Changing the file-id format must not orphan import edges: the import
- `test_file_node_id_uses_parent_dir_and_stem_no_extension(tmp_path)` — [`L27`](../../../../../raw/code/graphify/tests/test_file_node_id_spec.py#L27) — match/script/pipeline_step.py -> file node id 'match_script_pipeline_step'
- `test_nested_file_symbol_ids_unchanged(tmp_path)` — [`L83`](../../../../../raw/code/graphify/tests/test_file_node_id_spec.py#L83) — Regression guard: nested files (immediate parent identical in abs/rel form)
- `test_symbol_and_file_ids_share_the_same_stem(tmp_path)` — [`L97`](../../../../../raw/code/graphify/tests/test_file_node_id_spec.py#L97) — Symbol ids already use {parent}_{stem}_{name}; the file node must share
- `test_top_level_file_SYMBOL_ids_use_bare_stem(tmp_path)` — [`L58`](../../../../../raw/code/graphify/tests/test_file_node_id_spec.py#L58) — A SYMBOL in a root-level file must use the bare-stem prefix (`setup_configure`),
- `test_top_level_file_node_id_is_bare_stem(tmp_path)` — [`L46`](../../../../../raw/code/graphify/tests/test_file_node_id_spec.py#L46) — A file directly at the project root collapses to just its stem.

