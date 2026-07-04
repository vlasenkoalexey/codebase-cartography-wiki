---
title: 'Module: tests/unit/core/test_parser_error_recovery_properties.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_parser_error_recovery_properties.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_parser_error_recovery_properties`/
symbols:
  TestParserErrorRecoveryProperties.test_property_6_python_parser_does_not_crash_on_syntax_errors: TestParserErrorRecoveryProperties#test_property_6_python_parser_does_not_crash_on_syntax_errors().
  TestParserErrorRecoveryProperties.test_property_6_parser_returns_partial_results_for_mixed_code: TestParserErrorRecoveryProperties#test_property_6_parser_returns_partial_results_for_mixed_code().
  TestParserErrorDetectionProperties.test_property_6_parser_can_detect_errors_in_tree: TestParserErrorDetectionProperties#test_property_6_parser_can_detect_errors_in_tree().
  TestParserUnsupportedLanguageProperties.test_property_6_parser_handles_unsupported_language_gracefully: TestParserUnsupportedLanguageProperties#test_property_6_parser_handles_unsupported_language_gracefully().
  TestParserErrorRecoveryProperties.test_property_6_java_parser_does_not_crash_on_syntax_errors: TestParserErrorRecoveryProperties#test_property_6_java_parser_does_not_crash_on_syntax_errors().
  TestParserErrorRecoveryProperties.test_property_6_javascript_parser_does_not_crash_on_syntax_errors: TestParserErrorRecoveryProperties#test_property_6_javascript_parser_does_not_crash_on_syntax_errors().
  TestParserErrorRecoveryProperties.test_property_6_parser_handles_garbage_input_gracefully: TestParserErrorRecoveryProperties#test_property_6_parser_handles_garbage_input_gracefully().
  TestEngineErrorRecoveryProperties.test_property_6_engine_returns_result_for_invalid_python: TestEngineErrorRecoveryProperties#test_property_6_engine_returns_result_for_invalid_python().
  TestEngineErrorRecoveryProperties.test_property_6_engine_returns_result_for_invalid_javascript: TestEngineErrorRecoveryProperties#test_property_6_engine_returns_result_for_invalid_javascript().
  TestParserErrorDetectionProperties.test_property_6_parser_validates_ast_correctly: TestParserErrorDetectionProperties#test_property_6_parser_validates_ast_correctly().
  TestEngineErrorRecoveryProperties.test_property_6_engine_returns_result_for_invalid_java: TestEngineErrorRecoveryProperties#test_property_6_engine_returns_result_for_invalid_java().
  TestParserEmptyInputProperties.test_property_6_parser_handles_empty_string: TestParserEmptyInputProperties#test_property_6_parser_handles_empty_string().
  TestParserEmptyInputProperties.test_property_6_parser_handles_whitespace_only: TestParserEmptyInputProperties#test_property_6_parser_handles_whitespace_only().
  code_with_partial_errors: code_with_partial_errors().
  python_code_with_syntax_error: python_code_with_syntax_error().
  java_code_with_syntax_error: java_code_with_syntax_error().
  javascript_code_with_syntax_error: javascript_code_with_syntax_error().
  python_identifier: python_identifier.
  java_identifier: java_identifier.
  js_identifier: js_identifier.
  random_garbage_code: random_garbage_code().
  TestParserErrorRecoveryProperties: TestParserErrorRecoveryProperties#
  TestEngineErrorRecoveryProperties: TestEngineErrorRecoveryProperties#
  TestParserErrorDetectionProperties: TestParserErrorDetectionProperties#
  TestParserUnsupportedLanguageProperties: TestParserUnsupportedLanguageProperties#
  TestParserEmptyInputProperties: TestParserEmptyInputProperties#
---
# Module: [`tests/unit/core/test_parser_error_recovery_properties.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_parser_error_recovery_properties.py)

## Classes
### `TestEngineErrorRecoveryProperties`
- def: [`tests/unit/core/test_parser_error_recovery_properties.py:422`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_parser_error_recovery_properties.py#L422)
- doc: Property-based tests for AnalysisEngine error recovery.
- signature: `class TestEngineErrorRecoveryProperties:`
- members:
  - `test_property_6_engine_returns_result_for_invalid_java(self, code: str)` — [`L466`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_parser_error_recovery_properties.py#L466) — **Feature: test-coverage-improvement, Property 6: Parser Error Recovery**
  - `test_property_6_engine_returns_result_for_invalid_javascript(self, code: str)` — [`L493`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_parser_error_recovery_properties.py#L493) — **Feature: test-coverage-improvement, Property 6: Parser Error Recovery**
  - `test_property_6_engine_returns_result_for_invalid_python(self, code: str)` — [`L436`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_parser_error_recovery_properties.py#L436) — **Feature: test-coverage-improvement, Property 6: Parser Error Recovery**
- uses (calls/refs, reference-scoped): [`AnalysisResult`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult), [`language`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.language), [`UnifiedAnalysisEngine`](../../../tree_sitter_analyzer/core/analysis_engine.md#UnifiedAnalysisEngine), [`analyze_code`](../../../tree_sitter_analyzer/core/_analysis_engine_code_mixin.md#UnifiedAnalysisEngineCodeMixin.analyze_code)  (3 test-only)

### `TestParserEmptyInputProperties`
- def: [`tests/unit/core/test_parser_error_recovery_properties.py:640`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_parser_error_recovery_properties.py#L640)
- doc: Property-based tests for handling empty and edge case inputs.
- signature: `class TestParserEmptyInputProperties:`
- members:
  - `test_property_6_parser_handles_empty_string(self, language: str)` — [`L650`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_parser_error_recovery_properties.py#L650) — **Feature: test-coverage-improvement, Property 6: Parser Error Recovery**
  - `test_property_6_parser_handles_whitespace_only(self, whitespace: str, language: str)` — [`L676`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_parser_error_recovery_properties.py#L676) — **Feature: test-coverage-improvement, Property 6: Parser Error Recovery**
- uses (calls/refs, reference-scoped): [`Parser`](../../../tree_sitter_analyzer/core/parser.md#Parser), [`parse_code`](../../../tree_sitter_analyzer/core/parser.md#Parser.parse_code), [`ParseResult`](../../../tree_sitter_analyzer/core/parser.md#ParseResult), [`is_language_supported`](../../../tree_sitter_analyzer/core/parser.md#Parser.is_language_supported)

### `TestParserErrorDetectionProperties`
- def: [`tests/unit/core/test_parser_error_recovery_properties.py:520`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_parser_error_recovery_properties.py#L520)
- doc: Property-based tests for parser error detection capabilities.
- signature: `class TestParserErrorDetectionProperties:`
- members:
  - `test_property_6_parser_can_detect_errors_in_tree(self, code: str)` — [`L530`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_parser_error_recovery_properties.py#L530) — **Feature: test-coverage-improvement, Property 6: Parser Error Recovery**
  - `test_property_6_parser_validates_ast_correctly(self, data: tuple)` — [`L559`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_parser_error_recovery_properties.py#L559) — **Feature: test-coverage-improvement, Property 6: Parser Error Recovery**
- uses (calls/refs, reference-scoped): [`Parser`](../../../tree_sitter_analyzer/core/parser.md#Parser), [`tree`](../../../tree_sitter_analyzer/core/parser.md#ParseResult.tree), [`parse_code`](../../../tree_sitter_analyzer/core/parser.md#Parser.parse_code), [`success`](../../../tree_sitter_analyzer/core/parser.md#ParseResult.success), [`get_parse_errors`](../../../tree_sitter_analyzer/core/parser.md#Parser.get_parse_errors), [`validate_ast`](../../../tree_sitter_analyzer/core/parser.md#Parser.validate_ast)  (2 test-only)

### `TestParserErrorRecoveryProperties`
- def: [`tests/unit/core/test_parser_error_recovery_properties.py:279`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_parser_error_recovery_properties.py#L279)
- doc: Property-based tests for parser error recovery.
- signature: `class TestParserErrorRecoveryProperties:`
- members:
  - `test_property_6_java_parser_does_not_crash_on_syntax_errors(self, code: str)` — [`L316`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_parser_error_recovery_properties.py#L316) — **Feature: test-coverage-improvement, Property 6: Parser Error Recovery**
  - `test_property_6_javascript_parser_does_not_crash_on_syntax_errors(self, code: str)` — [`L340`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_parser_error_recovery_properties.py#L340) — **Feature: test-coverage-improvement, Property 6: Parser Error Recovery**
  - `test_property_6_parser_handles_garbage_input_gracefully(self, garbage: str)` — [`L397`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_parser_error_recovery_properties.py#L397) — **Feature: test-coverage-improvement, Property 6: Parser Error Recovery**
  - `test_property_6_parser_returns_partial_results_for_mixed_code(self, data: tuple)` — [`L366`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_parser_error_recovery_properties.py#L366) — **Feature: test-coverage-improvement, Property 6: Parser Error Recovery**
  - `test_property_6_python_parser_does_not_crash_on_syntax_errors(self, code: str)` — [`L289`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_parser_error_recovery_properties.py#L289) — **Feature: test-coverage-improvement, Property 6: Parser Error Recovery**
- uses (calls/refs, reference-scoped): [`Parser`](../../../tree_sitter_analyzer/core/parser.md#Parser), [`tree`](../../../tree_sitter_analyzer/core/parser.md#ParseResult.tree), [`parse_code`](../../../tree_sitter_analyzer/core/parser.md#Parser.parse_code), [`success`](../../../tree_sitter_analyzer/core/parser.md#ParseResult.success), [`ParseResult`](../../../tree_sitter_analyzer/core/parser.md#ParseResult), [`source_code`](../../../tree_sitter_analyzer/core/parser.md#ParseResult.source_code), [`language`](../../../tree_sitter_analyzer/core/parser.md#ParseResult.language), [`is_language_supported`](../../../tree_sitter_analyzer/core/parser.md#Parser.is_language_supported)  (5 test-only)

### `TestParserUnsupportedLanguageProperties`
- def: [`tests/unit/core/test_parser_error_recovery_properties.py:584`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_parser_error_recovery_properties.py#L584)
- doc: Property-based tests for handling unsupported languages.
- signature: `class TestParserUnsupportedLanguageProperties:`
- members:
  - `test_property_6_parser_handles_unsupported_language_gracefully(self, code: str, language: str)` — [`L605`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_parser_error_recovery_properties.py#L605) — **Feature: test-coverage-improvement, Property 6: Parser Error Recovery**
- uses (calls/refs, reference-scoped): [`Parser`](../../../tree_sitter_analyzer/core/parser.md#Parser), [`tree`](../../../tree_sitter_analyzer/core/parser.md#ParseResult.tree), [`parse_code`](../../../tree_sitter_analyzer/core/parser.md#Parser.parse_code), [`success`](../../../tree_sitter_analyzer/core/parser.md#ParseResult.success), [`ParseResult`](../../../tree_sitter_analyzer/core/parser.md#ParseResult), [`error_message`](../../../tree_sitter_analyzer/core/parser.md#ParseResult.error_message)

## Functions
- `code_with_partial_errors(draw)` — [`L222`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_parser_error_recovery_properties.py#L222) — Generate code that has both valid and invalid parts.
- `java_code_with_syntax_error(draw)` — [`L146`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_parser_error_recovery_properties.py#L146) — Generate Java code that contains syntax errors.
- `javascript_code_with_syntax_error(draw)` — [`L184`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_parser_error_recovery_properties.py#L184) — Generate JavaScript code that contains syntax errors.
- `python_code_with_syntax_error(draw)` — [`L98`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_parser_error_recovery_properties.py#L98) — Generate Python code that contains syntax errors.
- `random_garbage_code(draw)` — [`L242`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_parser_error_recovery_properties.py#L242) — Generate random garbage that should not crash the parser.

## Module values
- `java_identifier` — [`L51`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_parser_error_recovery_properties.py#L51)
- `js_identifier` — [`L73`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_parser_error_recovery_properties.py#L73)
- `python_identifier` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_parser_error_recovery_properties.py#L25)

