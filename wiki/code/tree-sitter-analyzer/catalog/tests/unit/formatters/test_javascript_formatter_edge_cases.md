---
title: 'Module: tests/unit/formatters/test_javascript_formatter_edge_cases.py'
type: catalog
provenance: extracted
module: tests/unit/formatters/test_javascript_formatter_edge_cases.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.formatters.test_javascript_formatter_edge_cases`/TestJavaScriptTableFormatterEdgeCases#
symbols:
  TestJavaScriptTableFormatterEdgeCases.formatter: formatter().
  TestJavaScriptTableFormatterEdgeCases.test_format_with_json_serialization_error: test_format_with_json_serialization_error().
  TestJavaScriptTableFormatterEdgeCases.test_format_with_json_serialization_error.NonSerializable: test_format_with_json_serialization_error().NonSerializable#
  TestJavaScriptTableFormatterEdgeCases: ''
  TestJavaScriptTableFormatterEdgeCases.test_format_with_none_data: test_format_with_none_data().
  TestJavaScriptTableFormatterEdgeCases.test_format_with_invalid_format_type: test_format_with_invalid_format_type().
  TestJavaScriptTableFormatterEdgeCases.test_format_with_missing_file_path: test_format_with_missing_file_path().
  TestJavaScriptTableFormatterEdgeCases.test_format_with_circular_references: test_format_with_circular_references().
  TestJavaScriptTableFormatterEdgeCases.test_format_with_extremely_long_names: test_format_with_extremely_long_names().
  TestJavaScriptTableFormatterEdgeCases.test_format_with_special_unicode_characters: test_format_with_special_unicode_characters().
  TestJavaScriptTableFormatterEdgeCases.test_format_with_control_characters: test_format_with_control_characters().
  TestJavaScriptTableFormatterEdgeCases.test_format_with_nested_data_structures: test_format_with_nested_data_structures().
  TestJavaScriptTableFormatterEdgeCases.test_format_with_binary_data: test_format_with_binary_data().
  TestJavaScriptTableFormatterEdgeCases.test_format_with_extremely_large_numbers: test_format_with_extremely_large_numbers().
  TestJavaScriptTableFormatterEdgeCases.test_format_with_malformed_json_strings: test_format_with_malformed_json_strings().
  TestJavaScriptTableFormatterEdgeCases.test_format_with_recursive_data_structures: test_format_with_recursive_data_structures().
  TestJavaScriptTableFormatterEdgeCases.test_format_with_memory_intensive_data: test_format_with_memory_intensive_data().
  TestJavaScriptTableFormatterEdgeCases.test_format_with_invalid_utf8_sequences: test_format_with_invalid_utf8_sequences().
  TestJavaScriptTableFormatterEdgeCases.test_format_with_zero_width_characters: test_format_with_zero_width_characters().
  TestJavaScriptTableFormatterEdgeCases.test_format_with_rtl_characters: test_format_with_rtl_characters().
  TestJavaScriptTableFormatterEdgeCases.test_format_with_mathematical_symbols: test_format_with_mathematical_symbols().
  TestJavaScriptTableFormatterEdgeCases.test_format_with_mixed_line_endings: test_format_with_mixed_line_endings().
  TestJavaScriptTableFormatterEdgeCases.test_format_with_tab_characters: test_format_with_tab_characters().
  TestJavaScriptTableFormatterEdgeCases.test_format_with_surrogate_pairs: test_format_with_surrogate_pairs().
  TestJavaScriptTableFormatterEdgeCases.test_format_with_combining_characters: test_format_with_combining_characters().
  TestJavaScriptTableFormatterEdgeCases.test_format_with_normalization_forms: test_format_with_normalization_forms().
  TestJavaScriptTableFormatterEdgeCases.test_format_with_exception_in_helper_methods: test_format_with_exception_in_helper_methods().
  TestJavaScriptTableFormatterEdgeCases.test_format_with_json_serialization_error.NonSerializable.__str__: test_format_with_json_serialization_error().NonSerializable#__str__().
  TestJavaScriptTableFormatterEdgeCases.test_format_with_csv_special_characters: test_format_with_csv_special_characters().
  TestJavaScriptTableFormatterEdgeCases.test_format_with_markdown_special_characters: test_format_with_markdown_special_characters().
  TestJavaScriptTableFormatterEdgeCases.test_format_with_html_entities: test_format_with_html_entities().
  TestJavaScriptTableFormatterEdgeCases.test_format_with_sql_injection_patterns: test_format_with_sql_injection_patterns().
  TestJavaScriptTableFormatterEdgeCases.test_format_with_script_injection_patterns: test_format_with_script_injection_patterns().
  TestJavaScriptTableFormatterEdgeCases.test_format_with_path_traversal_patterns: test_format_with_path_traversal_patterns().
  TestJavaScriptTableFormatterEdgeCases.test_format_with_regex_patterns: test_format_with_regex_patterns().
  TestJavaScriptTableFormatterEdgeCases.test_format_with_url_patterns: test_format_with_url_patterns().
  TestJavaScriptTableFormatterEdgeCases.test_format_with_base64_data: test_format_with_base64_data().
  TestJavaScriptTableFormatterEdgeCases.test_format_with_jwt_tokens: test_format_with_jwt_tokens().
  TestJavaScriptTableFormatterEdgeCases.test_format_with_hash_values: test_format_with_hash_values().
---
# Module: [`tests/unit/formatters/test_javascript_formatter_edge_cases.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_javascript_formatter_edge_cases.py)

## Classes
### `NonSerializable`
- def: [`tests/unit/formatters/test_javascript_formatter_edge_cases.py:404`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_javascript_formatter_edge_cases.py#L404)
- signature: `class NonSerializable:`
- protocol/private: `__str__`[`L405`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_javascript_formatter_edge_cases.py#L405)
- used by: (1 test-only callers)

### `TestJavaScriptTableFormatterEdgeCases`
- def: [`tests/unit/formatters/test_javascript_formatter_edge_cases.py:15`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_javascript_formatter_edge_cases.py#L15)
- doc: Edge case tests for JavaScript formatter
- signature: `class TestJavaScriptTableFormatterEdgeCases:`
- members:
  - `formatter(self)` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_javascript_formatter_edge_cases.py#L19) — Create a JavaScript formatter instance
  - `test_format_with_base64_data(self, formatter)` — [`L551`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_javascript_formatter_edge_cases.py#L551) — Test formatting with Base64 encoded data
  - `test_format_with_binary_data(self, formatter)` — [`L148`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_javascript_formatter_edge_cases.py#L148) — Test formatting with binary data in strings
  - `test_format_with_circular_references(self, formatter)` — [`L52`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_javascript_formatter_edge_cases.py#L52) — Test formatting with circular references in data
  - `test_format_with_combining_characters(self, formatter)` — [`L351`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_javascript_formatter_edge_cases.py#L351) — Test formatting with Unicode combining characters
  - `test_format_with_control_characters(self, formatter)` — [`L96`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_javascript_formatter_edge_cases.py#L96) — Test formatting with control characters
  - `test_format_with_csv_special_characters(self, formatter)` — [`L418`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_javascript_formatter_edge_cases.py#L418) — Test CSV formatting with special CSV characters
  - `test_format_with_exception_in_helper_methods(self, formatter)` — [`L384`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_javascript_formatter_edge_cases.py#L384) — Test formatting when helper methods raise exceptions
  - `test_format_with_extremely_large_numbers(self, formatter)` — [`L166`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_javascript_formatter_edge_cases.py#L166) — Test formatting with extremely large numbers
  - `test_format_with_extremely_long_names(self, formatter)` — [`L62`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_javascript_formatter_edge_cases.py#L62) — Test formatting with extremely long names
  - `test_format_with_hash_values(self, formatter)` — [`L595`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_javascript_formatter_edge_cases.py#L595) — Test formatting with various hash values
  - `test_format_with_html_entities(self, formatter)` — [`L444`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_javascript_formatter_edge_cases.py#L444) — Test formatting with HTML entities
  - `test_format_with_invalid_format_type(self, formatter)` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_javascript_formatter_edge_cases.py#L29) — Test formatting with invalid format type
  - `test_format_with_invalid_utf8_sequences(self, formatter)` — [`L220`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_javascript_formatter_edge_cases.py#L220) — Test formatting with invalid UTF-8 sequences
  - `test_format_with_json_serialization_error(self, formatter)` — [`L400`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_javascript_formatter_edge_cases.py#L400) — Test formatting when JSON serialization fails
  - `test_format_with_jwt_tokens(self, formatter)` — [`L573`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_javascript_formatter_edge_cases.py#L573) — Test formatting with JWT-like tokens
  - `test_format_with_malformed_json_strings(self, formatter)` — [`L178`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_javascript_formatter_edge_cases.py#L178) — Test formatting with malformed JSON strings
  - `test_format_with_markdown_special_characters(self, formatter)` — [`L432`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_javascript_formatter_edge_cases.py#L432) — Test formatting with Markdown special characters
  - `test_format_with_mathematical_symbols(self, formatter)` — [`L282`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_javascript_formatter_edge_cases.py#L282) — Test formatting with mathematical symbols
  - `test_format_with_memory_intensive_data(self, formatter)` — [`L206`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_javascript_formatter_edge_cases.py#L206) — Test formatting with memory-intensive data
  - `test_format_with_missing_file_path(self, formatter)` — [`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_javascript_formatter_edge_cases.py#L37) — Test formatting with missing file_path
  - `test_format_with_mixed_line_endings(self, formatter)` — [`L304`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_javascript_formatter_edge_cases.py#L304) — Test formatting with mixed line endings
  - `test_format_with_nested_data_structures(self, formatter)` — [`L113`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_javascript_formatter_edge_cases.py#L113) — Test formatting with deeply nested data structures
  - `test_format_with_none_data(self, formatter)` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_javascript_formatter_edge_cases.py#L23) — Test formatting with None data
  - `test_format_with_normalization_forms(self, formatter)` — [`L364`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_javascript_formatter_edge_cases.py#L364) — Test formatting with different Unicode normalization forms
  - `test_format_with_path_traversal_patterns(self, formatter)` — [`L492`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_javascript_formatter_edge_cases.py#L492) — Test formatting with path traversal patterns
  - `test_format_with_recursive_data_structures(self, formatter)` — [`L190`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_javascript_formatter_edge_cases.py#L190) — Test formatting with recursive data structures
  - `test_format_with_regex_patterns(self, formatter)` — [`L507`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_javascript_formatter_edge_cases.py#L507) — Test formatting with complex regex patterns
  - `test_format_with_rtl_characters(self, formatter)` — [`L252`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_javascript_formatter_edge_cases.py#L252) — Test formatting with right-to-left characters
  - `test_format_with_script_injection_patterns(self, formatter)` — [`L478`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_javascript_formatter_edge_cases.py#L478) — Test formatting with script injection-like patterns
  - `test_format_with_special_unicode_characters(self, formatter)` — [`L79`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_javascript_formatter_edge_cases.py#L79) — Test formatting with special Unicode characters
  - `test_format_with_sql_injection_patterns(self, formatter)` — [`L456`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_javascript_formatter_edge_cases.py#L456) — Test formatting with SQL injection-like patterns
  - `test_format_with_surrogate_pairs(self, formatter)` — [`L328`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_javascript_formatter_edge_cases.py#L328) — Test formatting with Unicode surrogate pairs
  - `test_format_with_tab_characters(self, formatter)` — [`L316`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_javascript_formatter_edge_cases.py#L316) — Test formatting with various tab characters
  - `test_format_with_url_patterns(self, formatter)` — [`L519`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_javascript_formatter_edge_cases.py#L519) — Test formatting with various URL patterns
  - `test_format_with_zero_width_characters(self, formatter)` — [`L238`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_javascript_formatter_edge_cases.py#L238) — Test formatting with zero-width characters
- uses (calls/refs, reference-scoped): [`JavaScriptTableFormatter`](../../../tree_sitter_analyzer/formatters/javascript_formatter.md#JavaScriptTableFormatter)  (1 test-only)

