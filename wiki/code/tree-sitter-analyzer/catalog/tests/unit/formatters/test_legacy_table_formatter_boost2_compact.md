---
title: 'Module: tests/unit/formatters/test_legacy_table_formatter_boost2_compact.py'
type: catalog
provenance: extracted
module: tests/unit/formatters/test_legacy_table_formatter_boost2_compact.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.formatters.test_legacy_table_formatter_boost2_compact`/Test
symbols:
  TestFormatMethodRowDetailed.test_basic: FormatMethodRowDetailed#test_basic().
  TestFormatMethodRowDetailed.test_with_javadoc_enabled: FormatMethodRowDetailed#test_with_javadoc_enabled().
  TestFormatMethodRowDetailed.test_static_method: FormatMethodRowDetailed#test_static_method().
  TestCreateCompactSignature.test_with_params: CreateCompactSignature#test_with_params().
  TestCreateCompactSignature.test_no_params: CreateCompactSignature#test_no_params().
  TestAbbreviateType.test_standard_types: AbbreviateType#test_standard_types().
  TestAbbreviateType.test_generic_type: AbbreviateType#test_generic_type().
  TestAbbreviateType.test_array_type: AbbreviateType#test_array_type().
  TestAbbreviateType.test_unknown_array: AbbreviateType#test_unknown_array().
  TestAbbreviateType.test_empty_type: AbbreviateType#test_empty_type().
  TestAbbreviateType.test_exception_type: AbbreviateType#test_exception_type().
  TestGetVisibilitySymbol.test_all_symbols: GetVisibilitySymbol#test_all_symbols().
  TestCompactTableEdgeCases.test_classes_is_none: CompactTableEdgeCases#test_classes_is_none().
  TestCompactTableEdgeCases.test_with_package_name: CompactTableEdgeCases#test_with_package_name().
  TestCompactTableEdgeCases.test_classes_empty_list: CompactTableEdgeCases#test_classes_empty_list().
  TestCompactTableEdgeCases.test_compact_with_methods: CompactTableEdgeCases#test_compact_with_methods().
  TestCompactTableEdgeCases.test_compact_with_fields: CompactTableEdgeCases#test_compact_with_fields().
  TestFormatMethodRowDetailed: FormatMethodRowDetailed#
  TestCreateCompactSignature: CreateCompactSignature#
  TestAbbreviateType: AbbreviateType#
  TestGetVisibilitySymbol: GetVisibilitySymbol#
  TestCompactTableEdgeCases: CompactTableEdgeCases#
---
# Module: [`tests/unit/formatters/test_legacy_table_formatter_boost2_compact.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_boost2_compact.py)

## Classes
### `TestAbbreviateType`
- def: [`tests/unit/formatters/test_legacy_table_formatter_boost2_compact.py:92`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_boost2_compact.py#L92)
- doc: Tests for _abbreviate_type.
- signature: `class TestAbbreviateType:`
- members:
  - `test_array_type(self)` — [`L108`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_boost2_compact.py#L108) — Lines 616-618: abbreviate array type.
  - `test_empty_type(self)` — [`L119`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_boost2_compact.py#L119) — Line 620: empty type -> '?'.
  - `test_exception_type(self)` — [`L124`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_boost2_compact.py#L124)
  - `test_generic_type(self)` — [`L102`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_boost2_compact.py#L102) — Lines 607-613: abbreviate generic type.
  - `test_standard_types(self)` — [`L95`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_boost2_compact.py#L95)
  - `test_unknown_array(self)` — [`L113`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_boost2_compact.py#L113) — Array of unknown type.
- uses (calls/refs, reference-scoped): [`LegacyTableFormatter`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter), [`_abbreviate_type`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter._abbreviate_type)

### `TestCompactTableEdgeCases`
- def: [`tests/unit/formatters/test_legacy_table_formatter_boost2_compact.py:153`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_boost2_compact.py#L153)
- doc: Tests for _format_compact_table edge cases.
- signature: `class TestCompactTableEdgeCases:`
- members:
  - `test_classes_empty_list(self)` — [`L184`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_boost2_compact.py#L184)
  - `test_classes_is_none(self)` — [`L156`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_boost2_compact.py#L156) — Bug #778 fixed: classes=None must not produce '# Unknown'.
  - `test_compact_with_fields(self)` — [`L212`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_boost2_compact.py#L212) — Compact table with fields.
  - `test_compact_with_methods(self)` — [`L191`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_boost2_compact.py#L191) — Compact table with methods (hits _format_compact_method_row).
  - `test_with_package_name(self)` — [`L163`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_boost2_compact.py#L163) — Lines 645-646, 658-659: with package name.
- uses (calls/refs, reference-scoped): [`LegacyTableFormatter`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter), [`format_structure`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter.format_structure)

### `TestCreateCompactSignature`
- def: [`tests/unit/formatters/test_legacy_table_formatter_boost2_compact.py:60`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_boost2_compact.py#L60)
- doc: Tests for _create_compact_signature.
- signature: `class TestCreateCompactSignature:`
- members:
  - `test_no_params(self)` — [`L76`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_boost2_compact.py#L76) — Compact signature with no parameters.
  - `test_with_params(self)` — [`L63`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_boost2_compact.py#L63) — Lines 568-578: compact signature with parameters.
- uses (calls/refs, reference-scoped): [`LegacyTableFormatter`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter), [`_create_compact_signature`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter._create_compact_signature)

### `TestFormatMethodRowDetailed`
- def: [`tests/unit/formatters/test_legacy_table_formatter_boost2_compact.py:7`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_boost2_compact.py#L7)
- doc: Tests for _format_method_row_detailed.
- signature: `class TestFormatMethodRowDetailed:`
- members:
  - `test_basic(self)` — [`L10`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_boost2_compact.py#L10)
  - `test_static_method(self)` — [`L40`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_boost2_compact.py#L40)
  - `test_with_javadoc_enabled(self)` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_boost2_compact.py#L26)
- uses (calls/refs, reference-scoped): [`LegacyTableFormatter`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter), [`_format_method_row_detailed`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter._format_method_row_detailed)

### `TestGetVisibilitySymbol`
- def: [`tests/unit/formatters/test_legacy_table_formatter_boost2_compact.py:134`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_boost2_compact.py#L134)
- doc: Tests for _get_visibility_symbol.
- signature: `class TestGetVisibilitySymbol:`
- members:
  - `test_all_symbols(self)` — [`L137`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_boost2_compact.py#L137)
- uses (calls/refs, reference-scoped): [`LegacyTableFormatter`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter), [`_get_visibility_symbol`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter._get_visibility_symbol)

