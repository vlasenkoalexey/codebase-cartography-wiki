---
title: 'Module: tree_sitter_analyzer/mcp/_server_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/_server_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp._server_helpers`/
symbols:
  attach_tool_aliases: attach_tool_aliases().
  resolve_project_root: resolve_project_root().
  build_initialization_options: build_initialization_options().
  _SERVER_INSTRUCTIONS: _SERVER_INSTRUCTIONS.
  init_universal_tool: init_universal_tool().
  detect_server_version: detect_server_version().
  _select_project_root: _select_project_root().
  _should_fallback_to_cwd: _should_fallback_to_cwd().
---
# Module: [`tree_sitter_analyzer/mcp/_server_helpers.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/_server_helpers.py)

## Functions
- `_select_project_root(cli_project_root: str | None, *, cwd_factory: Callable[[], Any], environ: Mapping[str, str], detect_project_root_func: Callable[[], str | None])` — [`L265`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/_server_helpers.py#L265) — Select a candidate project root using existing priority order.
- `_should_fallback_to_cwd(project_root: str | None, *, path_class: type[Any])` — [`L283`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/_server_helpers.py#L283) — Return whether a resolved project root is unusable.
- `attach_tool_aliases(target: Any, tools: Mapping[str, Any], project_root: str | None = None)` — [`L139`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/_server_helpers.py#L139) — Attach backward-compatible inner-tool attributes to the MCP server. — documented in [tree_sitter_analyzer-mcp-server](../../../concepts/tree_sitter_analyzer-mcp-server.md)
- `build_initialization_options(server_name: str, server_version: str, initialization_options_cls: type[Any])` — [`L12`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/_server_helpers.py#L12) — Build MCP initialization options without bloating the runtime method.
- `detect_server_version(base_version: str, *, platform_detector: type[Any], logger: Any)` — [`L218`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/_server_helpers.py#L218) — Return server version annotated with platform details when available.
- `init_universal_tool(project_root: str | None, *, universal_tool_available: bool, universal_tool_cls: type[Any] | None)` — [`L203`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/_server_helpers.py#L203) — Initialize the optional universal analysis tool.
- `resolve_project_root(cli_project_root: str | None, *, cwd_factory: Callable[[], Any] = Path.cwd, path_class: type[Any] = Path, environ: Mapping[str, str] = os.environ, detect_project_root_func: Callable[[], str | None], logger: Any)` — [`L237`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/_server_helpers.py#L237) — Resolve the MCP project root from CLI, environment, or auto-detection.

## Module values
- `_SERVER_INSTRUCTIONS` — [`L47`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/_server_helpers.py#L47)

