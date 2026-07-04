---
title: 'Module: tests/unit/mcp/tools/test_response_builder.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/tools/test_response_builder.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.tools.test_response_builder`/Test
symbols:
  TestBuildResponse.test_accepts_every_canonical_verdict: BuildResponse#test_accepts_every_canonical_verdict().
  TestCanonicalVerdictSet.test_set_is_frozen_and_matches_validator: CanonicalVerdictSet#test_set_is_frozen_and_matches_validator().
  TestBuildResponse.test_explicit_success_false_with_error_passes: BuildResponse#test_explicit_success_false_with_error_passes().
  TestBuildResponse.test_rejects_non_canonical_verdict: BuildResponse#test_rejects_non_canonical_verdict().
  TestBuildResponse.test_error_message_is_actionable: BuildResponse#test_error_message_is_actionable().
  TestBuildError.test_defaults_verdict_to_error: BuildError#test_defaults_verdict_to_error().
  TestBuildError.test_rejects_non_canonical_verdict: BuildError#test_rejects_non_canonical_verdict().
  TestBuildResponse.test_default_success_is_true_and_merges_fields: BuildResponse#test_default_success_is_true_and_merges_fields().
  TestBuildResponse.test_invalid_verdict_error_is_a_value_error: BuildResponse#test_invalid_verdict_error_is_a_value_error().
  TestWarnings.test_omits_warnings_key_when_none: Warnings#test_omits_warnings_key_when_none().
  TestWarnings.test_omits_warnings_key_when_empty_list: Warnings#test_omits_warnings_key_when_empty_list().
  TestWarnings.test_includes_and_copies_warnings: Warnings#test_includes_and_copies_warnings().
  TestBuildError.test_accepts_not_found_verdict_and_extra_fields: BuildError#test_accepts_not_found_verdict_and_extra_fields().
  TestCanonicalVerdictSet: CanonicalVerdictSet#
  TestBuildResponse: BuildResponse#
  TestWarnings: Warnings#
  TestBuildError: BuildError#
---
# Module: [`tests/unit/mcp/tools/test_response_builder.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_response_builder.py)

## Classes
### `TestBuildError`
- def: [`tests/unit/mcp/tools/test_response_builder.py:140`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_response_builder.py#L140)
- doc: `build_error` is a thin wrapper over `build_response`.
- signature: `class TestBuildError:`
- members:
  - `test_accepts_not_found_verdict_and_extra_fields(self)` — [`L148`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_response_builder.py#L148)
  - `test_defaults_verdict_to_error(self)` — [`L143`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_response_builder.py#L143)
  - `test_rejects_non_canonical_verdict(self)` — [`L158`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_response_builder.py#L158)
- uses (calls/refs, reference-scoped): [`build_error`](../../../../tree_sitter_analyzer/mcp/tools/_response_builder.md#build_error), [`validate_tool_response`](../../../../tree_sitter_analyzer/mcp/tools/tool_response.md#validate_tool_response), [`InvalidVerdictError`](../../../../tree_sitter_analyzer/mcp/tools/_response_builder.md#InvalidVerdictError)

### `TestBuildResponse`
- def: [`tests/unit/mcp/tools/test_response_builder.py:48`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_response_builder.py#L48)
- doc: Happy path + the rejection contract.
- signature: `class TestBuildResponse:`
- members:
  - `test_accepts_every_canonical_verdict(self, verdict: str)` — [`L52`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_response_builder.py#L52)
  - `test_default_success_is_true_and_merges_fields(self)` — [`L58`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_response_builder.py#L58)
  - `test_error_message_is_actionable(self)` — [`L106`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_response_builder.py#L106)
  - `test_explicit_success_false_with_error_passes(self)` — [`L71`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_response_builder.py#L71)
  - `test_invalid_verdict_error_is_a_value_error(self)` — [`L100`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_response_builder.py#L100)
  - `test_rejects_non_canonical_verdict(self, bad: str)` — [`L96`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_response_builder.py#L96)
- uses (calls/refs, reference-scoped): [`build_response`](../../../../tree_sitter_analyzer/mcp/tools/_response_builder.md#build_response), [`validate_tool_response`](../../../../tree_sitter_analyzer/mcp/tools/tool_response.md#validate_tool_response), [`CANONICAL_VERDICTS`](../../../../tree_sitter_analyzer/mcp/tools/_response_builder.md#CANONICAL_VERDICTS.CANONICAL_VERDICTS), [`InvalidVerdictError`](../../../../tree_sitter_analyzer/mcp/tools/_response_builder.md#InvalidVerdictError)

### `TestCanonicalVerdictSet`
- def: [`tests/unit/mcp/tools/test_response_builder.py:28`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_response_builder.py#L28)
- doc: The factory's vocabulary must match the validator's vocabulary.
- signature: `class TestCanonicalVerdictSet:`
- members:
  - `test_set_is_frozen_and_matches_validator(self)` — [`L31`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_response_builder.py#L31)
- uses (calls/refs, reference-scoped): [`CANONICAL_VERDICTS`](../../../../tree_sitter_analyzer/mcp/tools/tool_response.md#CANONICAL_VERDICTS.CANONICAL_VERDICTS), [`CANONICAL_VERDICTS`](../../../../tree_sitter_analyzer/mcp/tools/_response_builder.md#CANONICAL_VERDICTS.CANONICAL_VERDICTS)

### `TestWarnings`
- def: [`tests/unit/mcp/tools/test_response_builder.py:117`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_response_builder.py#L117)
- doc: Warnings list: included when present, omitted when empty/None.
- signature: `class TestWarnings:`
- members:
  - `test_includes_and_copies_warnings(self)` — [`L130`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_response_builder.py#L130)
  - `test_omits_warnings_key_when_empty_list(self)` — [`L124`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_response_builder.py#L124)
  - `test_omits_warnings_key_when_none(self)` — [`L120`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_response_builder.py#L120)
- uses (calls/refs, reference-scoped): [`build_response`](../../../../tree_sitter_analyzer/mcp/tools/_response_builder.md#build_response)

