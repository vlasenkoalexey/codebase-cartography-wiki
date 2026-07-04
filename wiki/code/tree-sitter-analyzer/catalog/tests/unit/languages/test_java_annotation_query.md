---
title: 'Module: tests/unit/languages/test_java_annotation_query.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_java_annotation_query.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_java_annotation_query`/
symbols:
  TestJavaAnnotationMethodQuery.test_single_marker_annotation: TestJavaAnnotationMethodQuery#test_single_marker_annotation().
  TestJavaAnnotationMethodQuery.test_annotation_with_parameters: TestJavaAnnotationMethodQuery#test_annotation_with_parameters().
  TestJavaAnnotationMethodQuery.test_multiple_annotations: TestJavaAnnotationMethodQuery#test_multiple_annotations().
  TestJavaAnnotationMethodQuery.test_mixed_methods_only_annotated_matched: TestJavaAnnotationMethodQuery#test_mixed_methods_only_annotated_matched().
  TestJavaAnnotationMethodQuery.test_query_returns_correct_capture_types: TestJavaAnnotationMethodQuery#test_query_returns_correct_capture_types().
  _write_temp_java_file: _write_temp_java_file().
  _cleanup_temp_file: _cleanup_temp_file().
  TestJavaAnnotationMethodQuery: TestJavaAnnotationMethodQuery#
---
# Module: [`tests/unit/languages/test_java_annotation_query.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_annotation_query.py)

## Classes
### `TestJavaAnnotationMethodQuery`
- def: [`tests/unit/languages/test_java_annotation_query.py:41`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_annotation_query.py#L41)
- doc: Test cases for the method_with_annotations query
- signature: `class TestJavaAnnotationMethodQuery:`
- members:
  - `test_annotation_with_parameters(self)` — [`L78`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_annotation_query.py#L78) — Test that query matches method with annotation that has parameters
  - `test_mixed_methods_only_annotated_matched(self)` — [`L137`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_annotation_query.py#L137) — Test that query only matches annotated methods, not regular methods
  - `test_multiple_annotations(self)` — [`L108`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_annotation_query.py#L108) — Test that query matches method with multiple annotations
  - `test_query_returns_correct_capture_types(self)` — [`L186`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_annotation_query.py#L186) — Test that query captures have the expected structure
  - `test_single_marker_annotation(self)` — [`L44`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_annotation_query.py#L44) — Test that query matches method with single marker annotation (@Override)
- uses (calls/refs, reference-scoped): [`execute_query`](../../../tree_sitter_analyzer/api.md#execute_query)  (2 test-only)

## Functions
- `_cleanup_temp_file(file_path: str)` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_annotation_query.py#L32) — Helper to clean up temp file
- `_write_temp_java_file(code: str)` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_annotation_query.py#L25) — Helper to write Java code to a temp file and return the path

