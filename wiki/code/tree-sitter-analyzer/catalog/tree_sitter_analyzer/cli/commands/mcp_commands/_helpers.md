---
title: 'Module: tree_sitter_analyzer/cli/commands/mcp_commands/_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/cli/commands/mcp_commands/_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.cli.commands.mcp_commands._helpers`/_
symbols:
  _build_error_envelope: build_error_envelope().
  _run_tool: run_tool().
  _verdict_exit_code: verdict_exit_code().
  _classify_error_type: classify_error_type().
  _VERDICT_ORDER: VERDICT_ORDER.
---
# Module: [`tree_sitter_analyzer/cli/commands/mcp_commands/_helpers.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/mcp_commands/_helpers.py)

## Functions
- `_build_error_envelope(flag_name: str, label: str, exc: BaseException, echo_fields: Mapping[str, Any] | None = None)` — [`L23`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/mcp_commands/_helpers.py#L23) — Build the canonical error envelope for MCP-bridged CLI commands.
- `_classify_error_type(exc: BaseException)` — [`L11`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/mcp_commands/_helpers.py#L11) — Classify an exception into the canonical error_type vocabulary.
- `_run_tool(args: Any, tool_cls: Callable[..., Any], tool_args: Mapping[str, Any], label: str, output_json_fn: Callable[[dict[str, Any]], None], output_error_fn: Callable[[str], None], output_format_fn: Callable[[], str], fail_on_verdict_worse_than: str | None = None)` — [`L90`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/mcp_commands/_helpers.py#L90) — Helper: instantiate tool, run execute(), print output.
- `_verdict_exit_code(result: dict[str, Any], threshold: str)` — [`L75`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/mcp_commands/_helpers.py#L75) — Return 1 if result verdict >= threshold in severity, else 0.

## Module values
- `_VERDICT_ORDER` — [`L72`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/mcp_commands/_helpers.py#L72)

