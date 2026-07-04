---
title: 'Module: tests/test_ts_import_require.py'
type: catalog
provenance: extracted
module: tests/test_ts_import_require.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_ts_import_require`/
symbols:
  _write: _write().
  test_import_require_bare_module_targets_ref_stub: test_import_require_bare_module_targets_ref_stub().
  test_import_require_parity_with_namespace_import: test_import_require_parity_with_namespace_import().
  test_esm_imports_unaffected: test_esm_imports_unaffected().
  test_import_require_relative_emits_file_edge: test_import_require_relative_emits_file_edge().
  test_import_require_single_quotes: test_import_require_single_quotes().
  _has_edge: _has_edge().
  test_import_require_parity_with_namespace_import.edges_from: test_import_require_parity_with_namespace_import().edges_from().
---
# Module: [`tests/test_ts_import_require.py`](../../../../../raw/code/graphify/tests/test_ts_import_require.py)

## Functions
- `_has_edge(result: dict, source: str, target: str, relation: str = "imports_from")` — [`L24`](../../../../../raw/code/graphify/tests/test_ts_import_require.py#L24)
- `_write(path: Path, text: str)` — [`L18`](../../../../../raw/code/graphify/tests/test_ts_import_require.py#L18)
- `edges_from(source_file: str)` — [`L90`](../../../../../raw/code/graphify/tests/test_ts_import_require.py#L90)
- `test_esm_imports_unaffected(tmp_path: Path)` — [`L102`](../../../../../raw/code/graphify/tests/test_ts_import_require.py#L102) — Regression guard: the restructured string scan must not change ESM handling
- `test_import_require_bare_module_targets_ref_stub(tmp_path: Path)` — [`L57`](../../../../../raw/code/graphify/tests/test_ts_import_require.py#L57)
- `test_import_require_parity_with_namespace_import(tmp_path: Path)` — [`L81`](../../../../../raw/code/graphify/tests/test_ts_import_require.py#L81) — `import x = require("./m")` must produce the same file-level edge as
- `test_import_require_relative_emits_file_edge(tmp_path: Path)` — [`L33`](../../../../../raw/code/graphify/tests/test_ts_import_require.py#L33)
- `test_import_require_single_quotes(tmp_path: Path)` — [`L45`](../../../../../raw/code/graphify/tests/test_ts_import_require.py#L45)

