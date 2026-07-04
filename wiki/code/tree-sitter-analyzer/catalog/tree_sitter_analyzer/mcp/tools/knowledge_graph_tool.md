---
title: 'Module: tree_sitter_analyzer/mcp/tools/knowledge_graph_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/knowledge_graph_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.knowledge_graph_tool`/
symbols:
  CodeGraphKnowledgeIndexTool.execute: CodeGraphKnowledgeIndexTool#execute().
  CodeGraphKnowledgeGraphTool.execute: CodeGraphKnowledgeGraphTool#execute().
  _snapshot_from_payload: _snapshot_from_payload().
  CodeGraphKnowledgeIndexTool._prepare_index: CodeGraphKnowledgeIndexTool#_prepare_index().
  CodeGraphKnowledgeIndexTool: CodeGraphKnowledgeIndexTool#
  CodeGraphKnowledgeGraphTool: CodeGraphKnowledgeGraphTool#
  CodeGraphKnowledgeGraphTool.validate_arguments: CodeGraphKnowledgeGraphTool#validate_arguments().
  CodeGraphKnowledgeGraphTool.get_tool_schema: CodeGraphKnowledgeGraphTool#get_tool_schema().
  CodeGraphKnowledgeIndexTool.validate_arguments: CodeGraphKnowledgeIndexTool#validate_arguments().
  _compact_sync_report: _compact_sync_report().
  CodeGraphKnowledgeIndexTool.get_tool_schema: CodeGraphKnowledgeIndexTool#get_tool_schema().
  CodeGraphKnowledgeIndexTool.get_tool_definition: CodeGraphKnowledgeIndexTool#get_tool_definition().
  CodeGraphKnowledgeGraphTool.get_tool_definition: CodeGraphKnowledgeGraphTool#get_tool_definition().
  _BACKENDS: _BACKENDS.
  _EXPORT_FORMATS: _EXPORT_FORMATS.
  _LOD_LEVELS: _LOD_LEVELS.
---
# Module: [`tree_sitter_analyzer/mcp/tools/knowledge_graph_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/knowledge_graph_tool.py)

## Classes
### `CodeGraphKnowledgeGraphTool`  ·  implements/extends BaseMCPTool
- def: [`tree_sitter_analyzer/mcp/tools/knowledge_graph_tool.py:174`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/knowledge_graph_tool.py#L174)
- doc: Read/export the materialized project knowledge graph.
- signature: `class CodeGraphKnowledgeGraphTool(BaseMCPTool):`
- members:
  - `execute(self, arguments: dict[str, Any])` — [`L245`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/knowledge_graph_tool.py#L245)
  - `get_tool_definition(self)` — [`L177`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/knowledge_graph_tool.py#L177)
  - `get_tool_schema(self)` — [`L195`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/knowledge_graph_tool.py#L195)
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L234`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/knowledge_graph_tool.py#L234)
- uses (calls/refs, reference-scoped): [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`project_root`](base_tool.md#BaseMCPTool.project_root), [`apply_toon_format_to_response`](../utils/format_helper.md#apply_toon_format_to_response), [`build_response`](_response_builder.md#build_response), [`to_graphology`](../../knowledge_graph/exporters.md#to_graphology), [`build_error`](_response_builder.md#build_error), [`_snapshot_from_payload`](knowledge_graph_tool.md#_snapshot_from_payload), [`summarize`](../../knowledge_graph/exporters.md#summarize), [`JsonKnowledgeGraphStore`](../../knowledge_graph/stores.md#JsonKnowledgeGraphStore), [`exists`](../../knowledge_graph/stores.md#JsonKnowledgeGraphStore.exists), [`read`](../../knowledge_graph/stores.md#JsonKnowledgeGraphStore.read), [`to_html_viewer`](../../knowledge_graph/html_viewer.md#to_html_viewer), [`_EXPORT_FORMATS`](knowledge_graph_tool.md#_EXPORT_FORMATS), [`_LOD_LEVELS`](knowledge_graph_tool.md#_LOD_LEVELS)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments), [`build_viz_facade`](viz_facade.md#build_viz_facade)  (6 test-only)

### `CodeGraphKnowledgeIndexTool`  ·  implements/extends BaseMCPTool
- def: [`tree_sitter_analyzer/mcp/tools/knowledge_graph_tool.py:26`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/knowledge_graph_tool.py#L26)
- doc: Build/update the materialized project knowledge graph.
- signature: `class CodeGraphKnowledgeIndexTool(BaseMCPTool):`
- members:
  - `execute(self, arguments: dict[str, Any])` — [`L101`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/knowledge_graph_tool.py#L101)
  - `get_tool_definition(self)` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/knowledge_graph_tool.py#L29)
  - `get_tool_schema(self)` — [`L47`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/knowledge_graph_tool.py#L47)
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L92`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/knowledge_graph_tool.py#L92)
- protocol/private: `_prepare_index`[`L155`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/knowledge_graph_tool.py#L155)
- uses (calls/refs, reference-scoped): [`ASTCache`](../../ast_cache.md#ASTCache), [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`project_root`](base_tool.md#BaseMCPTool.project_root), [`apply_toon_format_to_response`](../utils/format_helper.md#apply_toon_format_to_response), [`close`](../../ast_cache.md#ASTCache.close), [`index_project`](../../ast_cache.md#ASTCache.index_project), [`build_response`](_response_builder.md#build_response), [`write`](../../knowledge_graph/stores.md#LadybugKnowledgeGraphStore.write), [`build`](../../knowledge_graph/builder.md#KnowledgeGraphBuilder.build), [`sync`](../../incremental_sync.md#IncrementalSync.sync), [`IncrementalSync`](../../incremental_sync.md#IncrementalSync), [`build_error`](_response_builder.md#build_error), [`to_dict`](../../incremental_sync.md#SyncResult.to_dict), [`write`](../../knowledge_graph/stores.md#JsonKnowledgeGraphStore.write), [`summarize`](../../knowledge_graph/exporters.md#summarize), [`KnowledgeGraphBuilder`](../../knowledge_graph/builder.md#KnowledgeGraphBuilder), [`JsonKnowledgeGraphStore`](../../knowledge_graph/stores.md#JsonKnowledgeGraphStore), [`status`](../../knowledge_graph/stores.md#JsonKnowledgeGraphStore.status), [`status`](../../knowledge_graph/stores.md#LadybugKnowledgeGraphStore.status), [`LadybugKnowledgeGraphStore`](../../knowledge_graph/stores.md#LadybugKnowledgeGraphStore), [`LadybugUnavailableError`](../../knowledge_graph/stores.md#LadybugUnavailableError), [`_compact_sync_report`](knowledge_graph_tool.md#_compact_sync_report), [`_BACKENDS`](knowledge_graph_tool.md#_BACKENDS)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments), [`build_index_facade`](index_facade.md#build_index_facade), [`run_knowledge_graph_index`](../../cli/commands/codegraph_index_commands.md#run_knowledge_graph_index)  (5 test-only)

## Functions
- `_compact_sync_report(report: dict[str, Any])` — [`L324`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/knowledge_graph_tool.py#L324) — Drop per-file details from CLI/MCP responses; counts are enough here.
- `_snapshot_from_payload(payload: dict[str, Any])` — [`L299`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/knowledge_graph_tool.py#L299)

## Module values
- `_BACKENDS` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/knowledge_graph_tool.py#L21)
- `_EXPORT_FORMATS` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/knowledge_graph_tool.py#L22)
- `_LOD_LEVELS` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/knowledge_graph_tool.py#L23)

