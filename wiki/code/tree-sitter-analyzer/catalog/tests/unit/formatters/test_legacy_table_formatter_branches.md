---
title: 'Module: tests/unit/formatters/test_legacy_table_formatter_branches.py'
type: catalog
provenance: extracted
module: tests/unit/formatters/test_legacy_table_formatter_branches.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.formatters.test_legacy_table_formatter_branches`/Test
symbols:
  TestCreateFullSignatureBranches.test_static_method_signature: CreateFullSignatureBranches#test_static_method_signature().
  TestCreateFullSignatureBranches.test_string_param_signature: CreateFullSignatureBranches#test_string_param_signature().
  TestCreateFullSignatureBranches.test_fallback_param_signature: CreateFullSignatureBranches#test_fallback_param_signature().
  TestAbbreviateTypeAdvanced.test_generic_type_map: AbbreviateTypeAdvanced#test_generic_type_map().
  TestAbbreviateTypeAdvanced.test_generic_type_custom: AbbreviateTypeAdvanced#test_generic_type_custom().
  TestAbbreviateTypeAdvanced.test_array_type: AbbreviateTypeAdvanced#test_array_type().
  TestAbbreviateTypeAdvanced.test_empty_string_type: AbbreviateTypeAdvanced#test_empty_string_type().
  TestAbbreviateTypeAdvanced.test_unknown_type: AbbreviateTypeAdvanced#test_unknown_type().
  TestCompactTableClassesNone.test_compact_with_none_classes: CompactTableClassesNone#test_compact_with_none_classes().
  TestCompactTableClassesNone.test_compact_no_package: CompactTableClassesNone#test_compact_no_package().
  TestCompactTableClassesNone.test_compact_with_methods_and_fields: CompactTableClassesNone#test_compact_with_methods_and_fields().
  TestShortenTypeBranches.test_none_type: ShortenTypeBranches#test_none_type().
  TestShortenTypeBranches.test_non_string_type: ShortenTypeBranches#test_non_string_type().
  TestShortenTypeBranches.test_map_type: ShortenTypeBranches#test_map_type().
  TestShortenTypeBranches.test_list_type: ShortenTypeBranches#test_list_type().
  TestShortenTypeBranches.test_array_type: ShortenTypeBranches#test_array_type().
  TestShortenTypeBranches.test_empty_array_type: ShortenTypeBranches#test_empty_array_type().
  TestShortenTypeBranches.test_unmapped_type: ShortenTypeBranches#test_unmapped_type().
  TestDocSummaryAndCSVText.test_extract_doc_with_javadoc: DocSummaryAndCSVText#test_extract_doc_with_javadoc().
  TestDocSummaryAndCSVText.test_extract_doc_empty: DocSummaryAndCSVText#test_extract_doc_empty().
  TestDocSummaryAndCSVText.test_clean_csv_text_with_newlines: DocSummaryAndCSVText#test_clean_csv_text_with_newlines().
  TestDocSummaryAndCSVText.test_clean_csv_text_empty: DocSummaryAndCSVText#test_clean_csv_text_empty().
  TestDocSummaryAndCSVText.test_clean_csv_text_dash: DocSummaryAndCSVText#test_clean_csv_text_dash().
  TestDocSummaryAndCSVText.test_clean_csv_text_with_quotes: DocSummaryAndCSVText#test_clean_csv_text_with_quotes().
  TestCreateFullSignatureBranches: CreateFullSignatureBranches#
  TestAbbreviateTypeAdvanced: AbbreviateTypeAdvanced#
  TestCompactTableClassesNone: CompactTableClassesNone#
  TestShortenTypeBranches: ShortenTypeBranches#
  TestDocSummaryAndCSVText: DocSummaryAndCSVText#
---
# Module: [`tests/unit/formatters/test_legacy_table_formatter_branches.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_branches.py)

## Classes
### `TestAbbreviateTypeAdvanced`
- def: [`tests/unit/formatters/test_legacy_table_formatter_branches.py:56`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_branches.py#L56)
- doc: Cover _abbreviate_type generic and array branches.
- signature: `class TestAbbreviateTypeAdvanced:`
- members:
  - `test_array_type(self)` — [`L69`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_branches.py#L69)
  - `test_empty_string_type(self)` — [`L74`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_branches.py#L74)
  - `test_generic_type_custom(self)` — [`L64`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_branches.py#L64)
  - `test_generic_type_map(self)` — [`L59`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_branches.py#L59)
  - `test_unknown_type(self)` — [`L79`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_branches.py#L79)
- uses (calls/refs, reference-scoped): [`LegacyTableFormatter`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter), [`_abbreviate_type`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter._abbreviate_type)

### `TestCompactTableClassesNone`
- def: [`tests/unit/formatters/test_legacy_table_formatter_branches.py:90`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_branches.py#L90)
- doc: Cover _format_compact_table when classes is None.
- signature: `class TestCompactTableClassesNone:`
- members:
  - `test_compact_no_package(self)` — [`L104`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_branches.py#L104)
  - `test_compact_with_methods_and_fields(self)` — [`L114`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_branches.py#L114)
  - `test_compact_with_none_classes(self)` — [`L93`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_branches.py#L93)
- uses (calls/refs, reference-scoped): [`LegacyTableFormatter`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter), [`format_structure`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter.format_structure)

### `TestCreateFullSignatureBranches`
- def: [`tests/unit/formatters/test_legacy_table_formatter_branches.py:11`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_branches.py#L11)
- doc: Cover _create_full_signature with static, string/fallback params.
- signature: `class TestCreateFullSignatureBranches:`
- members:
  - `test_fallback_param_signature(self)` — [`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_branches.py#L39)
  - `test_static_method_signature(self)` — [`L14`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_branches.py#L14)
  - `test_string_param_signature(self)` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_branches.py#L27)
- uses (calls/refs, reference-scoped): [`LegacyTableFormatter`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter), [`_create_full_signature`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter._create_full_signature)

### `TestDocSummaryAndCSVText`
- def: [`tests/unit/formatters/test_legacy_table_formatter_branches.py:194`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_branches.py#L194)
- doc: Cover _extract_doc_summary and _clean_csv_text edge cases.
- signature: `class TestDocSummaryAndCSVText:`
- members:
  - `test_clean_csv_text_dash(self)` — [`L215`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_branches.py#L215)
  - `test_clean_csv_text_empty(self)` — [`L211`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_branches.py#L211)
  - `test_clean_csv_text_with_newlines(self)` — [`L206`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_branches.py#L206)
  - `test_clean_csv_text_with_quotes(self)` — [`L219`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_branches.py#L219)
  - `test_extract_doc_empty(self)` — [`L202`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_branches.py#L202)
  - `test_extract_doc_with_javadoc(self)` — [`L197`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_branches.py#L197)
- uses (calls/refs, reference-scoped): [`LegacyTableFormatter`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter), [`_clean_csv_text`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter._clean_csv_text), [`_extract_doc_summary`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter._extract_doc_summary)

### `TestShortenTypeBranches`
- def: [`tests/unit/formatters/test_legacy_table_formatter_branches.py:152`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_branches.py#L152)
- doc: Cover _shorten_type edge cases.
- signature: `class TestShortenTypeBranches:`
- members:
  - `test_array_type(self)` — [`L173`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_branches.py#L173)
  - `test_empty_array_type(self)` — [`L178`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_branches.py#L178)
  - `test_list_type(self)` — [`L168`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_branches.py#L168)
  - `test_map_type(self)` — [`L163`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_branches.py#L163)
  - `test_non_string_type(self)` — [`L159`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_branches.py#L159)
  - `test_none_type(self)` — [`L155`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_branches.py#L155)
  - `test_unmapped_type(self)` — [`L183`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_branches.py#L183)
- uses (calls/refs, reference-scoped): [`LegacyTableFormatter`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter), [`_shorten_type`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter._shorten_type)

