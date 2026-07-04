---
title: 'Module: tests/unit/mcp/test_agent_workflow_tool.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_agent_workflow_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_agent_workflow_tool`/
symbols:
  test_agent_workflow_tool_returns_full_json_pack: test_agent_workflow_tool_returns_full_json_pack().
  test_agent_workflow_tool_defaults_to_compact_toon: test_agent_workflow_tool_defaults_to_compact_toon().
  test_agent_workflow_toon_surfaces_queue_ledger_command: test_agent_workflow_toon_surfaces_queue_ledger_command().
  test_agent_workflow_tool_handles_long_target_path: test_agent_workflow_tool_handles_long_target_path().
  test_agent_workflow_tool_phase_routing_uses_canonical_routes: test_agent_workflow_tool_phase_routing_uses_canonical_routes().
  test_agent_workflow_tool_envelope_holds_for_both_formats: test_agent_workflow_tool_envelope_holds_for_both_formats().
  test_agent_workflow_tool_rejects_external_absolute_target: test_agent_workflow_tool_rejects_external_absolute_target().
  test_agent_workflow_tool_rejects_empty_and_whitespace_target: test_agent_workflow_tool_rejects_empty_and_whitespace_target().
  test_agent_workflow_tool_rejects_non_string_target_path: test_agent_workflow_tool_rejects_non_string_target_path().
  test_agent_workflow_tool_rejects_path_traversal_target: test_agent_workflow_tool_rejects_path_traversal_target().
  test_agent_workflow_tool_unsupported_extension_still_plans: test_agent_workflow_tool_unsupported_extension_still_plans().
  test_agent_workflow_tool_quotes_target_with_spaces_in_cli_commands: test_agent_workflow_tool_quotes_target_with_spaces_in_cli_commands().
  test_agent_workflow_tool_phase_selection_responds_to_target_presence: test_agent_workflow_tool_phase_selection_responds_to_target_presence().
  test_agent_workflow_tool_concurrent_calls_are_safe: test_agent_workflow_tool_concurrent_calls_are_safe().
  test_agent_workflow_tool_rejects_invalid_output_format: test_agent_workflow_tool_rejects_invalid_output_format().
  _assert_step_handoffs: _assert_step_handoffs().
  test_cli_builder_blocks_missing_file: test_cli_builder_blocks_missing_file().
  test_cli_builder_blocks_path_outside_project: test_cli_builder_blocks_path_outside_project().
  test_cli_builder_succeeds_for_existing_file: test_cli_builder_succeeds_for_existing_file().
  _assert_envelope_holds: _assert_envelope_holds().
  _assert_path_in_step_commands: _assert_path_in_step_commands().
  _assert_agent_summary: _assert_agent_summary().
  _assert_sprint_contract: _assert_sprint_contract().
---
# Module: [`tests/unit/mcp/test_agent_workflow_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_agent_workflow_tool.py)

## Functions
- `_assert_agent_summary(result: dict)` — [`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_agent_workflow_tool.py#L65) — Assert the agent_summary block of a full JSON workflow pack response.
- `_assert_envelope_holds(result: dict, target_path: str | None, output_format: str)` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_agent_workflow_tool.py#L28) — Assert core envelope invariants for one (target_path, format) combination.
- `_assert_path_in_step_commands(result: dict, step_name: str, path: str)` — [`L46`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_agent_workflow_tool.py#L46) — Assert every CLI command for *step_name* contains *path*.
- `_assert_sprint_contract(result: dict)` — [`L85`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_agent_workflow_tool.py#L85) — Assert the sprint_contract block of a full JSON workflow pack response.
- `_assert_step_handoffs(result: dict)` — [`L53`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_agent_workflow_tool.py#L53) — Assert that every step's handoff matches the PHASE_ROUTING table.
- `test_agent_workflow_tool_concurrent_calls_are_safe(tmp_path)` — [`L391`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_agent_workflow_tool.py#L391) — Parallel execute calls must each return an independent pack.
- `test_agent_workflow_tool_defaults_to_compact_toon(tmp_path)` — [`L139`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_agent_workflow_tool.py#L139) — TOON output keeps the MCP response compact but still actionable.
- `test_agent_workflow_tool_envelope_holds_for_both_formats(tmp_path)` — [`L478`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_agent_workflow_tool.py#L478) — Both JSON and TOON outputs carry a consistent envelope shape.
- `test_agent_workflow_tool_handles_long_target_path(tmp_path)` — [`L369`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_agent_workflow_tool.py#L369) — A deeply-nested target path embeds verbatim into every step's commands.
- `test_agent_workflow_tool_phase_routing_uses_canonical_routes(tmp_path)` — [`L440`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_agent_workflow_tool.py#L440) — Every phase's handoff metadata matches PHASE_ROUTING source-of-truth.
- `test_agent_workflow_tool_phase_selection_responds_to_target_presence(tmp_path)` — [`L335`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_agent_workflow_tool.py#L335) — Phase planning must flip cleanly between targeted and untargeted modes.
- `test_agent_workflow_tool_quotes_target_with_spaces_in_cli_commands(tmp_path)` — [`L290`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_agent_workflow_tool.py#L290) — Path tokens in generated workflow commands are shell-safe for spaces.
- `test_agent_workflow_tool_rejects_empty_and_whitespace_target(tmp_path)` — [`L216`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_agent_workflow_tool.py#L216) — Empty / whitespace-only target_path must fail at validation.
- `test_agent_workflow_tool_rejects_external_absolute_target(tmp_path)` — [`L201`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_agent_workflow_tool.py#L201) — MCP callers cannot generate workflow commands for outside paths.
- `test_agent_workflow_tool_rejects_invalid_output_format(tmp_path)` — [`L423`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_agent_workflow_tool.py#L423) — Invalid output_format must fail at validation.
- `test_agent_workflow_tool_rejects_non_string_target_path(tmp_path)` — [`L232`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_agent_workflow_tool.py#L232) — target_path that isn't a string fails fast.
- `test_agent_workflow_tool_rejects_path_traversal_target(tmp_path)` — [`L248`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_agent_workflow_tool.py#L248) — Relative paths with .. that escape the project root are rejected.
- `test_agent_workflow_tool_returns_full_json_pack(tmp_path)` — [`L98`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_agent_workflow_tool.py#L98) — MCP JSON output should mirror the CLI workflow pack shape.
- `test_agent_workflow_tool_unsupported_extension_still_plans(tmp_path)` — [`L262`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_agent_workflow_tool.py#L262) — An unsupported language extension still produces a workflow.
- `test_agent_workflow_toon_surfaces_queue_ledger_command(tmp_path)` — [`L173`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_agent_workflow_tool.py#L173) — Targeted TOON output should expose the scoped queue-ledger command.
- `test_cli_builder_blocks_missing_file(tmp_path)` — [`L506`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_agent_workflow_tool.py#L506) — build_agent_workflow_pack returns risk=blocked for non-existent target.
- `test_cli_builder_blocks_path_outside_project(tmp_path)` — [`L524`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_agent_workflow_tool.py#L524) — build_agent_workflow_pack returns risk=blocked for an external absolute path.
- `test_cli_builder_succeeds_for_existing_file(tmp_path)` — [`L539`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_agent_workflow_tool.py#L539) — build_agent_workflow_pack proceeds normally when target file exists.

