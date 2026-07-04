---
title: 'Module: tests/unit/test_api_result_helpers.py'
type: catalog
provenance: extracted
module: tests/unit/test_api_result_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_api_result_helpers`/
symbols:
  _make_elem: _make_elem().
  _make_analysis_result: _make_analysis_result().
  TestElementToDict.test_sql_parameter_dataclass_is_serialized_to_dict.FakeSQLParameter.direction: TestElementToDict#test_sql_parameter_dataclass_is_serialized_to_dict().FakeSQLParameter#direction.
  TestFileAnalysisResult.test_success_with_elements: TestFileAnalysisResult#test_success_with_elements().
  TestFileAnalysisResult.test_success_without_elements: TestFileAnalysisResult#test_success_without_elements().
  TestLocalFunctionStaysUnowned.test_span_less_sibling_is_skipped: TestLocalFunctionStaysUnowned#test_span_less_sibling_is_skipped().
  TestLocalFunctionStaysUnowned.test_span_less_class_is_skipped_in_find_class_name: TestLocalFunctionStaysUnowned#test_span_less_class_is_skipped_in_find_class_name().
  TestElementToDict.test_basic_fields: TestElementToDict#test_basic_fields().
  TestElementToDict.test_optional_fields_included_when_present: TestElementToDict#test_optional_fields_included_when_present().
  TestElementToDict.test_optional_fields_omitted_when_absent: TestElementToDict#test_optional_fields_omitted_when_absent().
  TestElementToDict.test_method_gets_class_name: TestElementToDict#test_method_gets_class_name().
  TestElementToDict.test_method_without_class_is_none: TestElementToDict#test_method_without_class_is_none().
  TestElementToDict.test_class_type_lowercase: TestElementToDict#test_class_type_lowercase().
  TestElementToDict.test_enum_class_type_surfaces_as_type_enum: TestElementToDict#test_enum_class_type_surfaces_as_type_enum().
  TestElementToDict.test_interface_class_type_surfaces_as_type_interface: TestElementToDict#test_interface_class_type_surfaces_as_type_interface().
  TestElementToDict.test_type_alias_class_type_surfaces_as_type_type: TestElementToDict#test_type_alias_class_type_surfaces_as_type_type().
  TestElementToDict.test_namespace_class_type_surfaces_as_type_namespace: TestElementToDict#test_namespace_class_type_surfaces_as_type_namespace().
  TestElementToDict.test_abstract_class_type_surfaces_as_type_abstract_class: TestElementToDict#test_abstract_class_type_surfaces_as_type_abstract_class().
  TestElementToDict.test_plain_class_with_default_class_type_stays_class: TestElementToDict#test_plain_class_with_default_class_type_stays_class().
  TestElementToDict.test_string_parameters_pass_through_unchanged: TestElementToDict#test_string_parameters_pass_through_unchanged().
  TestFindClassName.test_finds_enclosing_class: TestFindClassName#test_finds_enclosing_class().
  TestFindClassName.test_no_enclosing_class: TestFindClassName#test_no_enclosing_class().
  TestFindClassName.test_method_at_class_boundary_start: TestFindClassName#test_method_at_class_boundary_start().
  TestFindClassName.test_multiple_classes_picks_innermost: TestFindClassName#test_multiple_classes_picks_innermost().
  TestFindClassName.test_nested_container_innermost_wins: TestFindClassName#test_nested_container_innermost_wins().
  TestFindClassName.test_nested_namespace_innermost_wins: TestFindClassName#test_nested_namespace_innermost_wins().
  TestFindClassName.test_java_method_in_inner_class_gets_class_name: TestFindClassName#test_java_method_in_inner_class_gets_class_name().
  TestFileAnalysisResult.test_success_with_query_results: TestFileAnalysisResult#test_success_with_query_results().
  TestFileAnalysisResult.test_failed_analysis_with_error: TestFileAnalysisResult#test_failed_analysis_with_error().
  TestFileAnalysisResult.test_failed_analysis_without_error_message: TestFileAnalysisResult#test_failed_analysis_without_error_message().
  TestFileAnalysisResult.test_auto_detected_language: TestFileAnalysisResult#test_auto_detected_language().
  TestCodeAnalysisResult.test_success_response: TestCodeAnalysisResult#test_success_response().
  TestCodeAnalysisResult.test_failed_analysis: TestCodeAnalysisResult#test_failed_analysis().
  TestLocalFunctionStaysUnowned.test_local_function_gets_no_class_name: TestLocalFunctionStaysUnowned#test_local_function_gets_no_class_name().
  TestFileAnalysisError.test_basic_error: TestFileAnalysisError#test_basic_error().
  TestFileAnalysisError.test_none_language: TestFileAnalysisError#test_none_language().
  TestCodeAnalysisError.test_basic_error: TestCodeAnalysisError#test_basic_error().
  TestCodeAnalysisError.test_empty_language: TestCodeAnalysisError#test_empty_language().
  TestElementToDict.test_sql_parameter_dataclass_is_serialized_to_dict.FakeSQLParameter: TestElementToDict#test_sql_parameter_dataclass_is_serialized_to_dict().FakeSQLParameter#
  TestLocalFunctionStaysUnowned.test_span_less_sibling_is_skipped.Bare: TestLocalFunctionStaysUnowned#test_span_less_sibling_is_skipped().Bare#
  TestLocalFunctionStaysUnowned.test_span_less_class_is_skipped_in_find_class_name.BareClass: TestLocalFunctionStaysUnowned#test_span_less_class_is_skipped_in_find_class_name().BareClass#
  TestElementToDict: TestElementToDict#
  TestElementToDict.test_sql_parameter_dataclass_is_serialized_to_dict: TestElementToDict#test_sql_parameter_dataclass_is_serialized_to_dict().
  TestElementToDict.test_sql_parameter_dataclass_is_serialized_to_dict.FakeSQLParameter.name: TestElementToDict#test_sql_parameter_dataclass_is_serialized_to_dict().FakeSQLParameter#name.
  TestElementToDict.test_sql_parameter_dataclass_is_serialized_to_dict.FakeSQLParameter.data_type: TestElementToDict#test_sql_parameter_dataclass_is_serialized_to_dict().FakeSQLParameter#data_type.
  TestFindClassName: TestFindClassName#
  TestFileAnalysisResult: TestFileAnalysisResult#
  TestCodeAnalysisResult: TestCodeAnalysisResult#
  TestFileAnalysisError: TestFileAnalysisError#
  TestCodeAnalysisError: TestCodeAnalysisError#
  TestLocalFunctionStaysUnowned: TestLocalFunctionStaysUnowned#
---
# Module: [`tests/unit/test_api_result_helpers.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_result_helpers.py)

## Classes
### `Bare`
- def: [`tests/unit/test_api_result_helpers.py:373`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_result_helpers.py#L373)
- signature: `class Bare:`
- used by: (1 test-only callers)

### `BareClass`
- def: [`tests/unit/test_api_result_helpers.py:386`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_result_helpers.py#L386)
- signature: `class BareClass:`
- used by: (1 test-only callers)

### `FakeSQLParameter`
- def: [`tests/unit/test_api_result_helpers.py:153`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_result_helpers.py#L153)
- signature: `class FakeSQLParameter:`
- members:
  - `data_type` — [`L155`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_result_helpers.py#L155)
  - `direction` — [`L156`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_result_helpers.py#L156)
  - `name` — [`L154`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_result_helpers.py#L154)
- uses (calls/refs, reference-scoped): [`element_to_dict`](../../tree_sitter_analyzer/_api_result_helpers.md#element_to_dict)  (1 test-only)

### `TestCodeAnalysisError`
- def: [`tests/unit/test_api_result_helpers.py:341`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_result_helpers.py#L341)
- doc: Tests for code_analysis_error.
- signature: `class TestCodeAnalysisError:`
- members:
  - `test_basic_error(self)` — [`L344`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_result_helpers.py#L344)
  - `test_empty_language(self)` — [`L350`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_result_helpers.py#L350)
- uses (calls/refs, reference-scoped): [`code_analysis_error`](../../tree_sitter_analyzer/_api_result_helpers.md#code_analysis_error)

### `TestCodeAnalysisResult`
- def: [`tests/unit/test_api_result_helpers.py:304`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_result_helpers.py#L304)
- doc: Tests for code_analysis_result.
- signature: `class TestCodeAnalysisResult:`
- members:
  - `test_failed_analysis(self)` — [`L316`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_result_helpers.py#L316)
  - `test_success_response(self)` — [`L307`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_result_helpers.py#L307)
- uses (calls/refs, reference-scoped): [`code_analysis_result`](../../tree_sitter_analyzer/_api_result_helpers.md#code_analysis_result)  (1 test-only)

### `TestElementToDict`
- def: [`tests/unit/test_api_result_helpers.py:65`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_result_helpers.py#L65)
- doc: Tests for element_to_dict.
- signature: `class TestElementToDict:`
- members:
  - `test_abstract_class_type_surfaces_as_type_abstract_class(self)` — [`L131`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_result_helpers.py#L131) — #795: Class element with class_type='abstract_class' must output type='abstract_class'.
  - `test_basic_fields(self)` — [`L68`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_result_helpers.py#L68)
  - `test_class_type_lowercase(self)` — [`L102`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_result_helpers.py#L102)
  - `test_enum_class_type_surfaces_as_type_enum(self)` — [`L107`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_result_helpers.py#L107) — #795: Class element with class_type='enum' must output type='enum', not 'class'.
  - `test_interface_class_type_surfaces_as_type_interface(self)` — [`L113`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_result_helpers.py#L113) — #795: Class element with class_type='interface' must output type='interface'.
  - `test_method_gets_class_name(self)` — [`L89`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_result_helpers.py#L89)
  - `test_method_without_class_is_none(self)` — [`L97`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_result_helpers.py#L97)
  - `test_namespace_class_type_surfaces_as_type_namespace(self)` — [`L125`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_result_helpers.py#L125) — #795: Class element with class_type='namespace' must output type='namespace'.
  - `test_optional_fields_included_when_present(self)` — [`L77`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_result_helpers.py#L77)
  - `test_optional_fields_omitted_when_absent(self)` — [`L83`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_result_helpers.py#L83)
  - `test_plain_class_with_default_class_type_stays_class(self)` — [`L137`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_result_helpers.py#L137) — #795: Class element with class_type='class' (default) must still output type='class'.
  - `test_sql_parameter_dataclass_is_serialized_to_dict(self)` — [`L143`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_result_helpers.py#L143) — SQLParameter dataclass instances in parameters[] must become plain dicts.
  - `test_string_parameters_pass_through_unchanged(self)` — [`L173`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_result_helpers.py#L173) — String parameters (non-dataclass) are not modified.
  - `test_type_alias_class_type_surfaces_as_type_type(self)` — [`L119`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_result_helpers.py#L119) — #795: Class element with class_type='type' must output type='type'.
- uses (calls/refs, reference-scoped): [`element_to_dict`](../../tree_sitter_analyzer/_api_result_helpers.md#element_to_dict)  (1 test-only)

### `TestFileAnalysisError`
- def: [`tests/unit/test_api_result_helpers.py:324`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_result_helpers.py#L324)
- doc: Tests for file_analysis_error.
- signature: `class TestFileAnalysisError:`
- members:
  - `test_basic_error(self)` — [`L327`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_result_helpers.py#L327)
  - `test_none_language(self)` — [`L336`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_result_helpers.py#L336)
- uses (calls/refs, reference-scoped): [`file_analysis_error`](../../tree_sitter_analyzer/_api_result_helpers.md#file_analysis_error)

### `TestFileAnalysisResult`
- def: [`tests/unit/test_api_result_helpers.py:249`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_result_helpers.py#L249)
- doc: Tests for file_analysis_result.
- signature: `class TestFileAnalysisResult:`
- members:
  - `test_auto_detected_language(self)` — [`L296`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_result_helpers.py#L296)
  - `test_failed_analysis_with_error(self)` — [`L278`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_result_helpers.py#L278)
  - `test_failed_analysis_without_error_message(self)` — [`L287`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_result_helpers.py#L287)
  - `test_success_with_elements(self)` — [`L252`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_result_helpers.py#L252)
  - `test_success_with_query_results(self)` — [`L271`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_result_helpers.py#L271)
  - `test_success_without_elements(self)` — [`L263`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_result_helpers.py#L263)
- uses (calls/refs, reference-scoped): [`file_analysis_result`](../../tree_sitter_analyzer/_api_result_helpers.md#file_analysis_result)  (2 test-only)

### `TestFindClassName`
- def: [`tests/unit/test_api_result_helpers.py:180`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_result_helpers.py#L180)
- doc: Tests for find_class_name.
- signature: `class TestFindClassName:`
- members:
  - `test_finds_enclosing_class(self)` — [`L183`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_result_helpers.py#L183)
  - `test_java_method_in_inner_class_gets_class_name(self)` — [`L233`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_result_helpers.py#L233) — element_to_dict sets class_name for a function inside a nested class
  - `test_method_at_class_boundary_start(self)` — [`L193`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_result_helpers.py#L193)
  - `test_multiple_classes_picks_innermost(self)` — [`L198`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_result_helpers.py#L198) — When method is inside two classes, the innermost (smallest span) wins.
  - `test_nested_container_innermost_wins(self)` — [`L208`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_result_helpers.py#L208) — Method inside nested class → innermost (smallest span) class wins.
  - `test_nested_namespace_innermost_wins(self)` — [`L218`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_result_helpers.py#L218) — TS namespace wrapping a class: method inside class → class, not namespace.
  - `test_no_enclosing_class(self)` — [`L188`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_result_helpers.py#L188)
- uses (calls/refs, reference-scoped): [`element_to_dict`](../../tree_sitter_analyzer/_api_result_helpers.md#element_to_dict), [`find_class_name`](../../tree_sitter_analyzer/_api_result_helpers.md#find_class_name)  (1 test-only)

### `TestLocalFunctionStaysUnowned`
- def: [`tests/unit/test_api_result_helpers.py:355`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_result_helpers.py#L355)
- doc: Codex P2 on #570: a function nested inside another FUNCTION's span
- signature: `class TestLocalFunctionStaysUnowned:`
- members:
  - `test_local_function_gets_no_class_name(self)` — [`L360`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_result_helpers.py#L360)
  - `test_span_less_class_is_skipped_in_find_class_name(self)` — [`L383`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_result_helpers.py#L383) — A class-like element without line attrs (guard line) is skipped.
  - `test_span_less_sibling_is_skipped(self)` — [`L370`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_result_helpers.py#L370) — Elements without line attrs (line 70 guard) don't break containment.
- uses (calls/refs, reference-scoped): [`element_to_dict`](../../tree_sitter_analyzer/_api_result_helpers.md#element_to_dict), [`find_class_name`](../../tree_sitter_analyzer/_api_result_helpers.md#find_class_name)  (3 test-only)

## Functions
- `_make_analysis_result(success=True, language="python", node_count=10, line_count=5, error_message=None, elements=None, query_results=None)` — [`L44`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_result_helpers.py#L44) — Create a mock analysis result.
- `_make_elem(name="foo", cls_name="Function", start_line=1, end_line=5, raw_text="def foo(): pass", language="python", **extra)` — [`L15`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_result_helpers.py#L15) — Create a real (non-Mock) element.

