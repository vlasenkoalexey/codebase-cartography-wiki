---
title: 'Module: tests/unit/formatters/test_legacy_table_formatter_advanced.py'
type: catalog
provenance: extracted
module: tests/unit/formatters/test_legacy_table_formatter_advanced.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.formatters.test_legacy_table_formatter_advanced`/Test
symbols:
  TestFullTableMultiClassParamTypes.test_string_param_in_multi_class: FullTableMultiClassParamTypes#test_string_param_in_multi_class().
  TestFullTableMultiClassParamTypes.test_fallback_param_in_multi_class: FullTableMultiClassParamTypes#test_fallback_param_in_multi_class().
  TestPlatformNewlines.test_get_platform_newline: PlatformNewlines#test_get_platform_newline().
  TestPlatformNewlines.test_convert_to_platform_newlines: PlatformNewlines#test_convert_to_platform_newlines().
  TestPlatformNewlines.test_csv_skips_newline_conversion: PlatformNewlines#test_csv_skips_newline_conversion().
  TestEdgeCases.test_none_classes: EdgeCases#test_none_classes().
  TestEdgeCases.test_none_methods: EdgeCases#test_none_methods().
  TestEdgeCases.test_none_fields: EdgeCases#test_none_fields().
  TestEdgeCases.test_empty_package_name: EdgeCases#test_empty_package_name().
  TestEdgeCases.test_unknown_package: EdgeCases#test_unknown_package().
  TestEdgeCases.test_file_path_handling: EdgeCases#test_file_path_handling().
  TestEdgeCases.test_file_path_with_various_extensions: EdgeCases#test_file_path_with_various_extensions().
  TestEdgeCases.test_method_with_no_parameters: EdgeCases#test_method_with_no_parameters().
  TestEdgeCases.test_parameter_as_plain_string: EdgeCases#test_parameter_as_plain_string().
  TestEdgeCases.test_parameter_as_other_type: EdgeCases#test_parameter_as_other_type().
  TestEdgeCases.test_missing_line_range: EdgeCases#test_missing_line_range().
  TestDetailedFormatting.test_get_class_methods_basic: DetailedFormatting#test_get_class_methods_basic().
  TestDetailedFormatting.test_get_class_fields_basic: DetailedFormatting#test_get_class_fields_basic().
  TestDetailedFormatting.test_get_class_methods_excludes_nested: DetailedFormatting#test_get_class_methods_excludes_nested().
  TestDetailedFormatting.test_get_class_fields_excludes_nested: DetailedFormatting#test_get_class_fields_excludes_nested().
  TestLanguageSpecificFormatting.test_python_language_formatting: LanguageSpecificFormatting#test_python_language_formatting().
  TestLanguageSpecificFormatting.test_java_language_formatting: LanguageSpecificFormatting#test_java_language_formatting().
  TestLanguageSpecificFormatting.test_javascript_language_formatting: LanguageSpecificFormatting#test_javascript_language_formatting().
  TestCSVFieldAndParamCoverage.test_csv_with_field_rows: CSVFieldAndParamCoverage#test_csv_with_field_rows().
  TestCSVFieldAndParamCoverage.test_csv_method_with_string_params: CSVFieldAndParamCoverage#test_csv_method_with_string_params().
  TestCSVFieldAndParamCoverage.test_csv_method_with_fallback_params: CSVFieldAndParamCoverage#test_csv_method_with_fallback_params().
  TestCSVFieldAndParamCoverage.test_csv_method_is_static: CSVFieldAndParamCoverage#test_csv_method_is_static().
  TestCSVFieldAndParamCoverage.test_csv_method_is_final: CSVFieldAndParamCoverage#test_csv_method_is_final().
  TestCSVFieldAndParamCoverage.test_csv_constructor: CSVFieldAndParamCoverage#test_csv_constructor().
  TestCSVFieldAndParamCoverage.test_csv_class_with_final_modifier: CSVFieldAndParamCoverage#test_csv_class_with_final_modifier().
  TestCSVFieldAndParamCoverage.test_csv_field_with_is_static_flag: CSVFieldAndParamCoverage#test_csv_field_with_is_static_flag().
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
  TestDetailedFormatting.formatter_with_javadoc: DetailedFormatting#formatter_with_javadoc().
  TestFullTableMultiClassParamTypes._multi_class_data: FullTableMultiClassParamTypes#_multi_class_data().
  TestPlatformNewlines: PlatformNewlines#
  TestEdgeCases: EdgeCases#
  TestDetailedFormatting: DetailedFormatting#
  TestLanguageSpecificFormatting: LanguageSpecificFormatting#
  TestFullTableMultiClassParamTypes: FullTableMultiClassParamTypes#
  TestCSVFieldAndParamCoverage: CSVFieldAndParamCoverage#
  TestCreateFullSignatureBranches: CreateFullSignatureBranches#
  TestAbbreviateTypeAdvanced: AbbreviateTypeAdvanced#
  TestCompactTableClassesNone: CompactTableClassesNone#
  TestShortenTypeBranches: ShortenTypeBranches#
  TestDocSummaryAndCSVText: DocSummaryAndCSVText#
---
# Module: [`tests/unit/formatters/test_legacy_table_formatter_advanced.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_advanced.py)

## Classes
### `TestAbbreviateTypeAdvanced`
- def: [`tests/unit/formatters/test_legacy_table_formatter_advanced.py:485`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_advanced.py#L485)
- signature: `class TestAbbreviateTypeAdvanced:`
- members:
  - `test_array_type(self)` — [`L496`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_advanced.py#L496)
  - `test_empty_string_type(self)` — [`L501`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_advanced.py#L501)
  - `test_generic_type_custom(self)` — [`L491`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_advanced.py#L491)
  - `test_generic_type_map(self)` — [`L486`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_advanced.py#L486)
  - `test_unknown_type(self)` — [`L506`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_advanced.py#L506)
- uses (calls/refs, reference-scoped): [`LegacyTableFormatter`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter), [`_abbreviate_type`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter._abbreviate_type)

### `TestCSVFieldAndParamCoverage`
- def: [`tests/unit/formatters/test_legacy_table_formatter_advanced.py:310`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_advanced.py#L310)
- signature: `class TestCSVFieldAndParamCoverage:`
- members:
  - `test_csv_class_with_final_modifier(self)` — [`L412`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_advanced.py#L412)
  - `test_csv_constructor(self)` — [`L395`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_advanced.py#L395)
  - `test_csv_field_with_is_static_flag(self)` — [`L429`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_advanced.py#L429)
  - `test_csv_method_is_final(self)` — [`L378`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_advanced.py#L378)
  - `test_csv_method_is_static(self)` — [`L361`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_advanced.py#L361)
  - `test_csv_method_with_fallback_params(self)` — [`L345`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_advanced.py#L345)
  - `test_csv_method_with_string_params(self)` — [`L329`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_advanced.py#L329)
  - `test_csv_with_field_rows(self)` — [`L311`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_advanced.py#L311)
- uses (calls/refs, reference-scoped): [`LegacyTableFormatter`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter), [`format_structure`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter.format_structure)

### `TestCompactTableClassesNone`
- def: [`tests/unit/formatters/test_legacy_table_formatter_advanced.py:512`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_advanced.py#L512)
- signature: `class TestCompactTableClassesNone:`
- members:
  - `test_compact_no_package(self)` — [`L525`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_advanced.py#L525)
  - `test_compact_with_methods_and_fields(self)` — [`L535`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_advanced.py#L535)
  - `test_compact_with_none_classes(self)` — [`L513`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_advanced.py#L513)
- uses (calls/refs, reference-scoped): [`LegacyTableFormatter`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter), [`format_structure`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter.format_structure)

### `TestCreateFullSignatureBranches`
- def: [`tests/unit/formatters/test_legacy_table_formatter_advanced.py:447`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_advanced.py#L447)
- signature: `class TestCreateFullSignatureBranches:`
- members:
  - `test_fallback_param_signature(self)` — [`L473`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_advanced.py#L473)
  - `test_static_method_signature(self)` — [`L448`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_advanced.py#L448)
  - `test_string_param_signature(self)` — [`L461`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_advanced.py#L461)
- uses (calls/refs, reference-scoped): [`LegacyTableFormatter`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter), [`_create_full_signature`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter._create_full_signature)

### `TestDetailedFormatting`
- def: [`tests/unit/formatters/test_legacy_table_formatter_advanced.py:156`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_advanced.py#L156)
- signature: `class TestDetailedFormatting:`
- members:
  - `formatter_with_javadoc(self)` — [`L158`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_advanced.py#L158)
  - `test_get_class_fields_basic(self)` — [`L175`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_advanced.py#L175)
  - `test_get_class_fields_excludes_nested(self)` — [`L208`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_advanced.py#L208)
  - `test_get_class_methods_basic(self)` — [`L161`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_advanced.py#L161)
  - `test_get_class_methods_excludes_nested(self)` — [`L189`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_advanced.py#L189)
- uses (calls/refs, reference-scoped): [`LegacyTableFormatter`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter), [`_get_class_fields`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter._get_class_fields), [`_get_class_methods`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter._get_class_methods)

### `TestDocSummaryAndCSVText`
- def: [`tests/unit/formatters/test_legacy_table_formatter_advanced.py:603`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_advanced.py#L603)
- signature: `class TestDocSummaryAndCSVText:`
- members:
  - `test_clean_csv_text_dash(self)` — [`L622`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_advanced.py#L622)
  - `test_clean_csv_text_empty(self)` — [`L618`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_advanced.py#L618)
  - `test_clean_csv_text_with_newlines(self)` — [`L613`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_advanced.py#L613)
  - `test_clean_csv_text_with_quotes(self)` — [`L626`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_advanced.py#L626)
  - `test_extract_doc_empty(self)` — [`L609`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_advanced.py#L609)
  - `test_extract_doc_with_javadoc(self)` — [`L604`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_advanced.py#L604)
- uses (calls/refs, reference-scoped): [`LegacyTableFormatter`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter), [`_clean_csv_text`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter._clean_csv_text), [`_extract_doc_summary`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter._extract_doc_summary)

### `TestEdgeCases`
- def: [`tests/unit/formatters/test_legacy_table_formatter_advanced.py:41`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_advanced.py#L41)
- signature: `class TestEdgeCases:`
- members:
  - `test_empty_package_name(self)` — [`L60`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_advanced.py#L60)
  - `test_file_path_handling(self)` — [`L72`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_advanced.py#L72)
  - `test_file_path_with_various_extensions(self)` — [`L78`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_advanced.py#L78)
  - `test_method_with_no_parameters(self)` — [`L89`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_advanced.py#L89)
  - `test_missing_line_range(self)` — [`L140`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_advanced.py#L140)
  - `test_none_classes(self)` — [`L42`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_advanced.py#L42)
  - `test_none_fields(self)` — [`L54`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_advanced.py#L54)
  - `test_none_methods(self)` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_advanced.py#L48)
  - `test_parameter_as_other_type(self)` — [`L123`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_advanced.py#L123)
  - `test_parameter_as_plain_string(self)` — [`L106`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_advanced.py#L106)
  - `test_unknown_package(self)` — [`L66`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_advanced.py#L66)
- uses (calls/refs, reference-scoped): [`LegacyTableFormatter`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter), [`format_structure`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter.format_structure)

### `TestFullTableMultiClassParamTypes`
- def: [`tests/unit/formatters/test_legacy_table_formatter_advanced.py:257`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_advanced.py#L257)
- signature: `class TestFullTableMultiClassParamTypes:`
- members:
  - `test_fallback_param_in_multi_class(self)` — [`L293`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_advanced.py#L293)
  - `test_string_param_in_multi_class(self)` — [`L277`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_advanced.py#L277)
- protocol/private: `_multi_class_data`[`L258`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_advanced.py#L258)
- uses (calls/refs, reference-scoped): [`LegacyTableFormatter`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter), [`format_structure`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter.format_structure)

### `TestLanguageSpecificFormatting`
- def: [`tests/unit/formatters/test_legacy_table_formatter_advanced.py:228`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_advanced.py#L228)
- signature: `class TestLanguageSpecificFormatting:`
- members:
  - `test_java_language_formatting(self)` — [`L238`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_advanced.py#L238)
  - `test_javascript_language_formatting(self)` — [`L247`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_advanced.py#L247)
  - `test_python_language_formatting(self)` — [`L229`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_advanced.py#L229)
- uses (calls/refs, reference-scoped): [`LegacyTableFormatter`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter), [`format_structure`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter.format_structure)

### `TestPlatformNewlines`
- def: [`tests/unit/formatters/test_legacy_table_formatter_advanced.py:16`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_advanced.py#L16)
- signature: `class TestPlatformNewlines:`
- members:
  - `test_convert_to_platform_newlines(self)` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_advanced.py#L22)
  - `test_csv_skips_newline_conversion(self)` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_advanced.py#L32)
  - `test_get_platform_newline(self)` — [`L17`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_advanced.py#L17)
- uses (calls/refs, reference-scoped): [`LegacyTableFormatter`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter), [`format_structure`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter.format_structure), [`_convert_to_platform_newlines`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter._convert_to_platform_newlines), [`_get_platform_newline`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter._get_platform_newline)

### `TestShortenTypeBranches`
- def: [`tests/unit/formatters/test_legacy_table_formatter_advanced.py:568`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_advanced.py#L568)
- signature: `class TestShortenTypeBranches:`
- members:
  - `test_array_type(self)` — [`L587`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_advanced.py#L587)
  - `test_empty_array_type(self)` — [`L592`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_advanced.py#L592)
  - `test_list_type(self)` — [`L582`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_advanced.py#L582)
  - `test_map_type(self)` — [`L577`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_advanced.py#L577)
  - `test_non_string_type(self)` — [`L573`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_advanced.py#L573)
  - `test_none_type(self)` — [`L569`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_advanced.py#L569)
  - `test_unmapped_type(self)` — [`L597`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_formatter_advanced.py#L597)
- uses (calls/refs, reference-scoped): [`LegacyTableFormatter`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter), [`_shorten_type`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter._shorten_type)

