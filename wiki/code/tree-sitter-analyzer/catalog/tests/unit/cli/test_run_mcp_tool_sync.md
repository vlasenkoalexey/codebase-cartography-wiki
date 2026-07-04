---
title: 'Module: tests/unit/cli/test_run_mcp_tool_sync.py'
type: catalog
provenance: extracted
module: tests/unit/cli/test_run_mcp_tool_sync.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.cli.test_run_mcp_tool_sync`/
symbols:
  _make_context: _make_context().
  TestRunMcpToolSync.test_instantiates_tool_with_project_root: TestRunMcpToolSync#test_instantiates_tool_with_project_root().
  TestRunMcpToolSync.test_returns_one_when_success_false: TestRunMcpToolSync#test_returns_one_when_success_false().
  TestRunMcpToolSync.test_returns_one_when_success_key_absent: TestRunMcpToolSync#test_returns_one_when_success_key_absent().
  TestRunMcpToolSync.test_print_result_receives_full_envelope_in_json: TestRunMcpToolSync#test_print_result_receives_full_envelope_in_json().
  TestRunMcpToolSync.test_print_result_uses_output_toon_in_toon_mode: TestRunMcpToolSync#test_print_result_uses_output_toon_in_toon_mode().
  _make_args: _make_args().
  TestAntiDuplicationGuard.test_only_helper_contains_inline_asyncio_run_execute: TestAntiDuplicationGuard#test_only_helper_contains_inline_asyncio_run_execute().
  TestAntiDuplicationGuard._PATTERN: TestAntiDuplicationGuard#_PATTERN.
  TestRunMcpToolSync: TestRunMcpToolSync#
  TestAntiDuplicationGuard: TestAntiDuplicationGuard#
---
# Module: [`tests/unit/cli/test_run_mcp_tool_sync.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_run_mcp_tool_sync.py)

## Classes
### `TestAntiDuplicationGuard`
- def: [`tests/unit/cli/test_run_mcp_tool_sync.py:163`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_run_mcp_tool_sync.py#L163)
- doc: Lock down the helper as the only inline-asyncio-execute site.
- signature: `class TestAntiDuplicationGuard:`
- members:
  - `test_only_helper_contains_inline_asyncio_run_execute(self)` — [`L173`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_run_mcp_tool_sync.py#L173)
- protocol/private: `_PATTERN`[`L171`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_run_mcp_tool_sync.py#L171)

### `TestRunMcpToolSync`
- def: [`tests/unit/cli/test_run_mcp_tool_sync.py:54`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_run_mcp_tool_sync.py#L54)
- doc: Cover the four observable behaviours of `_run_mcp_tool_sync`.
- signature: `class TestRunMcpToolSync:`
- members:
  - `test_instantiates_tool_with_project_root(self)` — [`L57`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_run_mcp_tool_sync.py#L57)
  - `test_print_result_receives_full_envelope_in_json(self, monkeypatch)` — [`L113`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_run_mcp_tool_sync.py#L113) — The helper hands the awaited envelope to ``_print_result``.
  - `test_print_result_uses_output_toon_in_toon_mode(self, monkeypatch)` — [`L134`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_run_mcp_tool_sync.py#L134) — TOON path: ``_print_result`` routes through ``output_toon`` helper.
  - `test_returns_one_when_success_false(self)` — [`L81`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_run_mcp_tool_sync.py#L81)
  - `test_returns_one_when_success_key_absent(self)` — [`L97`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_run_mcp_tool_sync.py#L97)
- uses (calls/refs, reference-scoped): [`_run_mcp_tool_sync`](../../../tree_sitter_analyzer/cli/special_commands.md#_run_mcp_tool_sync)  (2 test-only)

## Functions
- `_make_args(format_: str = "json")` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_run_mcp_tool_sync.py#L49) — Build an argparse-like Namespace stub for ``_print_result``.
- `_make_context(asyncio_run: MagicMock, output_json: MagicMock)` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_run_mcp_tool_sync.py#L35) — Build a SpecialCommandContext whose dependencies are mocks.

