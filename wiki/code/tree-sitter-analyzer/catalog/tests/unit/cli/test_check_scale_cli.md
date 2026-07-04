---
title: 'Module: tests/unit/cli/test_check_scale_cli.py'
type: catalog
provenance: extracted
module: tests/unit/cli/test_check_scale_cli.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.cli.test_check_scale_cli`/
symbols:
  TestCheckScaleMcpCliParity.test_core_metric_keys_match_mcp_output: TestCheckScaleMcpCliParity#test_core_metric_keys_match_mcp_output().
  _make_context: _make_context().
  TestCheckScaleDispatch.test_returns_none_when_check_scale_absent: TestCheckScaleDispatch#test_returns_none_when_check_scale_absent().
  TestCheckScaleDispatch.test_returns_0_on_success: TestCheckScaleDispatch#test_returns_0_on_success().
  TestCheckScaleDispatch.test_returns_1_on_tool_failure: TestCheckScaleDispatch#test_returns_1_on_tool_failure().
  TestCheckScaleDispatch.test_missing_file_returns_1_with_json_error: TestCheckScaleDispatch#test_missing_file_returns_1_with_json_error().
  TestCheckScaleDispatch.test_project_root_resolves_relative_path: TestCheckScaleDispatch#test_project_root_resolves_relative_path().
  TestCheckScaleDispatch.test_language_override_forwarded: TestCheckScaleDispatch#test_language_override_forwarded().
  TestCheckScaleDispatch._base_args: TestCheckScaleDispatch#_base_args().
  TestCheckScaleParser.test_parser_accepts_check_scale: TestCheckScaleParser#test_parser_accepts_check_scale().
  TestCheckScaleParser.test_check_scale_in_help: TestCheckScaleParser#test_check_scale_in_help().
  TestCheckScaleParser.test_check_scale_absent_by_default: TestCheckScaleParser#test_check_scale_absent_by_default().
  TestCheckScaleParser: TestCheckScaleParser#
  TestCheckScaleDispatch: TestCheckScaleDispatch#
  TestCheckScaleMcpCliParity: TestCheckScaleMcpCliParity#
---
# Module: [`tests/unit/cli/test_check_scale_cli.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_check_scale_cli.py)

## Classes
### `TestCheckScaleDispatch`
- def: [`tests/unit/cli/test_check_scale_cli.py:80`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_check_scale_cli.py#L80)
- doc: handle_special_commands dispatches `--check-scale` correctly.
- signature: `class TestCheckScaleDispatch:`
- members:
  - `test_language_override_forwarded(self, tmp_path: Path)` — [`L205`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_check_scale_cli.py#L205) — --language reaches AnalyzeScaleTool (Codex P2 on #527).
  - `test_missing_file_returns_1_with_json_error(self, tmp_path: Path)` — [`L167`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_check_scale_cli.py#L167) — Nonexistent file → exit 1 with a JSON error envelope.
  - `test_project_root_resolves_relative_path(self, tmp_path: Path)` — [`L189`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_check_scale_cli.py#L189) — --project-root /repo --check-scale rel/path.py works from any CWD
  - `test_returns_0_on_success(self, tmp_path: Path)` — [`L126`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_check_scale_cli.py#L126) — Handler returns ``0`` when AnalyzeScaleTool returns success.
  - `test_returns_1_on_tool_failure(self, tmp_path: Path)` — [`L154`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_check_scale_cli.py#L154) — Handler returns ``1`` when AnalyzeScaleTool returns success=False.
  - `test_returns_none_when_check_scale_absent(self)` — [`L117`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_check_scale_cli.py#L117) — When ``check_scale`` is ``None``, handler returns ``None``.
- protocol/private: `_base_args`[`L83`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_check_scale_cli.py#L83)
- uses (calls/refs, reference-scoped): [`_handle_check_scale`](../../../tree_sitter_analyzer/cli/special_commands.md#_handle_check_scale)  (1 test-only)

### `TestCheckScaleMcpCliParity`
- def: [`tests/unit/cli/test_check_scale_cli.py:230`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_check_scale_cli.py#L230)
- doc: CLI path and MCP AnalyzeScaleTool.execute must agree on core metrics.
- signature: `class TestCheckScaleMcpCliParity:`
- members:
  - `test_core_metric_keys_match_mcp_output(self, tmp_path: Path)` — [`L233`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_check_scale_cli.py#L233) — CLI JSON output contains the same core keys as MCP execute response.
- uses (calls/refs, reference-scoped): [`AnalyzeScaleTool`](../../../tree_sitter_analyzer/mcp/tools/analyze_scale_tool.md#AnalyzeScaleTool), [`execute`](../../../tree_sitter_analyzer/mcp/tools/analyze_scale_tool.md#AnalyzeScaleTool.execute), [`_handle_check_scale`](../../../tree_sitter_analyzer/cli/special_commands.md#_handle_check_scale)  (1 test-only)

### `TestCheckScaleParser`
- def: [`tests/unit/cli/test_check_scale_cli.py:47`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_check_scale_cli.py#L47)
- doc: Parser wiring: `--check-scale FILE` must parse cleanly.
- signature: `class TestCheckScaleParser:`
- members:
  - `test_check_scale_absent_by_default(self)` — [`L70`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_check_scale_cli.py#L70) — Without the flag, ``args.check_scale`` is ``None``.
  - `test_check_scale_in_help(self)` — [`L58`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_check_scale_cli.py#L58) — ``--check-scale`` must appear in ``--help`` output.
  - `test_parser_accepts_check_scale(self, tmp_path: Path)` — [`L50`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_check_scale_cli.py#L50) — ``--check-scale FILE`` sets ``args.check_scale`` to the file path.
- uses (calls/refs, reference-scoped): [`create_argument_parser`](../../../tree_sitter_analyzer/cli_main.md#create_argument_parser)

## Functions
- `_make_context(**overrides)` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_check_scale_cli.py#L28) — Return a minimal SpecialCommandContext-like namespace.

