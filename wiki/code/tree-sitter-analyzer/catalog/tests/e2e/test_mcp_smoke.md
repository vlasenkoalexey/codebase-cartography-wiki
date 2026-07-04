---
title: 'Module: tests/e2e/test_mcp_smoke.py'
type: catalog
provenance: extracted
module: tests/e2e/test_mcp_smoke.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.e2e.test_mcp_smoke`/
symbols:
  TestToolLatencyBudgets.test_check_project_health_under_10s: TestToolLatencyBudgets#test_check_project_health_under_10s().
  TestStderrNoiseBudget.test_no_debug_lines_after_tool_call: TestStderrNoiseBudget#test_no_debug_lines_after_tool_call().
  TestStderrNoiseBudget.test_no_error_lines_after_normal_tool_call: TestStderrNoiseBudget#test_no_error_lines_after_normal_tool_call().
  TestToolLatencyBudgets._call_and_measure: TestToolLatencyBudgets#_call_and_measure().
  TestToolLatencyBudgets.test_safe_to_edit_under_5s: TestToolLatencyBudgets#test_safe_to_edit_under_5s().
  TestStartup.test_server_boots_and_responds_to_initialize: TestStartup#test_server_boots_and_responds_to_initialize().
  TestStartup.test_tools_list_returns_expected_minimum: TestStartup#test_tools_list_returns_expected_minimum().
  TestStderrCleanlinessAtStartup.test_no_jsonrpc_error_in_stderr_after_initialize: TestStderrCleanlinessAtStartup#test_no_jsonrpc_error_in_stderr_after_initialize().
  TestStderrCleanlinessAtStartup.test_no_unicode_decode_error_in_stderr: TestStderrCleanlinessAtStartup#test_no_unicode_decode_error_in_stderr().
  _CI_FACTOR: _CI_FACTOR.
  TestStartup.test_initialize_does_not_advertise_logging_capability: TestStartup#test_initialize_does_not_advertise_logging_capability().
  TestStartup.test_initialize_includes_agent_routing_instructions: TestStartup#test_initialize_includes_agent_routing_instructions().
  TestStartup.test_repeated_headless_initialize_stays_under_budget: TestStartup#test_repeated_headless_initialize_stays_under_budget().
  TestToolLatencyBudgets.test_codegraph_metrics_cold_cache_under_5s: TestToolLatencyBudgets#test_codegraph_metrics_cold_cache_under_5s().
  test_framework_self_check_root_resolves: test_framework_self_check_root_resolves().
  pytestmark: pytestmark.
  TestStartup: TestStartup#
  TestStderrCleanlinessAtStartup: TestStderrCleanlinessAtStartup#
  TestToolLatencyBudgets: TestToolLatencyBudgets#
  TestStderrNoiseBudget: TestStderrNoiseBudget#
---
# Module: [`tests/e2e/test_mcp_smoke.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/test_mcp_smoke.py)

## Classes
### `TestStartup`
- def: [`tests/e2e/test_mcp_smoke.py:25`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/test_mcp_smoke.py#L25)
- signature: `class TestStartup:`
- members:
  - `test_initialize_does_not_advertise_logging_capability(self, mcp_server: MCPClient)` — [`L41`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/test_mcp_smoke.py#L41) — Regression for the v1.15.1 fake-LoggingCapability bug.
  - `test_initialize_includes_agent_routing_instructions(self, mcp_server: MCPClient)` — [`L61`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/test_mcp_smoke.py#L61) — The initialize response should steer agents before any tool call.
  - `test_repeated_headless_initialize_stays_under_budget(self, mcp_server_factory: Any)` — [`L83`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/test_mcp_smoke.py#L83) — Repeated stdio spawn→initialize should not leave clients pending.
  - `test_server_boots_and_responds_to_initialize(self, mcp_server: MCPClient)` — [`L26`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/test_mcp_smoke.py#L26)
  - `test_tools_list_returns_expected_minimum(self, mcp_server: MCPClient)` — [`L109`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/test_mcp_smoke.py#L109) — Wave C2: the public ``tools/list`` surface is exactly the 8 domain
- uses (calls/refs, reference-scoped): (7 test-only callers)

### `TestStderrCleanlinessAtStartup`
- def: [`tests/e2e/test_mcp_smoke.py:142`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/test_mcp_smoke.py#L142)
- doc: The MCP server should not log any \[error\]-grade noise at boot.
- signature: `class TestStderrCleanlinessAtStartup:`
- members:
  - `test_no_jsonrpc_error_in_stderr_after_initialize(self, mcp_server: MCPClient)` — [`L145`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/test_mcp_smoke.py#L145) — Regression for v1.15.1 / PR #151.
  - `test_no_unicode_decode_error_in_stderr(self, mcp_server: MCPClient)` — [`L171`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/test_mcp_smoke.py#L171) — Regression for v1.15.1 / PR #153 (cp932 crash).
- uses (calls/refs, reference-scoped): (3 test-only callers)

### `TestStderrNoiseBudget`
- def: [`tests/e2e/test_mcp_smoke.py:307`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/test_mcp_smoke.py#L307)
- doc: Regression for v1.15.1 PERF/DEBUG log noise visible in client logs.
- signature: `class TestStderrNoiseBudget:`
- members:
  - `test_no_debug_lines_after_tool_call(self, mcp_server: MCPClient)` — [`L310`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/test_mcp_smoke.py#L310) — At default log level, a tool call must not emit DEBUG lines.
  - `test_no_error_lines_after_normal_tool_call(self, mcp_server: MCPClient)` — [`L334`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/test_mcp_smoke.py#L334) — A successful tool call must not produce any [error]-level log lines.
- uses (calls/refs, reference-scoped): (5 test-only callers)

### `TestToolLatencyBudgets`
- def: [`tests/e2e/test_mcp_smoke.py:209`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/test_mcp_smoke.py#L209)
- doc: Regression for v1.15.1: codegraph_metrics cold-cache took &gt;50s.
- signature: `class TestToolLatencyBudgets:`
- members:
  - `test_check_project_health_under_10s(self, mcp_server: MCPClient)` — [`L263`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/test_mcp_smoke.py#L263) — check_project_health on the TSA repo itself must complete in 10s (×3 in CI).
  - `test_codegraph_metrics_cold_cache_under_5s(self, mcp_server_factory: Any)` — [`L235`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/test_mcp_smoke.py#L235) — Regression for the 50s codegraph_metrics hang (PR #151).
  - `test_safe_to_edit_under_5s(self, mcp_server: MCPClient)` — [`L287`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/test_mcp_smoke.py#L287) — safe_to_edit on a known file must complete in 5s (×3 in CI).
- protocol/private: `_call_and_measure`[`L217`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/test_mcp_smoke.py#L217)
- uses (calls/refs, reference-scoped): (5 test-only callers)

## Functions
- `test_framework_self_check_root_resolves()` — [`L193`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/test_mcp_smoke.py#L193) — Sanity: the framework's ``REPO_ROOT`` actually points to the repo.

## Module values
- `_CI_FACTOR` — [`L22`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/test_mcp_smoke.py#L22)
- `pytestmark` — [`L17`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/test_mcp_smoke.py#L17)

