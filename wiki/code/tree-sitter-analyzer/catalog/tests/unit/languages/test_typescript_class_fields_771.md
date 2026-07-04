---
title: 'Module: tests/unit/languages/test_typescript_class_fields_771.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_typescript_class_fields_771.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_typescript_class_fields_771`/
symbols:
  _extract_variable_names: _extract_variable_names().
  test_exact_field_count: test_exact_field_count().
  _parse: _parse().
  TS_SRC: TS_SRC.
  test_base_entity_fields_captured: test_base_entity_fields_captured().
  test_user_service_fields_captured: test_user_service_fields_captured().
  test_async_data_processor_field_captured: test_async_data_processor_field_captured().
  test_application_fields_captured: test_application_fields_captured().
  test_method_body_const_excluded: test_method_body_const_excluded().
  test_method_body_let_excluded: test_method_body_let_excluded().
  test_body_locals_excluded_exactly: test_body_locals_excluded_exactly().
  test_promises_result_excluded: test_promises_result_excluded().
  test_interface_property_signatures_still_captured: test_interface_property_signatures_still_captured().
---
# Module: [`tests/unit/languages/test_typescript_class_fields_771.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_class_fields_771.py)

## Functions
- `_extract_variable_names(src: str = TS_SRC)` — [`L88`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_class_fields_771.py#L88)
- `_parse(src: str = TS_SRC)` — [`L82`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_class_fields_771.py#L82)
- `test_application_fields_captured()` — [`L119`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_class_fields_771.py#L119) — Application class fields must appear.
- `test_async_data_processor_field_captured()` — [`L113`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_class_fields_771.py#L113) — AsyncDataProcessor.cache class field must appear.
- `test_base_entity_fields_captured()` — [`L97`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_class_fields_771.py#L97) — BaseEntity protected readonly fields must appear.
- `test_body_locals_excluded_exactly()` — [`L156`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_class_fields_771.py#L156) — The set of body-locals from run() must all be absent.
- `test_exact_field_count()` — [`L184`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_class_fields_771.py#L184) — Pin the exact number of variables extracted from the fixture.
- `test_interface_property_signatures_still_captured()` — [`L174`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_class_fields_771.py#L174) — IUser interface property signatures must still be captured.
- `test_method_body_const_excluded()` — [`L129`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_class_fields_771.py#L129) — Local 'const deleted' inside delete() must NOT appear as a field.
- `test_method_body_let_excluded()` — [`L137`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_class_fields_771.py#L137) — Local 'let users' inside findAll() must NOT appear as a field.
- `test_promises_result_excluded()` — [`L164`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_class_fields_771.py#L164) — Locals 'result' and 'promises' inside fetchData() must NOT appear.
- `test_user_service_fields_captured()` — [`L105`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_class_fields_771.py#L105) — UserService private/static class property declarations must appear.

## Module values
- `TS_SRC` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_class_fields_771.py#L26)

