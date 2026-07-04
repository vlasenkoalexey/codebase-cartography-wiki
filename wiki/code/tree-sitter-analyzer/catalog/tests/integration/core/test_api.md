---
title: 'Module: tests/integration/core/test_api.py'
type: catalog
provenance: extracted
module: tests/integration/core/test_api.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.core.test_api`/TestAPIFacade
symbols:
  TestAPIFacadeIntegration.test_full_analysis_workflow: Integration#test_full_analysis_workflow().
  TestAPIFacade.test_get_framework_info: '#test_get_framework_info().'
  TestAPIFacadeIntegration.test_api_consistency_across_methods: Integration#test_api_consistency_across_methods().
  TestAPIFacade.test_analyze_file_java_success: '#test_analyze_file_java_success().'
  TestAPIFacade.test_analyze_file_python_success: '#test_analyze_file_python_success().'
  TestAPIFacade.test_analyze_file_with_language_override: '#test_analyze_file_with_language_override().'
  TestAPIFacade.test_analyze_file_with_options: '#test_analyze_file_with_options().'
  TestAPIFacade.test_analyze_file_nonexistent: '#test_analyze_file_nonexistent().'
  TestAPIFacade.test_analyze_file_with_path_object: '#test_analyze_file_with_path_object().'
  TestAPIFacade.test_analyze_code_java_success: '#test_analyze_code_java_success().'
  TestAPIFacade.test_analyze_code_python_success: '#test_analyze_code_python_success().'
  TestAPIFacade.test_extract_elements_java: '#test_extract_elements_java().'
  TestAPIFacade.test_extract_elements_python: '#test_extract_elements_python().'
  TestAPIFacade.test_extract_elements_with_types: '#test_extract_elements_with_types().'
  TestAPIFacade.test_get_supported_languages: '#test_get_supported_languages().'
  TestAPIFacade.test_is_language_supported: '#test_is_language_supported().'
  TestAPIFacade.test_detect_language: '#test_detect_language().'
  TestAPIFacade.test_get_available_queries: '#test_get_available_queries().'
  TestAPIFacade.test_execute_query: '#test_execute_query().'
  TestAPIFacade.test_validate_file: '#test_validate_file().'
  TestAPIFacadeErrorHandling.test_analyze_code_empty_content: ErrorHandling#test_analyze_code_empty_content().
  TestAPIFacadeErrorHandling.test_analyze_code_malformed_content: ErrorHandling#test_analyze_code_malformed_content().
  TestAPIFacadeErrorHandling.test_analyze_file_unsupported_language: ErrorHandling#test_analyze_file_unsupported_language().
  TestAPIFacadeErrorHandling.test_extract_elements_nonexistent_file: ErrorHandling#test_extract_elements_nonexistent_file().
  TestAPIFacadeErrorHandling.test_execute_query_invalid_query_name: ErrorHandling#test_execute_query_invalid_query_name().
  TestAPIFacadeErrorHandling.test_validate_file_nonexistent: ErrorHandling#test_validate_file_nonexistent().
  TestAPIFacadeIntegration.test_multiple_file_analysis: Integration#test_multiple_file_analysis().
  TestAPIFacadeIntegration.test_api_performance_with_large_file: Integration#test_api_performance_with_large_file().
  TestAPIFacade: '#'
  TestAPIFacade.sample_java_file: '#sample_java_file().'
  TestAPIFacade.sample_python_file: '#sample_python_file().'
  TestAPIFacadeErrorHandling: ErrorHandling#
  TestAPIFacadeIntegration: Integration#
---
# Module: [`tests/integration/core/test_api.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_api.py)

## Classes
### `TestAPIFacade`
- def: [`tests/integration/core/test_api.py:17`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_api.py#L17)
- doc: Test cases for the unified API facade
- signature: `class TestAPIFacade:`
- members:
  - `sample_java_file(self)` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_api.py#L21) — Create a temporary Java file for testing
  - `sample_python_file(self)` — [`L47`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_api.py#L47) — Create a temporary Python file for testing
  - `test_analyze_code_java_success(self)` — [`L152`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_api.py#L152) — Test successful Java code analysis through API
  - `test_analyze_code_python_success(self)` — [`L168`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_api.py#L168) — Test successful Python code analysis through API
  - `test_analyze_file_java_success(self, sample_java_file: str)` — [`L77`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_api.py#L77) — Test successful Java file analysis through API
  - `test_analyze_file_nonexistent(self)` — [`L134`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_api.py#L134) — Test analysis of non-existent file
  - `test_analyze_file_python_success(self, sample_python_file: str)` — [`L93`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_api.py#L93) — Test successful Python file analysis through API
  - `test_analyze_file_with_language_override(self, sample_java_file: str)` — [`L108`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_api.py#L108) — Test file analysis with explicit language specification
  - `test_analyze_file_with_options(self, sample_java_file: str)` — [`L120`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_api.py#L120) — Test file analysis with additional options
  - `test_analyze_file_with_path_object(self, sample_java_file: str)` — [`L139`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_api.py#L139) — Test file analysis with Path object
  - `test_detect_language(self, sample_java_file: str)` — [`L242`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_api.py#L242) — Test language detection from file
  - `test_execute_query(self, sample_java_file: str)` — [`L259`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_api.py#L259) — Test query execution on file
  - `test_extract_elements_java(self, sample_java_file: str)` — [`L187`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_api.py#L187) — Test element extraction from Java file
  - `test_extract_elements_python(self, sample_python_file: str)` — [`L200`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_api.py#L200) — Test element extraction from Python file
  - `test_extract_elements_with_types(self, sample_java_file: str)` — [`L213`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_api.py#L213) — Test element extraction with specific types
  - `test_get_available_queries(self)` — [`L252`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_api.py#L252) — Test getting available queries for a language
  - `test_get_framework_info(self)` — [`L283`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_api.py#L283) — Test getting framework information
  - `test_get_supported_languages(self)` — [`L227`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_api.py#L227) — Test getting list of supported languages
  - `test_is_language_supported(self)` — [`L235`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_api.py#L235) — Test checking if language is supported
  - `test_validate_file(self, sample_java_file: str)` — [`L270`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_api.py#L270) — Test file validation
- uses (calls/refs, reference-scoped): [`analyze_file`](../../../tree_sitter_analyzer/api.md#analyze_file), [`analyze_code`](../../../tree_sitter_analyzer/api.md#analyze_code), [`execute_query`](../../../tree_sitter_analyzer/api.md#execute_query), [`validate_file`](../../../tree_sitter_analyzer/api.md#validate_file), [`extract_elements`](../../../tree_sitter_analyzer/api.md#extract_elements), [`detect_language`](../../../tree_sitter_analyzer/api.md#detect_language), [`get_framework_info`](../../../tree_sitter_analyzer/api.md#get_framework_info), [`__version__`](../../../tree_sitter_analyzer/__init__.md#__version__), [`get_supported_languages`](../../../tree_sitter_analyzer/api.md#get_supported_languages), [`get_available_queries`](../../../tree_sitter_analyzer/api.md#get_available_queries), [`is_language_supported`](../../../tree_sitter_analyzer/api.md#is_language_supported)

### `TestAPIFacadeErrorHandling`
- def: [`tests/integration/core/test_api.py:294`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_api.py#L294)
- doc: Test error handling in API facade
- signature: `class TestAPIFacadeErrorHandling:`
- members:
  - `test_analyze_code_empty_content(self)` — [`L297`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_api.py#L297) — Test analysis of empty code content
  - `test_analyze_code_malformed_content(self)` — [`L305`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_api.py#L305) — Test analysis of malformed code content
  - `test_analyze_file_unsupported_language(self)` — [`L317`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_api.py#L317) — Test analysis with unsupported language
  - `test_execute_query_invalid_query_name(self)` — [`L340`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_api.py#L340) — Test query execution with invalid query name
  - `test_extract_elements_nonexistent_file(self)` — [`L332`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_api.py#L332) — Test element extraction from non-existent file
  - `test_validate_file_nonexistent(self)` — [`L356`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_api.py#L356) — Test validation of non-existent file
- uses (calls/refs, reference-scoped): [`analyze_file`](../../../tree_sitter_analyzer/api.md#analyze_file), [`analyze_code`](../../../tree_sitter_analyzer/api.md#analyze_code), [`execute_query`](../../../tree_sitter_analyzer/api.md#execute_query), [`validate_file`](../../../tree_sitter_analyzer/api.md#validate_file), [`extract_elements`](../../../tree_sitter_analyzer/api.md#extract_elements)

### `TestAPIFacadeIntegration`
- def: [`tests/integration/core/test_api.py:365`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_api.py#L365)
- doc: Integration tests for API facade
- signature: `class TestAPIFacadeIntegration:`
- members:
  - `test_api_consistency_across_methods(self)` — [`L470`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_api.py#L470) — Test that API methods return consistent results
  - `test_api_performance_with_large_file(self)` — [`L508`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_api.py#L508) — Test API performance with large code files
  - `test_full_analysis_workflow(self)` — [`L368`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_api.py#L368) — Test complete analysis workflow through API
  - `test_multiple_file_analysis(self)` — [`L436`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/test_api.py#L436) — Test analysis of multiple files through API
- uses (calls/refs, reference-scoped): [`analyze_file`](../../../tree_sitter_analyzer/api.md#analyze_file), [`analyze_code`](../../../tree_sitter_analyzer/api.md#analyze_code), [`execute_query`](../../../tree_sitter_analyzer/api.md#execute_query), [`extract_elements`](../../../tree_sitter_analyzer/api.md#extract_elements), [`detect_language`](../../../tree_sitter_analyzer/api.md#detect_language), [`get_available_queries`](../../../tree_sitter_analyzer/api.md#get_available_queries)

