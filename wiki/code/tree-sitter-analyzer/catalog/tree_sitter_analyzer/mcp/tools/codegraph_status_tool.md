---
title: 'Module: tree_sitter_analyzer/mcp/tools/codegraph_status_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/codegraph_status_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.codegraph_status_tool`/
symbols:
  CodeGraphStatusTool.execute: CodeGraphStatusTool#execute().
  CodeGraphStatusTool: CodeGraphStatusTool#
  CodeGraphStatusTool._safe_get_stats: CodeGraphStatusTool#_safe_get_stats().
  CodeGraphStatusTool._newest_source_mtime: CodeGraphStatusTool#_newest_source_mtime().
  CodeGraphStatusTool._is_rebuilding: CodeGraphStatusTool#_is_rebuilding().
  logger: logger.
  _storage_fields: _storage_fields().
  CodeGraphStatusTool._compute_lag: CodeGraphStatusTool#_compute_lag().
  CodeGraphStatusTool.get_tool_definition: CodeGraphStatusTool#get_tool_definition().
  _LAG_WALK_FILE_CAP: _LAG_WALK_FILE_CAP.
  _LAG_SOURCE_EXTS: _LAG_SOURCE_EXTS.
  _LAG_SKIP_DIRS: _LAG_SKIP_DIRS.
  _DB_STORAGE_KEYS: _DB_STORAGE_KEYS.
  CodeGraphStatusTool.get_tool_schema: CodeGraphStatusTool#get_tool_schema().
  CodeGraphStatusTool.validate_arguments: CodeGraphStatusTool#validate_arguments().
---
# Module: [`tree_sitter_analyzer/mcp/tools/codegraph_status_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_status_tool.py)

## Classes
### `CodeGraphStatusTool`  ·  implements/extends BaseMCPTool
- def: [`tree_sitter_analyzer/mcp/tools/codegraph_status_tool.py:61`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_status_tool.py#L61)
- doc: MCP Tool for index health at-a-glance (CodeGraph parity).
- signature: `class CodeGraphStatusTool(BaseMCPTool):`
- members:
  - `_is_rebuilding(self)` — [`L253`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_status_tool.py#L253) — True while a full rebuild is replacing the cache (#578).
  - `execute(self, arguments: dict[str, Any])` — [`L112`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_status_tool.py#L112)
  - `get_tool_definition(self)` — [`L64`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_status_tool.py#L64)
  - `get_tool_schema(self)` — [`L84`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_status_tool.py#L84)
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L106`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_status_tool.py#L106)
- protocol/private: `_compute_lag`[`L304`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_status_tool.py#L304), `_newest_source_mtime`[`L317`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_status_tool.py#L317), `_safe_get_stats`[`L270`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_status_tool.py#L270)
- uses (calls/refs, reference-scoped): [`ASTCache`](../../ast_cache.md#ASTCache), [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`project_root`](base_tool.md#BaseMCPTool.project_root), [`apply_toon_format_to_response`](../utils/format_helper.md#apply_toon_format_to_response), [`close`](../../ast_cache.md#ASTCache.close), [`build_response`](_response_builder.md#build_response), [`get_stats`](../../ast_cache.md#ASTCache.get_stats), [`is_index_rebuilding`](index_rebuild_signal.md#is_index_rebuilding), [`is_indexed`](../utils/auto_index_guard.md#is_indexed), [`_storage_fields`](codegraph_status_tool.md#_storage_fields), [`logger`](codegraph_status_tool.md#logger), [`_LAG_SKIP_DIRS`](codegraph_status_tool.md#_LAG_SKIP_DIRS), [`_LAG_SOURCE_EXTS`](codegraph_status_tool.md#_LAG_SOURCE_EXTS), [`_LAG_WALK_FILE_CAP`](codegraph_status_tool.md#_LAG_WALK_FILE_CAP)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments), [`build_index_facade`](index_facade.md#build_index_facade)  (15 test-only)

## Functions
- `_storage_fields(stats: dict[str, Any] | None)` — [`L342`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_status_tool.py#L342)

## Module values
- `_DB_STORAGE_KEYS` — [`L51`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_status_tool.py#L51)
- `_LAG_SKIP_DIRS` — [`L34`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_status_tool.py#L34)
- `_LAG_SOURCE_EXTS` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_status_tool.py#L30)
- `_LAG_WALK_FILE_CAP` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_status_tool.py#L26)
- `logger` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_status_tool.py#L22)

