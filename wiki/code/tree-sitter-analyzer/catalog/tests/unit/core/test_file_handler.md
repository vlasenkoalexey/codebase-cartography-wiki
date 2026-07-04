---
title: 'Module: tests/unit/core/test_file_handler.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_file_handler.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_file_handler`/Test
symbols:
  TestIntegration.test_full_workflow: Integration#test_full_workflow().
  TestLoggingFunctions.test_log_error: LoggingFunctions#test_log_error().
  TestLoggingFunctions.test_log_error_with_args: LoggingFunctions#test_log_error_with_args().
  TestLoggingFunctions.test_log_info: LoggingFunctions#test_log_info().
  TestLoggingFunctions.test_log_info_with_args: LoggingFunctions#test_log_info_with_args().
  TestLoggingFunctions.test_log_warning: LoggingFunctions#test_log_warning().
  TestLoggingFunctions.test_log_warning_with_kwargs: LoggingFunctions#test_log_warning_with_kwargs().
  TestDetectLanguageFromExtension.test_detect_java: DetectLanguageFromExtension#test_detect_java().
  TestDetectLanguageFromExtension.test_detect_python: DetectLanguageFromExtension#test_detect_python().
  TestDetectLanguageFromExtension.test_detect_javascript: DetectLanguageFromExtension#test_detect_javascript().
  TestDetectLanguageFromExtension.test_detect_typescript: DetectLanguageFromExtension#test_detect_typescript().
  TestDetectLanguageFromExtension.test_detect_cpp: DetectLanguageFromExtension#test_detect_cpp().
  TestDetectLanguageFromExtension.test_detect_c: DetectLanguageFromExtension#test_detect_c().
  TestDetectLanguageFromExtension.test_detect_csharp: DetectLanguageFromExtension#test_detect_csharp().
  TestDetectLanguageFromExtension.test_detect_go: DetectLanguageFromExtension#test_detect_go().
  TestDetectLanguageFromExtension.test_detect_rust: DetectLanguageFromExtension#test_detect_rust().
  TestDetectLanguageFromExtension.test_detect_ruby: DetectLanguageFromExtension#test_detect_ruby().
  TestDetectLanguageFromExtension.test_detect_php: DetectLanguageFromExtension#test_detect_php().
  TestDetectLanguageFromExtension.test_detect_kotlin: DetectLanguageFromExtension#test_detect_kotlin().
  TestDetectLanguageFromExtension.test_detect_scala: DetectLanguageFromExtension#test_detect_scala().
  TestDetectLanguageFromExtension.test_detect_swift: DetectLanguageFromExtension#test_detect_swift().
  TestDetectLanguageFromExtension.test_detect_unknown_extension: DetectLanguageFromExtension#test_detect_unknown_extension().
  TestDetectLanguageFromExtension.test_detect_no_extension: DetectLanguageFromExtension#test_detect_no_extension().
  TestDetectLanguageFromExtension.test_detect_case_insensitive: DetectLanguageFromExtension#test_detect_case_insensitive().
  TestDetectLanguageFromExtension.test_detect_multiple_dots: DetectLanguageFromExtension#test_detect_multiple_dots().
  TestReadFileWithFallback.test_read_existing_file: ReadFileWithFallback#test_read_existing_file().
  TestReadFileWithFallback.test_read_nonexistent_file: ReadFileWithFallback#test_read_nonexistent_file().
  TestReadFileWithFallback.test_read_file_with_encoding_detection: ReadFileWithFallback#test_read_file_with_encoding_detection().
  TestReadFileWithFallback.test_read_file_exception_handling: ReadFileWithFallback#test_read_file_exception_handling().
  TestReadFileWithFallback.test_read_file_with_different_encoding: ReadFileWithFallback#test_read_file_with_different_encoding().
  TestReadFilePartial.test_read_partial_lines: ReadFilePartial#test_read_partial_lines().
  TestReadFilePartial.test_read_partial_single_line: ReadFilePartial#test_read_partial_single_line().
  TestReadFilePartial.test_read_partial_from_start: ReadFilePartial#test_read_partial_from_start().
  TestReadFilePartial.test_read_partial_to_end: ReadFilePartial#test_read_partial_to_end().
  TestReadFilePartial.test_read_partial_with_columns: ReadFilePartial#test_read_partial_with_columns().
  TestReadFilePartial.test_read_partial_with_start_column_only: ReadFilePartial#test_read_partial_with_start_column_only().
  TestReadFilePartial.test_read_partial_with_end_column_only: ReadFilePartial#test_read_partial_with_end_column_only().
  TestReadFilePartial.test_read_partial_single_line_with_columns: ReadFilePartial#test_read_partial_single_line_with_columns().
  TestReadFilePartial.test_read_partial_nonexistent_file: ReadFilePartial#test_read_partial_nonexistent_file().
  TestReadFilePartial.test_read_partial_invalid_start_line: ReadFilePartial#test_read_partial_invalid_start_line().
  TestReadFilePartial.test_read_partial_negative_start_line: ReadFilePartial#test_read_partial_negative_start_line().
  TestReadFilePartial.test_read_partial_invalid_range: ReadFilePartial#test_read_partial_invalid_range().
  TestReadFilePartial.test_read_partial_beyond_file_length: ReadFilePartial#test_read_partial_beyond_file_length().
  TestReadFilePartial.test_read_partial_empty_file: ReadFilePartial#test_read_partial_empty_file().
  TestReadFilePartial.test_read_partial_preserve_newlines: ReadFilePartial#test_read_partial_preserve_newlines().
  TestReadFilePartial.test_read_partial_column_beyond_line_length: ReadFilePartial#test_read_partial_column_beyond_line_length().
  TestReadFilePartial.test_read_partial_invalid_column_range: ReadFilePartial#test_read_partial_invalid_column_range().
  TestReadFilePartial.test_read_partial_exception_handling: ReadFilePartial#test_read_partial_exception_handling().
  TestReadFileLinesRange.test_read_lines_range: ReadFileLinesRange#test_read_lines_range().
  TestReadFileLinesRange.test_read_lines_range_to_end: ReadFileLinesRange#test_read_lines_range_to_end().
  TestReadFileLinesRange.test_read_lines_range_single_line: ReadFileLinesRange#test_read_lines_range_single_line().
  TestReadFileLinesRange.test_read_lines_range_nonexistent_file: ReadFileLinesRange#test_read_lines_range_nonexistent_file().
  TestReadFileLinesRange.test_read_lines_range_invalid_start: ReadFileLinesRange#test_read_lines_range_invalid_start().
  TestReadFileLinesRange.test_read_lines_range_invalid_range: ReadFileLinesRange#test_read_lines_range_invalid_range().
  TestReadFileLinesRange.test_read_lines_range_beyond_file: ReadFileLinesRange#test_read_lines_range_beyond_file().
  TestEdgeCases.test_read_partial_large_file: EdgeCases#test_read_partial_large_file().
  TestEdgeCases.test_read_partial_unicode_content: EdgeCases#test_read_partial_unicode_content().
  TestEdgeCases.test_detect_language_path_with_spaces: EdgeCases#test_detect_language_path_with_spaces().
  TestEdgeCases.test_detect_language_special_characters: EdgeCases#test_detect_language_special_characters().
  TestIntegration.test_multiple_partial_reads: Integration#test_multiple_partial_reads().
  TestIntegration.test_read_partial_with_columns_and_newlines: Integration#test_read_partial_with_columns_and_newlines().
  TestLoggingFunctions: LoggingFunctions#
  TestDetectLanguageFromExtension: DetectLanguageFromExtension#
  TestReadFileWithFallback: ReadFileWithFallback#
  TestReadFilePartial: ReadFilePartial#
  TestReadFileLinesRange: ReadFileLinesRange#
  TestEdgeCases: EdgeCases#
  TestIntegration: Integration#
---
# Module: [`tests/unit/core/test_file_handler.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_handler.py)

## Classes
### `TestDetectLanguageFromExtension`
- def: [`tests/unit/core/test_file_handler.py:63`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_handler.py#L63)
- doc: Test detect_language_from_extension function.
- signature: `class TestDetectLanguageFromExtension:`
- members:
  - `test_detect_c(self)` — [`L91`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_handler.py#L91) — Test C file detection.
  - `test_detect_case_insensitive(self)` — [`L138`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_handler.py#L138) — Test extension detection is case insensitive.
  - `test_detect_cpp(self)` — [`L86`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_handler.py#L86) — Test C++ file detection.
  - `test_detect_csharp(self)` — [`L96`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_handler.py#L96) — Test C# file detection.
  - `test_detect_go(self)` — [`L100`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_handler.py#L100) — Test Go file detection.
  - `test_detect_java(self)` — [`L66`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_handler.py#L66) — Test Java file detection.
  - `test_detect_javascript(self)` — [`L76`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_handler.py#L76) — Test JavaScript file detection.
  - `test_detect_kotlin(self)` — [`L116`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_handler.py#L116) — Test Kotlin file detection.
  - `test_detect_multiple_dots(self)` — [`L145`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_handler.py#L145) — Test file with multiple dots in name.
  - `test_detect_no_extension(self)` — [`L133`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_handler.py#L133) — Test file without extension.
  - `test_detect_php(self)` — [`L112`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_handler.py#L112) — Test PHP file detection.
  - `test_detect_python(self)` — [`L71`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_handler.py#L71) — Test Python file detection.
  - `test_detect_ruby(self)` — [`L108`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_handler.py#L108) — Test Ruby file detection.
  - `test_detect_rust(self)` — [`L104`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_handler.py#L104) — Test Rust file detection.
  - `test_detect_scala(self)` — [`L120`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_handler.py#L120) — Test Scala file detection.
  - `test_detect_swift(self)` — [`L124`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_handler.py#L124) — Test Swift file detection.
  - `test_detect_typescript(self)` — [`L81`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_handler.py#L81) — Test TypeScript file detection.
  - `test_detect_unknown_extension(self)` — [`L128`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_handler.py#L128) — Test unknown file extension.
- uses (calls/refs, reference-scoped): [`detect_language_from_extension`](../../../tree_sitter_analyzer/file_handler.md#detect_language_from_extension)

### `TestEdgeCases`
- def: [`tests/unit/core/test_file_handler.py:430`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_handler.py#L430)
- doc: Test edge cases and special scenarios.
- signature: `class TestEdgeCases:`
- members:
  - `test_detect_language_path_with_spaces(self)` — [`L452`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_handler.py#L452) — Test language detection with spaces in path.
  - `test_detect_language_special_characters(self)` — [`L456`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_handler.py#L456) — Test language detection with special characters.
  - `test_read_partial_large_file(self, tmp_path)` — [`L433`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_handler.py#L433) — Test reading from large file.
  - `test_read_partial_unicode_content(self, tmp_path)` — [`L443`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_handler.py#L443) — Test reading Unicode content.
- uses (calls/refs, reference-scoped): [`read_file_partial`](../../../tree_sitter_analyzer/file_handler.md#read_file_partial), [`detect_language_from_extension`](../../../tree_sitter_analyzer/file_handler.md#detect_language_from_extension)

### `TestIntegration`
- def: [`tests/unit/core/test_file_handler.py:462`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_handler.py#L462)
- doc: Integration tests for file_handler module.
- signature: `class TestIntegration:`
- members:
  - `test_full_workflow(self, tmp_path)` — [`L465`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_handler.py#L465) — Test complete workflow: detect language and read file.
  - `test_multiple_partial_reads(self, tmp_path)` — [`L485`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_handler.py#L485) — Test multiple partial reads from same file.
  - `test_read_partial_with_columns_and_newlines(self, tmp_path)` — [`L500`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_handler.py#L500) — Test column extraction with different newline types.
- uses (calls/refs, reference-scoped): [`read_file_partial`](../../../tree_sitter_analyzer/file_handler.md#read_file_partial), [`detect_language_from_extension`](../../../tree_sitter_analyzer/file_handler.md#detect_language_from_extension), [`read_file_with_fallback`](../../../tree_sitter_analyzer/file_handler.md#read_file_with_fallback)

### `TestLoggingFunctions`
- def: [`tests/unit/core/test_file_handler.py:21`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_handler.py#L21)
- doc: Test logging wrapper functions.
- signature: `class TestLoggingFunctions:`
- members:
  - `test_log_error(self, mock_logger)` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_handler.py#L25) — Test log_error function.
  - `test_log_error_with_args(self, mock_logger)` — [`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_handler.py#L31) — Test log_error with arguments.
  - `test_log_info(self, mock_logger)` — [`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_handler.py#L37) — Test log_info function.
  - `test_log_info_with_args(self, mock_logger)` — [`L43`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_handler.py#L43) — Test log_info with arguments.
  - `test_log_warning(self, mock_logger)` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_handler.py#L49) — Test log_warning function.
  - `test_log_warning_with_kwargs(self, mock_logger)` — [`L55`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_handler.py#L55) — Test log_warning with keyword arguments.
- uses (calls/refs, reference-scoped): [`log_error`](../../../tree_sitter_analyzer/file_handler.md#log_error), [`log_info`](../../../tree_sitter_analyzer/file_handler.md#log_info), [`log_warning`](../../../tree_sitter_analyzer/file_handler.md#log_warning)

### `TestReadFileLinesRange`
- def: [`tests/unit/core/test_file_handler.py:369`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_handler.py#L369)
- doc: Test read_file_lines_range function.
- signature: `class TestReadFileLinesRange:`
- members:
  - `test_read_lines_range(self, tmp_path)` — [`L372`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_handler.py#L372) — Test reading lines range.
  - `test_read_lines_range_beyond_file(self, tmp_path)` — [`L420`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_handler.py#L420) — Test reading beyond file length.
  - `test_read_lines_range_invalid_range(self, tmp_path)` — [`L412`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_handler.py#L412) — Test with invalid range.
  - `test_read_lines_range_invalid_start(self, tmp_path)` — [`L404`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_handler.py#L404) — Test with invalid start line.
  - `test_read_lines_range_nonexistent_file(self, tmp_path)` — [`L399`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_handler.py#L399) — Test reading from non-existent file.
  - `test_read_lines_range_single_line(self, tmp_path)` — [`L390`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_handler.py#L390) — Test reading single line.
  - `test_read_lines_range_to_end(self, tmp_path)` — [`L381`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_handler.py#L381) — Test reading lines range to end.
- uses (calls/refs, reference-scoped): [`read_file_lines_range`](../../../tree_sitter_analyzer/file_handler.md#read_file_lines_range)

### `TestReadFilePartial`
- def: [`tests/unit/core/test_file_handler.py:201`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_handler.py#L201)
- doc: Test read_file_partial function.
- signature: `class TestReadFilePartial:`
- members:
  - `test_read_partial_beyond_file_length(self, tmp_path)` — [`L309`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_handler.py#L309) — Test reading beyond file length.
  - `test_read_partial_column_beyond_line_length(self, tmp_path)` — [`L337`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_handler.py#L337) — Test column beyond line length.
  - `test_read_partial_empty_file(self, tmp_path)` — [`L318`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_handler.py#L318) — Test reading from empty file.
  - `test_read_partial_exception_handling(self, tmp_path)` — [`L355`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_handler.py#L355) — Test exception handling.
  - `test_read_partial_from_start(self, tmp_path)` — [`L222`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_handler.py#L222) — Test reading from start of file.
  - `test_read_partial_invalid_column_range(self, tmp_path)` — [`L346`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_handler.py#L346) — Test with invalid column range (end < start).
  - `test_read_partial_invalid_range(self, tmp_path)` — [`L301`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_handler.py#L301) — Test with invalid range (end < start).
  - `test_read_partial_invalid_start_line(self, tmp_path)` — [`L285`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_handler.py#L285) — Test with invalid start line (zero).
  - `test_read_partial_lines(self, tmp_path)` — [`L204`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_handler.py#L204) — Test reading partial lines from file.
  - `test_read_partial_negative_start_line(self, tmp_path)` — [`L293`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_handler.py#L293) — Test with negative start line.
  - `test_read_partial_nonexistent_file(self, tmp_path)` — [`L280`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_handler.py#L280) — Test reading from non-existent file.
  - `test_read_partial_preserve_newlines(self, tmp_path)` — [`L326`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_handler.py#L326) — Test that newlines are handled correctly.
  - `test_read_partial_single_line(self, tmp_path)` — [`L213`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_handler.py#L213) — Test reading a single line.
  - `test_read_partial_single_line_with_columns(self, tmp_path)` — [`L271`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_handler.py#L271) — Test reading single line with column range.
  - `test_read_partial_to_end(self, tmp_path)` — [`L231`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_handler.py#L231) — Test reading to end of file.
  - `test_read_partial_with_columns(self, tmp_path)` — [`L240`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_handler.py#L240) — Test reading with column range.
  - `test_read_partial_with_end_column_only(self, tmp_path)` — [`L261`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_handler.py#L261) — Test reading with end column only.
  - `test_read_partial_with_start_column_only(self, tmp_path)` — [`L251`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_handler.py#L251) — Test reading with start column only.
- uses (calls/refs, reference-scoped): [`read_file_partial`](../../../tree_sitter_analyzer/file_handler.md#read_file_partial)

### `TestReadFileWithFallback`
- def: [`tests/unit/core/test_file_handler.py:151`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_handler.py#L151)
- doc: Test read_file_with_fallback function.
- signature: `class TestReadFileWithFallback:`
- members:
  - `test_read_existing_file(self, tmp_path)` — [`L154`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_handler.py#L154) — Test reading an existing file.
  - `test_read_file_exception_handling(self, mock_read, tmp_path)` — [`L178`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_handler.py#L178) — Test exception handling when reading file.
  - `test_read_file_with_different_encoding(self, mock_read, tmp_path)` — [`L189`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_handler.py#L189) — Test reading file with different detected encoding.
  - `test_read_file_with_encoding_detection(self, tmp_path)` — [`L168`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_handler.py#L168) — Test reading file with encoding detection.
  - `test_read_nonexistent_file(self, tmp_path)` — [`L163`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_handler.py#L163) — Test reading a non-existent file.
- uses (calls/refs, reference-scoped): [`read_file_with_fallback`](../../../tree_sitter_analyzer/file_handler.md#read_file_with_fallback)

