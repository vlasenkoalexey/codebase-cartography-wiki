---
title: 'Module: tests/test_ts_decorators.py'
type: catalog
provenance: extracted
module: tests/test_ts_decorators.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_ts_decorators`/
symbols:
  _has_deco: _has_deco().
  _class_nid: _class_nid().
  test_method_decorator_attributes_to_method: test_method_decorator_attributes_to_method().
  _write: _write().
  test_class_decorator_on_exported_class: test_class_decorator_on_exported_class().
  test_class_decorator_on_plain_class: test_class_decorator_on_plain_class().
  test_stacked_class_decorators: test_stacked_class_decorators().
  test_stacked_method_decorators: test_stacked_method_decorators().
  test_field_decorator_attributes_to_class: test_field_decorator_attributes_to_class().
  test_parameter_decorator_attributes_to_constructor: test_parameter_decorator_attributes_to_constructor().
  test_namespaced_decorator_uses_property_name: test_namespaced_decorator_uses_property_name().
  _method_nid: _method_nid().
  test_external_decorator_stub_disambiguated_per_file: test_external_decorator_stub_disambiguated_per_file().
---
# Module: [`tests/test_ts_decorators.py`](../../../../../raw/code/graphify/tests/test_ts_decorators.py)

## Functions
- `_class_nid(file: str, cls: str)` — [`L24`](../../../../../raw/code/graphify/tests/test_ts_decorators.py#L24)
- `_has_deco(result: dict, owner_nid: str, deco: str)` — [`L32`](../../../../../raw/code/graphify/tests/test_ts_decorators.py#L32) — True if owner_nid references the (cross-file, bare-stub) decorator symbol.
- `_method_nid(file: str, cls: str, method: str)` — [`L28`](../../../../../raw/code/graphify/tests/test_ts_decorators.py#L28)
- `_write(path: Path, text: str)` — [`L18`](../../../../../raw/code/graphify/tests/test_ts_decorators.py#L18)
- `test_class_decorator_on_exported_class(tmp_path)` — [`L44`](../../../../../raw/code/graphify/tests/test_ts_decorators.py#L44)
- `test_class_decorator_on_plain_class(tmp_path)` — [`L53`](../../../../../raw/code/graphify/tests/test_ts_decorators.py#L53)
- `test_external_decorator_stub_disambiguated_per_file(tmp_path)` — [`L120`](../../../../../raw/code/graphify/tests/test_ts_decorators.py#L120) — An external decorator (definition absent from the corpus — the common
- `test_field_decorator_attributes_to_class(tmp_path)` — [`L91`](../../../../../raw/code/graphify/tests/test_ts_decorators.py#L91)
- `test_method_decorator_attributes_to_method(tmp_path)` — [`L69`](../../../../../raw/code/graphify/tests/test_ts_decorators.py#L69)
- `test_namespaced_decorator_uses_property_name(tmp_path)` — [`L113`](../../../../../raw/code/graphify/tests/test_ts_decorators.py#L113)
- `test_parameter_decorator_attributes_to_constructor(tmp_path)` — [`L104`](../../../../../raw/code/graphify/tests/test_ts_decorators.py#L104)
- `test_stacked_class_decorators(tmp_path)` — [`L60`](../../../../../raw/code/graphify/tests/test_ts_decorators.py#L60)
- `test_stacked_method_decorators(tmp_path)` — [`L80`](../../../../../raw/code/graphify/tests/test_ts_decorators.py#L80)

