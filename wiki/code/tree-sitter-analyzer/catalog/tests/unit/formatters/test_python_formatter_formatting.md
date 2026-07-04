---
title: 'Module: tests/unit/formatters/test_python_formatter_formatting.py'
type: catalog
provenance: extracted
module: tests/unit/formatters/test_python_formatter_formatting.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.formatters.test_python_formatter_formatting`/TestPythonFormatter
symbols:
  TestPythonFormatterDocstringHandling.formatter: DocstringHandling#formatter().
  TestPythonFormatterDecoratorHandling.formatter: DecoratorHandling#formatter().
  TestPythonFormatterPerformanceEdgeCases.formatter: PerformanceEdgeCases#formatter().
  TestPythonFormatterFormatSummary.formatter: FormatSummary#formatter().
  TestPythonFormatterFormatAdvanced.formatter: FormatAdvanced#formatter().
  TestPythonFormatterFullTable.formatter: FullTable#formatter().
  TestPythonFormatterCompactTable.formatter: CompactTable#formatter().
  TestPythonFormatterCreateCompactSignature.formatter: CreateCompactSignature#formatter().
  TestPythonFormatterFormatTableMethod.formatter: FormatTableMethod#formatter().
  TestPythonFormatterFormatJsonError.formatter: FormatJsonError#formatter().
  TestPythonFormatterDocstringHandling: DocstringHandling#
  TestPythonFormatterDocstringHandling.test_extract_module_docstring_with_comments_before: DocstringHandling#test_extract_module_docstring_with_comments_before().
  TestPythonFormatterDocstringHandling.test_extract_module_docstring_with_imports_before: DocstringHandling#test_extract_module_docstring_with_imports_before().
  TestPythonFormatterDocstringHandling.test_extract_module_docstring_malformed: DocstringHandling#test_extract_module_docstring_malformed().
  TestPythonFormatterDocstringHandling.test_extract_module_docstring_mixed_quotes: DocstringHandling#test_extract_module_docstring_mixed_quotes().
  TestPythonFormatterDocstringHandling.test_extract_module_docstring_very_long: DocstringHandling#test_extract_module_docstring_very_long().
  TestPythonFormatterDecoratorHandling: DecoratorHandling#
  TestPythonFormatterDecoratorHandling.test_format_decorators_with_arguments: DecoratorHandling#test_format_decorators_with_arguments().
  TestPythonFormatterDecoratorHandling.test_format_decorators_with_complex_expressions: DecoratorHandling#test_format_decorators_with_complex_expressions().
  TestPythonFormatterDecoratorHandling.test_format_decorators_empty_and_none: DecoratorHandling#test_format_decorators_empty_and_none().
  TestPythonFormatterDecoratorHandling.test_format_decorators_with_duplicates: DecoratorHandling#test_format_decorators_with_duplicates().
  TestPythonFormatterDecoratorHandling.test_format_decorators_mixed_important_and_custom: DecoratorHandling#test_format_decorators_mixed_important_and_custom().
  TestPythonFormatterPerformanceEdgeCases: PerformanceEdgeCases#
  TestPythonFormatterPerformanceEdgeCases.test_format_with_recursive_data_structures: PerformanceEdgeCases#test_format_with_recursive_data_structures().
  TestPythonFormatterPerformanceEdgeCases.test_format_with_memory_intensive_data: PerformanceEdgeCases#test_format_with_memory_intensive_data().
  TestPythonFormatterPerformanceEdgeCases.test_format_with_many_small_objects: PerformanceEdgeCases#test_format_with_many_small_objects().
  TestPythonFormatterFormatSummary: FormatSummary#
  TestPythonFormatterFormatSummary.test_format_summary: FormatSummary#test_format_summary().
  TestPythonFormatterFormatAdvanced: FormatAdvanced#
  TestPythonFormatterFormatAdvanced.test_format_advanced_json: FormatAdvanced#test_format_advanced_json().
  TestPythonFormatterFormatAdvanced.test_format_advanced_csv: FormatAdvanced#test_format_advanced_csv().
  TestPythonFormatterFormatAdvanced.test_format_advanced_fallback_to_full: FormatAdvanced#test_format_advanced_fallback_to_full().
  TestPythonFormatterFullTable: FullTable#
  TestPythonFormatterFullTable.test_full_table_none_data: FullTable#test_full_table_none_data().
  TestPythonFormatterFullTable.test_full_table_invalid_type: FullTable#test_full_table_invalid_type().
  TestPythonFormatterFullTable.test_full_table_none_file_path: FullTable#test_full_table_none_file_path().
  TestPythonFormatterFullTable.test_full_table_with_package: FullTable#test_full_table_with_package().
  TestPythonFormatterFullTable.test_full_table_with_imports: FullTable#test_full_table_with_imports().
  TestPythonFormatterFullTable.test_full_table_single_class_with_methods: FullTable#test_full_table_single_class_with_methods().
  TestPythonFormatterFullTable.test_full_table_multiple_classes: FullTable#test_full_table_multiple_classes().
  TestPythonFormatterFullTable.test_full_table_per_class_sections: FullTable#test_full_table_per_class_sections().
  TestPythonFormatterCompactTable: CompactTable#
  TestPythonFormatterCompactTable.test_compact_table_basic: CompactTable#test_compact_table_basic().
  TestPythonFormatterCompactTable.test_compact_table_with_methods: CompactTable#test_compact_table_with_methods().
  TestPythonFormatterCompactTable.test_compact_table_with_classes: CompactTable#test_compact_table_with_classes().
  TestPythonFormatterCompactTable.test_compact_table_with_none_class: CompactTable#test_compact_table_with_none_class().
  TestPythonFormatterCreateCompactSignature: CreateCompactSignature#
  TestPythonFormatterCreateCompactSignature.test_compact_signature_none_method: CreateCompactSignature#test_compact_signature_none_method().
  TestPythonFormatterCreateCompactSignature.test_compact_signature_invalid_type: CreateCompactSignature#test_compact_signature_invalid_type().
  TestPythonFormatterCreateCompactSignature.test_compact_signature_string_params: CreateCompactSignature#test_compact_signature_string_params().
  TestPythonFormatterCreateCompactSignature.test_compact_signature_none_type: CreateCompactSignature#test_compact_signature_none_type().
  TestPythonFormatterFormatTableMethod: FormatTableMethod#
  TestPythonFormatterFormatTableMethod.test_format_table_restores_format_type: FormatTableMethod#test_format_table_restores_format_type().
  TestPythonFormatterFormatJsonError: FormatJsonError#
  TestPythonFormatterFormatJsonError.test_format_json_with_set: FormatJsonError#test_format_json_with_set().
---
# Module: [`tests/unit/formatters/test_python_formatter_formatting.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_formatting.py)

## Classes
### `TestPythonFormatterCompactTable`
- def: [`tests/unit/formatters/test_python_formatter_formatting.py:479`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_formatting.py#L479)
- doc: Test _format_compact_table
- signature: `class TestPythonFormatterCompactTable:`
- members:
  - `formatter(self)` — [`L483`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_formatting.py#L483)
  - `test_compact_table_basic(self, formatter)` — [`L486`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_formatting.py#L486)
  - `test_compact_table_with_classes(self, formatter)` — [`L521`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_formatting.py#L521)
  - `test_compact_table_with_methods(self, formatter)` — [`L498`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_formatting.py#L498)
  - `test_compact_table_with_none_class(self, formatter)` — [`L536`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_formatting.py#L536)
- uses (calls/refs, reference-scoped): [`PythonTableFormatter`](../../../tree_sitter_analyzer/formatters/python_formatter.md#PythonTableFormatter)

### `TestPythonFormatterCreateCompactSignature`
- def: [`tests/unit/formatters/test_python_formatter_formatting.py:556`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_formatting.py#L556)
- doc: Test _create_compact_signature edge cases
- signature: `class TestPythonFormatterCreateCompactSignature:`
- members:
  - `formatter(self)` — [`L560`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_formatting.py#L560)
  - `test_compact_signature_invalid_type(self, formatter)` — [`L567`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_formatting.py#L567)
  - `test_compact_signature_none_method(self, formatter)` — [`L563`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_formatting.py#L563)
  - `test_compact_signature_none_type(self, formatter)` — [`L580`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_formatting.py#L580)
  - `test_compact_signature_string_params(self, formatter)` — [`L571`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_formatting.py#L571)
- uses (calls/refs, reference-scoped): [`PythonTableFormatter`](../../../tree_sitter_analyzer/formatters/python_formatter.md#PythonTableFormatter)

### `TestPythonFormatterDecoratorHandling`
- def: [`tests/unit/formatters/test_python_formatter_formatting.py:80`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_formatting.py#L80)
- doc: Test Python formatter decorator handling edge cases.
- signature: `class TestPythonFormatterDecoratorHandling:`
- members:
  - `formatter(self)` — [`L84`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_formatting.py#L84) — Create a Python table formatter instance.
  - `test_format_decorators_empty_and_none(self, formatter)` — [`L110`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_formatting.py#L110) — Test formatting empty and None decorators.
  - `test_format_decorators_mixed_important_and_custom(self, formatter)` — [`L122`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_formatting.py#L122) — Test formatting mix of important and custom decorators.
  - `test_format_decorators_with_arguments(self, formatter)` — [`L88`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_formatting.py#L88) — Test formatting decorators with arguments.
  - `test_format_decorators_with_complex_expressions(self, formatter)` — [`L99`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_formatting.py#L99) — Test formatting decorators with complex expressions.
  - `test_format_decorators_with_duplicates(self, formatter)` — [`L115`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_formatting.py#L115) — Test formatting decorators with duplicates.
- uses (calls/refs, reference-scoped): [`PythonTableFormatter`](../../../tree_sitter_analyzer/formatters/python_formatter.md#PythonTableFormatter)

### `TestPythonFormatterDocstringHandling`
- def: [`tests/unit/formatters/test_python_formatter_formatting.py:9`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_formatting.py#L9)
- doc: Test Python formatter docstring handling edge cases.
- signature: `class TestPythonFormatterDocstringHandling:`
- members:
  - `formatter(self)` — [`L13`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_formatting.py#L13) — Create a Python table formatter instance.
  - `test_extract_module_docstring_malformed(self, formatter)` — [`L46`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_formatting.py#L46) — Test extracting malformed module docstring.
  - `test_extract_module_docstring_mixed_quotes(self, formatter)` — [`L58`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_formatting.py#L58) — Test extracting module docstring with mixed quote types.
  - `test_extract_module_docstring_very_long(self, formatter)` — [`L70`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_formatting.py#L70) — Test extracting very long module docstring.
  - `test_extract_module_docstring_with_comments_before(self, formatter)` — [`L17`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_formatting.py#L17) — Test extracting module docstring with comments before it.
  - `test_extract_module_docstring_with_imports_before(self, formatter)` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_formatting.py#L32) — Test extracting module docstring with imports before it.
- uses (calls/refs, reference-scoped): [`PythonTableFormatter`](../../../tree_sitter_analyzer/formatters/python_formatter.md#PythonTableFormatter)

### `TestPythonFormatterFormatAdvanced`
- def: [`tests/unit/formatters/test_python_formatter_formatting.py:251`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_formatting.py#L251)
- doc: Test format_advanced with different output formats
- signature: `class TestPythonFormatterFormatAdvanced:`
- members:
  - `formatter(self)` — [`L255`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_formatting.py#L255)
  - `test_format_advanced_csv(self, formatter)` — [`L263`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_formatting.py#L263)
  - `test_format_advanced_fallback_to_full(self, formatter)` — [`L268`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_formatting.py#L268)
  - `test_format_advanced_json(self, formatter)` — [`L258`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_formatting.py#L258)
- uses (calls/refs, reference-scoped): [`PythonTableFormatter`](../../../tree_sitter_analyzer/formatters/python_formatter.md#PythonTableFormatter)

### `TestPythonFormatterFormatJsonError`
- def: [`tests/unit/formatters/test_python_formatter_formatting.py:604`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_formatting.py#L604)
- doc: Test _format_json error path
- signature: `class TestPythonFormatterFormatJsonError:`
- members:
  - `formatter(self)` — [`L608`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_formatting.py#L608)
  - `test_format_json_with_set(self, formatter)` — [`L611`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_formatting.py#L611)
- uses (calls/refs, reference-scoped): [`PythonTableFormatter`](../../../tree_sitter_analyzer/formatters/python_formatter.md#PythonTableFormatter)

### `TestPythonFormatterFormatSummary`
- def: [`tests/unit/formatters/test_python_formatter_formatting.py:226`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_formatting.py#L226)
- doc: Test format_summary delegates to compact table
- signature: `class TestPythonFormatterFormatSummary:`
- members:
  - `formatter(self)` — [`L230`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_formatting.py#L230)
  - `test_format_summary(self, formatter)` — [`L233`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_formatting.py#L233)
- uses (calls/refs, reference-scoped): [`PythonTableFormatter`](../../../tree_sitter_analyzer/formatters/python_formatter.md#PythonTableFormatter)

### `TestPythonFormatterFormatTableMethod`
- def: [`tests/unit/formatters/test_python_formatter_formatting.py:590`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_formatting.py#L590)
- doc: Test format_table method
- signature: `class TestPythonFormatterFormatTableMethod:`
- members:
  - `formatter(self)` — [`L594`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_formatting.py#L594)
  - `test_format_table_restores_format_type(self, formatter)` — [`L597`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_formatting.py#L597)
- uses (calls/refs, reference-scoped): [`PythonTableFormatter`](../../../tree_sitter_analyzer/formatters/python_formatter.md#PythonTableFormatter)

### `TestPythonFormatterFullTable`
- def: [`tests/unit/formatters/test_python_formatter_formatting.py:281`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_formatting.py#L281)
- doc: Test _format_full_table variants
- signature: `class TestPythonFormatterFullTable:`
- members:
  - `formatter(self)` — [`L285`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_formatting.py#L285)
  - `test_full_table_invalid_type(self, formatter)` — [`L292`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_formatting.py#L292)
  - `test_full_table_multiple_classes(self, formatter)` — [`L401`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_formatting.py#L401)
  - `test_full_table_none_data(self, formatter)` — [`L288`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_formatting.py#L288)
  - `test_full_table_none_file_path(self, formatter)` — [`L296`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_formatting.py#L296)
  - `test_full_table_per_class_sections(self, formatter)` — [`L429`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_formatting.py#L429)
  - `test_full_table_single_class_with_methods(self, formatter)` — [`L351`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_formatting.py#L351)
  - `test_full_table_with_imports(self, formatter)` — [`L327`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_formatting.py#L327)
  - `test_full_table_with_package(self, formatter)` — [`L307`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_formatting.py#L307)
- uses (calls/refs, reference-scoped): [`PythonTableFormatter`](../../../tree_sitter_analyzer/formatters/python_formatter.md#PythonTableFormatter)

### `TestPythonFormatterPerformanceEdgeCases`
- def: [`tests/unit/formatters/test_python_formatter_formatting.py:137`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_formatting.py#L137)
- doc: Test Python formatter performance edge cases.
- signature: `class TestPythonFormatterPerformanceEdgeCases:`
- members:
  - `formatter(self)` — [`L141`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_formatting.py#L141) — Create a Python table formatter instance.
  - `test_format_with_many_small_objects(self, formatter)` — [`L193`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_formatting.py#L193) — Test formatting with many small objects.
  - `test_format_with_memory_intensive_data(self, formatter)` — [`L169`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_formatting.py#L169) — Test formatting with memory-intensive data.
  - `test_format_with_recursive_data_structures(self, formatter)` — [`L145`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_formatting.py#L145) — Test formatting with recursive data structures.
- uses (calls/refs, reference-scoped): [`PythonTableFormatter`](../../../tree_sitter_analyzer/formatters/python_formatter.md#PythonTableFormatter)

