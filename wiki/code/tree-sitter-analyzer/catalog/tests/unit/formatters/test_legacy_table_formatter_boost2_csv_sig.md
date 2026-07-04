---
title: 'Module: tests/unit/formatters/test_legacy_table_formatter_boost2_csv_sig.py'
type: catalog
provenance: extracted
module: tests/unit/formatters/test_legacy_table_formatter_boost2_csv_sig.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.formatters.test_legacy_table_formatter_boost2_csv_sig`/Test
symbols:
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
  TestCsvFormat: CsvFormat#
  TestCreateFullSignature: CreateFullSignature#
  TestShortenType: ShortenType#
  TestConvertVisibility: ConvertVisibility#
  TestExtractDocSummary: ExtractDocSummary#
  TestCleanCsvText: CleanCsvText#
---
# Module: [`tests/unit/formatters/test_legacy_table_formatter_boost2_csv_sig.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_boost2_csv_sig.py)

## Classes
### `TestCleanCsvText`
- def: [`tests/unit/formatters/test_legacy_table_formatter_boost2_csv_sig.py:318`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_boost2_csv_sig.py#L318)
- doc: Tests for _clean_csv_text.
- signature: `class TestCleanCsvText:`
- members:
  - `test_dash_text(self)` — [`L326`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_boost2_csv_sig.py#L326) — Lines 917-918: '-' -> '-'.
  - `test_empty_text(self)` — [`L321`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_boost2_csv_sig.py#L321) — Lines 917-918: empty text -> '-'.
  - `test_extra_whitespace(self)` — [`L343`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_boost2_csv_sig.py#L343)
  - `test_text_with_newlines(self)` — [`L331`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_boost2_csv_sig.py#L331) — Line 921: newlines collapsed.
  - `test_text_with_quotes(self)` — [`L337`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_boost2_csv_sig.py#L337) — Line 924: quotes doubled.
- uses (calls/refs, reference-scoped): [`LegacyTableFormatter`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter), [`_clean_csv_text`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter._clean_csv_text)

### `TestConvertVisibility`
- def: [`tests/unit/formatters/test_legacy_table_formatter_boost2_csv_sig.py:257`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_boost2_csv_sig.py#L257)
- doc: Tests for _convert_visibility.
- signature: `class TestConvertVisibility:`
- members:
  - `test_all_values(self)` — [`L260`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_boost2_csv_sig.py#L260)
- uses (calls/refs, reference-scoped): [`LegacyTableFormatter`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter), [`_convert_visibility`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter._convert_visibility)

### `TestCreateFullSignature`
- def: [`tests/unit/formatters/test_legacy_table_formatter_boost2_csv_sig.py:125`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_boost2_csv_sig.py#L125)
- doc: Tests for _create_full_signature with all parameter types.
- signature: `class TestCreateFullSignature:`
- members:
  - `test_fallback_parameter(self)` — [`L139`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_boost2_csv_sig.py#L139) — Lines 828-830: fallback for non-dict non-string params.
  - `test_mixed_parameter_types(self)` — [`L171`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_boost2_csv_sig.py#L171) — Mix of dict, string, and other parameters.
  - `test_non_static_method(self)` — [`L160`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_boost2_csv_sig.py#L160) — Line 842: modifier_str empty -> no modifier.
  - `test_static_method(self)` — [`L149`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_boost2_csv_sig.py#L149) — Lines 836-837, 842-843: static method modifier.
  - `test_string_parameter(self)` — [`L128`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_boost2_csv_sig.py#L128) — Lines 825-827: string parameter (not dict).
- uses (calls/refs, reference-scoped): [`LegacyTableFormatter`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter), [`_create_full_signature`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter._create_full_signature)

### `TestCsvFormat`
- def: [`tests/unit/formatters/test_legacy_table_formatter_boost2_csv_sig.py:8`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_boost2_csv_sig.py#L8)
- doc: Tests for _format_csv method rows and field rows.
- signature: `class TestCsvFormat:`
- members:
  - `test_csv_fields_modifier_fallback(self)` — [`L41`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_boost2_csv_sig.py#L41) — Field static/final via is_static/is_final attributes.
  - `test_csv_with_fields(self)` — [`L11`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_boost2_csv_sig.py#L11) — CSV output with field rows (lines 787-801).
  - `test_csv_with_methods_and_fields(self)` — [`L62`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_boost2_csv_sig.py#L62) — CSV output with both methods and fields.
  - `test_csv_with_parameter_types(self)` — [`L93`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_boost2_csv_sig.py#L93) — CSV method row with parameters (line 776).
- uses (calls/refs, reference-scoped): [`LegacyTableFormatter`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter), [`format_structure`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter.format_structure)

### `TestExtractDocSummary`
- def: [`tests/unit/formatters/test_legacy_table_formatter_boost2_csv_sig.py:274`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_boost2_csv_sig.py#L274)
- doc: Tests for _extract_doc_summary.
- signature: `class TestExtractDocSummary:`
- members:
  - `test_empty_javadoc(self)` — [`L277`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_boost2_csv_sig.py#L277) — Lines 899-900: empty javadoc -> '-'.
  - `test_multiline(self)` — [`L300`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_boost2_csv_sig.py#L300)
  - `test_no_period(self)` — [`L293`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_boost2_csv_sig.py#L293) — Lines 908-913: javadoc without period.
  - `test_none_javadoc(self)` — [`L282`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_boost2_csv_sig.py#L282)
  - `test_single_sentence(self)` — [`L286`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_boost2_csv_sig.py#L286) — Lines 908-911: javadoc with a single sentence.
  - `test_with_return_tag(self)` — [`L306`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_boost2_csv_sig.py#L306)
- uses (calls/refs, reference-scoped): [`LegacyTableFormatter`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter), [`_extract_doc_summary`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter._extract_doc_summary)

### `TestShortenType`
- def: [`tests/unit/formatters/test_legacy_table_formatter_boost2_csv_sig.py:193`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_boost2_csv_sig.py#L193)
- doc: Tests for _shorten_type with all branches.
- signature: `class TestShortenType:`
- members:
  - `test_all_known_mappings(self)` — [`L233`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_boost2_csv_sig.py#L233)
  - `test_array_known_type(self)` — [`L218`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_boost2_csv_sig.py#L218) — Lines 883-886: String[] -> S[].
  - `test_array_unknown_type(self)` — [`L223`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_boost2_csv_sig.py#L223)
  - `test_empty_array(self)` — [`L228`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_boost2_csv_sig.py#L228) — Lines 887-888: '[]' with empty base -> 'O[]'.
  - `test_list_generic(self)` — [`L212`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_boost2_csv_sig.py#L212) — Lines 879-880: List<String> -> L<S>.
  - `test_map_generic(self)` — [`L206`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_boost2_csv_sig.py#L206) — Lines 871-876: Map<String,Object> -> M<S,O>.
  - `test_non_string_type(self)` — [`L201`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_boost2_csv_sig.py#L201) — Lines 853-854: non-string type_name.
  - `test_none_type(self)` — [`L196`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_boost2_csv_sig.py#L196) — Lines 849-850: type_name is None -> 'O'.
  - `test_unknown_type(self)` — [`L247`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_boost2_csv_sig.py#L247)
- uses (calls/refs, reference-scoped): [`LegacyTableFormatter`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter), [`_shorten_type`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter._shorten_type)

