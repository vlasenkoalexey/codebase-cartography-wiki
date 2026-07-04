---
title: 'Module: tests/unit/languages/test_cpp_plugin_analysis_helpers.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_cpp_plugin_analysis_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_cpp_plugin_analysis_helpers`/Test
symbols:
  TestEmptyCppAnalysisResult.test_returns_correct_result: EmptyCppAnalysisResult#test_returns_correct_result().
  TestBuildCppAnalysisResult.test_builds_result: BuildCppAnalysisResult#test_builds_result().
  TestCppAnalysisErrorResult.test_error_result: CppAnalysisErrorResult#test_error_result().
  TestCppParserFailureResult.test_includes_error_message: CppParserFailureResult#test_includes_error_message().
  TestEmptyCppAnalysisResult.test_single_line: EmptyCppAnalysisResult#test_single_line().
  TestEmptyCppAnalysisResult.test_empty_content: EmptyCppAnalysisResult#test_empty_content().
  TestCppParserFailureResult.test_line_count: CppParserFailureResult#test_line_count().
  TestCreateCppParser.test_constructor_fallback_failure: CreateCppParser#test_constructor_fallback_failure().
  TestCreateCppParser.test_set_language_path: CreateCppParser#test_set_language_path().
  TestCreateCppParser.test_language_attr_path: CreateCppParser#test_language_attr_path().
  TestCreateCppParser.test_constructor_fallback_success: CreateCppParser#test_constructor_fallback_success().
  TestLoadCppTreeSitterLanguage.test_import_error_returns_none: LoadCppTreeSitterLanguage#test_import_error_returns_none().
  TestLoadCppTreeSitterLanguage.test_general_exception_returns_none: LoadCppTreeSitterLanguage#test_general_exception_returns_none().
  TestFlattenCppElements.test_merges_all_keys: FlattenCppElements#test_merges_all_keys().
  TestFlattenCppElements.test_missing_keys_default_empty: FlattenCppElements#test_missing_keys_default_empty().
  TestFlattenCppElements.test_empty_dict: FlattenCppElements#test_empty_dict().
  TestEmptyCppAnalysisResult: EmptyCppAnalysisResult#
  TestCppParserFailureResult: CppParserFailureResult#
  TestCreateCppParser: CreateCppParser#
  TestLoadCppTreeSitterLanguage: LoadCppTreeSitterLanguage#
  TestFlattenCppElements: FlattenCppElements#
  TestBuildCppAnalysisResult: BuildCppAnalysisResult#
  TestCppAnalysisErrorResult: CppAnalysisErrorResult#
---
# Module: [`tests/unit/languages/test_cpp_plugin_analysis_helpers.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_analysis_helpers.py)

## Classes
### `TestBuildCppAnalysisResult`
- def: [`tests/unit/languages/test_cpp_plugin_analysis_helpers.py:135`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_analysis_helpers.py#L135)
- signature: `class TestBuildCppAnalysisResult:`
- members:
  - `test_builds_result(self)` — [`L136`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_analysis_helpers.py#L136)
- uses (calls/refs, reference-scoped): [`elements`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.elements), [`language`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.language), [`file_path`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.file_path), [`line_count`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.line_count), [`node_count`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.node_count), [`build_cpp_analysis_result`](../../../tree_sitter_analyzer/languages/_cpp_plugin_analysis_helpers.md#build_cpp_analysis_result)

### `TestCppAnalysisErrorResult`
- def: [`tests/unit/languages/test_cpp_plugin_analysis_helpers.py:145`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_analysis_helpers.py#L145)
- signature: `class TestCppAnalysisErrorResult:`
- members:
  - `test_error_result(self)` — [`L146`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_analysis_helpers.py#L146)
- uses (calls/refs, reference-scoped): [`file_path`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.file_path), [`success`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.success), [`line_count`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.line_count), [`error_message`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.error_message), [`cpp_analysis_error_result`](../../../tree_sitter_analyzer/languages/_cpp_plugin_analysis_helpers.md#cpp_analysis_error_result)

### `TestCppParserFailureResult`
- def: [`tests/unit/languages/test_cpp_plugin_analysis_helpers.py:39`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_analysis_helpers.py#L39)
- signature: `class TestCppParserFailureResult:`
- members:
  - `test_includes_error_message(self)` — [`L40`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_analysis_helpers.py#L40)
  - `test_line_count(self)` — [`L47`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_analysis_helpers.py#L47)
- uses (calls/refs, reference-scoped): [`elements`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.elements), [`success`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.success), [`line_count`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.line_count), [`error_message`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.error_message), [`cpp_parser_failure_result`](../../../tree_sitter_analyzer/languages/_cpp_plugin_analysis_helpers.md#cpp_parser_failure_result)

### `TestCreateCppParser`
- def: [`tests/unit/languages/test_cpp_plugin_analysis_helpers.py:52`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_analysis_helpers.py#L52)
- signature: `class TestCreateCppParser:`
- members:
  - `test_constructor_fallback_failure(self, MockParser)` — [`L84`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_analysis_helpers.py#L84)
  - `test_constructor_fallback_success(self, MockParser)` — [`L74`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_analysis_helpers.py#L74)
  - `test_language_attr_path(self, MockParser)` — [`L64`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_analysis_helpers.py#L64)
  - `test_set_language_path(self, MockParser)` — [`L54`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_analysis_helpers.py#L54)
- uses (calls/refs, reference-scoped): [`success`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.success), [`create_cpp_parser`](../../../tree_sitter_analyzer/languages/_cpp_plugin_analysis_helpers.md#create_cpp_parser)

### `TestEmptyCppAnalysisResult`
- def: [`tests/unit/languages/test_cpp_plugin_analysis_helpers.py:17`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_analysis_helpers.py#L17)
- signature: `class TestEmptyCppAnalysisResult:`
- members:
  - `test_empty_content(self)` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_analysis_helpers.py#L32)
  - `test_returns_correct_result(self)` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_analysis_helpers.py#L18)
  - `test_single_line(self)` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_analysis_helpers.py#L28)
- uses (calls/refs, reference-scoped): [`AnalysisResult`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult), [`elements`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.elements), [`language`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.language), [`file_path`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.file_path), [`success`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.success), [`line_count`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.line_count), [`source_code`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.source_code), [`empty_cpp_analysis_result`](../../../tree_sitter_analyzer/languages/_cpp_plugin_analysis_helpers.md#empty_cpp_analysis_result)

### `TestFlattenCppElements`
- def: [`tests/unit/languages/test_cpp_plugin_analysis_helpers.py:115`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_analysis_helpers.py#L115)
- signature: `class TestFlattenCppElements:`
- members:
  - `test_empty_dict(self)` — [`L131`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_analysis_helpers.py#L131)
  - `test_merges_all_keys(self)` — [`L116`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_analysis_helpers.py#L116)
  - `test_missing_keys_default_empty(self)` — [`L127`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_analysis_helpers.py#L127)
- uses (calls/refs, reference-scoped): [`flatten_cpp_elements`](../../../tree_sitter_analyzer/languages/_cpp_plugin_analysis_helpers.md#flatten_cpp_elements)

### `TestLoadCppTreeSitterLanguage`
- def: [`tests/unit/languages/test_cpp_plugin_analysis_helpers.py:94`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_analysis_helpers.py#L94)
- signature: `class TestLoadCppTreeSitterLanguage:`
- members:
  - `test_general_exception_returns_none(self)` — [`L100`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_analysis_helpers.py#L100)
  - `test_import_error_returns_none(self)` — [`L95`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_cpp_plugin_analysis_helpers.py#L95)
- uses (calls/refs, reference-scoped): [`load_cpp_tree_sitter_language`](../../../tree_sitter_analyzer/languages/_cpp_plugin_analysis_helpers.md#load_cpp_tree_sitter_language)

