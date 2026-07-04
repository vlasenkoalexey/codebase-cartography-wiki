---
title: 'Module: tests/unit/mcp/utils/test_verdict_safety_net.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/utils/test_verdict_safety_net.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.utils.test_verdict_safety_net`/TestVerdictSafetyNet
symbols:
  TestVerdictSafetyNetJSON.test_success_without_verdict_gets_info: JSON#test_success_without_verdict_gets_info().
  TestVerdictSafetyNetJSON.test_explicit_verdict_is_preserved: JSON#test_explicit_verdict_is_preserved().
  TestVerdictSafetyNetJSON.test_failure_responses_are_not_touched: JSON#test_failure_responses_are_not_touched().
  TestVerdictSafetyNetJSON.test_non_dict_inputs_are_not_touched: JSON#test_non_dict_inputs_are_not_touched().
  TestVerdictSafetyNetTOON.test_success_without_verdict_gets_info_in_toon: TOON#test_success_without_verdict_gets_info_in_toon().
  TestVerdictSafetyNetTOON.test_explicit_verdict_survives_toon_compaction: TOON#test_explicit_verdict_survives_toon_compaction().
  TestVerdictSafetyNetIdempotence.test_double_application_stays_info: Idempotence#test_double_application_stays_info().
  TestVerdictSafetyNetIdempotence.test_does_not_overwrite_existing_value: Idempotence#test_does_not_overwrite_existing_value().
  TestVerdictSafetyNetJSON: JSON#
  TestVerdictSafetyNetTOON: TOON#
  TestVerdictSafetyNetIdempotence: Idempotence#
---
# Module: [`tests/unit/mcp/utils/test_verdict_safety_net.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/utils/test_verdict_safety_net.py)

## Classes
### `TestVerdictSafetyNetIdempotence`
- def: [`tests/unit/mcp/utils/test_verdict_safety_net.py:63`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/utils/test_verdict_safety_net.py#L63)
- doc: Repeated calls must converge — important when wrapper helpers
- signature: `class TestVerdictSafetyNetIdempotence:`
- members:
  - `test_does_not_overwrite_existing_value(self)` — [`L72`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/utils/test_verdict_safety_net.py#L72)
  - `test_double_application_stays_info(self)` — [`L67`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/utils/test_verdict_safety_net.py#L67)
- uses (calls/refs, reference-scoped): [`apply_toon_format_to_response`](../../../../tree_sitter_analyzer/mcp/utils/format_helper.md#apply_toon_format_to_response)

### `TestVerdictSafetyNetJSON`
- def: [`tests/unit/mcp/utils/test_verdict_safety_net.py:19`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/utils/test_verdict_safety_net.py#L19)
- doc: JSON callers must also see the default verdict.
- signature: `class TestVerdictSafetyNetJSON:`
- members:
  - `test_explicit_verdict_is_preserved(self)` — [`L26`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/utils/test_verdict_safety_net.py#L26)
  - `test_failure_responses_are_not_touched(self)` — [`L32`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/utils/test_verdict_safety_net.py#L32)
  - `test_non_dict_inputs_are_not_touched(self)` — [`L41`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/utils/test_verdict_safety_net.py#L41)
  - `test_success_without_verdict_gets_info(self)` — [`L22`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/utils/test_verdict_safety_net.py#L22)
- uses (calls/refs, reference-scoped): [`apply_toon_format_to_response`](../../../../tree_sitter_analyzer/mcp/utils/format_helper.md#apply_toon_format_to_response)

### `TestVerdictSafetyNetTOON`
- def: [`tests/unit/mcp/utils/test_verdict_safety_net.py:48`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/utils/test_verdict_safety_net.py#L48)
- doc: TOON callers must also see the default verdict.
- signature: `class TestVerdictSafetyNetTOON:`
- members:
  - `test_explicit_verdict_survives_toon_compaction(self)` — [`L56`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/utils/test_verdict_safety_net.py#L56)
  - `test_success_without_verdict_gets_info_in_toon(self)` — [`L51`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/utils/test_verdict_safety_net.py#L51)
- uses (calls/refs, reference-scoped): [`apply_toon_format_to_response`](../../../../tree_sitter_analyzer/mcp/utils/format_helper.md#apply_toon_format_to_response)

