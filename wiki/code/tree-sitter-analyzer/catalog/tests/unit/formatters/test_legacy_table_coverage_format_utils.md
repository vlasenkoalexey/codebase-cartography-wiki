---
title: 'Module: tests/unit/formatters/test_legacy_table_coverage_format_utils.py'
type: catalog
provenance: extracted
module: tests/unit/formatters/test_legacy_table_coverage_format_utils.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.formatters.test_legacy_table_coverage_format_utils`/Test
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
  TestCsvFormat.test_csv_with_fields: CsvFormat#test_csv_with_fields().
  TestCsvFormat.test_csv_fields_modifier_fallback: CsvFormat#test_csv_fields_modifier_fallback().
  TestCsvFormat.test_csv_with_methods_and_fields: CsvFormat#test_csv_with_methods_and_fields().
  TestCsvFormat.test_csv_with_parameter_types: CsvFormat#test_csv_with_parameter_types().
  TestCreateFullSignature.test_string_parameter: CreateFullSignature#test_string_parameter().
  TestCreateFullSignature.test_fallback_parameter: CreateFullSignature#test_fallback_parameter().
  TestCreateFullSignature.test_static_method: CreateFullSignature#test_static_method().
  TestCreateFullSignature.test_non_static_method: CreateFullSignature#test_non_static_method().
  TestCreateFullSignature.test_mixed_parameter_types: CreateFullSignature#test_mixed_parameter_types().
  TestShortenType.test_none_type: ShortenType#test_none_type().
  TestShortenType.test_non_string_type: ShortenType#test_non_string_type().
  TestShortenType.test_map_generic: ShortenType#test_map_generic().
  TestShortenType.test_list_generic: ShortenType#test_list_generic().
  TestShortenType.test_array_known_type: ShortenType#test_array_known_type().
  TestShortenType.test_array_unknown_type: ShortenType#test_array_unknown_type().
  TestShortenType.test_empty_array: ShortenType#test_empty_array().
  TestShortenType.test_all_known_mappings: ShortenType#test_all_known_mappings().
  TestShortenType.test_unknown_type: ShortenType#test_unknown_type().
  TestConvertVisibility.test_all_values: ConvertVisibility#test_all_values().
  TestExtractDocSummary.test_empty_javadoc: ExtractDocSummary#test_empty_javadoc().
  TestExtractDocSummary.test_none_javadoc: ExtractDocSummary#test_none_javadoc().
  TestExtractDocSummary.test_single_sentence: ExtractDocSummary#test_single_sentence().
  TestExtractDocSummary.test_no_period: ExtractDocSummary#test_no_period().
  TestExtractDocSummary.test_multiline: ExtractDocSummary#test_multiline().
  TestExtractDocSummary.test_with_return_tag: ExtractDocSummary#test_with_return_tag().
  TestCleanCsvText.test_empty_text: CleanCsvText#test_empty_text().
  TestCleanCsvText.test_dash_text: CleanCsvText#test_dash_text().
  TestCleanCsvText.test_text_with_newlines: CleanCsvText#test_text_with_newlines().
  TestCleanCsvText.test_text_with_quotes: CleanCsvText#test_text_with_quotes().
  TestCleanCsvText.test_extra_whitespace: CleanCsvText#test_extra_whitespace().
  TestFormatMethodRowDetailed: FormatMethodRowDetailed#
  TestCreateCompactSignature: CreateCompactSignature#
  TestAbbreviateType: AbbreviateType#
  TestGetVisibilitySymbol: GetVisibilitySymbol#
  TestCompactTableEdgeCases: CompactTableEdgeCases#
  TestCsvFormat: CsvFormat#
  TestCreateFullSignature: CreateFullSignature#
  TestShortenType: ShortenType#
  TestConvertVisibility: ConvertVisibility#
  TestExtractDocSummary: ExtractDocSummary#
  TestCleanCsvText: CleanCsvText#
---
# Module: [`tests/unit/formatters/test_legacy_table_coverage_format_utils.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_format_utils.py)

## Classes
### `TestAbbreviateType`
- def: [`tests/unit/formatters/test_legacy_table_coverage_format_utils.py:99`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_format_utils.py#L99)
- doc: Tests for _abbreviate_type.
- signature: `class TestAbbreviateType:`
- members:
  - `test_array_type(self)` — [`L115`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_format_utils.py#L115) — Lines 616-618: abbreviate array type.
  - `test_empty_type(self)` — [`L126`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_format_utils.py#L126) — Line 620: empty type -> '?'.
  - `test_exception_type(self)` — [`L131`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_format_utils.py#L131)
  - `test_generic_type(self)` — [`L109`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_format_utils.py#L109) — Lines 607-613: abbreviate generic type.
  - `test_standard_types(self)` — [`L102`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_format_utils.py#L102)
  - `test_unknown_array(self)` — [`L120`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_format_utils.py#L120) — Array of unknown type.
- uses (calls/refs, reference-scoped): [`LegacyTableFormatter`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter), [`_abbreviate_type`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter._abbreviate_type)

### `TestCleanCsvText`
- def: [`tests/unit/formatters/test_legacy_table_coverage_format_utils.py:514`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_format_utils.py#L514)
- doc: Tests for _clean_csv_text.
- signature: `class TestCleanCsvText:`
- members:
  - `test_dash_text(self)` — [`L522`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_format_utils.py#L522) — Lines 917-918: '-' -> '-'. — documented in [tree_sitter_analyzer-legacy_table_formatter](../../../../concepts/tree_sitter_analyzer-legacy_table_formatter.md)
  - `test_empty_text(self)` — [`L517`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_format_utils.py#L517) — Lines 917-918: empty text -> '-'.
  - `test_extra_whitespace(self)` — [`L539`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_format_utils.py#L539)
  - `test_text_with_newlines(self)` — [`L527`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_format_utils.py#L527) — Line 921: newlines collapsed.
  - `test_text_with_quotes(self)` — [`L533`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_format_utils.py#L533) — Line 924: quotes doubled. — documented in [tree_sitter_analyzer-legacy_table_formatter](../../../../concepts/tree_sitter_analyzer-legacy_table_formatter.md)
- uses (calls/refs, reference-scoped): [`LegacyTableFormatter`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter), [`_clean_csv_text`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter._clean_csv_text)

### `TestCompactTableEdgeCases`
- def: [`tests/unit/formatters/test_legacy_table_coverage_format_utils.py:150`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_format_utils.py#L150)
- doc: Tests for _format_compact_table edge cases.
- signature: `class TestCompactTableEdgeCases:`
- members:
  - `test_classes_empty_list(self)` — [`L181`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_format_utils.py#L181)
  - `test_classes_is_none(self)` — [`L153`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_format_utils.py#L153) — Bug #778 fixed: classes=None must not yield '# Unknown'. — documented in [tree_sitter_analyzer-legacy_table_formatter](../../../../concepts/tree_sitter_analyzer-legacy_table_formatter.md)
  - `test_compact_with_fields(self)` — [`L209`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_format_utils.py#L209) — Compact table with fields.
  - `test_compact_with_methods(self)` — [`L188`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_format_utils.py#L188) — Compact table with methods (hits _format_compact_method_row).
  - `test_with_package_name(self)` — [`L160`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_format_utils.py#L160) — Lines 645-646, 658-659: with package name.
- uses (calls/refs, reference-scoped): [`LegacyTableFormatter`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter), [`format_structure`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter.format_structure)

### `TestConvertVisibility`
- def: [`tests/unit/formatters/test_legacy_table_coverage_format_utils.py:463`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_format_utils.py#L463)
- doc: Tests for _convert_visibility.
- signature: `class TestConvertVisibility:`
- members:
  - `test_all_values(self)` — [`L466`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_format_utils.py#L466)
- uses (calls/refs, reference-scoped): [`LegacyTableFormatter`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter), [`_convert_visibility`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter._convert_visibility)

### `TestCreateCompactSignature`
- def: [`tests/unit/formatters/test_legacy_table_coverage_format_utils.py:72`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_format_utils.py#L72)
- doc: Tests for _create_compact_signature.
- signature: `class TestCreateCompactSignature:`
- members:
  - `test_no_params(self)` — [`L88`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_format_utils.py#L88) — Compact signature with no parameters.
  - `test_with_params(self)` — [`L75`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_format_utils.py#L75) — Lines 568-578: compact signature with parameters.
- uses (calls/refs, reference-scoped): [`LegacyTableFormatter`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter), [`_create_compact_signature`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter._create_compact_signature)

### `TestCreateFullSignature`
- def: [`tests/unit/formatters/test_legacy_table_coverage_format_utils.py:341`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_format_utils.py#L341)
- doc: Tests for _create_full_signature with all parameter types.
- signature: `class TestCreateFullSignature:`
- members:
  - `test_fallback_parameter(self)` — [`L355`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_format_utils.py#L355) — Lines 828-830: fallback for non-dict non-string params. — documented in [tree_sitter_analyzer-legacy_table_formatter](../../../../concepts/tree_sitter_analyzer-legacy_table_formatter.md)
  - `test_mixed_parameter_types(self)` — [`L387`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_format_utils.py#L387) — Mix of dict, string, and other parameters.
  - `test_non_static_method(self)` — [`L376`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_format_utils.py#L376) — Line 842: modifier_str empty -> no modifier.
  - `test_static_method(self)` — [`L365`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_format_utils.py#L365) — Lines 836-837, 842-843: static method modifier.
  - `test_string_parameter(self)` — [`L344`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_format_utils.py#L344) — Lines 825-827: string parameter (not dict).
- uses (calls/refs, reference-scoped): [`LegacyTableFormatter`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter), [`_create_full_signature`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter._create_full_signature)

### `TestCsvFormat`
- def: [`tests/unit/formatters/test_legacy_table_coverage_format_utils.py:229`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_format_utils.py#L229)
- doc: Tests for _format_csv method rows and field rows.
- signature: `class TestCsvFormat:`
- members:
  - `test_csv_fields_modifier_fallback(self)` — [`L262`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_format_utils.py#L262) — Field static/final via is_static/is_final attributes.
  - `test_csv_with_fields(self)` — [`L232`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_format_utils.py#L232) — CSV output with field rows (lines 787-801).
  - `test_csv_with_methods_and_fields(self)` — [`L283`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_format_utils.py#L283) — CSV output with both methods and fields.
  - `test_csv_with_parameter_types(self)` — [`L314`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_format_utils.py#L314) — CSV method row with parameters (line 776).
- uses (calls/refs, reference-scoped): [`LegacyTableFormatter`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter), [`format_structure`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter.format_structure)

### `TestExtractDocSummary`
- def: [`tests/unit/formatters/test_legacy_table_coverage_format_utils.py:475`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_format_utils.py#L475)
- doc: Tests for _extract_doc_summary.
- signature: `class TestExtractDocSummary:`
- members:
  - `test_empty_javadoc(self)` — [`L478`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_format_utils.py#L478) — Lines 899-900: empty javadoc -> '-'.
  - `test_multiline(self)` — [`L501`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_format_utils.py#L501)
  - `test_no_period(self)` — [`L494`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_format_utils.py#L494) — Lines 908-913: javadoc without period.
  - `test_none_javadoc(self)` — [`L483`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_format_utils.py#L483)
  - `test_single_sentence(self)` — [`L487`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_format_utils.py#L487) — Lines 908-911: javadoc with a single sentence.
  - `test_with_return_tag(self)` — [`L507`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_format_utils.py#L507)
- uses (calls/refs, reference-scoped): [`LegacyTableFormatter`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter), [`_extract_doc_summary`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter._extract_doc_summary)

### `TestFormatMethodRowDetailed`
- def: [`tests/unit/formatters/test_legacy_table_coverage_format_utils.py:24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_format_utils.py#L24)
- doc: Tests for _format_method_row_detailed.
- signature: `class TestFormatMethodRowDetailed:`
- members:
  - `test_basic(self)` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_format_utils.py#L27)
  - `test_static_method(self)` — [`L57`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_format_utils.py#L57)
  - `test_with_javadoc_enabled(self)` — [`L43`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_format_utils.py#L43)
- uses (calls/refs, reference-scoped): [`LegacyTableFormatter`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter), [`_format_method_row_detailed`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter._format_method_row_detailed)

### `TestGetVisibilitySymbol`
- def: [`tests/unit/formatters/test_legacy_table_coverage_format_utils.py:136`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_format_utils.py#L136)
- doc: Tests for _get_visibility_symbol.
- signature: `class TestGetVisibilitySymbol:`
- members:
  - `test_all_symbols(self)` — [`L139`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_format_utils.py#L139)
- uses (calls/refs, reference-scoped): [`LegacyTableFormatter`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter), [`_get_visibility_symbol`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter._get_visibility_symbol)

### `TestShortenType`
- def: [`tests/unit/formatters/test_legacy_table_coverage_format_utils.py:404`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_format_utils.py#L404)
- doc: Tests for _shorten_type with all branches.
- signature: `class TestShortenType:`
- members:
  - `test_all_known_mappings(self)` — [`L444`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_format_utils.py#L444)
  - `test_array_known_type(self)` — [`L429`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_format_utils.py#L429) — Lines 883-886: String[] -> S[].
  - `test_array_unknown_type(self)` — [`L434`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_format_utils.py#L434)
  - `test_empty_array(self)` — [`L439`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_format_utils.py#L439) — Lines 887-888: '[]' with empty base -> 'O[]'.
  - `test_list_generic(self)` — [`L423`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_format_utils.py#L423) — Lines 879-880: List<String> -> L<S>.
  - `test_map_generic(self)` — [`L417`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_format_utils.py#L417) — Lines 871-876: Map<String,Object> -> M<S,O>.
  - `test_non_string_type(self)` — [`L412`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_format_utils.py#L412) — Lines 853-854: non-string type_name.
  - `test_none_type(self)` — [`L407`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_format_utils.py#L407) — Lines 849-850: type_name is None -> 'O'.
  - `test_unknown_type(self)` — [`L458`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_format_utils.py#L458)
- uses (calls/refs, reference-scoped): [`LegacyTableFormatter`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter), [`_shorten_type`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter._shorten_type)

