---
title: 'Module: tests/unit/languages/test_kotlin_property_extraction_758.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_kotlin_property_extraction_758.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_kotlin_property_extraction_758`/
symbols:
  extractor: extractor().
  kotlin_parser: kotlin_parser().
  TestKotlinPropertyNameExtraction: TestKotlinPropertyNameExtraction#
  TestKotlinPropertyNameExtraction.test_val_with_type_annotation_name: TestKotlinPropertyNameExtraction#test_val_with_type_annotation_name().
  TestKotlinPropertyNameExtraction.test_var_with_type_annotation_name: TestKotlinPropertyNameExtraction#test_var_with_type_annotation_name().
  TestKotlinPropertyNameExtraction.test_const_val_name: TestKotlinPropertyNameExtraction#test_const_val_name().
  TestKotlinPropertyNameExtraction.test_val_without_type_annotation_name: TestKotlinPropertyNameExtraction#test_val_without_type_annotation_name().
  TestKotlinPropertyNameExtraction.test_class_property_names: TestKotlinPropertyNameExtraction#test_class_property_names().
  TestKotlinPropertyTypeExtraction: TestKotlinPropertyTypeExtraction#
  TestKotlinPropertyTypeExtraction.test_val_with_string_type: TestKotlinPropertyTypeExtraction#test_val_with_string_type().
  TestKotlinPropertyTypeExtraction.test_var_with_int_type: TestKotlinPropertyTypeExtraction#test_var_with_int_type().
  TestKotlinPropertyTypeExtraction.test_const_val_with_type: TestKotlinPropertyTypeExtraction#test_const_val_with_type().
  TestKotlinPropertyTypeExtraction.test_val_without_type_stays_inferred: TestKotlinPropertyTypeExtraction#test_val_without_type_stays_inferred().
  TestKotlinConstValFlags: TestKotlinConstValFlags#
  TestKotlinConstValFlags.test_const_val_is_static_and_readonly: TestKotlinConstValFlags#test_const_val_is_static_and_readonly().
  TestKotlinConstValFlags.test_plain_val_is_not_static: TestKotlinConstValFlags#test_plain_val_is_not_static().
  TestKotlinConstValFlags.test_var_is_not_readonly: TestKotlinConstValFlags#test_var_is_not_readonly().
---
# Module: [`tests/unit/languages/test_kotlin_property_extraction_758.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_property_extraction_758.py)

## Classes
### `TestKotlinConstValFlags`
- def: [`tests/unit/languages/test_kotlin_property_extraction_758.py:139`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_property_extraction_758.py#L139)
- doc: Issue #758: const val must set is_static=True and is_readonly=True.
- signature: `class TestKotlinConstValFlags:`
- members:
  - `test_const_val_is_static_and_readonly(self, extractor, kotlin_parser)` — [`L142`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_property_extraction_758.py#L142) — const val MAX_USERS: Int = 100 — must be static and readonly.
  - `test_plain_val_is_not_static(self, extractor, kotlin_parser)` — [`L153`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_property_extraction_758.py#L153) — Plain val must NOT be marked static.
  - `test_var_is_not_readonly(self, extractor, kotlin_parser)` — [`L162`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_property_extraction_758.py#L162) — var must NOT be marked readonly.

### `TestKotlinPropertyNameExtraction`
- def: [`tests/unit/languages/test_kotlin_property_extraction_758.py:43`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_property_extraction_758.py#L43)
- doc: Issue #758: property names must not be 'unknown'.
- signature: `class TestKotlinPropertyNameExtraction:`
- members:
  - `test_class_property_names(self, extractor, kotlin_parser)` — [`L82`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_property_extraction_758.py#L82) — Properties inside a class body must carry real names.
  - `test_const_val_name(self, extractor, kotlin_parser)` — [`L64`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_property_extraction_758.py#L64) — const val MAX_USERS: Int — name must be 'MAX_USERS'.
  - `test_val_with_type_annotation_name(self, extractor, kotlin_parser)` — [`L46`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_property_extraction_758.py#L46) — val name: String — name must be 'name', not 'unknown'.
  - `test_val_without_type_annotation_name(self, extractor, kotlin_parser)` — [`L73`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_property_extraction_758.py#L73) — val version = "1.0" — name must be 'version', not 'unknown'.
  - `test_var_with_type_annotation_name(self, extractor, kotlin_parser)` — [`L55`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_property_extraction_758.py#L55) — var total: Int — name must be 'total'.

### `TestKotlinPropertyTypeExtraction`
- def: [`tests/unit/languages/test_kotlin_property_extraction_758.py:99`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_property_extraction_758.py#L99)
- doc: Issue #758: declared types must be extracted, not hardcoded 'Inferred'.
- signature: `class TestKotlinPropertyTypeExtraction:`
- members:
  - `test_const_val_with_type(self, extractor, kotlin_parser)` — [`L120`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_property_extraction_758.py#L120) — const val MAX_USERS: Int — type must be 'Int'.
  - `test_val_with_string_type(self, extractor, kotlin_parser)` — [`L102`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_property_extraction_758.py#L102) — val name: String — type must be 'String'.
  - `test_val_without_type_stays_inferred(self, extractor, kotlin_parser)` — [`L129`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_property_extraction_758.py#L129) — val version = "1.0" — no annotation, so type must be 'Inferred'.
  - `test_var_with_int_type(self, extractor, kotlin_parser)` — [`L111`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_property_extraction_758.py#L111) — var total: Int — type must be 'Int'.

## Functions
- `extractor()` — [`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_property_extraction_758.py#L39)
- `kotlin_parser()` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_property_extraction_758.py#L23) — Build a tree-sitter Kotlin parser (module-scoped for speed).

