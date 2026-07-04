---
title: 'Module: tree_sitter_analyzer/mcp/tools/doc_sync_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/doc_sync_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.doc_sync_tool`/
symbols:
  DocSyncTool: DocSyncTool#
  DocSyncTool.execute: DocSyncTool#execute().
  logger: logger.
  DocSyncTool.get_tool_definition: DocSyncTool#get_tool_definition().
  DocSyncTool.get_tool_schema: DocSyncTool#get_tool_schema().
  DocSyncTool._to_toon: DocSyncTool#_to_toon().
  DocSyncTool.validate_arguments: DocSyncTool#validate_arguments().
---
# Module: [`tree_sitter_analyzer/mcp/tools/doc_sync_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/doc_sync_tool.py)

## Classes
### `DocSyncTool`  ·  implements/extends BaseMCPTool
- def: [`tree_sitter_analyzer/mcp/tools/doc_sync_tool.py:12`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/doc_sync_tool.py#L12)
- doc: MCP Tool: check documentation files for stale file-path references.
- signature: `class DocSyncTool(BaseMCPTool):`
- members:
  - `execute(self, arguments: dict[str, Any])` — [`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/doc_sync_tool.py#L65)
  - `get_tool_definition(self)` — [`L15`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/doc_sync_tool.py#L15)
  - `get_tool_schema(self)` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/doc_sync_tool.py#L36)
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L59`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/doc_sync_tool.py#L59)
- protocol/private: `_to_toon`[`L114`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/doc_sync_tool.py#L114)
- uses (calls/refs, reference-scoped): [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`project_root`](base_tool.md#BaseMCPTool.project_root), [`run_doc_sync`](../../doc_sync.md#run_doc_sync)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments), [`build_project_facade`](project_facade.md#build_project_facade)  (1 test-only)

## Module values
- `logger` — [`L9`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/doc_sync_tool.py#L9)

