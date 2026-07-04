---
title: 'Module: tests/unit/formatters/test_python_formatter_comprehensive_advanced.py'
type: catalog
provenance: extracted
module: tests/unit/formatters/test_python_formatter_comprehensive_advanced.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.formatters.test_python_formatter_comprehensive_advanced`/TestPythonTableFormatter
symbols:
  TestPythonTableFormatterSignatures.formatter: Signatures#formatter().
  TestPythonTableFormatterTypeShortening.formatter: TypeShortening#formatter().
  TestPythonTableFormatterUtilities.formatter: Utilities#formatter().
  TestPythonTableFormatterEdgeCases.formatter: EdgeCases#formatter().
  TestPythonTableFormatterSignatures: Signatures#
  TestPythonTableFormatterSignatures.test_create_compact_signature_basic: Signatures#test_create_compact_signature_basic().
  TestPythonTableFormatterSignatures.test_create_compact_signature_complex_types: Signatures#test_create_compact_signature_complex_types().
  TestPythonTableFormatterSignatures.test_create_compact_signature_no_types: Signatures#test_create_compact_signature_no_types().
  TestPythonTableFormatterSignatures.test_format_python_signature_with_types: Signatures#test_format_python_signature_with_types().
  TestPythonTableFormatterSignatures.test_format_python_signature_without_types: Signatures#test_format_python_signature_without_types().
  TestPythonTableFormatterSignatures.test_format_python_signature_mixed_types: Signatures#test_format_python_signature_mixed_types().
  TestPythonTableFormatterTypeShortening: TypeShortening#
  TestPythonTableFormatterTypeShortening.test_shorten_basic_types: TypeShortening#test_shorten_basic_types().
  TestPythonTableFormatterTypeShortening.test_shorten_collection_types: TypeShortening#test_shorten_collection_types().
  TestPythonTableFormatterTypeShortening.test_shorten_generic_types: TypeShortening#test_shorten_generic_types().
  TestPythonTableFormatterTypeShortening.test_shorten_custom_types: TypeShortening#test_shorten_custom_types().
  TestPythonTableFormatterTypeShortening.test_shorten_none_type: TypeShortening#test_shorten_none_type().
  TestPythonTableFormatterTypeShortening.test_shorten_non_string_type: TypeShortening#test_shorten_non_string_type().
  TestPythonTableFormatterUtilities: Utilities#
  TestPythonTableFormatterUtilities.test_extract_module_docstring_single_line: Utilities#test_extract_module_docstring_single_line().
  TestPythonTableFormatterUtilities.test_extract_module_docstring_multi_line: Utilities#test_extract_module_docstring_multi_line().
  TestPythonTableFormatterUtilities.test_extract_module_docstring_single_quotes: Utilities#test_extract_module_docstring_single_quotes().
  TestPythonTableFormatterUtilities.test_extract_module_docstring_none: Utilities#test_extract_module_docstring_none().
  TestPythonTableFormatterUtilities.test_extract_module_docstring_no_source: Utilities#test_extract_module_docstring_no_source().
  TestPythonTableFormatterUtilities.test_get_python_visibility_symbol: Utilities#test_get_python_visibility_symbol().
  TestPythonTableFormatterUtilities.test_format_decorators_empty: Utilities#test_format_decorators_empty().
  TestPythonTableFormatterUtilities.test_format_decorators_important: Utilities#test_format_decorators_important().
  TestPythonTableFormatterUtilities.test_format_decorators_single: Utilities#test_format_decorators_single().
  TestPythonTableFormatterUtilities.test_format_decorators_multiple_non_important: Utilities#test_format_decorators_multiple_non_important().
  TestPythonTableFormatterEdgeCases: EdgeCases#
  TestPythonTableFormatterEdgeCases.test_format_with_missing_data_fields: EdgeCases#test_format_with_missing_data_fields().
  TestPythonTableFormatterEdgeCases.test_format_with_malformed_line_ranges: EdgeCases#test_format_with_malformed_line_ranges().
  TestPythonTableFormatterEdgeCases.test_format_with_unicode_content: EdgeCases#test_format_with_unicode_content().
  TestPythonTableFormatterEdgeCases.test_format_with_very_long_names: EdgeCases#test_format_with_very_long_names().
  TestPythonTableFormatterEdgeCases.test_format_with_empty_collections: EdgeCases#test_format_with_empty_collections().
  TestPythonTableFormatterEdgeCases.test_format_with_none_values: EdgeCases#test_format_with_none_values().
  TestPythonTableFormatterEdgeCases.test_format_performance_with_large_data: EdgeCases#test_format_performance_with_large_data().
---
# Module: [`tests/unit/formatters/test_python_formatter_comprehensive_advanced.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_comprehensive_advanced.py)

## Classes
### `TestPythonTableFormatterEdgeCases`
- def: [`tests/unit/formatters/test_python_formatter_comprehensive_advanced.py:246`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_comprehensive_advanced.py#L246)
- doc: Test Python table formatter edge cases.
- signature: `class TestPythonTableFormatterEdgeCases:`
- members:
  - `formatter(self)` — [`L250`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_comprehensive_advanced.py#L250) — Create a Python table formatter instance.
  - `test_format_performance_with_large_data(self, formatter)` — [`L398`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_comprehensive_advanced.py#L398) — Test formatting performance with large datasets.
  - `test_format_with_empty_collections(self, formatter)` — [`L356`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_comprehensive_advanced.py#L356) — Test formatting with empty collections.
  - `test_format_with_malformed_line_ranges(self, formatter)` — [`L265`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_comprehensive_advanced.py#L265) — Test formatting with malformed line ranges.
  - `test_format_with_missing_data_fields(self, formatter)` — [`L254`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_comprehensive_advanced.py#L254) — Test formatting with missing data fields.
  - `test_format_with_none_values(self, formatter)` — [`L372`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_comprehensive_advanced.py#L372) — Test formatting with None values in data.
  - `test_format_with_unicode_content(self, formatter)` — [`L287`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_comprehensive_advanced.py#L287) — Test formatting with Unicode content.
  - `test_format_with_very_long_names(self, formatter)` — [`L319`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_comprehensive_advanced.py#L319) — Test formatting with very long names.
- uses (calls/refs, reference-scoped): [`PythonTableFormatter`](../../../tree_sitter_analyzer/formatters/python_formatter.md#PythonTableFormatter)

### `TestPythonTableFormatterSignatures`
- def: [`tests/unit/formatters/test_python_formatter_comprehensive_advanced.py:11`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_comprehensive_advanced.py#L11)
- doc: Test Python table formatter signature creation.
- signature: `class TestPythonTableFormatterSignatures:`
- members:
  - `formatter(self)` — [`L15`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_comprehensive_advanced.py#L15) — Create a Python table formatter instance.
  - `test_create_compact_signature_basic(self, formatter)` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_comprehensive_advanced.py#L19) — Test basic compact signature creation.
  - `test_create_compact_signature_complex_types(self, formatter)` — [`L34`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_comprehensive_advanced.py#L34) — Test compact signature with complex types.
  - `test_create_compact_signature_no_types(self, formatter)` — [`L51`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_comprehensive_advanced.py#L51) — Test compact signature with no type information.
  - `test_format_python_signature_mixed_types(self, formatter)` — [`L88`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_comprehensive_advanced.py#L88) — Test Python signature formatting with mixed type information.
  - `test_format_python_signature_with_types(self, formatter)` — [`L62`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_comprehensive_advanced.py#L62) — Test Python signature formatting with types.
  - `test_format_python_signature_without_types(self, formatter)` — [`L77`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_comprehensive_advanced.py#L77) — Test Python signature formatting without types.
- uses (calls/refs, reference-scoped): [`PythonTableFormatter`](../../../tree_sitter_analyzer/formatters/python_formatter.md#PythonTableFormatter)

### `TestPythonTableFormatterTypeShortening`
- def: [`tests/unit/formatters/test_python_formatter_comprehensive_advanced.py:106`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_comprehensive_advanced.py#L106)
- doc: Test Python table formatter type shortening functionality.
- signature: `class TestPythonTableFormatterTypeShortening:`
- members:
  - `formatter(self)` — [`L110`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_comprehensive_advanced.py#L110) — Create a Python table formatter instance.
  - `test_shorten_basic_types(self, formatter)` — [`L114`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_comprehensive_advanced.py#L114) — Test shortening of basic Python types.
  - `test_shorten_collection_types(self, formatter)` — [`L123`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_comprehensive_advanced.py#L123) — Test shortening of collection types.
  - `test_shorten_custom_types(self, formatter)` — [`L137`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_comprehensive_advanced.py#L137) — Test shortening of custom types.
  - `test_shorten_generic_types(self, formatter)` — [`L130`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_comprehensive_advanced.py#L130) — Test shortening of generic types.
  - `test_shorten_non_string_type(self, formatter)` — [`L147`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_comprehensive_advanced.py#L147) — Test shortening of non-string types.
  - `test_shorten_none_type(self, formatter)` — [`L143`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_comprehensive_advanced.py#L143) — Test shortening of None type.
- uses (calls/refs, reference-scoped): [`PythonTableFormatter`](../../../tree_sitter_analyzer/formatters/python_formatter.md#PythonTableFormatter)

### `TestPythonTableFormatterUtilities`
- def: [`tests/unit/formatters/test_python_formatter_comprehensive_advanced.py:153`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_comprehensive_advanced.py#L153)
- doc: Test Python table formatter utility functions.
- signature: `class TestPythonTableFormatterUtilities:`
- members:
  - `formatter(self)` — [`L157`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_comprehensive_advanced.py#L157) — Create a Python table formatter instance.
  - `test_extract_module_docstring_multi_line(self, formatter)` — [`L171`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_comprehensive_advanced.py#L171) — Test extracting multi-line module docstring.
  - `test_extract_module_docstring_no_source(self, formatter)` — [`L201`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_comprehensive_advanced.py#L201) — Test extracting module docstring with no source code.
  - `test_extract_module_docstring_none(self, formatter)` — [`L193`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_comprehensive_advanced.py#L193) — Test extracting module docstring when none exists.
  - `test_extract_module_docstring_single_line(self, formatter)` — [`L161`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_comprehensive_advanced.py#L161) — Test extracting single-line module docstring.
  - `test_extract_module_docstring_single_quotes(self, formatter)` — [`L183`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_comprehensive_advanced.py#L183) — Test extracting module docstring with single quotes.
  - `test_format_decorators_empty(self, formatter)` — [`L217`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_comprehensive_advanced.py#L217) — Test formatting empty decorators list.
  - `test_format_decorators_important(self, formatter)` — [`L223`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_comprehensive_advanced.py#L223) — Test formatting important decorators.
  - `test_format_decorators_multiple_non_important(self, formatter)` — [`L238`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_comprehensive_advanced.py#L238) — Test formatting multiple non-important decorators.
  - `test_format_decorators_single(self, formatter)` — [`L231`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_comprehensive_advanced.py#L231) — Test formatting single decorator.
  - `test_get_python_visibility_symbol(self, formatter)` — [`L209`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_comprehensive_advanced.py#L209) — Test Python visibility symbol mapping.
- uses (calls/refs, reference-scoped): [`PythonTableFormatter`](../../../tree_sitter_analyzer/formatters/python_formatter.md#PythonTableFormatter)

