---
title: 'Module: tests/test_ts_inheritance.py'
type: catalog
provenance: extracted
module: tests/test_ts_inheritance.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_ts_inheritance`/
symbols:
  _has_inherits: _has_inherits().
  _write: _write().
  test_interface_extends_same_file: test_interface_extends_same_file().
  test_interface_extends_multiple_same_file: test_interface_extends_multiple_same_file().
  test_class_extends_same_file: test_class_extends_same_file().
  test_interface_extends_generic_base_same_file: test_interface_extends_generic_base_same_file().
  test_interface_extends_imported: test_interface_extends_imported().
  test_imported_class_extends_still_works: test_imported_class_extends_still_works().
  test_class_implements_same_file_interface: test_class_implements_same_file_interface().
---
# Module: [`tests/test_ts_inheritance.py`](../../../../../raw/code/graphify/tests/test_ts_inheritance.py)

## Functions
- `_has_inherits(result: dict, src_file: str, src_sym: str, tgt_file: str, tgt_sym: str, relation: str = "inherits")` — [`L23`](../../../../../raw/code/graphify/tests/test_ts_inheritance.py#L23)
- `_write(path: Path, text: str)` — [`L17`](../../../../../raw/code/graphify/tests/test_ts_inheritance.py#L17)
- `test_class_extends_same_file(tmp_path)` — [`L51`](../../../../../raw/code/graphify/tests/test_ts_inheritance.py#L51)
- `test_class_implements_same_file_interface(tmp_path)` — [`L86`](../../../../../raw/code/graphify/tests/test_ts_inheritance.py#L86)
- `test_imported_class_extends_still_works(tmp_path)` — [`L76`](../../../../../raw/code/graphify/tests/test_ts_inheritance.py#L76) — Regression guard: the originally-working imported-class case must stay.
- `test_interface_extends_generic_base_same_file(tmp_path)` — [`L59`](../../../../../raw/code/graphify/tests/test_ts_inheritance.py#L59)
- `test_interface_extends_imported(tmp_path)` — [`L67`](../../../../../raw/code/graphify/tests/test_ts_inheritance.py#L67)
- `test_interface_extends_multiple_same_file(tmp_path)` — [`L41`](../../../../../raw/code/graphify/tests/test_ts_inheritance.py#L41)
- `test_interface_extends_same_file(tmp_path)` — [`L33`](../../../../../raw/code/graphify/tests/test_ts_inheritance.py#L33)

