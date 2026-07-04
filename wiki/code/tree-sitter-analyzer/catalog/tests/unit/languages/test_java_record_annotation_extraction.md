---
title: 'Module: tests/unit/languages/test_java_record_annotation_extraction.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_java_record_annotation_extraction.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_java_record_annotation_extraction`/
symbols:
  _extract_classes: _extract_classes().
  test_record_method_still_extracted: test_record_method_still_extracted().
  JAVA_SRC: JAVA_SRC.
  test_record_declarations_extracted: test_record_declarations_extracted().
  test_annotation_type_declarations_extracted: test_annotation_type_declarations_extracted().
  test_existing_kinds_unchanged: test_existing_kinds_unchanged().
---
# Module: [`tests/unit/languages/test_java_record_annotation_extraction.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_record_annotation_extraction.py)

## Functions
- `_extract_classes()` — [`L42`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_record_annotation_extraction.py#L42)
- `test_annotation_type_declarations_extracted()` — [`L59`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_record_annotation_extraction.py#L59)
- `test_existing_kinds_unchanged()` — [`L67`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_record_annotation_extraction.py#L67) — The graduation must not disturb class/enum extraction.
- `test_record_declarations_extracted()` — [`L51`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_record_annotation_extraction.py#L51)
- `test_record_method_still_extracted()` — [`L74`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_record_annotation_extraction.py#L74) — Methods inside a record body must be visible as functions.

## Module values
- `JAVA_SRC` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_record_annotation_extraction.py#L19)

