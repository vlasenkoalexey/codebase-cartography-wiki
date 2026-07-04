---
title: 'Module: tests/unit/tools/test_kuzu_import_indexing.py'
type: catalog
provenance: extracted
module: tests/unit/tools/test_kuzu_import_indexing.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `tests.unit.tools.test_kuzu_import_indexing`/
symbols:
  test_kuzu_indexes_typescript_import_rows_without_full_import_name: test_kuzu_indexes_typescript_import_rows_without_full_import_name().
  _new_kuzu_driver: _new_kuzu_driver().
  _KuzuDBAdapter.get_driver: _KuzuDBAdapter#get_driver().
  test_kuzu_indexes_typescript_scoped_package_import: test_kuzu_indexes_typescript_scoped_package_import().
  test_kuzu_indexes_import_rows_with_missing_optional_fields: test_kuzu_indexes_import_rows_with_missing_optional_fields().
  test_kuzu_migrates_existing_module_schema_without_full_import_name: test_kuzu_migrates_existing_module_schema_without_full_import_name().
  kuzu: kuzu.
  _KuzuDBAdapter: _KuzuDBAdapter#
  _KuzuDBAdapter._driver: _KuzuDBAdapter#_driver.
  _KuzuDBAdapter.__init__: _KuzuDBAdapter#__init__().
  _KuzuDBAdapter.get_backend_type: _KuzuDBAdapter#get_backend_type().
---
# Module: [`tests/unit/tools/test_kuzu_import_indexing.py`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_kuzu_import_indexing.py)

## Classes
### `_KuzuDBAdapter`
- def: [`tests/unit/tools/test_kuzu_import_indexing.py:13`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_kuzu_import_indexing.py#L13)
- signature: `class _KuzuDBAdapter:`
- members:
  - `get_backend_type(self)` — [`L20`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_kuzu_import_indexing.py#L20)
  - `get_driver(self)` — [`L17`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_kuzu_import_indexing.py#L17)
- protocol/private: `__init__`[`L14`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_kuzu_import_indexing.py#L14), `_driver`[`L15`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_kuzu_import_indexing.py#L15)
- used by: (1 test-only callers)

## Functions
- `_new_kuzu_driver(tmp_path: Path)` — [`L24`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_kuzu_import_indexing.py#L24)
- `test_kuzu_indexes_import_rows_with_missing_optional_fields(tmp_path)` — [`L115`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_kuzu_import_indexing.py#L115)
- `test_kuzu_indexes_typescript_import_rows_without_full_import_name(tmp_path)` — [`L29`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_kuzu_import_indexing.py#L29)
- `test_kuzu_indexes_typescript_scoped_package_import(tmp_path)` — [`L67`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_kuzu_import_indexing.py#L67)
- `test_kuzu_migrates_existing_module_schema_without_full_import_name(tmp_path)` — [`L153`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_kuzu_import_indexing.py#L153)

## Module values
- `kuzu` — [`L10`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_kuzu_import_indexing.py#L10)

