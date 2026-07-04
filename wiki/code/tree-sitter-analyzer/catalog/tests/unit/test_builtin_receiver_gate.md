---
title: 'Module: tests/unit/test_builtin_receiver_gate.py'
type: catalog
provenance: extracted
module: tests/unit/test_builtin_receiver_gate.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_builtin_receiver_gate`/
symbols:
  _index: _index().
  _edges_for: _edges_for().
  test_dict_get_does_not_bind_to_project_search_cache_get: test_dict_get_does_not_bind_to_project_search_cache_get().
  test_imported_search_cache_get_still_binds: test_imported_search_cache_get_still_binds().
  test_untyped_param_receiver_unique_method_binds: test_untyped_param_receiver_unique_method_binds().
  test_self_attr_receiver_unique_method_binds: test_self_attr_receiver_unique_method_binds().
  test_singleton_receiver_unique_method_binds: test_singleton_receiver_unique_method_binds().
---
# Module: [`tests/unit/test_builtin_receiver_gate.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_builtin_receiver_gate.py)

## Functions
- `_edges_for(db_path: str, callee_name: str)` — [`L53`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_builtin_receiver_gate.py#L53) — Return all CALLS edges for callee_name as dicts.
- `_index(tmp_path: Path, files: dict[str, str])` — [`L38`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_builtin_receiver_gate.py#L38) — Index files under tmp_path and return the .ast-cache DB path.
- `test_dict_get_does_not_bind_to_project_search_cache_get(tmp_path: Path)` — [`L68`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_builtin_receiver_gate.py#L68) — Bug repro #447 (adjusted for new-design): ``result = {}; result.get()`` in
- `test_imported_search_cache_get_still_binds(tmp_path: Path)` — [`L120`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_builtin_receiver_gate.py#L120) — Counter-case: when the caller IMPORTS SearchCache and uses an instance,
- `test_self_attr_receiver_unique_method_binds(tmp_path: Path)` — [`L195`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_builtin_receiver_gate.py#L195) — P1 adversarial case: ``self._store.get()`` where DataStore.get is unique
- `test_singleton_receiver_unique_method_binds(tmp_path: Path)` — [`L232`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_builtin_receiver_gate.py#L232) — P3 adversarial case: module-level singleton ``CACHE.get()`` where
- `test_untyped_param_receiver_unique_method_binds(tmp_path: Path)` — [`L158`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_builtin_receiver_gate.py#L158) — P1 adversarial regression: untyped param ``store`` calling ``store.get()``

