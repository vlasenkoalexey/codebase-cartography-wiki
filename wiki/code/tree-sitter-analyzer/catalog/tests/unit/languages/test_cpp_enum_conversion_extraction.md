---
title: 'Module: tests/unit/languages/test_cpp_enum_conversion_extraction.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_cpp_enum_conversion_extraction.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_cpp_enum_conversion_extraction`/
symbols:
  _extract: _extract().
  test_enum_extractor_exception_returns_none: test_enum_extractor_exception_returns_none().
  CPP_SRC: CPP_SRC.
  test_plain_enum_extracted: test_plain_enum_extracted().
  test_enum_class_extracted: test_enum_class_extracted().
  test_conversion_operator_extracted: test_conversion_operator_extracted().
  test_existing_extraction_unchanged: test_existing_extraction_unchanged().
  test_operator_cast_without_type_child_yields_no_name: test_operator_cast_without_type_child_yields_no_name().
---
# Module: [`tests/unit/languages/test_cpp_enum_conversion_extraction.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_enum_conversion_extraction.py)

## Functions
- `_extract()` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_enum_conversion_extraction.py#L36)
- `test_conversion_operator_extracted()` — [`L56`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_enum_conversion_extraction.py#L56)
- `test_enum_class_extracted()` — [`L51`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_enum_conversion_extraction.py#L51)
- `test_enum_extractor_exception_returns_none()` — [`L68`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_enum_conversion_extraction.py#L68) — An exploding node must be caught and yield None (error path).
- `test_existing_extraction_unchanged()` — [`L61`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_enum_conversion_extraction.py#L61)
- `test_operator_cast_without_type_child_yields_no_name()` — [`L86`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_enum_conversion_extraction.py#L86) — operator_cast with no recognizable type child -> parser returns None.
- `test_plain_enum_extracted()` — [`L46`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_enum_conversion_extraction.py#L46)

## Module values
- `CPP_SRC` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_enum_conversion_extraction.py#L19)

