---
title: 'Module: tests/unit/languages/test_rust_enum_variants_796.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_rust_enum_variants_796.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_rust_enum_variants_796`/
symbols:
  TestRustEnumVariantExtraction.test_enum_variant_has_correct_variable_type: TestRustEnumVariantExtraction#test_enum_variant_has_correct_variable_type().
  TestRustEnumVariantExtraction.test_enum_variant_receiver_type_is_enum_name: TestRustEnumVariantExtraction#test_enum_variant_receiver_type_is_enum_name().
  TestRustEnumVariantExtraction.test_enum_variant_visibility_inherits_enum_visibility: TestRustEnumVariantExtraction#test_enum_variant_visibility_inherits_enum_visibility().
  TestRustEnumVariantExtraction.test_enum_variant_line_range_within_enum_span: TestRustEnumVariantExtraction#test_enum_variant_line_range_within_enum_span().
  TestRustEnumVariantExtraction.test_multiple_enums_variants_separate: TestRustEnumVariantExtraction#test_multiple_enums_variants_separate().
  _parse_rust: _parse_rust().
  TestRustEnumVariantExtraction.test_simple_enum_variants_are_extracted: TestRustEnumVariantExtraction#test_simple_enum_variants_are_extracted().
  TestRustEnumVariantExtraction.test_option_like_enum_variants: TestRustEnumVariantExtraction#test_option_like_enum_variants().
  TestRustEnumVariantExtraction.test_struct_fields_and_enum_variants_coexist: TestRustEnumVariantExtraction#test_struct_fields_and_enum_variants_coexist().
  TestRustEnumVariantExtraction.test_struct_like_enum_variant_fields_do_not_leak: TestRustEnumVariantExtraction#test_struct_like_enum_variant_fields_do_not_leak().
  _TS_RUST_AVAILABLE: _TS_RUST_AVAILABLE.
  TestRustEnumVariantExtraction: TestRustEnumVariantExtraction#
---
# Module: [`tests/unit/languages/test_rust_enum_variants_796.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_enum_variants_796.py)

## Classes
### `TestRustEnumVariantExtraction`
- def: [`tests/unit/languages/test_rust_enum_variants_796.py:44`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_enum_variants_796.py#L44)
- doc: extract_variables() must yield one Variable per enum variant.
- signature: `class TestRustEnumVariantExtraction:`
- members:
  - `test_enum_variant_has_correct_variable_type(self)` — [`L83`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_enum_variants_796.py#L83) — Each variant must carry variable_type == 'enum_variant'.
  - `test_enum_variant_line_range_within_enum_span(self)` — [`L193`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_enum_variants_796.py#L193) — Variant start_line must be within the enclosing enum's line span.
  - `test_enum_variant_receiver_type_is_enum_name(self)` — [`L103`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_enum_variants_796.py#L103) — Each variant's receiver_type must be the containing enum name.
  - `test_enum_variant_visibility_inherits_enum_visibility(self)` — [`L175`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_enum_variants_796.py#L175) — Variants inherit the enclosing enum visibility for API consumers (#960).
  - `test_multiple_enums_variants_separate(self)` — [`L212`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_enum_variants_796.py#L212) — Two enums in one file: each set of variants has the correct receiver_type.
  - `test_option_like_enum_variants(self)` — [`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_enum_variants_796.py#L65) — Option<T>-style enum: None and Some variants extracted.
  - `test_simple_enum_variants_are_extracted(self)` — [`L47`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_enum_variants_796.py#L47) — Direction enum: four unit variants must each become a Variable.
  - `test_struct_fields_and_enum_variants_coexist(self)` — [`L122`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_enum_variants_796.py#L122) — Struct fields (field_declaration) must not be crowded out by enum variant extraction.
  - `test_struct_like_enum_variant_fields_do_not_leak(self)` — [`L149`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_enum_variants_796.py#L149) — Struct-like enum body fields are not ordinary struct fields (#960).
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`start_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`RustElementExtractor`](../../../tree_sitter_analyzer/languages/rust_plugin.md#RustElementExtractor), [`variable_type`](../../../tree_sitter_analyzer/models/base.md#Variable.variable_type), [`visibility`](../../../tree_sitter_analyzer/models/base.md#Variable.visibility), [`extract_variables`](../../../tree_sitter_analyzer/languages/rust_plugin.md#RustElementExtractor.extract_variables), [`receiver_type`](../../../tree_sitter_analyzer/models/base.md#Variable.receiver_type)  (2 test-only)

## Functions
- `_parse_rust(code: str)` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_enum_variants_796.py#L26) — Parse Rust code with tree-sitter-rust. Returns (tree, language) or None.

## Module values
- `_TS_RUST_AVAILABLE` — [`L17`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_enum_variants_796.py#L17)

