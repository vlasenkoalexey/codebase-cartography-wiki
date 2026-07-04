---
title: 'Module: benchmarks/codegraph_compare/adapters/claude_runner.py'
type: catalog
provenance: extracted
module: benchmarks/codegraph_compare/adapters/claude_runner.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `benchmarks.codegraph_compare.adapters.claude_runner`/
symbols:
  run_one: run_one().
  _ARM_ALLOWED_TOOLS._ARM_ALLOWED_TOOLS: _ARM_ALLOWED_TOOLS._ARM_ALLOWED_TOOLS.
  _build_agent_cmd: _build_agent_cmd().
  _usage_int: _usage_int().
  _parse_codex_tool_calls_from_stream: _parse_codex_tool_calls_from_stream().
  _write_arm_mcp_config: _write_arm_mcp_config().
  _extract_cost_accounting: _extract_cost_accounting().
  _BASE_TOOLS: _BASE_TOOLS.
  _parse_codex_stream: _parse_codex_stream().
  _extract_usage_metrics: _extract_usage_metrics().
  _ARM_DISALLOWED_TOOLS._ARM_DISALLOWED_TOOLS: _ARM_DISALLOWED_TOOLS._ARM_DISALLOWED_TOOLS.
  _CODEGRAPH_TOOLS: _CODEGRAPH_TOOLS.
  _TSA_TOOLS: _TSA_TOOLS.
  _codex_sandbox_for_arm: _codex_sandbox_for_arm().
  _parse_codex_stream._is_reconnect_error: _parse_codex_stream()._is_reconnect_error().
  _MCP_CONFIG_DIR: _MCP_CONFIG_DIR.
  _DEFAULT_MODELS: _DEFAULT_MODELS.
  _make_run_id: _make_run_id().
  _extract_citations: _extract_citations().
  _parse_tool_calls_from_stream: _parse_tool_calls_from_stream().
  _looks_like_shell_read: _looks_like_shell_read().
  _looks_like_shell_search: _looks_like_shell_search().
  _looks_like_index_query: _looks_like_index_query().
  _parse_claude_result_from_stream: _parse_claude_result_from_stream().
  _ANALYZER_ROOT: _ANALYZER_ROOT.
---
# Module: [`benchmarks/codegraph_compare/adapters/claude_runner.py`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/claude_runner.py)

## Functions
- `_build_agent_cmd(arm_id: str, model: str, repo_path: Path, run_config: RunConfig, allowed_tools_str: str, disallowed_tools_str: str, agent_backend: str)` — [`L336`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/claude_runner.py#L336) — Build the CLI command list for the given agent backend.
- `_codex_sandbox_for_arm(arm_id: str)` — [`L124`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/claude_runner.py#L124) — Return the least-permissive Codex sandbox that still lets indexes query.
- `_extract_citations(text: str, repo_path: Path)` — [`L99`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/claude_runner.py#L99) — Extract answer citations that correspond to real files in repo_path.
- `_extract_cost_accounting(raw_result: dict[str, Any])` — [`L440`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/claude_runner.py#L440) — Pull the provider's REAL cost/cache accounting from a result block.
- `_extract_usage_metrics(usage: dict[str, Any], agent_backend: str)` — [`L408`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/claude_runner.py#L408) — Return input, cached input, output, reasoning output, total tokens.
- `_is_reconnect_error(message: Any)` — [`L225`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/claude_runner.py#L225)
- `_looks_like_index_query(command: str)` — [`L183`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/claude_runner.py#L183)
- `_looks_like_shell_read(command: str)` — [`L175`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/claude_runner.py#L175)
- `_looks_like_shell_search(command: str)` — [`L179`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/claude_runner.py#L179)
- `_make_run_id(question_id: str, arm_id: str, repeat: int, agent_backend: str)` — [`L95`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/claude_runner.py#L95)
- `_parse_claude_result_from_stream(stream_lines: list[str])` — [`L268`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/claude_runner.py#L268) — Extract answer, error, and raw_result from a claude stream-json output.
- `_parse_codex_stream(lines: list[str])` — [`L220`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/claude_runner.py#L220)
- `_parse_codex_tool_calls_from_stream(lines: list[str])` — [`L187`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/claude_runner.py#L187) — Count Codex CLI command_execution events by benchmark category.
- `_parse_tool_calls_from_stream(lines: list[str])` — [`L131`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/claude_runner.py#L131) — Count tool calls by category from stream-json event lines.
- `_usage_int(usage: dict[str, Any], key: str)` — [`L403`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/claude_runner.py#L403)
- `_write_arm_mcp_config(arm_id: str, repo_path: Path)` — [`L298`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/claude_runner.py#L298) — Write a per-arm MCP config so each arm sees ONLY its own MCP server.
- `run_one(question_id: str, question_prompt: str, arm_id: str, repo_path: Path, repeat: int, run_config: RunConfig, results_dir: Path, timeout_seconds: int = 1200, model: str | None = None, agent_backend: str = "claude", dry_run: bool = False, session_id: str = "")` — [`L478`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/claude_runner.py#L478) — Run one benchmark trial via the configured agent CLI.

## Module values
- `_ANALYZER_ROOT` — [`L294`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/claude_runner.py#L294)
- `_ARM_ALLOWED_TOOLS` — [`L55`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/claude_runner.py#L55)
- `_ARM_DISALLOWED_TOOLS` — [`L65`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/claude_runner.py#L65)
- `_BASE_TOOLS` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/claude_runner.py#L33)
- `_CODEGRAPH_TOOLS` — [`L34`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/claude_runner.py#L34)
- `_DEFAULT_MODELS` — [`L89`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/claude_runner.py#L89)
- `_MCP_CONFIG_DIR` — [`L295`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/claude_runner.py#L295)
- `_TSA_TOOLS` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/claude_runner.py#L45)

