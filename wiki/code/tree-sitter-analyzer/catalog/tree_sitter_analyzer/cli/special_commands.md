---
title: 'Module: tree_sitter_analyzer/cli/special_commands.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/cli/special_commands.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.cli.special_commands`/
symbols:
  SpecialCommandContext: SpecialCommandContext#
  handle_special_commands: handle_special_commands().
  _handle_outline: _handle_outline().
  SpecialCommandContext.output_error: SpecialCommandContext#output_error.
  SpecialCommandContext.output_json: SpecialCommandContext#output_json.
  _handle_check_scale: _handle_check_scale().
  SpecialCommandContext.output_list: SpecialCommandContext#output_list.
  SpecialCommandContext.output_info: SpecialCommandContext#output_info.
  SpecialCommandContext.query_loader: SpecialCommandContext#query_loader.
  _run_mcp_tool_sync: _run_mcp_tool_sync().
  _handle_sql_platform_commands: _handle_sql_platform_commands().
  SpecialCommandContext.asyncio_run: SpecialCommandContext#asyncio_run.
  _handle_batch_partial_read: _handle_batch_partial_read().
  _emit_cli_error: _emit_cli_error().
  _handle_install_skills: _handle_install_skills().
  _handle_batch_metrics: _handle_batch_metrics().
  _emit_show_common_queries: _emit_show_common_queries().
  _handle_health_check: _handle_health_check().
  _handle_mcp_commands: _handle_mcp_commands().
  _emit_show_query_languages: _emit_show_query_languages().
  _handle_query_language_commands: _handle_query_language_commands().
  _handle_knowledge_graph_index: _handle_knowledge_graph_index().
  _handle_agent_skills: _handle_agent_skills().
  _handle_agent_workflow: _handle_agent_workflow().
  _handle_check_constraints: _handle_check_constraints().
  _print_result: _print_result().
  _tool_output_format: _tool_output_format().
  _handle_autoindex: _handle_autoindex().
  _handle_full_index: _handle_full_index().
  _handle_codegraph_metrics: _handle_codegraph_metrics().
  _handle_incremental_sync: _handle_incremental_sync().
  _handle_clean_state: _handle_clean_state().
  _handle_affected: _handle_affected().
  _resolve_outline_file: _resolve_outline_file().
  _handle_nav_actions_lazy: _handle_nav_actions_lazy().
  _handle_watch_health: _handle_watch_health().
  OutputMessageFn: OutputMessageFn.
  _validate_partial_read_options: _validate_partial_read_options().
  _effective_output_format: _effective_output_format().
  OutputJsonFn: OutputJsonFn.
  _load_requests_payload: _load_requests_payload().
  _load_file_paths: _load_file_paths().
  _is_batch_partial_read: _is_batch_partial_read().
---
# Module: [`tree_sitter_analyzer/cli/special_commands.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/special_commands.py)

## Classes
### `SpecialCommandContext`
- def: [`tree_sitter_analyzer/cli/special_commands.py:16`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/special_commands.py#L16)
- doc: Runtime dependencies injected by cli_main for testable special commands.
- signature: `class SpecialCommandContext:`
- members:
  - `asyncio_run` — [`L19`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/special_commands.py#L19)
  - `output_error` — [`L21`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/special_commands.py#L21)
  - `output_info` — [`L22`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/special_commands.py#L22)
  - `output_json` — [`L20`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/special_commands.py#L20)
  - `output_list` — [`L23`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/special_commands.py#L23)
  - `query_loader` — [`L24`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/special_commands.py#L24)
- uses (calls/refs, reference-scoped): [`OutputMessageFn`](special_commands.md#OutputMessageFn), [`OutputJsonFn`](special_commands.md#OutputJsonFn)
- used by: [`handle_special_commands`](../cli_main.md#handle_special_commands), [`handle_special_commands`](special_commands.md#handle_special_commands), [`_handle_outline`](special_commands.md#_handle_outline), [`handle_nav_actions`](nav_special_commands.md#handle_nav_actions), [`_handle_check_scale`](special_commands.md#_handle_check_scale), [`_handle_sql_platform_commands`](special_commands.md#_handle_sql_platform_commands), [`_run_mcp_tool_sync`](special_commands.md#_run_mcp_tool_sync), [`_handle_batch_partial_read`](special_commands.md#_handle_batch_partial_read), [`_emit_cli_error`](special_commands.md#_emit_cli_error), [`_handle_install_skills`](special_commands.md#_handle_install_skills), [`_emit_show_common_queries`](special_commands.md#_emit_show_common_queries), [`_handle_batch_metrics`](special_commands.md#_handle_batch_metrics), [`_emit_show_query_languages`](special_commands.md#_emit_show_query_languages), [`_handle_health_check`](special_commands.md#_handle_health_check), [`_handle_mcp_commands`](special_commands.md#_handle_mcp_commands), [`_handle_query_language_commands`](special_commands.md#_handle_query_language_commands), [`_handle_knowledge_graph_index`](special_commands.md#_handle_knowledge_graph_index), [`_handle_agent_skills`](special_commands.md#_handle_agent_skills), [`_handle_agent_workflow`](special_commands.md#_handle_agent_workflow), [`_handle_check_constraints`](special_commands.md#_handle_check_constraints), [`_execute_nav_facade`](nav_special_commands.md#_execute_nav_facade), [`_handle_affected`](special_commands.md#_handle_affected), [`_handle_autoindex`](special_commands.md#_handle_autoindex), [`_handle_clean_state`](special_commands.md#_handle_clean_state), [`_handle_codegraph_metrics`](special_commands.md#_handle_codegraph_metrics), [`_handle_full_index`](special_commands.md#_handle_full_index), [`_handle_incremental_sync`](special_commands.md#_handle_incremental_sync), [`_dispatch_co_change`](nav_special_commands.md#_dispatch_co_change), [`_dispatch_test_map`](nav_special_commands.md#_dispatch_test_map), [`_handle_nav_actions_lazy`](special_commands.md#_handle_nav_actions_lazy), [`_handle_watch_health`](special_commands.md#_handle_watch_health), [`_resolve_outline_file`](special_commands.md#_resolve_outline_file)  (20 test-only)

## Functions
- `_effective_output_format(args: Any)` — [`L143`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/special_commands.py#L143) — Return the user-visible output format.
- `_emit_cli_error(args: Any, context: SpecialCommandContext, flag_name: str, message: str, *, error_type: str = "validation")` — [`L312`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/special_commands.py#L312) — r37al (dogfood): emit error in JSON envelope when caller asked for JSON.
- `_emit_show_common_queries(args: Any, context: SpecialCommandContext)` — [`L764`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/special_commands.py#L764) — Emit ``--show-common-queries`` in the active JSON-or-text format.
- `_emit_show_query_languages(args: Any, context: SpecialCommandContext)` — [`L720`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/special_commands.py#L720) — Emit ``--show-query-languages`` in the active JSON-or-text format.
- `_handle_affected(args: Any, context: SpecialCommandContext)` — [`L599`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/special_commands.py#L599) — Dispatch ``--affected FILE [FILE...]`` (CodeGraph CLI parity).
- `_handle_agent_skills(args: Any, context: SpecialCommandContext)` — [`L104`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/special_commands.py#L104) — Return the project-local agent skill inventory.
- `_handle_agent_workflow(args: Any, context: SpecialCommandContext)` — [`L122`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/special_commands.py#L122) — Return the SMART workflow pack as a structured CLI response.
- `_handle_autoindex(args: Any, context: SpecialCommandContext)` — [`L525`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/special_commands.py#L525) — Dispatch ``--autoindex`` → ``codegraph_autoindex`` MCP tool.
- `_handle_batch_metrics(args: Any, context: SpecialCommandContext)` — [`L458`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/special_commands.py#L458) — Run the scale-analysis tool for batch metrics mode.
- `_handle_batch_partial_read(args: Any, context: SpecialCommandContext)` — [`L244`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/special_commands.py#L244) — Run the MCP read-partial tool for batch partial-read requests.
- `_handle_check_constraints(args: Any, context: SpecialCommandContext)` — [`L500`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/special_commands.py#L500) — Run the architectural-constraint DSL evaluator for ``--check-constraints``.
- `_handle_check_scale(args: Any, context: SpecialCommandContext)` — [`L348`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/special_commands.py#L348) — Run AnalyzeScaleTool for a single file (``--check-scale FILE``).
- `_handle_clean_state(args: Any, context: SpecialCommandContext)` — [`L584`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/special_commands.py#L584) — Dispatch ``--clean-state`` / ``--clean-state-dry-run``.
- `_handle_codegraph_metrics(args: Any, context: SpecialCommandContext)` — [`L549`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/special_commands.py#L549) — Dispatch ``--codegraph-metrics`` → ``codegraph_metrics`` MCP tool.
- `_handle_full_index(args: Any, context: SpecialCommandContext)` — [`L537`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/special_commands.py#L537) — Dispatch ``--full-index`` → ``codegraph_full_index`` MCP tool.
- `_handle_health_check(args: Any, context: SpecialCommandContext)` — [`L279`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/special_commands.py#L279) — Run the project health tool for --health-check.
- `_handle_incremental_sync(args: Any, context: SpecialCommandContext)` — [`L561`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/special_commands.py#L561) — Dispatch ``--incremental-sync`` → ``codegraph_incremental_sync`` MCP tool.
- `_handle_install_skills(args: Any, context: SpecialCommandContext)` — [`L67`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/special_commands.py#L67) — Run ``--install-skills`` / ``--install-skills-global``.
- `_handle_knowledge_graph_index(args: Any, context: SpecialCommandContext)` — [`L573`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/special_commands.py#L573) — Dispatch ``--knowledge-graph-index`` → ``codegraph_knowledge_index``.
- `_handle_mcp_commands(args: Any, context: SpecialCommandContext)` — [`L655`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/special_commands.py#L655) — Delegate MCP-equivalent CLI commands to the command table.
- `_handle_nav_actions_lazy(args: Any, context: SpecialCommandContext)` — [`L611`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/special_commands.py#L611) — Delegate --test-map/--co-change to nav_special_commands (lazy import
- `_handle_outline(args: Any, context: SpecialCommandContext)` — [`L412`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/special_commands.py#L412) — Run GetCodeOutlineTool for a single file (``--outline FILE``).
- `_handle_query_language_commands(args: Any, context: SpecialCommandContext)` — [`L702`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/special_commands.py#L702) — Handle query-language discovery commands.
- `_handle_sql_platform_commands(args: Any, context: SpecialCommandContext)` — [`L804`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/special_commands.py#L804) — Handle SQL platform compatibility commands.
- `_handle_watch_health(args: Any, context: SpecialCommandContext)` — [`L622`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/special_commands.py#L622) — Start the health-grade watching daemon (--watch-health).
- `_is_batch_partial_read(args: Any)` — [`L236`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/special_commands.py#L236) — Return True when partial-read batch mode is active.
- `_load_file_paths(args: Any)` — [`L217`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/special_commands.py#L217) — Load and de-duplicate file paths for batch metrics.
- `_load_requests_payload(args: Any)` — [`L196`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/special_commands.py#L196) — Load batch partial-read requests from inline JSON or a file.
- `_print_result(result: dict[str, Any], args: Any, output_json: OutputJsonFn)` — [`L155`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/special_commands.py#L155) — Print tool output in the requested visible format.
- `_resolve_outline_file(args: Any, context: SpecialCommandContext)` — [`L390`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/special_commands.py#L390) — Resolve --outline's file path; returns None (skip), str, or int(1).
- `_run_mcp_tool_sync(tool_cls: Callable[..., Any], payload: dict[str, Any], *, project_root: str, args: Any, context: SpecialCommandContext)` — [`L175`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/special_commands.py#L175) — Instantiate, sync-run, print, and map an MCP tool to a 0/1 exit code.
- `_tool_output_format(args: Any)` — [`L149`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/special_commands.py#L149) — Return the json/toon output format accepted by MCP-equivalent tools.
- `_validate_partial_read_options(args: Any, output_error: OutputMessageFn)` — [`L674`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/special_commands.py#L674) — Validate single-range partial-read options.
- `handle_special_commands(args: Any, context: SpecialCommandContext)` — [`L27`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/special_commands.py#L27) — Handle CLI commands that bypass the normal file-analysis command path.

## Module values
- `OutputJsonFn` — [`L11`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/special_commands.py#L11)
- `OutputMessageFn` — [`L12`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/special_commands.py#L12)

