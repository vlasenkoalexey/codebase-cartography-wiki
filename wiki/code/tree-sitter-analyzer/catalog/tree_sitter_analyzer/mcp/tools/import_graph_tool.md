---
title: 'Module: tree_sitter_analyzer/mcp/tools/import_graph_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/import_graph_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.import_graph_tool`/
symbols:
  CodeGraphImportGraphTool.execute: CodeGraphImportGraphTool#execute().
  CodeGraphImportGraphTool: CodeGraphImportGraphTool#
  CodeGraphImportGraphTool._get_graph: CodeGraphImportGraphTool#_get_graph().
  CodeGraphImportGraphTool.validate_arguments: CodeGraphImportGraphTool#validate_arguments().
  CodeGraphImportGraphTool.__init__: CodeGraphImportGraphTool#__init__().
  CodeGraphImportGraphTool._effective_mode: CodeGraphImportGraphTool#_effective_mode().
  CodeGraphImportGraphTool._graph: CodeGraphImportGraphTool#_graph.
  CodeGraphImportGraphTool.get_tool_definition: CodeGraphImportGraphTool#get_tool_definition().
  logger: logger.
  CodeGraphImportGraphTool._on_project_root_changed: CodeGraphImportGraphTool#_on_project_root_changed().
  CodeGraphImportGraphTool.get_tool_schema: CodeGraphImportGraphTool#get_tool_schema().
  _imports_agent_summary: _imports_agent_summary().
---
# Module: [`tree_sitter_analyzer/mcp/tools/import_graph_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/import_graph_tool.py)

## Classes
### `CodeGraphImportGraphTool`  ·  implements/extends BaseMCPTool
- def: [`tree_sitter_analyzer/mcp/tools/import_graph_tool.py:26`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/import_graph_tool.py#L26)
- doc: MCP Tool for file-level import dependency analysis (CodeGraph parity).
- signature: `class CodeGraphImportGraphTool(BaseMCPTool):`
- members:
  - `_effective_mode(arguments: dict[str, Any])` — [`L106`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/import_graph_tool.py#L106) — #575: resolve the mode when omitted. A bare ``file_path`` means the
  - `execute(self, arguments: dict[str, Any])` — [`L134`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/import_graph_tool.py#L134)
  - `get_tool_definition(self)` — [`L43`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/import_graph_tool.py#L43)
  - `get_tool_schema(self)` — [`L63`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/import_graph_tool.py#L63)
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L116`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/import_graph_tool.py#L116)
- protocol/private: `__init__`[`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/import_graph_tool.py#L29), `_get_graph`[`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/import_graph_tool.py#L36), `_graph`[`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/import_graph_tool.py#L30), `_on_project_root_changed`[`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/import_graph_tool.py#L33)
- uses (calls/refs, reference-scoped): [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`project_root`](base_tool.md#BaseMCPTool.project_root), [`apply_toon_format_to_response`](../utils/format_helper.md#apply_toon_format_to_response), [`resolve_and_validate_file_path`](base_tool.md#BaseMCPTool.resolve_and_validate_file_path), [`__init__`](base_tool.md#BaseMCPTool.__init__), [`build`](../../import_graph.md#ImportGraph.build), [`invalid_enum_error`](_validators.md#invalid_enum_error), [`summary`](../../import_graph.md#ImportGraph.summary), [`blast_radius`](../../import_graph.md#ImportGraph.blast_radius), [`dependents_of`](../../import_graph.md#ImportGraph.dependents_of), [`dependencies_of`](../../import_graph.md#ImportGraph.dependencies_of), [`ImportGraph`](../../import_graph.md#ImportGraph), [`cycles`](../../import_graph.md#ImportGraphResult.cycles), [`_imports_agent_summary`](import_graph_tool.md#_imports_agent_summary)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments), [`_on_project_root_changed`](base_tool.md#BaseMCPTool._on_project_root_changed), [`build_health_facade`](health_facade.md#build_health_facade)  (8 test-only)

## Functions
- `_imports_agent_summary(mode: str, verdict: str, result: dict[str, Any])` — [`L241`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/import_graph_tool.py#L241) — Build a concise agent_summary block for codegraph_import_graph results.

## Module values
- `logger` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/import_graph_tool.py#L23)

