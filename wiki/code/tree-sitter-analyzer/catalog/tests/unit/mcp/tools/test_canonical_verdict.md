---
title: 'Module: tests/unit/mcp/tools/test_canonical_verdict.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/tools/test_canonical_verdict.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.tools.test_canonical_verdict`/Test
symbols:
  TestValidateToolResponseVerdict.test_accepts_every_canonical_verdict: ValidateToolResponseVerdict#test_accepts_every_canonical_verdict().
  TestCanonicalVerdictSet.test_set_is_frozen: CanonicalVerdictSet#test_set_is_frozen().
  TestCanonicalVerdictSet.test_set_contents_match_documented_contract: CanonicalVerdictSet#test_set_contents_match_documented_contract().
  TestCanonicalVerdictSet.test_no_lowercase_or_mixed_case_aliases: CanonicalVerdictSet#test_no_lowercase_or_mixed_case_aliases().
  TestValidateToolResponseVerdict.test_accepts_payload_with_no_verdict_key: ValidateToolResponseVerdict#test_accepts_payload_with_no_verdict_key().
  TestValidateToolResponseVerdict.test_rejects_non_canonical_strings: ValidateToolResponseVerdict#test_rejects_non_canonical_strings().
  TestValidateToolResponseVerdict.test_rejects_non_string_verdict: ValidateToolResponseVerdict#test_rejects_non_string_verdict().
  TestValidateToolResponseVerdict.test_error_message_names_the_tool: ValidateToolResponseVerdict#test_error_message_names_the_tool().
  TestCanonicalVerdictSet: CanonicalVerdictSet#
  TestValidateToolResponseVerdict: ValidateToolResponseVerdict#
---
# Module: [`tests/unit/mcp/tools/test_canonical_verdict.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_canonical_verdict.py)

## Classes
### `TestCanonicalVerdictSet`
- def: [`tests/unit/mcp/tools/test_canonical_verdict.py:22`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_canonical_verdict.py#L22)
- doc: The vocabulary itself is part of the public contract.
- signature: `class TestCanonicalVerdictSet:`
- members:
  - `test_no_lowercase_or_mixed_case_aliases(self)` — [`L43`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_canonical_verdict.py#L43)
  - `test_set_contents_match_documented_contract(self)` — [`L29`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_canonical_verdict.py#L29)
  - `test_set_is_frozen(self)` — [`L25`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_canonical_verdict.py#L25)
- uses (calls/refs, reference-scoped): [`CANONICAL_VERDICTS`](../../../../tree_sitter_analyzer/mcp/tools/tool_response.md#CANONICAL_VERDICTS.CANONICAL_VERDICTS)

### `TestValidateToolResponseVerdict`
- def: [`tests/unit/mcp/tools/test_canonical_verdict.py:50`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_canonical_verdict.py#L50)
- doc: The verdict check is the gate that prevents pains #9/#93 recurring.
- signature: `class TestValidateToolResponseVerdict:`
- members:
  - `test_accepts_every_canonical_verdict(self, verdict: str)` — [`L59`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_canonical_verdict.py#L59)
  - `test_accepts_payload_with_no_verdict_key(self)` — [`L53`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_canonical_verdict.py#L53)
  - `test_error_message_names_the_tool(self)` — [`L86`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_canonical_verdict.py#L86)
  - `test_rejects_non_canonical_strings(self, bad: str)` — [`L76`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_canonical_verdict.py#L76)
  - `test_rejects_non_string_verdict(self)` — [`L80`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_canonical_verdict.py#L80)
- uses (calls/refs, reference-scoped): [`validate_tool_response`](../../../../tree_sitter_analyzer/mcp/tools/tool_response.md#validate_tool_response), [`CANONICAL_VERDICTS`](../../../../tree_sitter_analyzer/mcp/tools/tool_response.md#CANONICAL_VERDICTS.CANONICAL_VERDICTS)

