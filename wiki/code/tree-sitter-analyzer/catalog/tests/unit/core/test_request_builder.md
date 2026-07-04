---
title: 'Module: tests/unit/core/test_request_builder.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_request_builder.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_request_builder`/Test
symbols:
  TestBuildRequestFromParams.test_defaults_with_file_path_only: BuildRequestFromParams#test_defaults_with_file_path_only().
  TestBuildRequestFromParams.test_all_params_explicit: BuildRequestFromParams#test_all_params_explicit().
  TestUpdateRequestFromParams.test_update_boolean_fields: UpdateRequestFromParams#test_update_boolean_fields().
  TestUpdateRequestFromParams.test_no_changes_when_none: UpdateRequestFromParams#test_no_changes_when_none().
  TestUpdateRequestFromParams.test_update_language: UpdateRequestFromParams#test_update_language().
  TestUpdateRequestFromParams.test_update_format_type: UpdateRequestFromParams#test_update_format_type().
  TestUpdateRequestFromParams.test_update_queries: UpdateRequestFromParams#test_update_queries().
  TestUpdateRequestFromParams.test_update_does_not_mutate_file_path: UpdateRequestFromParams#test_update_does_not_mutate_file_path().
  TestUpdateRequestFromParams.test_include_details_false_is_respected: UpdateRequestFromParams#test_include_details_false_is_respected().
  TestBuildRequestFromParams.test_format_type_none_defaults_to_json: BuildRequestFromParams#test_format_type_none_defaults_to_json().
  TestBuildRequestFromParams.test_include_details_none_defaults_to_false: BuildRequestFromParams#test_include_details_none_defaults_to_false().
  TestBuildRequestFromParams.test_include_complexity_none_defaults_to_true: BuildRequestFromParams#test_include_complexity_none_defaults_to_true().
  TestBuildRequestFromParams: BuildRequestFromParams#
  TestUpdateRequestFromParams: UpdateRequestFromParams#
---
# Module: [`tests/unit/core/test_request_builder.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_request_builder.py)

## Classes
### `TestBuildRequestFromParams`
- def: [`tests/unit/core/test_request_builder.py:10`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_request_builder.py#L10)
- signature: `class TestBuildRequestFromParams:`
- members:
  - `test_all_params_explicit(self)` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_request_builder.py#L22)
  - `test_defaults_with_file_path_only(self)` — [`L11`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_request_builder.py#L11)
  - `test_format_type_none_defaults_to_json(self)` — [`L41`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_request_builder.py#L41)
  - `test_include_complexity_none_defaults_to_true(self)` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_request_builder.py#L49)
  - `test_include_details_none_defaults_to_false(self)` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_request_builder.py#L45)
- uses (calls/refs, reference-scoped): [`file_path`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest.file_path), [`language`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest.language), [`include_complexity`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest.include_complexity), [`include_details`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest.include_details), [`build_request_from_params`](../../../tree_sitter_analyzer/core/request_builder.md#build_request_from_params), [`format_type`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest.format_type), [`include_queries`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest.include_queries), [`queries`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest.queries), [`include_elements`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest.include_elements)

### `TestUpdateRequestFromParams`
- def: [`tests/unit/core/test_request_builder.py:54`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_request_builder.py#L54)
- signature: `class TestUpdateRequestFromParams:`
- members:
  - `test_include_details_false_is_respected(self)` — [`L97`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_request_builder.py#L97)
  - `test_no_changes_when_none(self)` — [`L84`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_request_builder.py#L84)
  - `test_update_boolean_fields(self)` — [`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_request_builder.py#L65)
  - `test_update_does_not_mutate_file_path(self)` — [`L92`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_request_builder.py#L92)
  - `test_update_format_type(self)` — [`L60`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_request_builder.py#L60)
  - `test_update_language(self)` — [`L55`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_request_builder.py#L55)
  - `test_update_queries(self)` — [`L79`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_request_builder.py#L79)
- uses (calls/refs, reference-scoped): [`file_path`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest.file_path), [`language`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest.language), [`include_complexity`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest.include_complexity), [`include_details`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest.include_details), [`build_request_from_params`](../../../tree_sitter_analyzer/core/request_builder.md#build_request_from_params), [`format_type`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest.format_type), [`update_request_from_params`](../../../tree_sitter_analyzer/core/request_builder.md#update_request_from_params), [`include_queries`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest.include_queries), [`queries`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest.queries), [`include_elements`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest.include_elements)

