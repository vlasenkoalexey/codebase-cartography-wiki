---
title: 'Module: tests/unit/core/test_parser.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_parser.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_parser`/
symbols:
  TestParserParseFile.test_parse_file_success: TestParserParseFile#test_parse_file_success().
  TestParseResult.test_parse_result_success: TestParseResult#test_parse_result_success().
  TestParseResult.test_parse_result_failure: TestParseResult#test_parse_result_failure().
  TestParseResult.test_parse_result_without_file_path: TestParseResult#test_parse_result_without_file_path().
  TestParserParseFile.test_parse_file_not_found: TestParserParseFile#test_parse_file_not_found().
  TestParserParseCode.test_parse_code_success: TestParserParseCode#test_parse_code_success().
  TestParserCache.test_cache_invalidates_on_mtime_change: TestParserCache#test_cache_invalidates_on_mtime_change().
  TestParserParseCode.test_parse_code_unsupported_language: TestParserParseCode#test_parse_code_unsupported_language().
  TestParserValidation.test_validate_ast_valid: TestParserValidation#test_validate_ast_valid().
  TestParserValidation.test_get_parse_errors_no_errors: TestParserValidation#test_get_parse_errors_no_errors().
  TestParserValidation.test_get_parse_errors_with_errors: TestParserValidation#test_get_parse_errors_with_errors().
  TestParserCache.test_cache_clear_resets_state: TestParserCache#test_cache_clear_resets_state().
  TestParserEdgeCases.test_parse_code_exception_handling: TestParserEdgeCases#test_parse_code_exception_handling().
  TestParserParseFile.test_parse_file_permission_denied: TestParserParseFile#test_parse_file_permission_denied().
  TestParserParseFile.test_parse_file_cache_hit: TestParserParseFile#test_parse_file_cache_hit().
  TestParserParseFile.test_parse_file_with_path_object: TestParserParseFile#test_parse_file_with_path_object().
  TestParserParseCode.test_parse_code_with_filename: TestParserParseCode#test_parse_code_with_filename().
  TestParserParseCode.test_parse_code_without_filename: TestParserParseCode#test_parse_code_without_filename().
  TestParserParseCode.test_parse_code_empty_string: TestParserParseCode#test_parse_code_empty_string().
  TestParserCache.test_cache_info_exposes_counters: TestParserCache#test_cache_info_exposes_counters().
  TestParserEdgeCases.test_parse_file_exception_handling: TestParserEdgeCases#test_parse_file_exception_handling().
  TestParserInit.test_parser_init: TestParserInit#test_parser_init().
  TestParserEdgeCases.test_is_language_supported_exception_handling: TestParserEdgeCases#test_is_language_supported_exception_handling().
  TestParserEdgeCases.test_get_supported_languages_exception_handling: TestParserEdgeCases#test_get_supported_languages_exception_handling().
  TestParserInit.test_parser_class_cache_exists: TestParserInit#test_parser_class_cache_exists().
  TestParserLanguageSupport.test_is_language_supported_true: TestParserLanguageSupport#test_is_language_supported_true().
  TestParserLanguageSupport.test_is_language_supported_false: TestParserLanguageSupport#test_is_language_supported_false().
  TestParserLanguageSupport.test_get_supported_languages: TestParserLanguageSupport#test_get_supported_languages().
  TestParserValidation.test_validate_ast_none: TestParserValidation#test_validate_ast_none().
  TestParserCache.setup_method: TestParserCache#setup_method().
  TestParserCache.test_cache_is_lru_cache: TestParserCache#test_cache_is_lru_cache().
  TestParserCache.test_cache_maxsize: TestParserCache#test_cache_maxsize().
  TestParserCache.test_cache_shared_across_instances: TestParserCache#test_cache_shared_across_instances().
  TestParserEdgeCases.test_validate_ast_exception_handling: TestParserEdgeCases#test_validate_ast_exception_handling().
  TestParserEdgeCases.test_get_parse_errors_exception_handling: TestParserEdgeCases#test_get_parse_errors_exception_handling().
  parser: parser().
  TestParseResult: TestParseResult#
  TestParserInit: TestParserInit#
  TestParserParseFile: TestParserParseFile#
  TestParserParseCode: TestParserParseCode#
  TestParserLanguageSupport: TestParserLanguageSupport#
  TestParserValidation: TestParserValidation#
  TestParserCache: TestParserCache#
  TestParserEdgeCases: TestParserEdgeCases#
  temp_file: temp_file().
---
# Module: [`tests/unit/core/test_parser.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_parser.py)

## Classes
### `TestParseResult`
- def: [`tests/unit/core/test_parser.py:19`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_parser.py#L19)
- doc: Tests for ParseResult NamedTuple.
- signature: `class TestParseResult:`
- members:
  - `test_parse_result_failure(self)` — [`L40`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_parser.py#L40) — Test ParseResult with failed parsing.
  - `test_parse_result_success(self)` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_parser.py#L22) — Test ParseResult with successful parsing.
  - `test_parse_result_without_file_path(self)` — [`L57`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_parser.py#L57) — Test ParseResult without file path.
- uses (calls/refs, reference-scoped): [`tree`](../../../tree_sitter_analyzer/core/parser.md#ParseResult.tree), [`success`](../../../tree_sitter_analyzer/core/parser.md#ParseResult.success), [`ParseResult`](../../../tree_sitter_analyzer/core/parser.md#ParseResult), [`error_message`](../../../tree_sitter_analyzer/core/parser.md#ParseResult.error_message), [`source_code`](../../../tree_sitter_analyzer/core/parser.md#ParseResult.source_code), [`language`](../../../tree_sitter_analyzer/core/parser.md#ParseResult.language), [`file_path`](../../../tree_sitter_analyzer/core/parser.md#ParseResult.file_path)

### `TestParserCache`
- def: [`tests/unit/core/test_parser.py:243`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_parser.py#L243)
- doc: Tests for Parser caching functionality.
- signature: `class TestParserCache:`
- members:
  - `setup_method(self, method)` — [`L249`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_parser.py#L249)
  - `test_cache_clear_resets_state(self, tmp_path)` — [`L292`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_parser.py#L292)
  - `test_cache_info_exposes_counters(self, tmp_path)` — [`L273`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_parser.py#L273) — PERF-2: cache_info() exposes hits/misses/stat_hits for diagnostics.
  - `test_cache_invalidates_on_mtime_change(self, tmp_path)` — [`L307`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_parser.py#L307) — PERF-2: stat fast-path must not return a stale tree after the file
  - `test_cache_is_lru_cache(self)` — [`L252`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_parser.py#L252) — Test that Parser cache is LRUCache.
  - `test_cache_maxsize(self)` — [`L258`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_parser.py#L258) — PERF-2: cache must be sized for medium projects (>=1000) by default.
  - `test_cache_shared_across_instances(self)` — [`L267`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_parser.py#L267) — Test that cache is shared across Parser instances.
- uses (calls/refs, reference-scoped): [`Parser`](../../../tree_sitter_analyzer/core/parser.md#Parser), [`success`](../../../tree_sitter_analyzer/core/parser.md#ParseResult.success), [`parse_file`](../../../tree_sitter_analyzer/core/parser.md#Parser.parse_file), [`source_code`](../../../tree_sitter_analyzer/core/parser.md#ParseResult.source_code), [`cache_clear`](../../../tree_sitter_analyzer/core/parser.md#Parser.cache_clear), [`cache_info`](../../../tree_sitter_analyzer/core/parser.md#Parser.cache_info), [`_cache`](../../../tree_sitter_analyzer/core/parser.md#Parser._cache)

### `TestParserEdgeCases`
- def: [`tests/unit/core/test_parser.py:330`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_parser.py#L330)
- doc: Tests for edge cases and error handling.
- signature: `class TestParserEdgeCases:`
- members:
  - `test_get_parse_errors_exception_handling(self, parser: Parser)` — [`L381`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_parser.py#L381) — Test that exceptions in get_parse_errors are handled.
  - `test_get_supported_languages_exception_handling(self, parser: Parser)` — [`L361`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_parser.py#L361) — Test that exceptions in get_supported_languages are handled.
  - `test_is_language_supported_exception_handling(self, parser: Parser)` — [`L351`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_parser.py#L351) — Test that exceptions in is_language_supported are handled.
  - `test_parse_code_exception_handling(self, parser: Parser)` — [`L333`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_parser.py#L333) — Test that exceptions in parse_code are handled gracefully.
  - `test_parse_file_exception_handling(self, parser: Parser, temp_file: Path)` — [`L342`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_parser.py#L342) — Test that exceptions in parse_file are handled gracefully.
  - `test_validate_ast_exception_handling(self, parser: Parser)` — [`L371`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_parser.py#L371) — Test that exceptions in validate_ast are handled.
- uses (calls/refs, reference-scoped): [`Parser`](../../../tree_sitter_analyzer/core/parser.md#Parser), [`parse_code`](../../../tree_sitter_analyzer/core/parser.md#Parser.parse_code), [`success`](../../../tree_sitter_analyzer/core/parser.md#ParseResult.success), [`parse_file`](../../../tree_sitter_analyzer/core/parser.md#Parser.parse_file), [`error_message`](../../../tree_sitter_analyzer/core/parser.md#ParseResult.error_message), [`is_language_supported`](../../../tree_sitter_analyzer/core/parser.md#Parser.is_language_supported), [`_loader`](../../../tree_sitter_analyzer/core/parser.md#Parser._loader), [`get_supported_languages`](../../../tree_sitter_analyzer/core/parser.md#Parser.get_supported_languages), [`get_parse_errors`](../../../tree_sitter_analyzer/core/parser.md#Parser.get_parse_errors), [`validate_ast`](../../../tree_sitter_analyzer/core/parser.md#Parser.validate_ast)

### `TestParserInit`
- def: [`tests/unit/core/test_parser.py:71`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_parser.py#L71)
- doc: Tests for Parser initialization.
- signature: `class TestParserInit:`
- members:
  - `test_parser_class_cache_exists(self)` — [`L80`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_parser.py#L80) — Test that Parser has class-level cache.
  - `test_parser_init(self)` — [`L74`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_parser.py#L74) — Test Parser initialization.
- uses (calls/refs, reference-scoped): [`Parser`](../../../tree_sitter_analyzer/core/parser.md#Parser), [`_cache`](../../../tree_sitter_analyzer/core/parser.md#Parser._cache), [`_loader`](../../../tree_sitter_analyzer/core/parser.md#Parser._loader), [`_encoding_manager`](../../../tree_sitter_analyzer/core/parser.md#Parser._encoding_manager)

### `TestParserLanguageSupport`
- def: [`tests/unit/core/test_parser.py:186`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_parser.py#L186)
- doc: Tests for Parser language support methods.
- signature: `class TestParserLanguageSupport:`
- members:
  - `test_get_supported_languages(self, parser: Parser)` — [`L197`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_parser.py#L197) — Test getting list of supported languages.
  - `test_is_language_supported_false(self, parser: Parser)` — [`L193`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_parser.py#L193) — Test checking unsupported language.
  - `test_is_language_supported_true(self, parser: Parser)` — [`L189`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_parser.py#L189) — Test checking supported language.
- uses (calls/refs, reference-scoped): [`Parser`](../../../tree_sitter_analyzer/core/parser.md#Parser), [`is_language_supported`](../../../tree_sitter_analyzer/core/parser.md#Parser.is_language_supported), [`get_supported_languages`](../../../tree_sitter_analyzer/core/parser.md#Parser.get_supported_languages)

### `TestParserParseCode`
- def: [`tests/unit/core/test_parser.py:144`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_parser.py#L144)
- doc: Tests for Parser.parse_code method.
- signature: `class TestParserParseCode:`
- members:
  - `test_parse_code_empty_string(self, parser: Parser)` — [`L179`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_parser.py#L179) — Test parsing empty code string.
  - `test_parse_code_success(self, parser: Parser)` — [`L147`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_parser.py#L147) — Test successful code parsing.
  - `test_parse_code_unsupported_language(self, parser: Parser)` — [`L157`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_parser.py#L157) — Test parsing code with unsupported language.
  - `test_parse_code_with_filename(self, parser: Parser)` — [`L165`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_parser.py#L165) — Test parsing code with filename.
  - `test_parse_code_without_filename(self, parser: Parser)` — [`L172`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_parser.py#L172) — Test parsing code without filename.
- uses (calls/refs, reference-scoped): [`Parser`](../../../tree_sitter_analyzer/core/parser.md#Parser), [`tree`](../../../tree_sitter_analyzer/core/parser.md#ParseResult.tree), [`parse_code`](../../../tree_sitter_analyzer/core/parser.md#Parser.parse_code), [`success`](../../../tree_sitter_analyzer/core/parser.md#ParseResult.success), [`error_message`](../../../tree_sitter_analyzer/core/parser.md#ParseResult.error_message), [`source_code`](../../../tree_sitter_analyzer/core/parser.md#ParseResult.source_code), [`language`](../../../tree_sitter_analyzer/core/parser.md#ParseResult.language), [`file_path`](../../../tree_sitter_analyzer/core/parser.md#ParseResult.file_path)

### `TestParserParseFile`
- def: [`tests/unit/core/test_parser.py:86`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_parser.py#L86)
- doc: Tests for Parser.parse_file method.
- signature: `class TestParserParseFile:`
- members:
  - `test_parse_file_cache_hit(self, parser: Parser, temp_file: Path)` — [`L126`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_parser.py#L126) — Test that cache is used for repeated file parsing.
  - `test_parse_file_not_found(self, parser: Parser)` — [`L100`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_parser.py#L100) — Test parsing non-existent file.
  - `test_parse_file_permission_denied(self, parser: Parser, temp_file: Path)` — [`L109`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_parser.py#L109) — Test parsing file with permission denied.
  - `test_parse_file_success(self, parser: Parser, temp_file: Path)` — [`L89`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_parser.py#L89) — Test successful file parsing.
  - `test_parse_file_with_path_object(self, parser: Parser, temp_file: Path)` — [`L137`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_parser.py#L137) — Test parsing file with Path object.
- uses (calls/refs, reference-scoped): [`Parser`](../../../tree_sitter_analyzer/core/parser.md#Parser), [`tree`](../../../tree_sitter_analyzer/core/parser.md#ParseResult.tree), [`success`](../../../tree_sitter_analyzer/core/parser.md#ParseResult.success), [`parse_file`](../../../tree_sitter_analyzer/core/parser.md#Parser.parse_file), [`error_message`](../../../tree_sitter_analyzer/core/parser.md#ParseResult.error_message), [`source_code`](../../../tree_sitter_analyzer/core/parser.md#ParseResult.source_code), [`language`](../../../tree_sitter_analyzer/core/parser.md#ParseResult.language), [`file_path`](../../../tree_sitter_analyzer/core/parser.md#ParseResult.file_path)

### `TestParserValidation`
- def: [`tests/unit/core/test_parser.py:208`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_parser.py#L208)
- doc: Tests for Parser validation methods.
- signature: `class TestParserValidation:`
- members:
  - `test_get_parse_errors_no_errors(self, parser: Parser, temp_file: Path)` — [`L223`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_parser.py#L223) — Test getting parse errors from valid code.
  - `test_get_parse_errors_with_errors(self, parser: Parser)` — [`L231`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_parser.py#L231) — Test getting parse errors from invalid code.
  - `test_validate_ast_none(self, parser: Parser)` — [`L218`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_parser.py#L218) — Test validating None AST.
  - `test_validate_ast_valid(self, parser: Parser, temp_file: Path)` — [`L211`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_parser.py#L211) — Test validating a valid AST.
- uses (calls/refs, reference-scoped): [`Parser`](../../../tree_sitter_analyzer/core/parser.md#Parser), [`tree`](../../../tree_sitter_analyzer/core/parser.md#ParseResult.tree), [`parse_code`](../../../tree_sitter_analyzer/core/parser.md#Parser.parse_code), [`success`](../../../tree_sitter_analyzer/core/parser.md#ParseResult.success), [`parse_file`](../../../tree_sitter_analyzer/core/parser.md#Parser.parse_file), [`get_parse_errors`](../../../tree_sitter_analyzer/core/parser.md#Parser.get_parse_errors), [`validate_ast`](../../../tree_sitter_analyzer/core/parser.md#Parser.validate_ast)

## Functions
- `parser()` — [`L391`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_parser.py#L391) — Create a Parser instance for testing.
- `temp_file()` — [`L397`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_parser.py#L397) — Create a temporary Python file for testing.

