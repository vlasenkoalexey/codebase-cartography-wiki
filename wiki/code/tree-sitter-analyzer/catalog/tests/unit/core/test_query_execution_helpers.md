---
title: 'Module: tests/unit/core/test_query_execution_helpers.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_query_execution_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_query_execution_helpers`/
symbols:
  _make_executor: _make_executor().
  _safe_query: _safe_query().
  TestExecuteQueryByName.test_none_tree: TestExecuteQueryByName#test_none_tree().
  TestExecuteQueryByName.test_query_not_found: TestExecuteQueryByName#test_query_not_found().
  TestExecuteQueryByName.test_success: TestExecuteQueryByName#test_success().
  TestExecuteQueryByName.test_exception_increments_failed: TestExecuteQueryByName#test_exception_increments_failed().
  TestExecuteQueryByExplicitLanguage.test_none_tree: TestExecuteQueryByExplicitLanguage#test_none_tree().
  TestExecuteQueryByExplicitLanguage.test_empty_language_name_becomes_unknown: TestExecuteQueryByExplicitLanguage#test_empty_language_name_becomes_unknown().
  TestExecuteQueryByExplicitLanguage.test_success: TestExecuteQueryByExplicitLanguage#test_success().
  TestExecuteQueryByExplicitLanguage.test_whitespace_language_name_stripped: TestExecuteQueryByExplicitLanguage#test_whitespace_language_name_stripped().
  TestExecuteRawQueryString.test_none_tree: TestExecuteRawQueryString#test_none_tree().
  TestExecuteRawQueryString.test_success: TestExecuteRawQueryString#test_success().
  TestExecuteRawQueryString.test_exception: TestExecuteRawQueryString#test_exception().
  TestInputError.test_none_tree_returns_error: TestInputError#test_none_tree_returns_error().
  TestInputError.test_none_language_returns_error: TestInputError#test_none_language_returns_error().
  TestInputError.test_both_valid_returns_none: TestInputError#test_both_valid_returns_none().
  TestInputError.test_without_query_name: TestInputError#test_without_query_name().
  TestLanguageNameFromObject.test_fallback_class_name: TestLanguageNameFromObject#test_fallback_class_name().
  TestExecuteQueryStringInternal.test_captures_processed: TestExecuteQueryStringInternal#test_captures_processed().
  TestExecuteQueryStringInternal.test_process_captures_returns_error_dict: TestExecuteQueryStringInternal#test_process_captures_returns_error_dict().
  TestExecuteQueryStringInternal.test_exception_during_query: TestExecuteQueryStringInternal#test_exception_during_query().
  TestExecuteQueryStringInternal.test_exception_without_query_name: TestExecuteQueryStringInternal#test_exception_without_query_name().
  TestProcessCapturesOrError.test_success: TestProcessCapturesOrError#test_success().
  TestProcessCapturesOrError.test_exception: TestProcessCapturesOrError#test_exception().
  TestProcessCapturesOrError.test_exception_no_query_name: TestProcessCapturesOrError#test_exception_no_query_name().
  TestLanguageNameFromObject.test_name_attribute: TestLanguageNameFromObject#test_name_attribute().
  TestLanguageNameFromObject.test_private_name_attribute: TestLanguageNameFromObject#test_private_name_attribute().
  TestLanguageNameFromObject.test_unknown_when_no_name: TestLanguageNameFromObject#test_unknown_when_no_name().
  TestLanguageNameFromObject.test_unknown_when_none_string: TestLanguageNameFromObject#test_unknown_when_none_string().
  TestSuccessResult.test_basic: TestSuccessResult#test_basic().
  TestSuccessResult.test_with_query_string_field: TestSuccessResult#test_with_query_string_field().
  TestSuccessResult.test_no_optional_fields: TestSuccessResult#test_no_optional_fields().
  TestUnpackCapture.test_tuple: TestUnpackCapture#test_tuple().
  TestUnpackCapture.test_dict: TestUnpackCapture#test_dict().
  TestUnpackCapture.test_invalid_returns_none: TestUnpackCapture#test_invalid_returns_none().
  TestProcessCapturesResults.test_empty: TestProcessCapturesResults#test_empty().
  TestProcessCapturesResults.test_tuple_captures: TestProcessCapturesResults#test_tuple_captures().
  TestProcessCapturesResults.test_dict_captures: TestProcessCapturesResults#test_dict_captures().
  TestProcessCapturesResults.test_none_node_skipped: TestProcessCapturesResults#test_none_node_skipped().
  TestProcessCapturesResults.test_bad_capture_format_skipped: TestProcessCapturesResults#test_bad_capture_format_skipped().
  TestCreateResultDictResults.test_normal: TestCreateResultDictResults#test_normal().
  TestCreateResultDictResults.test_exception_in_text: TestCreateResultDictResults#test_exception_in_text().
  TestCreateErrorResultResults.test_basic: TestCreateErrorResultResults#test_basic().
  TestCreateErrorResultResults.test_with_query_name: TestCreateErrorResultResults#test_with_query_name().
  TestCreateErrorResultResults.test_extra_kwargs: TestCreateErrorResultResults#test_extra_kwargs().
  TestQueryStatisticsResults.test_empty: TestQueryStatisticsResults#test_empty().
  TestQueryStatisticsResults.test_with_data: TestQueryStatisticsResults#test_with_data().
  TestQueryStatisticsResults.test_does_not_mutate_input: TestQueryStatisticsResults#test_does_not_mutate_input().
  TestLanguageNameFromObject.test_fallback_class_name._Language: TestLanguageNameFromObject#test_fallback_class_name()._Language#
  TestInputError: TestInputError#
  TestLanguageNameFromObject: TestLanguageNameFromObject#
  TestSuccessResult: TestSuccessResult#
  TestExecuteQueryByName: TestExecuteQueryByName#
  TestExecuteQueryByExplicitLanguage: TestExecuteQueryByExplicitLanguage#
  TestExecuteRawQueryString: TestExecuteRawQueryString#
  TestExecuteQueryStringInternal: TestExecuteQueryStringInternal#
  TestProcessCapturesOrError: TestProcessCapturesOrError#
  TestUnpackCapture: TestUnpackCapture#
  TestProcessCapturesResults: TestProcessCapturesResults#
  TestCreateResultDictResults: TestCreateResultDictResults#
  TestCreateErrorResultResults: TestCreateErrorResultResults#
  TestQueryStatisticsResults: TestQueryStatisticsResults#
---
# Module: [`tests/unit/core/test_query_execution_helpers.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_execution_helpers.py)

## Classes
### `TestCreateErrorResultResults`
- def: [`tests/unit/core/test_query_execution_helpers.py:384`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_execution_helpers.py#L384)
- signature: `class TestCreateErrorResultResults:`
- members:
  - `test_basic(self)` — [`L385`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_execution_helpers.py#L385)
  - `test_extra_kwargs(self)` — [`L396`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_execution_helpers.py#L396)
  - `test_with_query_name(self)` — [`L392`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_execution_helpers.py#L392)
- uses (calls/refs, reference-scoped): [`create_error_result`](../../../tree_sitter_analyzer/core/_query_results.md#create_error_result)

### `TestCreateResultDictResults`
- def: [`tests/unit/core/test_query_execution_helpers.py:359`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_execution_helpers.py#L359)
- signature: `class TestCreateResultDictResults:`
- members:
  - `test_exception_in_text(self)` — [`L374`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_execution_helpers.py#L374)
  - `test_normal(self)` — [`L360`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_execution_helpers.py#L360)
- uses (calls/refs, reference-scoped): [`create_result_dict`](../../../tree_sitter_analyzer/core/_query_results.md#create_result_dict)

### `TestExecuteQueryByExplicitLanguage`
- def: [`tests/unit/core/test_query_execution_helpers.py:171`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_execution_helpers.py#L171)
- signature: `class TestExecuteQueryByExplicitLanguage:`
- members:
  - `test_empty_language_name_becomes_unknown(self)` — [`L179`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_execution_helpers.py#L179)
  - `test_none_tree(self)` — [`L172`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_execution_helpers.py#L172)
  - `test_success(self)` — [`L187`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_execution_helpers.py#L187)
  - `test_whitespace_language_name_stripped(self)` — [`L203`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_execution_helpers.py#L203)
- uses (calls/refs, reference-scoped): [`execute_query_by_explicit_language`](../../../tree_sitter_analyzer/core/_query_execution.md#execute_query_by_explicit_language)  (2 test-only)

### `TestExecuteQueryByName`
- def: [`tests/unit/core/test_query_execution_helpers.py:126`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_execution_helpers.py#L126)
- signature: `class TestExecuteQueryByName:`
- members:
  - `test_exception_increments_failed(self)` — [`L159`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_execution_helpers.py#L159)
  - `test_none_tree(self)` — [`L127`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_execution_helpers.py#L127)
  - `test_query_not_found(self)` — [`L135`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_execution_helpers.py#L135)
  - `test_success(self)` — [`L146`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_execution_helpers.py#L146)
- uses (calls/refs, reference-scoped): [`execute_query_by_name`](../../../tree_sitter_analyzer/core/_query_execution.md#execute_query_by_name)  (2 test-only)

### `TestExecuteQueryStringInternal`
- def: [`tests/unit/core/test_query_execution_helpers.py:244`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_execution_helpers.py#L244)
- signature: `class TestExecuteQueryStringInternal:`
- members:
  - `test_captures_processed(self)` — [`L245`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_execution_helpers.py#L245)
  - `test_exception_during_query(self)` — [`L264`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_execution_helpers.py#L264)
  - `test_exception_without_query_name(self)` — [`L280`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_execution_helpers.py#L280)
  - `test_process_captures_returns_error_dict(self)` — [`L255`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_execution_helpers.py#L255)
- uses (calls/refs, reference-scoped): [`_execute_query_string`](../../../tree_sitter_analyzer/core/_query_execution.md#_execute_query_string)  (1 test-only)

### `TestExecuteRawQueryString`
- def: [`tests/unit/core/test_query_execution_helpers.py:213`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_execution_helpers.py#L213)
- signature: `class TestExecuteRawQueryString:`
- members:
  - `test_exception(self)` — [`L235`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_execution_helpers.py#L235)
  - `test_none_tree(self)` — [`L214`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_execution_helpers.py#L214)
  - `test_success(self)` — [`L221`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_execution_helpers.py#L221)
- uses (calls/refs, reference-scoped): [`execute_raw_query_string`](../../../tree_sitter_analyzer/core/_query_execution.md#execute_raw_query_string)  (2 test-only)

### `TestInputError`
- def: [`tests/unit/core/test_query_execution_helpers.py:51`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_execution_helpers.py#L51)
- signature: `class TestInputError:`
- members:
  - `test_both_valid_returns_none(self)` — [`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_execution_helpers.py#L65)
  - `test_none_language_returns_error(self)` — [`L59`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_execution_helpers.py#L59)
  - `test_none_tree_returns_error(self)` — [`L52`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_execution_helpers.py#L52)
  - `test_without_query_name(self)` — [`L69`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_execution_helpers.py#L69)
- uses (calls/refs, reference-scoped): [`_input_error`](../../../tree_sitter_analyzer/core/_query_execution.md#_input_error)  (1 test-only)

### `TestLanguageNameFromObject`
- def: [`tests/unit/core/test_query_execution_helpers.py:76`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_execution_helpers.py#L76)
- signature: `class TestLanguageNameFromObject:`
- members:
  - `test_fallback_class_name(self)` — [`L87`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_execution_helpers.py#L87)
  - `test_name_attribute(self)` — [`L77`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_execution_helpers.py#L77)
  - `test_private_name_attribute(self)` — [`L82`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_execution_helpers.py#L82)
  - `test_unknown_when_no_name(self)` — [`L95`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_execution_helpers.py#L95)
  - `test_unknown_when_none_string(self)` — [`L100`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_execution_helpers.py#L100)
- uses (calls/refs, reference-scoped): [`_language_name_from_object`](../../../tree_sitter_analyzer/core/_query_execution.md#_language_name_from_object)  (1 test-only)

### `TestProcessCapturesOrError`
- def: [`tests/unit/core/test_query_execution_helpers.py:290`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_execution_helpers.py#L290)
- signature: `class TestProcessCapturesOrError:`
- members:
  - `test_exception(self)` — [`L297`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_execution_helpers.py#L297)
  - `test_exception_no_query_name(self)` — [`L304`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_execution_helpers.py#L304)
  - `test_success(self)` — [`L291`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_execution_helpers.py#L291)
- uses (calls/refs, reference-scoped): [`_process_captures_or_error`](../../../tree_sitter_analyzer/core/_query_execution.md#_process_captures_or_error)  (1 test-only)

### `TestProcessCapturesResults`
- def: [`tests/unit/core/test_query_execution_helpers.py:328`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_execution_helpers.py#L328)
- signature: `class TestProcessCapturesResults:`
- members:
  - `test_bad_capture_format_skipped(self)` — [`L354`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_execution_helpers.py#L354)
  - `test_dict_captures(self)` — [`L343`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_execution_helpers.py#L343)
  - `test_empty(self)` — [`L329`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_execution_helpers.py#L329)
  - `test_none_node_skipped(self)` — [`L350`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_execution_helpers.py#L350)
  - `test_tuple_captures(self)` — [`L332`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_execution_helpers.py#L332)
- uses (calls/refs, reference-scoped): [`process_captures`](../../../tree_sitter_analyzer/core/_query_results.md#process_captures)

### `TestQueryStatisticsResults`
- def: [`tests/unit/core/test_query_execution_helpers.py:401`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_execution_helpers.py#L401)
- signature: `class TestQueryStatisticsResults:`
- members:
  - `test_does_not_mutate_input(self)` — [`L426`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_execution_helpers.py#L426)
  - `test_empty(self)` — [`L402`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_execution_helpers.py#L402)
  - `test_with_data(self)` — [`L414`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_execution_helpers.py#L414)
- uses (calls/refs, reference-scoped): [`query_statistics`](../../../tree_sitter_analyzer/core/_query_results.md#query_statistics)

### `TestSuccessResult`
- def: [`tests/unit/core/test_query_execution_helpers.py:107`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_execution_helpers.py#L107)
- signature: `class TestSuccessResult:`
- members:
  - `test_basic(self)` — [`L108`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_execution_helpers.py#L108)
  - `test_no_optional_fields(self)` — [`L120`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_execution_helpers.py#L120)
  - `test_with_query_string_field(self)` — [`L116`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_execution_helpers.py#L116)
- uses (calls/refs, reference-scoped): [`_success_result`](../../../tree_sitter_analyzer/core/_query_execution.md#_success_result)

### `TestUnpackCapture`
- def: [`tests/unit/core/test_query_execution_helpers.py:312`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_execution_helpers.py#L312)
- signature: `class TestUnpackCapture:`
- members:
  - `test_dict(self)` — [`L317`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_execution_helpers.py#L317)
  - `test_invalid_returns_none(self)` — [`L321`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_execution_helpers.py#L321)
  - `test_tuple(self)` — [`L313`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_execution_helpers.py#L313)
- uses (calls/refs, reference-scoped): [`_unpack_capture`](../../../tree_sitter_analyzer/core/_query_results.md#_unpack_capture)

### `_Language`
- def: [`tests/unit/core/test_query_execution_helpers.py:88`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_execution_helpers.py#L88)
- signature: `class _Language:`
- used by: (1 test-only callers)

## Functions
- `_make_executor(**overrides)` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_execution_helpers.py#L28)
- `_safe_query(*args, **kwargs)` — [`L47`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_execution_helpers.py#L47)

