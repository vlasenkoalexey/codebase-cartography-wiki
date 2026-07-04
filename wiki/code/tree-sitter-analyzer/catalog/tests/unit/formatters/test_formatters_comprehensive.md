---
title: 'Module: tests/unit/formatters/test_formatters_comprehensive.py'
type: catalog
provenance: extracted
module: tests/unit/formatters/test_formatters_comprehensive.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.formatters.test_formatters_comprehensive`/Test
symbols:
  TestFormatterRegistry.test_create_formatter_for_java: FormatterRegistry#test_create_formatter_for_java().
  TestFormatterRegistry.test_create_formatter_for_python: FormatterRegistry#test_create_formatter_for_python().
  TestFormatterRegistry.test_create_formatter_for_javascript: FormatterRegistry#test_create_formatter_for_javascript().
  TestFormatterRegistry.test_create_formatter_for_typescript: FormatterRegistry#test_create_formatter_for_typescript().
  TestFormatterRegistry.test_create_formatter_for_unsupported_language: FormatterRegistry#test_create_formatter_for_unsupported_language().
  TestBaseTableFormatter.test_platform_newline_detection: BaseTableFormatter#test_platform_newline_detection().
  TestBaseTableFormatter.test_newline_conversion: BaseTableFormatter#test_newline_conversion().
  TestBaseTableFormatter.test_format_structure_with_invalid_type: BaseTableFormatter#test_format_structure_with_invalid_type().
  TestFormatterRegistry.test_create_formatter_case_insensitive: FormatterRegistry#test_create_formatter_case_insensitive().
  TestFormatterRegistry.test_create_formatter_with_format_type: FormatterRegistry#test_create_formatter_with_format_type().
  TestFormatterRegistry.test_get_supported_languages: FormatterRegistry#test_get_supported_languages().
  TestFormatterRegistry.test_is_language_supported: FormatterRegistry#test_is_language_supported().
  TestJavaTableFormatter.test_java_formatter_creation: JavaTableFormatter#test_java_formatter_creation().
  TestJavaTableFormatter.test_java_formatter_with_different_format_types: JavaTableFormatter#test_java_formatter_with_different_format_types().
  TestJavaTableFormatter.test_format_java_structure_basic: JavaTableFormatter#test_format_java_structure_basic().
  TestJavaTableFormatter.test_format_java_structure_with_methods_and_fields: JavaTableFormatter#test_format_java_structure_with_methods_and_fields().
  TestJavaTableFormatter.test_format_java_structure_compact: JavaTableFormatter#test_format_java_structure_compact().
  TestJavaTableFormatter.test_format_java_structure_csv: JavaTableFormatter#test_format_java_structure_csv().
  TestPythonTableFormatter.test_python_formatter_creation: PythonTableFormatter#test_python_formatter_creation().
  TestPythonTableFormatter.test_python_formatter_with_different_format_types: PythonTableFormatter#test_python_formatter_with_different_format_types().
  TestPythonTableFormatter.test_format_python_structure_basic: PythonTableFormatter#test_format_python_structure_basic().
  TestPythonTableFormatter.test_format_python_structure_with_functions_and_classes: PythonTableFormatter#test_format_python_structure_with_functions_and_classes().
  TestPythonTableFormatter.test_format_python_structure_compact: PythonTableFormatter#test_format_python_structure_compact().
  TestPythonTableFormatter.test_format_python_structure_csv: PythonTableFormatter#test_format_python_structure_csv().
  TestFormatterErrorHandling.test_formatter_with_none_data: FormatterErrorHandling#test_formatter_with_none_data().
  TestFormatterErrorHandling.test_formatter_with_empty_data: FormatterErrorHandling#test_formatter_with_empty_data().
  TestFormatterErrorHandling.test_formatter_with_malformed_data: FormatterErrorHandling#test_formatter_with_malformed_data().
  TestFormatterIntegration.test_formatter_with_realistic_java_data: FormatterIntegration#test_formatter_with_realistic_java_data().
  TestFormatterIntegration.test_all_format_types_produce_output: FormatterIntegration#test_all_format_types_produce_output().
  TestBaseTableFormatter.test_platform_newline_detection.TestFormatter: BaseTableFormatter#test_platform_newline_detection().TestFormatter#
  TestBaseTableFormatter.test_newline_conversion.TestFormatter: BaseTableFormatter#test_newline_conversion().TestFormatter#
  TestBaseTableFormatter.test_format_structure_with_invalid_type.TestFormatter: BaseTableFormatter#test_format_structure_with_invalid_type().TestFormatter#
  TestBaseTableFormatter.test_base_formatter_is_abstract: BaseTableFormatter#test_base_formatter_is_abstract().
  TestBaseTableFormatter.test_base_formatter_interface: BaseTableFormatter#test_base_formatter_interface().
  TestBaseTableFormatter: BaseTableFormatter#
  TestBaseTableFormatter.test_platform_newline_detection.TestFormatter._format_full_table: BaseTableFormatter#test_platform_newline_detection().TestFormatter#_format_full_table().
  TestBaseTableFormatter.test_platform_newline_detection.TestFormatter._format_compact_table: BaseTableFormatter#test_platform_newline_detection().TestFormatter#_format_compact_table().
  TestBaseTableFormatter.test_platform_newline_detection.TestFormatter._format_csv: BaseTableFormatter#test_platform_newline_detection().TestFormatter#_format_csv().
  TestBaseTableFormatter.test_newline_conversion.TestFormatter._format_full_table: BaseTableFormatter#test_newline_conversion().TestFormatter#_format_full_table().
  TestBaseTableFormatter.test_newline_conversion.TestFormatter._format_compact_table: BaseTableFormatter#test_newline_conversion().TestFormatter#_format_compact_table().
  TestBaseTableFormatter.test_newline_conversion.TestFormatter._format_csv: BaseTableFormatter#test_newline_conversion().TestFormatter#_format_csv().
  TestBaseTableFormatter.test_format_structure_with_invalid_type.TestFormatter._format_full_table: BaseTableFormatter#test_format_structure_with_invalid_type().TestFormatter#_format_full_table().
  TestBaseTableFormatter.test_format_structure_with_invalid_type.TestFormatter._format_compact_table: BaseTableFormatter#test_format_structure_with_invalid_type().TestFormatter#_format_compact_table().
  TestBaseTableFormatter.test_format_structure_with_invalid_type.TestFormatter._format_csv: BaseTableFormatter#test_format_structure_with_invalid_type().TestFormatter#_format_csv().
  TestFormatterRegistry: FormatterRegistry#
  TestJavaTableFormatter: JavaTableFormatter#
  TestPythonTableFormatter: PythonTableFormatter#
  TestFormatterErrorHandling: FormatterErrorHandling#
  TestFormatterIntegration: FormatterIntegration#
---
# Module: [`tests/unit/formatters/test_formatters_comprehensive.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_formatters_comprehensive.py)

## Classes
### `TestBaseTableFormatter`
- def: [`tests/unit/formatters/test_formatters_comprehensive.py:24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_formatters_comprehensive.py#L24)
- doc: Test the base table formatter functionality.
- signature: `class TestBaseTableFormatter:`
- members:
  - `test_base_formatter_interface(self)` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_formatters_comprehensive.py#L32) — Test that BaseTableFormatter defines the expected interface.
  - `test_base_formatter_is_abstract(self)` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_formatters_comprehensive.py#L27) — Test that BaseTableFormatter cannot be instantiated directly.
  - `test_format_structure_with_invalid_type(self)` — [`L83`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_formatters_comprehensive.py#L83) — Test format_structure with invalid format type.
  - `test_newline_conversion(self)` — [`L64`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_formatters_comprehensive.py#L64) — Test newline conversion functionality.
  - `test_platform_newline_detection(self)` — [`L42`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_formatters_comprehensive.py#L42) — Test platform newline detection.
- uses (calls/refs, reference-scoped): [`format_structure`](../../../tree_sitter_analyzer/formatters/base_formatter.md#BaseTableFormatter.format_structure), [`BaseTableFormatter`](../../../tree_sitter_analyzer/formatters/base_formatter.md#BaseTableFormatter), [`_convert_to_platform_newlines`](../../../tree_sitter_analyzer/formatters/base_formatter.md#BaseTableFormatter._convert_to_platform_newlines), [`_get_platform_newline`](../../../tree_sitter_analyzer/formatters/base_formatter.md#BaseTableFormatter._get_platform_newline)  (3 test-only)

### `TestFormatter`  ·  implements/extends BaseTableFormatter
- def: [`tests/unit/formatters/test_formatters_comprehensive.py:86`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_formatters_comprehensive.py#L86)
- signature: `class TestFormatter(BaseTableFormatter):`
- protocol/private: `_format_compact_table`[`L50`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_formatters_comprehensive.py#L50), `_format_compact_table`[`L71`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_formatters_comprehensive.py#L71), `_format_compact_table`[`L90`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_formatters_comprehensive.py#L90), `_format_csv`[`L53`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_formatters_comprehensive.py#L53), `_format_csv`[`L74`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_formatters_comprehensive.py#L74), `_format_csv`[`L93`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_formatters_comprehensive.py#L93), `_format_full_table`[`L47`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_formatters_comprehensive.py#L47), `_format_full_table`[`L68`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_formatters_comprehensive.py#L68), `_format_full_table`[`L87`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_formatters_comprehensive.py#L87)
- uses (calls/refs, reference-scoped): [`BaseTableFormatter`](../../../tree_sitter_analyzer/formatters/base_formatter.md#BaseTableFormatter)
- used by: [`BaseTableFormatter`](../../../tree_sitter_analyzer/formatters/base_formatter.md#BaseTableFormatter), [`_format_csv`](../../../tree_sitter_analyzer/formatters/base_formatter.md#BaseTableFormatter._format_csv), [`_format_compact_table`](../../../tree_sitter_analyzer/formatters/base_formatter.md#BaseTableFormatter._format_compact_table), [`_format_full_table`](../../../tree_sitter_analyzer/formatters/base_formatter.md#BaseTableFormatter._format_full_table)  (1 test-only)

### `TestFormatterErrorHandling`
- def: [`tests/unit/formatters/test_formatters_comprehensive.py:397`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_formatters_comprehensive.py#L397)
- doc: Test error handling in formatters.
- signature: `class TestFormatterErrorHandling:`
- members:
  - `test_formatter_with_empty_data(self)` — [`L412`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_formatters_comprehensive.py#L412) — Test formatters with empty data structures.
  - `test_formatter_with_malformed_data(self)` — [`L427`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_formatters_comprehensive.py#L427) — Test formatters with malformed data structures.
  - `test_formatter_with_none_data(self)` — [`L400`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_formatters_comprehensive.py#L400) — Test formatters handle None data gracefully.
- uses (calls/refs, reference-scoped): [`format_structure`](../../../tree_sitter_analyzer/formatters/base_formatter.md#BaseTableFormatter.format_structure), [`JavaTableFormatter`](../../../tree_sitter_analyzer/formatters/java_formatter.md#JavaTableFormatter), [`PythonTableFormatter`](../../../tree_sitter_analyzer/formatters/python_formatter.md#PythonTableFormatter), [`format_structure`](../../../tree_sitter_analyzer/formatters/python_formatter.md#PythonTableFormatter.format_structure)

### `TestFormatterIntegration`
- def: [`tests/unit/formatters/test_formatters_comprehensive.py:449`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_formatters_comprehensive.py#L449)
- doc: Integration tests for formatter functionality.
- signature: `class TestFormatterIntegration:`
- members:
  - `test_all_format_types_produce_output(self)` — [`L487`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_formatters_comprehensive.py#L487) — Test that all format types produce valid output.
  - `test_formatter_with_realistic_java_data(self)` — [`L452`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_formatters_comprehensive.py#L452) — Test formatters with realistic Java analysis data.
- uses (calls/refs, reference-scoped): [`FormatterRegistry`](../../../tree_sitter_analyzer/formatters/formatter_registry.md#FormatterRegistry), [`get_formatter_for_language`](../../../tree_sitter_analyzer/formatters/formatter_registry.md#FormatterRegistry.get_formatter_for_language)

### `TestFormatterRegistry`
- def: [`tests/unit/formatters/test_formatters_comprehensive.py:101`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_formatters_comprehensive.py#L101)
- doc: Test the formatter registry functionality.
- signature: `class TestFormatterRegistry:`
- members:
  - `test_create_formatter_case_insensitive(self)` — [`L138`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_formatters_comprehensive.py#L138) — Test that formatter registry is case insensitive.
  - `test_create_formatter_for_java(self)` — [`L104`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_formatters_comprehensive.py#L104) — Test creating formatter for Java language.
  - `test_create_formatter_for_javascript(self)` — [`L116`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_formatters_comprehensive.py#L116) — Test creating formatter for JavaScript language.
  - `test_create_formatter_for_python(self)` — [`L110`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_formatters_comprehensive.py#L110) — Test creating formatter for Python language.
  - `test_create_formatter_for_typescript(self)` — [`L127`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_formatters_comprehensive.py#L127) — Test creating formatter for TypeScript language.
  - `test_create_formatter_for_unsupported_language(self)` — [`L149`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_formatters_comprehensive.py#L149) — Test creating formatter for unsupported language uses default.
  - `test_create_formatter_with_format_type(self)` — [`L144`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_formatters_comprehensive.py#L144) — Test creating formatter with specific format type.
  - `test_get_supported_languages(self)` — [`L155`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_formatters_comprehensive.py#L155) — Test getting list of supported languages.
  - `test_is_language_supported(self)` — [`L164`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_formatters_comprehensive.py#L164) — Test checking if language is supported.
- uses (calls/refs, reference-scoped): [`FormatterRegistry`](../../../tree_sitter_analyzer/formatters/formatter_registry.md#FormatterRegistry), [`JavaTableFormatter`](../../../tree_sitter_analyzer/formatters/java_formatter.md#JavaTableFormatter), [`PythonTableFormatter`](../../../tree_sitter_analyzer/formatters/python_formatter.md#PythonTableFormatter), [`JavaScriptTableFormatter`](../../../tree_sitter_analyzer/formatters/javascript_formatter.md#JavaScriptTableFormatter), [`get_formatter_for_language`](../../../tree_sitter_analyzer/formatters/formatter_registry.md#FormatterRegistry.get_formatter_for_language), [`TypeScriptTableFormatter`](../../../tree_sitter_analyzer/formatters/typescript_formatter.md#TypeScriptTableFormatter), [`format_type`](../../../tree_sitter_analyzer/formatters/java_formatter.md#JavaTableFormatter.format_type), [`format_type`](../../../tree_sitter_analyzer/formatters/javascript_formatter.md#JavaScriptTableFormatter.format_type), [`format_type`](../../../tree_sitter_analyzer/formatters/python_formatter.md#PythonTableFormatter.format_type), [`format_type`](../../../tree_sitter_analyzer/formatters/typescript_formatter.md#TypeScriptTableFormatter.format_type), [`DefaultTableFormatter`](../../../tree_sitter_analyzer/default_table_formatter.md#DefaultTableFormatter), [`format_type`](../../../tree_sitter_analyzer/default_table_formatter.md#DefaultTableFormatter.format_type), [`get_supported_languages`](../../../tree_sitter_analyzer/formatters/formatter_registry.md#FormatterRegistry.get_supported_languages)

### `TestJavaTableFormatter`
- def: [`tests/unit/formatters/test_formatters_comprehensive.py:173`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_formatters_comprehensive.py#L173)
- doc: Test Java-specific table formatting functionality.
- signature: `class TestJavaTableFormatter:`
- members:
  - `test_format_java_structure_basic(self)` — [`L189`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_formatters_comprehensive.py#L189) — Test formatting a basic Java structure.
  - `test_format_java_structure_compact(self)` — [`L251`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_formatters_comprehensive.py#L251) — Test formatting Java structure in compact format.
  - `test_format_java_structure_csv(self)` — [`L270`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_formatters_comprehensive.py#L270) — Test formatting Java structure in CSV format.
  - `test_format_java_structure_with_methods_and_fields(self)` — [`L215`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_formatters_comprehensive.py#L215) — Test formatting Java structure with methods and fields.
  - `test_java_formatter_creation(self)` — [`L176`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_formatters_comprehensive.py#L176) — Test that JavaTableFormatter can be created.
  - `test_java_formatter_with_different_format_types(self)` — [`L182`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_formatters_comprehensive.py#L182) — Test JavaTableFormatter with different format types.
- uses (calls/refs, reference-scoped): [`format_structure`](../../../tree_sitter_analyzer/formatters/base_formatter.md#BaseTableFormatter.format_structure), [`JavaTableFormatter`](../../../tree_sitter_analyzer/formatters/java_formatter.md#JavaTableFormatter), [`format_type`](../../../tree_sitter_analyzer/formatters/java_formatter.md#JavaTableFormatter.format_type)

### `TestPythonTableFormatter`
- def: [`tests/unit/formatters/test_formatters_comprehensive.py:289`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_formatters_comprehensive.py#L289)
- doc: Test Python-specific table formatting functionality.
- signature: `class TestPythonTableFormatter:`
- members:
  - `test_format_python_structure_basic(self)` — [`L305`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_formatters_comprehensive.py#L305) — Test formatting a basic Python structure.
  - `test_format_python_structure_compact(self)` — [`L370`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_formatters_comprehensive.py#L370) — Test formatting Python structure in compact format.
  - `test_format_python_structure_csv(self)` — [`L383`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_formatters_comprehensive.py#L383) — Test formatting Python structure in CSV format.
  - `test_format_python_structure_with_functions_and_classes(self)` — [`L330`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_formatters_comprehensive.py#L330) — Test formatting complex Python structure.
  - `test_python_formatter_creation(self)` — [`L292`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_formatters_comprehensive.py#L292) — Test that PythonTableFormatter can be created.
  - `test_python_formatter_with_different_format_types(self)` — [`L298`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_formatters_comprehensive.py#L298) — Test PythonTableFormatter with different format types.
- uses (calls/refs, reference-scoped): [`PythonTableFormatter`](../../../tree_sitter_analyzer/formatters/python_formatter.md#PythonTableFormatter), [`format_structure`](../../../tree_sitter_analyzer/formatters/python_formatter.md#PythonTableFormatter.format_structure), [`format_type`](../../../tree_sitter_analyzer/formatters/python_formatter.md#PythonTableFormatter.format_type)

