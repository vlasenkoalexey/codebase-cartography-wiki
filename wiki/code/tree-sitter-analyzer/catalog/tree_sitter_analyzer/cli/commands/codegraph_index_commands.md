---
title: 'Module: tree_sitter_analyzer/cli/commands/codegraph_index_commands.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/cli/commands/codegraph_index_commands.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.cli.commands.codegraph_index_commands`/
symbols:
  run_autoindex: run_autoindex().
  run_knowledge_graph_index: run_knowledge_graph_index().
  run_full_index: run_full_index().
  run_incremental_sync: run_incremental_sync().
  run_codegraph_metrics: run_codegraph_metrics().
  _project_root: _project_root().
  _print: _print().
  _exit_code_for: _exit_code_for().
  _output_format: _output_format().
  OutputErrorFn: OutputErrorFn.
  _autoindex_payload: _autoindex_payload().
  _full_index_payload: _full_index_payload().
  _incremental_sync_payload: _incremental_sync_payload().
  _knowledge_graph_index_payload: _knowledge_graph_index_payload().
  _metrics_payload: _metrics_payload().
  OutputJsonFn: OutputJsonFn.
---
# Module: [`tree_sitter_analyzer/cli/commands/codegraph_index_commands.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/codegraph_index_commands.py)

## Functions
- `_autoindex_payload(args: Any, output_format: str)` — [`L54`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/codegraph_index_commands.py#L54)
- `_exit_code_for(result: dict[str, Any])` — [`L50`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/codegraph_index_commands.py#L50)
- `_full_index_payload(args: Any, output_format: str)` — [`L62`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/codegraph_index_commands.py#L62)
- `_incremental_sync_payload(args: Any, output_format: str)` — [`L73`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/codegraph_index_commands.py#L73)
- `_knowledge_graph_index_payload(args: Any, output_format: str)` — [`L81`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/codegraph_index_commands.py#L81)
- `_metrics_payload(args: Any, output_format: str)` — [`L93`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/codegraph_index_commands.py#L93)
- `_output_format(args: Any)` — [`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/codegraph_index_commands.py#L31) — Map argparse-visible output format to MCP tool format.
- `_print(result: dict[str, Any], output_format: str)` — [`L42`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/codegraph_index_commands.py#L42) — Write the MCP tool response to stdout in the requested shape.
- `_project_root(args: Any)` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/codegraph_index_commands.py#L27)
- `run_autoindex(args: Any, output_error: OutputErrorFn)` — [`L101`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/codegraph_index_commands.py#L101) — Dispatch ``--autoindex`` → ``codegraph_autoindex`` MCP tool.
- `run_codegraph_metrics(args: Any, output_error: OutputErrorFn)` — [`L185`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/codegraph_index_commands.py#L185) — Dispatch ``--codegraph-metrics`` → ``codegraph_metrics`` MCP tool.
- `run_full_index(args: Any, output_error: OutputErrorFn)` — [`L121`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/codegraph_index_commands.py#L121) — Dispatch ``--full-index`` → ``codegraph_full_index`` MCP tool.
- `run_incremental_sync(args: Any, output_error: OutputErrorFn)` — [`L141`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/codegraph_index_commands.py#L141) — Dispatch ``--incremental-sync`` → ``codegraph_incremental_sync`` MCP tool.
- `run_knowledge_graph_index(args: Any, output_error: OutputErrorFn)` — [`L163`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/codegraph_index_commands.py#L163) — Dispatch ``--knowledge-graph-index`` → ``codegraph_knowledge_index``.

## Module values
- `OutputErrorFn` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/codegraph_index_commands.py#L24)
- `OutputJsonFn` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/codegraph_index_commands.py#L23)

