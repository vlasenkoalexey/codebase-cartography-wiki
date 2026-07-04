---
title: 'Module: tests/unit/mcp/test_utils/test_format_helper.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_utils/test_format_helper.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_utils.test_format_helper`/Test
symbols:
  TestIntegration.test_format_workflow_json: Integration#test_format_workflow_json().
  TestIntegration.test_format_workflow_toon: Integration#test_format_workflow_toon().
  TestGetFormatter.test_get_formatter_json: GetFormatter#test_get_formatter_json().
  TestGetFormatter.test_get_formatter_default: GetFormatter#test_get_formatter_default().
  TestGetFormatter.test_get_formatter_toon_import_error: GetFormatter#test_get_formatter_toon_import_error().
  TestJsonFormatter.test_json_formatter_format: JsonFormatter#test_json_formatter_format().
  TestJsonFormatter.test_json_formatter_format_nested: JsonFormatter#test_json_formatter_format_nested().
  TestJsonFormatter.test_json_formatter_format_list: JsonFormatter#test_json_formatter_format_list().
  TestIntegration.test_attach_vs_apply_toon_difference: Integration#test_attach_vs_apply_toon_difference().
  TestFormatOutput.test_format_output_json: FormatOutput#test_format_output_json().
  TestFormatOutput.test_format_output_toon: FormatOutput#test_format_output_toon().
  TestFormatOutput.test_format_output_default_format: FormatOutput#test_format_output_default_format().
  TestFormatOutput.test_format_output_empty_dict: FormatOutput#test_format_output_empty_dict().
  TestFormatOutput.test_format_output_nested_dict: FormatOutput#test_format_output_nested_dict().
  TestFormatAsJson.test_format_as_json_simple: FormatAsJson#test_format_as_json_simple().
  TestFormatAsJson.test_format_as_json_with_numbers: FormatAsJson#test_format_as_json_with_numbers().
  TestFormatAsJson.test_format_as_json_with_lists: FormatAsJson#test_format_as_json_with_lists().
  TestFormatAsJson.test_format_as_json_with_unicode: FormatAsJson#test_format_as_json_with_unicode().
  TestFormatAsJson.test_format_as_json_with_special_chars: FormatAsJson#test_format_as_json_with_special_chars().
  TestFormatAsToon.test_format_as_toon_success: FormatAsToon#test_format_as_toon_success().
  TestFormatAsToon.test_format_as_toon_import_error_fallback: FormatAsToon#test_format_as_toon_import_error_fallback().
  TestFormatAsToon.test_format_as_toon_exception_fallback: FormatAsToon#test_format_as_toon_exception_fallback().
  TestGetFormatter.test_get_formatter_toon: GetFormatter#test_get_formatter_toon().
  TestApplyOutputFormat.test_apply_output_format_return_dict: ApplyOutputFormat#test_apply_output_format_return_dict().
  TestApplyOutputFormat.test_apply_output_format_return_string_json: ApplyOutputFormat#test_apply_output_format_return_string_json().
  TestApplyOutputFormat.test_apply_output_format_return_string_toon: ApplyOutputFormat#test_apply_output_format_return_string_toon().
  TestApplyOutputFormat.test_apply_output_format_default_params: ApplyOutputFormat#test_apply_output_format_default_params().
  TestFormatForFileOutput.test_format_for_file_output_json: FormatForFileOutput#test_format_for_file_output_json().
  TestFormatForFileOutput.test_format_for_file_output_toon: FormatForFileOutput#test_format_for_file_output_toon().
  TestFormatForFileOutput.test_format_for_file_output_default_format: FormatForFileOutput#test_format_for_file_output_default_format().
  TestApplyToonFormatToResponse.test_apply_toon_format_json_unchanged: ApplyToonFormatToResponse#test_apply_toon_format_json_unchanged().
  TestApplyToonFormatToResponse.test_apply_toon_format_toon_with_results: ApplyToonFormatToResponse#test_apply_toon_format_toon_with_results().
  TestApplyToonFormatToResponse.test_apply_toon_format_toon_with_matches: ApplyToonFormatToResponse#test_apply_toon_format_toon_with_matches().
  TestApplyToonFormatToResponse.test_apply_toon_format_toon_with_content: ApplyToonFormatToResponse#test_apply_toon_format_toon_with_content().
  TestApplyToonFormatToResponse.test_apply_toon_format_toon_with_multiple_redundant_fields: ApplyToonFormatToResponse#test_apply_toon_format_toon_with_multiple_redundant_fields().
  TestApplyToonFormatToResponse.test_apply_toon_format_toon_no_field_duplication: ApplyToonFormatToResponse#test_apply_toon_format_toon_no_field_duplication().
  TestApplyToonFormatToResponse.test_apply_toon_format_exception_fallback: ApplyToonFormatToResponse#test_apply_toon_format_exception_fallback().
  TestAttachToonContentToResponse.test_attach_toon_content_success: AttachToonContentToResponse#test_attach_toon_content_success().
  TestAttachToonContentToResponse.test_attach_toon_content_preserves_original: AttachToonContentToResponse#test_attach_toon_content_preserves_original().
  TestAttachToonContentToResponse.test_attach_toon_content_does_not_modify_original: AttachToonContentToResponse#test_attach_toon_content_does_not_modify_original().
  TestAttachToonContentToResponse.test_attach_toon_content_exception_fallback: AttachToonContentToResponse#test_attach_toon_content_exception_fallback().
  TestIntegration.test_get_formatter_and_format: Integration#test_get_formatter_and_format().
  TestFormatOutput: FormatOutput#
  TestFormatAsJson: FormatAsJson#
  TestFormatAsToon: FormatAsToon#
  TestGetFormatter: GetFormatter#
  TestJsonFormatter: JsonFormatter#
  TestApplyOutputFormat: ApplyOutputFormat#
  TestFormatForFileOutput: FormatForFileOutput#
  TestApplyToonFormatToResponse: ApplyToonFormatToResponse#
  TestAttachToonContentToResponse: AttachToonContentToResponse#
  TestIntegration: Integration#
---
# Module: [`tests/unit/mcp/test_utils/test_format_helper.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_format_helper.py)

## Classes
### `TestApplyOutputFormat`
- def: [`tests/unit/mcp/test_utils/test_format_helper.py:203`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_format_helper.py#L203)
- doc: Tests for apply_output_format function.
- signature: `class TestApplyOutputFormat:`
- members:
  - `test_apply_output_format_default_params(self)` — [`L226`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_format_helper.py#L226) — Test apply_output_format with default parameters.
  - `test_apply_output_format_return_dict(self)` — [`L206`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_format_helper.py#L206) — Test apply_output_format returns dict when return_formatted_string=False.
  - `test_apply_output_format_return_string_json(self)` — [`L213`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_format_helper.py#L213) — Test apply_output_format returns JSON string when requested.
  - `test_apply_output_format_return_string_toon(self)` — [`L220`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_format_helper.py#L220) — Test apply_output_format returns TOON string when requested.
- uses (calls/refs, reference-scoped): [`apply_output_format`](../../../../tree_sitter_analyzer/mcp/utils/format_helper.md#apply_output_format)

### `TestApplyToonFormatToResponse`
- def: [`tests/unit/mcp/test_utils/test_format_helper.py:261`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_format_helper.py#L261)
- doc: Tests for apply_toon_format_to_response function.
- signature: `class TestApplyToonFormatToResponse:`
- members:
  - `test_apply_toon_format_exception_fallback(self, mock_format_as_toon)` — [`L376`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_format_helper.py#L376) — Test apply_toon_format_to_response falls back on exception.
  - `test_apply_toon_format_json_unchanged(self)` — [`L264`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_format_helper.py#L264) — Test apply_toon_format_to_response returns original for JSON format.
  - `test_apply_toon_format_toon_no_field_duplication(self)` — [`L348`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_format_helper.py#L348) — Bulk-data field (``results``) is stripped; all other small
  - `test_apply_toon_format_toon_with_content(self)` — [`L301`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_format_helper.py#L301) — ``content`` is bulk data and is removed; ``file_path`` stays as metadata.
  - `test_apply_toon_format_toon_with_matches(self)` — [`L289`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_format_helper.py#L289) — ``matches`` is bulk data and is removed; ``query`` is metadata and stays.
  - `test_apply_toon_format_toon_with_multiple_redundant_fields(self)` — [`L313`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_format_helper.py#L313) — RFC-0012 Phase 2: all bulk list/dict fields and large-string fields
  - `test_apply_toon_format_toon_with_results(self)` — [`L271`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_format_helper.py#L271) — Redundant ``results`` payload is dropped; RFC-0012 Phase 2 also strips
- uses (calls/refs, reference-scoped): [`apply_toon_format_to_response`](../../../../tree_sitter_analyzer/mcp/utils/format_helper.md#apply_toon_format_to_response)

### `TestAttachToonContentToResponse`
- def: [`tests/unit/mcp/test_utils/test_format_helper.py:384`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_format_helper.py#L384)
- doc: Tests for attach_toon_content_to_response function.
- signature: `class TestAttachToonContentToResponse:`
- members:
  - `test_attach_toon_content_does_not_modify_original(self)` — [`L426`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_format_helper.py#L426) — Test attach_toon_content_to_response does not modify original dict.
  - `test_attach_toon_content_exception_fallback(self, mock_format_as_toon)` — [`L438`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_format_helper.py#L438) — Test attach_toon_content_to_response falls back on exception.
  - `test_attach_toon_content_preserves_original(self)` — [`L400`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_format_helper.py#L400) — Test attach_toon_content_to_response preserves all original fields.
  - `test_attach_toon_content_success(self)` — [`L387`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_format_helper.py#L387) — Test attach_toon_content_to_response adds TOON content.
- uses (calls/refs, reference-scoped): [`attach_toon_content_to_response`](../../../../tree_sitter_analyzer/mcp/utils/format_helper.md#attach_toon_content_to_response)

### `TestFormatAsJson`
- def: [`tests/unit/mcp/test_utils/test_format_helper.py:62`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_format_helper.py#L62)
- doc: Tests for format_as_json function.
- signature: `class TestFormatAsJson:`
- members:
  - `test_format_as_json_simple(self)` — [`L65`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_format_helper.py#L65) — Test format_as_json with simple dictionary.
  - `test_format_as_json_with_lists(self)` — [`L78`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_format_helper.py#L78) — Test format_as_json with lists.
  - `test_format_as_json_with_numbers(self)` — [`L71`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_format_helper.py#L71) — Test format_as_json with numbers.
  - `test_format_as_json_with_special_chars(self)` — [`L93`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_format_helper.py#L93) — Test format_as_json with special characters.
  - `test_format_as_json_with_unicode(self)` — [`L87`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_format_helper.py#L87) — Test format_as_json with Unicode characters.
- uses (calls/refs, reference-scoped): [`format_as_json`](../../../../tree_sitter_analyzer/mcp/utils/format_helper.md#format_as_json)

### `TestFormatAsToon`
- def: [`tests/unit/mcp/test_utils/test_format_helper.py:101`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_format_helper.py#L101)
- doc: Tests for format_as_toon function.
- signature: `class TestFormatAsToon:`
- members:
  - `test_format_as_toon_exception_fallback(self, mock_formatter_class)` — [`L129`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_format_helper.py#L129) — Test format_as_toon falls back to JSON on general exception.
  - `test_format_as_toon_import_error_fallback(self, mock_formatter_class)` — [`L119`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_format_helper.py#L119) — Test format_as_toon falls back to JSON on ImportError.
  - `test_format_as_toon_success(self, mock_formatter_class)` — [`L105`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_format_helper.py#L105) — Test format_as_toon with successful TOON formatting.
- uses (calls/refs, reference-scoped): [`format_as_toon`](../../../../tree_sitter_analyzer/mcp/utils/format_helper.md#format_as_toon)

### `TestFormatForFileOutput`
- def: [`tests/unit/mcp/test_utils/test_format_helper.py:234`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_format_helper.py#L234)
- doc: Tests for format_for_file_output function.
- signature: `class TestFormatForFileOutput:`
- members:
  - `test_format_for_file_output_default_format(self)` — [`L252`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_format_helper.py#L252) — Test format_for_file_output with default format (JSON).
  - `test_format_for_file_output_json(self)` — [`L237`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_format_helper.py#L237) — Test format_for_file_output with JSON format.
  - `test_format_for_file_output_toon(self)` — [`L245`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_format_helper.py#L245) — Test format_for_file_output with TOON format.
- uses (calls/refs, reference-scoped): [`format_for_file_output`](../../../../tree_sitter_analyzer/mcp/utils/format_helper.md#format_for_file_output)

### `TestFormatOutput`
- def: [`tests/unit/mcp/test_utils/test_format_helper.py:23`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_format_helper.py#L23)
- doc: Tests for format_output function.
- signature: `class TestFormatOutput:`
- members:
  - `test_format_output_default_format(self)` — [`L40`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_format_helper.py#L40) — Test format_output with default format (JSON).
  - `test_format_output_empty_dict(self)` — [`L47`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_format_helper.py#L47) — Test format_output with empty dictionary.
  - `test_format_output_json(self)` — [`L26`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_format_helper.py#L26) — Test format_output with JSON format.
  - `test_format_output_nested_dict(self)` — [`L53`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_format_helper.py#L53) — Test format_output with nested dictionary.
  - `test_format_output_toon(self)` — [`L34`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_format_helper.py#L34) — Test format_output with TOON format.
- uses (calls/refs, reference-scoped): [`format_output`](../../../../tree_sitter_analyzer/mcp/utils/format_helper.md#format_output)

### `TestGetFormatter`
- def: [`tests/unit/mcp/test_utils/test_format_helper.py:141`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_format_helper.py#L141)
- doc: Tests for get_formatter function.
- signature: `class TestGetFormatter:`
- members:
  - `test_get_formatter_default(self)` — [`L149`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_format_helper.py#L149) — Test get_formatter returns JsonFormatter for default format.
  - `test_get_formatter_json(self)` — [`L144`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_format_helper.py#L144) — Test get_formatter returns JsonFormatter for JSON format.
  - `test_get_formatter_toon(self, mock_formatter_class)` — [`L155`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_format_helper.py#L155) — Test get_formatter returns ToonFormatter for TOON format.
  - `test_get_formatter_toon_import_error(self, mock_formatter_class)` — [`L166`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_format_helper.py#L166) — Test get_formatter falls back to JsonFormatter on ImportError.
- uses (calls/refs, reference-scoped): [`get_formatter`](../../../../tree_sitter_analyzer/mcp/utils/format_helper.md#get_formatter), [`JsonFormatter`](../../../../tree_sitter_analyzer/mcp/utils/format_helper.md#JsonFormatter)

### `TestIntegration`
- def: [`tests/unit/mcp/test_utils/test_format_helper.py:448`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_format_helper.py#L448)
- doc: Integration tests for format_helper module.
- signature: `class TestIntegration:`
- members:
  - `test_attach_vs_apply_toon_difference(self)` — [`L506`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_format_helper.py#L506) — Test difference between attach and apply TOON functions.
  - `test_format_workflow_json(self)` — [`L451`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_format_helper.py#L451) — Test complete formatting workflow for JSON.
  - `test_format_workflow_toon(self)` — [`L469`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_format_helper.py#L469) — Test complete formatting workflow for TOON.
  - `test_get_formatter_and_format(self)` — [`L492`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_format_helper.py#L492) — Test getting formatter and using it to format data.
- uses (calls/refs, reference-scoped): [`apply_toon_format_to_response`](../../../../tree_sitter_analyzer/mcp/utils/format_helper.md#apply_toon_format_to_response), [`format_for_file_output`](../../../../tree_sitter_analyzer/mcp/utils/format_helper.md#format_for_file_output), [`format_output`](../../../../tree_sitter_analyzer/mcp/utils/format_helper.md#format_output), [`get_formatter`](../../../../tree_sitter_analyzer/mcp/utils/format_helper.md#get_formatter), [`attach_toon_content_to_response`](../../../../tree_sitter_analyzer/mcp/utils/format_helper.md#attach_toon_content_to_response), [`apply_output_format`](../../../../tree_sitter_analyzer/mcp/utils/format_helper.md#apply_output_format)

### `TestJsonFormatter`
- def: [`tests/unit/mcp/test_utils/test_format_helper.py:175`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_format_helper.py#L175)
- doc: Tests for JsonFormatter class.
- signature: `class TestJsonFormatter:`
- members:
  - `test_json_formatter_format(self)` — [`L178`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_format_helper.py#L178) — Test JsonFormatter.format method.
  - `test_json_formatter_format_list(self)` — [`L195`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_format_helper.py#L195) — Test JsonFormatter.format with list data.
  - `test_json_formatter_format_nested(self)` — [`L187`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_format_helper.py#L187) — Test JsonFormatter.format with nested data.
- uses (calls/refs, reference-scoped): [`JsonFormatter`](../../../../tree_sitter_analyzer/mcp/utils/format_helper.md#JsonFormatter), [`format`](../../../../tree_sitter_analyzer/mcp/utils/format_helper.md#JsonFormatter.format)

