---
title: 'Module: tree_sitter_analyzer/mcp/facade_map.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/facade_map.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.facade_map`/
symbols:
  LEGACY_TOOL_MAP.LEGACY_TOOL_MAP: LEGACY_TOOL_MAP.LEGACY_TOOL_MAP.
  NEW_ACTION_PARITY.NEW_ACTION_PARITY: NEW_ACTION_PARITY.NEW_ACTION_PARITY.
  FACADE_NAMES.FACADE_NAMES: FACADE_NAMES.FACADE_NAMES.
  is_legacy_name: is_legacy_name().
  legacy_to_facade: legacy_to_facade().
  is_facade_name: is_facade_name().
  SET_PROJECT_PATH_TOOL_NAME: SET_PROJECT_PATH_TOOL_NAME.
---
# Module: [`tree_sitter_analyzer/mcp/facade_map.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/facade_map.py)

## Functions
- `is_facade_name(name: str)` — [`L146`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/facade_map.py#L146) — True if ``name`` is one of the 8 live facade names.
- `is_legacy_name(name: str)` — [`L151`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/facade_map.py#L151) — True if ``name`` is a deprecated v1.x tool name shimmed by LEGACY_TOOL_MAP.
- `legacy_to_facade(name: str)` — [`L141`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/facade_map.py#L141) — Return ``(facade, action)`` for a legacy tool name, else ``None``.

## Module values
- `FACADE_NAMES` — [`L41`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/facade_map.py#L41)
- `LEGACY_TOOL_MAP` — [`L58`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/facade_map.py#L58)
- `NEW_ACTION_PARITY` — [`L172`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/facade_map.py#L172)
- `SET_PROJECT_PATH_TOOL_NAME` — [`L38`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/facade_map.py#L38)

