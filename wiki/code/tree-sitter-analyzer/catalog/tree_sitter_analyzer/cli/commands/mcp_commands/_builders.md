---
title: 'Module: tree_sitter_analyzer/cli/commands/mcp_commands/_builders.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/cli/commands/mcp_commands/_builders.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.cli.commands.mcp_commands._builders`/_
symbols:
  _dependency_mode_requires_file: dependency_mode_requires_file().
  _build_dependency_tool_args: build_dependency_tool_args().
  _build_uml_tool_args: build_uml_tool_args().
  _normalize_dependency_mode: normalize_dependency_mode().
  _build_change_impact_tool_args: build_change_impact_tool_args().
  _DEPENDENCY_FILE_SCOPED_MODES: DEPENDENCY_FILE_SCOPED_MODES.
  _build_detect_routes_tool_args: build_detect_routes_tool_args().
  _build_parser_readiness_tool_args: build_parser_readiness_tool_args().
  _build_trace_impact_tool_args: build_trace_impact_tool_args().
  _build_safe_to_edit_tool_args: build_safe_to_edit_tool_args().
  _build_batch_search_tool_args: build_batch_search_tool_args().
  _build_modification_guard_tool_args: build_modification_guard_tool_args().
  _build_decision_journal_tool_args: build_decision_journal_tool_args().
  _build_check_tools_tool_args: build_check_tools_tool_args().
  _build_build_project_index_tool_args: build_build_project_index_tool_args().
  _build_codegraph_status_tool_args: build_codegraph_status_tool_args().
  _build_codegraph_explore_tool_args: build_codegraph_explore_tool_args().
  _build_codegraph_query_tool_args: build_codegraph_query_tool_args().
  _build_code_similarity_tool_args: build_code_similarity_tool_args().
  _DEPENDENCY_MODE_ALIASES: DEPENDENCY_MODE_ALIASES.
---
# Module: [`tree_sitter_analyzer/cli/commands/mcp_commands/_builders.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/mcp_commands/_builders.py)

## Functions
- `_build_batch_search_tool_args(args: Any, output_format: str)` — [`L107`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/mcp_commands/_builders.py#L107) — Build tool args for --batch-search (T2 round-37d parity fix).
- `_build_build_project_index_tool_args(args: Any, output_format: str)` — [`L218`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/mcp_commands/_builders.py#L218) — Build tool args for --build-project-index.
- `_build_change_impact_tool_args(args: Any, output_format: str)` — [`L238`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/mcp_commands/_builders.py#L238)
- `_build_check_tools_tool_args(args: Any, output_format: str)` — [`L208`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/mcp_commands/_builders.py#L208) — Build tool args for --check-tools.
- `_build_code_similarity_tool_args(args: Any, output_format: str)` — [`L285`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/mcp_commands/_builders.py#L285)
- `_build_codegraph_explore_tool_args(args: Any, output_format: str)` — [`L264`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/mcp_commands/_builders.py#L264)
- `_build_codegraph_query_tool_args(args: Any, output_format: str)` — [`L274`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/mcp_commands/_builders.py#L274)
- `_build_codegraph_status_tool_args(args: Any, output_format: str)` — [`L257`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/mcp_commands/_builders.py#L257)
- `_build_decision_journal_tool_args(args: Any, output_format: str)` — [`L173`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/mcp_commands/_builders.py#L173) — Build tool args for --decision-journal (r37fG CLI-MCP parity).
- `_build_dependency_tool_args(args: Any, output_format: str)` — [`L24`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/mcp_commands/_builders.py#L24)
- `_build_detect_routes_tool_args(args: Any, output_format: str)` — [`L35`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/mcp_commands/_builders.py#L35) — Build tool args for --detect-routes, omitting empty optional keys.
- `_build_modification_guard_tool_args(args: Any, output_format: str)` — [`L146`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/mcp_commands/_builders.py#L146) — Build tool args for --modification-guard (T1 round-37c parity fix).
- `_build_parser_readiness_tool_args(args: Any, output_format: str)` — [`L51`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/mcp_commands/_builders.py#L51) — Build tool args for parser-readiness CLI alias and flag modes.
- `_build_safe_to_edit_tool_args(args: Any, output_format: str)` — [`L85`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/mcp_commands/_builders.py#L85) — Build tool args for --safe-to-edit, rejecting directory inputs (#1002).
- `_build_trace_impact_tool_args(args: Any, output_format: str)` — [`L63`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/mcp_commands/_builders.py#L63) — Build tool args for --trace-impact, omitting empty optional keys.
- `_build_uml_tool_args(args: Any, output_format: str)` — [`L298`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/mcp_commands/_builders.py#L298)
- `_dependency_mode_requires_file(args: Any)` — [`L17`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/mcp_commands/_builders.py#L17)
- `_normalize_dependency_mode(mode: str | None)` — [`L13`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/mcp_commands/_builders.py#L13)

## Module values
- `_DEPENDENCY_FILE_SCOPED_MODES` — [`L9`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/mcp_commands/_builders.py#L9)
- `_DEPENDENCY_MODE_ALIASES` — [`L10`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/mcp_commands/_builders.py#L10)

