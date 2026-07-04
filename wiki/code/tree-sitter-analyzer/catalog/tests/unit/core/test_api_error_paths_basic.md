---
title: 'Module: tests/unit/core/test_api_error_paths_basic.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_api_error_paths_basic.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_api_error_paths_basic`/Test
symbols:
  TestAnalyzeFileErrors.test_analyze_failure_with_error_message: AnalyzeFileErrors#test_analyze_failure_with_error_message().
  TestAnalyzeFileErrors.test_analyze_elements_with_module_path: AnalyzeFileErrors#test_analyze_elements_with_module_path().
  TestAnalyzeFileErrors.test_analyze_failure_no_elements_no_queries: AnalyzeFileErrors#test_analyze_failure_no_elements_no_queries().
  TestAnalyzeCode.test_analyze_code_failure_with_error_message: AnalyzeCode#test_analyze_code_failure_with_error_message().
  TestAnalyzeCode.test_analyze_code_with_elements: AnalyzeCode#test_analyze_code_with_elements().
  TestAnalyzeCode.test_analyze_code_failure_no_elements: AnalyzeCode#test_analyze_code_failure_no_elements().
  TestAnalyzeCode.test_analyze_code_exception: AnalyzeCode#test_analyze_code_exception().
  TestExceptionPaths.test_get_supported_languages_exception: ExceptionPaths#test_get_supported_languages_exception().
  TestExceptionPaths.test_get_available_queries_exception: ExceptionPaths#test_get_available_queries_exception().
  TestExceptionPaths.test_is_language_supported_exception: ExceptionPaths#test_is_language_supported_exception().
  TestExceptionPaths.test_detect_language_exception: ExceptionPaths#test_detect_language_exception().
  TestExceptionPaths.test_get_file_extensions_exception: ExceptionPaths#test_get_file_extensions_exception().
  TestExceptionPaths.test_get_framework_info_exception: ExceptionPaths#test_get_framework_info_exception().
  TestDetectLanguageEdgeCases.test_empty_file_path: DetectLanguageEdgeCases#test_empty_file_path().
  TestDetectLanguageEdgeCases.test_nonexistent_file: DetectLanguageEdgeCases#test_nonexistent_file().
  TestDetectLanguageEdgeCases.test_whitespace_result: DetectLanguageEdgeCases#test_whitespace_result().
  TestGetFileExtensions.test_with_get_extensions_method: GetFileExtensions#test_with_get_extensions_method().
  TestGetFileExtensions.test_fallback_extension_map: GetFileExtensions#test_fallback_extension_map().
  TestGetFileExtensions.test_fallback_unknown_language: GetFileExtensions#test_fallback_unknown_language().
  TestValidateFile.test_nonexistent_file: ValidateFile#test_nonexistent_file().
  TestValidateFile.test_validation_exception: ValidateFile#test_validation_exception().
  TestExecuteQuery.test_execute_query_error: ExecuteQuery#test_execute_query_error().
  TestExtractElements.test_extract_elements_error: ExtractElements#test_extract_elements_error().
  TestExtractElements.test_extract_elements_exception: ExtractElements#test_extract_elements_exception().
  TestConvenienceFunctions.test_analyze_alias: ConvenienceFunctions#test_analyze_alias().
  TestConvenienceFunctions.test_get_languages_alias: ConvenienceFunctions#test_get_languages_alias().
  TestGroupCaptures.test_list_capture_path: GroupCaptures#test_list_capture_path().
  TestAnalyzeFileErrors: AnalyzeFileErrors#
  TestAnalyzeCode: AnalyzeCode#
  TestExceptionPaths: ExceptionPaths#
  TestDetectLanguageEdgeCases: DetectLanguageEdgeCases#
  TestGetFileExtensions: GetFileExtensions#
  TestValidateFile: ValidateFile#
  TestExecuteQuery: ExecuteQuery#
  TestExtractElements: ExtractElements#
  TestConvenienceFunctions: ConvenienceFunctions#
  TestGroupCaptures: GroupCaptures#
---
# Module: [`tests/unit/core/test_api_error_paths_basic.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_api_error_paths_basic.py)

## Classes
### `TestAnalyzeCode`
- def: [`tests/unit/core/test_api_error_paths_basic.py:104`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_api_error_paths_basic.py#L104)
- doc: Tests for analyze_code error and edge case paths.
- signature: `class TestAnalyzeCode:`
- members:
  - `test_analyze_code_exception(self)` — [`L174`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_api_error_paths_basic.py#L174) — Lines 322-324: analyze_code exception handler.
  - `test_analyze_code_failure_no_elements(self)` — [`L158`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_api_error_paths_basic.py#L158) — Lines 311-318: code analysis failure removing elements/queries.
  - `test_analyze_code_failure_with_error_message(self)` — [`L107`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_api_error_paths_basic.py#L107) — Lines 238-240: code analysis failure.
  - `test_analyze_code_with_elements(self)` — [`L124`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_api_error_paths_basic.py#L124) — Lines 244-284: elements with all attributes.
- uses (calls/refs, reference-scoped): [`analyze_code`](../../../tree_sitter_analyzer/api.md#analyze_code)

### `TestAnalyzeFileErrors`
- def: [`tests/unit/core/test_api_error_paths_basic.py:31`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_api_error_paths_basic.py#L31)
- doc: Tests for analyze_file error and edge case paths.
- signature: `class TestAnalyzeFileErrors:`
- members:
  - `test_analyze_elements_with_module_path(self)` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_api_error_paths_basic.py#L49) — Line 256: elements with module_path attribute.
  - `test_analyze_failure_no_elements_no_queries(self)` — [`L81`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_api_error_paths_basic.py#L81) — Lines 170-177: error when elements/query_results not present.
  - `test_analyze_failure_with_error_message(self)` — [`L34`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_api_error_paths_basic.py#L34) — Lines 97-99: analysis failure with error_message.
- uses (calls/refs, reference-scoped): [`analyze_file`](../../../tree_sitter_analyzer/api.md#analyze_file)

### `TestConvenienceFunctions`
- def: [`tests/unit/core/test_api_error_paths_basic.py:409`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_api_error_paths_basic.py#L409)
- doc: Tests for convenience/alias functions.
- signature: `class TestConvenienceFunctions:`
- members:
  - `test_analyze_alias(self)` — [`L412`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_api_error_paths_basic.py#L412) — Line 742: analyze() aliases to analyze_file().
  - `test_get_languages_alias(self)` — [`L428`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_api_error_paths_basic.py#L428) — Line 747: get_languages() aliases to get_supported_languages().
- uses (calls/refs, reference-scoped): [`analyze`](../../../tree_sitter_analyzer/api.md#analyze), [`get_languages`](../../../tree_sitter_analyzer/api.md#get_languages)

### `TestDetectLanguageEdgeCases`
- def: [`tests/unit/core/test_api_error_paths_basic.py:257`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_api_error_paths_basic.py#L257)
- doc: Tests for detect_language edge cases.
- signature: `class TestDetectLanguageEdgeCases:`
- members:
  - `test_empty_file_path(self)` — [`L260`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_api_error_paths_basic.py#L260) — Line 396: empty file_path returns 'unknown'.
  - `test_nonexistent_file(self)` — [`L265`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_api_error_paths_basic.py#L265) — Line 404: empty detection result returns 'unknown'.
  - `test_whitespace_result(self)` — [`L275`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_api_error_paths_basic.py#L275) — Line 404: whitespace-only result returns 'unknown'.
- uses (calls/refs, reference-scoped): [`detect_language`](../../../tree_sitter_analyzer/api.md#detect_language)

### `TestExceptionPaths`
- def: [`tests/unit/core/test_api_error_paths_basic.py:190`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_api_error_paths_basic.py#L190)
- doc: Tests for exception handling paths in various API functions.
- signature: `class TestExceptionPaths:`
- members:
  - `test_detect_language_exception(self)` — [`L220`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_api_error_paths_basic.py#L220) — Lines 407-409: detect_language exception.
  - `test_get_available_queries_exception(self)` — [`L202`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_api_error_paths_basic.py#L202) — Lines 360-362: get_available_queries exception.
  - `test_get_file_extensions_exception(self)` — [`L232`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_api_error_paths_basic.py#L232) — Lines 441-443: get_file_extensions exception.
  - `test_get_framework_info_exception(self)` — [`L241`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_api_error_paths_basic.py#L241) — Lines 537-539: get_framework_info exception.
  - `test_get_supported_languages_exception(self)` — [`L193`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_api_error_paths_basic.py#L193) — Lines 342-344: get_supported_languages exception.
  - `test_is_language_supported_exception(self)` — [`L211`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_api_error_paths_basic.py#L211) — Lines 378-380: is_language_supported exception.
- uses (calls/refs, reference-scoped): [`detect_language`](../../../tree_sitter_analyzer/api.md#detect_language), [`get_framework_info`](../../../tree_sitter_analyzer/api.md#get_framework_info), [`get_file_extensions`](../../../tree_sitter_analyzer/api.md#get_file_extensions), [`get_supported_languages`](../../../tree_sitter_analyzer/api.md#get_supported_languages), [`get_available_queries`](../../../tree_sitter_analyzer/api.md#get_available_queries), [`is_language_supported`](../../../tree_sitter_analyzer/api.md#is_language_supported)

### `TestExecuteQuery`
- def: [`tests/unit/core/test_api_error_paths_basic.py:357`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_api_error_paths_basic.py#L357)
- doc: Tests for execute_query edge cases.
- signature: `class TestExecuteQuery:`
- members:
  - `test_execute_query_error(self)` — [`L360`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_api_error_paths_basic.py#L360) — Lines 667-676: execute_query error path.
- uses (calls/refs, reference-scoped): [`execute_query`](../../../tree_sitter_analyzer/api.md#execute_query)

### `TestExtractElements`
- def: [`tests/unit/core/test_api_error_paths_basic.py:380`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_api_error_paths_basic.py#L380)
- doc: Tests for extract_elements edge cases.
- signature: `class TestExtractElements:`
- members:
  - `test_extract_elements_error(self)` — [`L383`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_api_error_paths_basic.py#L383) — Lines 734-736: extract_elements error.
  - `test_extract_elements_exception(self)` — [`L395`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_api_error_paths_basic.py#L395) — Exception handler.
- uses (calls/refs, reference-scoped): [`extract_elements`](../../../tree_sitter_analyzer/api.md#extract_elements)

### `TestGetFileExtensions`
- def: [`tests/unit/core/test_api_error_paths_basic.py:291`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_api_error_paths_basic.py#L291)
- doc: Tests for get_file_extensions edge cases.
- signature: `class TestGetFileExtensions:`
- members:
  - `test_fallback_extension_map(self)` — [`L306`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_api_error_paths_basic.py#L306) — Lines 430-440: fallback to extension_map.
  - `test_fallback_unknown_language(self)` — [`L318`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_api_error_paths_basic.py#L318) — Fallback for unknown language returns empty list.
  - `test_with_get_extensions_method(self)` — [`L294`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_api_error_paths_basic.py#L294) — Lines 425-427: hasattr get_extensions_for_language.
- uses (calls/refs, reference-scoped): [`get_file_extensions`](../../../tree_sitter_analyzer/api.md#get_file_extensions)

### `TestGroupCaptures`
- def: [`tests/unit/core/test_api_error_paths_basic.py:443`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_api_error_paths_basic.py#L443)
- doc: Tests for _group_captures_by_main_node internal function.
- signature: `class TestGroupCaptures:`
- members:
  - `test_list_capture_path(self)` — [`L446`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_api_error_paths_basic.py#L446) — Lines 608-610: existing capture is a list (multiple sub-captures).
- uses (calls/refs, reference-scoped): [`_group_captures_by_main_node`](../../../tree_sitter_analyzer/api.md#_group_captures_by_main_node)

### `TestValidateFile`
- def: [`tests/unit/core/test_api_error_paths_basic.py:336`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_api_error_paths_basic.py#L336)
- doc: Tests for validate_file.
- signature: `class TestValidateFile:`
- members:
  - `test_nonexistent_file(self)` — [`L339`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_api_error_paths_basic.py#L339) — File doesn't exist.
  - `test_validation_exception(self)` — [`L344`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_api_error_paths_basic.py#L344) — Lines 500-501: top-level validation exception.
- uses (calls/refs, reference-scoped): [`validate_file`](../../../tree_sitter_analyzer/api.md#validate_file)

