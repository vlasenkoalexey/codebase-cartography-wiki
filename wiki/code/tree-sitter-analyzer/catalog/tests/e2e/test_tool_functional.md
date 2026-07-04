---
title: 'Module: tests/e2e/test_tool_functional.py'
type: catalog
provenance: extracted
module: tests/e2e/test_tool_functional.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.e2e.test_tool_functional`/
symbols:
  TestFacadeWireContract.test_all_facades_have_stdio_tools_call_envelopes: TestFacadeWireContract#test_all_facades_have_stdio_tools_call_envelopes().
  TestSafeToEdit.test_known_safe_file_returns_safe_verdict: TestSafeToEdit#test_known_safe_file_returns_safe_verdict().
  TestSafeToEdit.test_negative_fixture_returns_unsafe_verdict: TestSafeToEdit#test_negative_fixture_returns_unsafe_verdict().
  TestSafeToEdit.test_nonexistent_file_returns_error_or_verdict: TestSafeToEdit#test_nonexistent_file_returns_error_or_verdict().
  TestCheckFileHealth.test_returns_health_score_for_known_file: TestCheckFileHealth#test_returns_health_score_for_known_file().
  TestCheckFileHealth.test_large_complex_file_returns_result_not_crash: TestCheckFileHealth#test_large_complex_file_returns_result_not_crash().
  TestCheckProjectHealth.test_returns_summary_with_grade: TestCheckProjectHealth#test_returns_summary_with_grade().
  TestCheckProjectHealth.test_returns_file_count_greater_than_zero: TestCheckProjectHealth#test_returns_file_count_greater_than_zero().
  TestCodegraphStatus.test_returns_status_response: TestCodegraphStatus#test_returns_status_response().
  TestCodegraphStatus.test_status_contains_index_info: TestCodegraphStatus#test_status_contains_index_info().
  TestFacadeWireContract.test_facade_wire_cases_cover_all_public_facades: TestFacadeWireContract#test_facade_wire_cases_cover_all_public_facades().
  FACADE_WIRE_CASES: FACADE_WIRE_CASES.
  EXPECTED_FACADE_NAMES: EXPECTED_FACADE_NAMES.
  _json_text_payload: _json_text_payload().
  _assert_agent_wire_envelope: _assert_agent_wire_envelope().
  pytestmark: pytestmark.
  TestFacadeWireContract: TestFacadeWireContract#
  TestSafeToEdit: TestSafeToEdit#
  TestCheckFileHealth: TestCheckFileHealth#
  TestCheckProjectHealth: TestCheckProjectHealth#
  TestCodegraphStatus: TestCodegraphStatus#
---
# Module: [`tests/e2e/test_tool_functional.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/test_tool_functional.py)

## Classes
### `TestCheckFileHealth`
- def: [`tests/e2e/test_tool_functional.py:228`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/test_tool_functional.py#L228)
- signature: `class TestCheckFileHealth:`
- members:
  - `test_large_complex_file_returns_result_not_crash(self, mcp_server: MCPClient)` — [`L249`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/test_tool_functional.py#L249) — The project_graph.py module is large; the tool must not crash.
  - `test_returns_health_score_for_known_file(self, mcp_server: MCPClient)` — [`L229`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/test_tool_functional.py#L229) — check_file_health on a real source file must return a score.
- uses (calls/refs, reference-scoped): (3 test-only callers)

### `TestCheckProjectHealth`
- def: [`tests/e2e/test_tool_functional.py:268`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/test_tool_functional.py#L268)
- signature: `class TestCheckProjectHealth:`
- members:
  - `test_returns_file_count_greater_than_zero(self, mcp_server: MCPClient)` — [`L282`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/test_tool_functional.py#L282) — The TSA repo has many files; the summary must count more than zero.
  - `test_returns_summary_with_grade(self, mcp_server: MCPClient)` — [`L269`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/test_tool_functional.py#L269) — check_project_health on the TSA repo must return a grade.
- uses (calls/refs, reference-scoped): (3 test-only callers)

### `TestCodegraphStatus`
- def: [`tests/e2e/test_tool_functional.py:304`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/test_tool_functional.py#L304)
- signature: `class TestCodegraphStatus:`
- members:
  - `test_returns_status_response(self, mcp_server: MCPClient)` — [`L305`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/test_tool_functional.py#L305) — codegraph_status must always return a response (not crash).
  - `test_status_contains_index_info(self, mcp_server: MCPClient)` — [`L313`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/test_tool_functional.py#L313) — When TSA's own index exists, codegraph_status describes it.
- uses (calls/refs, reference-scoped): (3 test-only callers)

### `TestFacadeWireContract`
- def: [`tests/e2e/test_tool_functional.py:133`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/test_tool_functional.py#L133)
- signature: `class TestFacadeWireContract:`
- members:
  - `test_all_facades_have_stdio_tools_call_envelopes(self, mcp_server: MCPClient, facade_name: str, arguments: dict)` — [`L139`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/test_tool_functional.py#L139) — Issue #691: cover the real client→stdio→tools/call boundary.
  - `test_facade_wire_cases_cover_all_public_facades(self)` — [`L153`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/test_tool_functional.py#L153)
- uses (calls/refs, reference-scoped): (7 test-only callers)

### `TestSafeToEdit`
- def: [`tests/e2e/test_tool_functional.py:163`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/test_tool_functional.py#L163)
- signature: `class TestSafeToEdit:`
- members:
  - `test_known_safe_file_returns_safe_verdict(self, mcp_server: MCPClient)` — [`L164`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/test_tool_functional.py#L164) — A simple utility file should be flagged SAFE.
  - `test_negative_fixture_returns_unsafe_verdict(self, mcp_server: MCPClient)` — [`L180`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/test_tool_functional.py#L180) — java_plugin.py is a negative fixture: intentionally complex.
  - `test_nonexistent_file_returns_error_or_verdict(self, mcp_server: MCPClient)` — [`L206`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/test_tool_functional.py#L206) — A nonexistent file should not crash the server.
- uses (calls/refs, reference-scoped): (3 test-only callers)

## Functions
- `_assert_agent_wire_envelope(payload: dict, facade_name: str)` — [`L116`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/test_tool_functional.py#L116) — Assert the envelope an MCP stdio client actually receives.
- `_json_text_payload(response: dict)` — [`L103`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/test_tool_functional.py#L103) — Return the JSON payload embedded in a JSON-RPC tools/call response.

## Module values
- `EXPECTED_FACADE_NAMES` — [`L91`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/test_tool_functional.py#L91)
- `FACADE_WIRE_CASES` — [`L30`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/test_tool_functional.py#L30)
- `pytestmark` — [`L28`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/test_tool_functional.py#L28)

