---
title: 'Module: tree_sitter_analyzer/mcp/tools/find_and_grep_execution.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/find_and_grep_execution.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.find_and_grep_execution`/
symbols:
  resolve_real_total: resolve_real_total().
  resolve_fd_no_ignore: resolve_fd_no_ignore().
  build_fd_command_from_arguments: build_fd_command_from_arguments().
  build_rg_command_from_arguments: build_rg_command_from_arguments().
  build_rg_recount_command: build_rg_recount_command().
  apply_match_limits: apply_match_limits().
  logger: logger.
  RECOUNT_BUDGET_MS: RECOUNT_BUDGET_MS.
  build_fd_error_response: build_fd_error_response().
  parse_fd_output: parse_fd_output().
  sort_files: sort_files().
  build_rg_error_response: build_rg_error_response().
  _build_rg_targets: _build_rg_targets().
  _looks_like_glob: _looks_like_glob().
---
# Module: [`tree_sitter_analyzer/mcp/tools/find_and_grep_execution.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_execution.py)

## Functions
- `_build_rg_targets(files: list[str])` — [`L196`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_execution.py#L196) — Return parent directories and exact filename globs for ripgrep.
- `_looks_like_glob(pattern: Any)` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_execution.py#L45) — Return True if ``pattern`` looks like a filename glob (``*.py``,
- `apply_match_limits(matches: list[dict[str, Any]], arguments: dict[str, Any])` — [`L183`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_execution.py#L183) — Truncate matches to user max_count or the hard cap.
- `build_fd_command_from_arguments(arguments: dict[str, Any], roots: list[str], *, fd_limit: int, no_ignore: bool)` — [`L64`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_execution.py#L64) — Build the fd command from validated find_and_grep arguments.
- `build_fd_error_response(err: bytes, rc: int)` — [`L98`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_execution.py#L98) — Build the error response returned when fd fails.
- `build_rg_command_from_arguments(arguments: dict[str, Any], files: list[str])` — [`L141`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_execution.py#L141) — Build the ripgrep command for the discovered files.
- `build_rg_error_response(err: bytes, rc: int)` — [`L174`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_execution.py#L174) — Build the error response returned when ripgrep fails.
- `build_rg_recount_command(arguments: dict[str, Any], files: list[str])` — [`L208`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_execution.py#L208) — Build a ripgrep --count-matches command on the same fd-discovered files.
- `parse_fd_output(out: bytes, fd_limit: int)` — [`L107`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_execution.py#L107) — Parse fd stdout into a capped file list and truncation flag.
- `resolve_fd_no_ignore(arguments: dict[str, Any], project_root: str | None, *, detector_factory: Any = get_default_detector)` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_execution.py#L21) — Resolve whether fd should bypass ignore rules for this search.
- `resolve_real_total(*, truncated: bool, displayed_count: int, arguments: dict[str, Any], files: list[str])` — [`L246`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_execution.py#L246) — Return ``(real_total, total_count_known)`` for find_and_grep.
- `sort_files(files: list[str], sort_mode: str | None)` — [`L120`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_execution.py#L120) — Sort files by path, mtime, or size.

## Module values
- `RECOUNT_BUDGET_MS` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_execution.py#L18)
- `logger` — [`L13`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/find_and_grep_execution.py#L13)

