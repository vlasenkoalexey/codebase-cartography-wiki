---
title: 'Module: tests/unit/cli/test_outline_cli.py'
type: catalog
provenance: extracted
module: tests/unit/cli/test_outline_cli.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.cli.test_outline_cli`/
symbols:
  _make_context: _make_context().
  TestOutlineMcpCliParity.test_core_schema_keys_match_mcp_output: TestOutlineMcpCliParity#test_core_schema_keys_match_mcp_output().
  TestOutlineDispatch.test_returns_none_when_outline_absent: TestOutlineDispatch#test_returns_none_when_outline_absent().
  TestOutlineDispatch.test_returns_0_on_success: TestOutlineDispatch#test_returns_0_on_success().
  TestOutlineDispatch.test_returns_1_on_tool_failure: TestOutlineDispatch#test_returns_1_on_tool_failure().
  TestOutlineDispatch.test_missing_file_returns_1_with_json_error: TestOutlineDispatch#test_missing_file_returns_1_with_json_error().
  TestOutlineDispatch.test_project_root_resolves_relative_path: TestOutlineDispatch#test_project_root_resolves_relative_path().
  TestOutlineDispatch.test_language_override_forwarded: TestOutlineDispatch#test_language_override_forwarded().
  TestOutlineDispatch.test_listed_cap_forwarded: TestOutlineDispatch#test_listed_cap_forwarded().
  TestOutlineMcpCliParity.test_parse_error_signal_keys_match_mcp_output: TestOutlineMcpCliParity#test_parse_error_signal_keys_match_mcp_output().
  TestOutlineMcpCliParity.test_encoding_signal_keys_match_mcp_output: TestOutlineMcpCliParity#test_encoding_signal_keys_match_mcp_output().
  TestBareOutlineValidation.test_bare_outline_without_any_file_errors: TestBareOutlineValidation#test_bare_outline_without_any_file_errors().
  TestOutlineDispatch._base_args: TestOutlineDispatch#_base_args().
  TestOutlineMcpCliParity._run_cli_outline: TestOutlineMcpCliParity#_run_cli_outline().
  TestOutlineDispatch: TestOutlineDispatch#
  TestOutlineParser.test_parser_accepts_outline_file: TestOutlineParser#test_parser_accepts_outline_file().
  TestOutlineParser.test_outline_in_help: TestOutlineParser#test_outline_in_help().
  TestOutlineParser.test_outline_absent_by_default: TestOutlineParser#test_outline_absent_by_default().
  TestOutlineParser.test_outline_listed_cap_default: TestOutlineParser#test_outline_listed_cap_default().
  TestOutlineParser.test_outline_listed_cap_override: TestOutlineParser#test_outline_listed_cap_override().
  TestBareOutlineValidation: TestBareOutlineValidation#
  TestOutlineDispatch.fake_asyncio_run: TestOutlineDispatch#fake_asyncio_run().
  TestOutlineParser: TestOutlineParser#
  TestOutlineMcpCliParity: TestOutlineMcpCliParity#
---
# Module: [`tests/unit/cli/test_outline_cli.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_outline_cli.py)

## Classes
### `TestBareOutlineValidation`  ·  implements/extends TestOutlineDispatch
- def: [`tests/unit/cli/test_outline_cli.py:446`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_outline_cli.py#L446)
- signature: `class TestBareOutlineValidation(TestOutlineDispatch):`
- members:
  - `test_bare_outline_without_any_file_errors(self)` — [`L447`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_outline_cli.py#L447) — Codex P3 on #582: bare --outline with no file must fail with a
- uses (calls/refs, reference-scoped): [`_handle_outline`](../../../tree_sitter_analyzer/cli/special_commands.md#_handle_outline)  (3 test-only)
- used by: (1 test-only callers)

### `TestOutlineDispatch`
- def: [`tests/unit/cli/test_outline_cli.py:97`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_outline_cli.py#L97)
- doc: handle_special_commands dispatches `--outline` correctly.
- signature: `class TestOutlineDispatch:`
- members:
  - `fake_asyncio_run(coro)` — [`L253`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_outline_cli.py#L253)
  - `test_language_override_forwarded(self, tmp_path: Path)` — [`L224`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_outline_cli.py#L224) — --language reaches GetCodeOutlineTool.
  - `test_listed_cap_forwarded(self, tmp_path: Path)` — [`L244`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_outline_cli.py#L244) — --outline-listed-cap is forwarded to GetCodeOutlineTool.
  - `test_missing_file_returns_1_with_json_error(self, tmp_path: Path)` — [`L186`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_outline_cli.py#L186) — Nonexistent file → exit 1 with a JSON error envelope.
  - `test_project_root_resolves_relative_path(self, tmp_path: Path)` — [`L206`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_outline_cli.py#L206) — --project-root /repo --outline rel/path.py works from any CWD.
  - `test_returns_0_on_success(self, tmp_path: Path)` — [`L145`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_outline_cli.py#L145) — Handler returns ``0`` when GetCodeOutlineTool returns success.
  - `test_returns_1_on_tool_failure(self, tmp_path: Path)` — [`L173`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_outline_cli.py#L173) — Handler returns ``1`` when GetCodeOutlineTool returns success=False.
  - `test_returns_none_when_outline_absent(self)` — [`L136`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_outline_cli.py#L136) — When ``outline`` is ``None``, handler returns ``None``.
- protocol/private: `_base_args`[`L100`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_outline_cli.py#L100)
- uses (calls/refs, reference-scoped): [`_handle_outline`](../../../tree_sitter_analyzer/cli/special_commands.md#_handle_outline)  (2 test-only)
- used by: (2 test-only callers)

### `TestOutlineMcpCliParity`
- def: [`tests/unit/cli/test_outline_cli.py:284`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_outline_cli.py#L284)
- doc: CLI path and MCP GetCodeOutlineTool.execute must agree on core schema keys.
- signature: `class TestOutlineMcpCliParity:`
- members:
  - `test_core_schema_keys_match_mcp_output(self, tmp_path: Path)` — [`L309`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_outline_cli.py#L309) — CLI JSON output contains the same core keys as MCP execute response.
  - `test_encoding_signal_keys_match_mcp_output(self, tmp_path: Path)` — [`L412`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_outline_cli.py#L412) — #707: CLI must preserve non-UTF8 outline signals from MCP.
  - `test_parse_error_signal_keys_match_mcp_output(self, tmp_path: Path)` — [`L387`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_outline_cli.py#L387) — #707: CLI must preserve outline parse-error signals from MCP.
- protocol/private: `_run_cli_outline`[`L288`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_outline_cli.py#L288)
- uses (calls/refs, reference-scoped): [`GetCodeOutlineTool`](../../../tree_sitter_analyzer/mcp/tools/get_code_outline_tool.md#GetCodeOutlineTool), [`execute`](../../../tree_sitter_analyzer/mcp/tools/get_code_outline_tool.md#GetCodeOutlineTool.execute), [`_handle_outline`](../../../tree_sitter_analyzer/cli/special_commands.md#_handle_outline)  (1 test-only)

### `TestOutlineParser`
- def: [`tests/unit/cli/test_outline_cli.py:48`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_outline_cli.py#L48)
- doc: Parser wiring: `--outline FILE` must parse cleanly.
- signature: `class TestOutlineParser:`
- members:
  - `test_outline_absent_by_default(self)` — [`L71`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_outline_cli.py#L71) — Without the flag, ``args.outline`` is ``None``.
  - `test_outline_in_help(self)` — [`L59`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_outline_cli.py#L59) — ``--outline`` must appear in ``--help`` output.
  - `test_outline_listed_cap_default(self)` — [`L77`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_outline_cli.py#L77) — ``--outline-listed-cap`` defaults to 50.
  - `test_outline_listed_cap_override(self, tmp_path: Path)` — [`L83`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_outline_cli.py#L83) — ``--outline-listed-cap N`` sets the cap.
  - `test_parser_accepts_outline_file(self, tmp_path: Path)` — [`L51`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_outline_cli.py#L51) — ``--outline FILE`` sets ``args.outline`` to the file path.
- uses (calls/refs, reference-scoped): [`create_argument_parser`](../../../tree_sitter_analyzer/cli_main.md#create_argument_parser)

## Functions
- `_make_context(**overrides)` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_outline_cli.py#L29) — Return a minimal SpecialCommandContext-like namespace.

