---
title: 'Module: tree_sitter_analyzer/mcp/legacy_shim.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/legacy_shim.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.legacy_shim`/
symbols:
  dispatch_legacy: dispatch_legacy().
  is_legacy_name: is_legacy_name().
  _emit_stderr_warning: _emit_stderr_warning().
  _deprecation_field: _deprecation_field().
  _LEGACY_EXTRA_ARGS._LEGACY_EXTRA_ARGS: _LEGACY_EXTRA_ARGS._LEGACY_EXTRA_ARGS.
---
# Module: [`tree_sitter_analyzer/mcp/legacy_shim.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/legacy_shim.py)

## Functions
- `_deprecation_field(old_name: str, facade: str, action: str)` — [`L58`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/legacy_shim.py#L58) — Channel 2 payload: the ``deprecation`` envelope field agents can read.
- `_emit_stderr_warning(old_name: str, facade: str, action: str)` — [`L45`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/legacy_shim.py#L45) — Channel 1: one-line stderr deprecation notice (CLAUDE.md §3 compliant).
- `dispatch_legacy(server: Any, name: str, arguments: dict[str, Any])` — [`L72`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/legacy_shim.py#L72) — Forward a legacy tool name to its facade and annotate the response.
- `is_legacy_name(name: str)` — [`L40`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/legacy_shim.py#L40) — True if ``name`` is a deprecated 1.x tool name with a facade route.

## Module values
- `_LEGACY_EXTRA_ARGS` — [`L35`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/legacy_shim.py#L35)

