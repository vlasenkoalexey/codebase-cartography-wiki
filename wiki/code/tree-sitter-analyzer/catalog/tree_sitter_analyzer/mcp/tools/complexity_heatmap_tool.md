---
title: 'Module: tree_sitter_analyzer/mcp/tools/complexity_heatmap_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/complexity_heatmap_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.complexity_heatmap_tool`/
symbols:
  CodeGraphComplexityHeatmapTool.execute: CodeGraphComplexityHeatmapTool#execute().
  CodeGraphComplexityHeatmapTool._execute_file: CodeGraphComplexityHeatmapTool#_execute_file().
  CodeGraphComplexityHeatmapTool._execute_function: CodeGraphComplexityHeatmapTool#_execute_function().
  CodeGraphComplexityHeatmapTool._get_cache: CodeGraphComplexityHeatmapTool#_get_cache().
  CodeGraphComplexityHeatmapTool._execute_project: CodeGraphComplexityHeatmapTool#_execute_project().
  CodeGraphComplexityHeatmapTool: CodeGraphComplexityHeatmapTool#
  CodeGraphComplexityHeatmapTool._analyze_file_cached: CodeGraphComplexityHeatmapTool#_analyze_file_cached().
  CodeGraphComplexityHeatmapTool.validate_arguments: CodeGraphComplexityHeatmapTool#validate_arguments().
  CodeGraphComplexityHeatmapTool.get_tool_definition: CodeGraphComplexityHeatmapTool#get_tool_definition().
  CodeGraphComplexityHeatmapTool._cache: CodeGraphComplexityHeatmapTool#_cache.
  logger: logger.
  CodeGraphComplexityHeatmapTool.__init__: CodeGraphComplexityHeatmapTool#__init__().
  CodeGraphComplexityHeatmapTool._on_project_root_changed: CodeGraphComplexityHeatmapTool#_on_project_root_changed().
  CodeGraphComplexityHeatmapTool.get_tool_schema: CodeGraphComplexityHeatmapTool#get_tool_schema().
---
# Module: [`tree_sitter_analyzer/mcp/tools/complexity_heatmap_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/complexity_heatmap_tool.py)

## Classes
### `CodeGraphComplexityHeatmapTool`  ·  implements/extends BaseMCPTool
- def: [`tree_sitter_analyzer/mcp/tools/complexity_heatmap_tool.py:36`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/complexity_heatmap_tool.py#L36)
- doc: MCP Tool for cyclomatic complexity heatmap (CodeGraph parity).
- signature: `class CodeGraphComplexityHeatmapTool(BaseMCPTool):`
- members:
  - `execute(self, arguments: dict[str, Any])` — [`L137`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/complexity_heatmap_tool.py#L137)
  - `get_tool_definition(self)` — [`L64`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/complexity_heatmap_tool.py#L64)
  - `get_tool_schema(self)` — [`L83`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/complexity_heatmap_tool.py#L83)
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L128`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/complexity_heatmap_tool.py#L128)
- protocol/private: `__init__`[`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/complexity_heatmap_tool.py#L39), `_analyze_file_cached`[`L293`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/complexity_heatmap_tool.py#L293), `_cache`[`L40`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/complexity_heatmap_tool.py#L40), `_execute_file`[`L191`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/complexity_heatmap_tool.py#L191), `_execute_function`[`L244`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/complexity_heatmap_tool.py#L244), `_execute_project`[`L155`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/complexity_heatmap_tool.py#L155), `_get_cache`[`L46`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/complexity_heatmap_tool.py#L46), `_on_project_root_changed`[`L43`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/complexity_heatmap_tool.py#L43)
- uses (calls/refs, reference-scoped): [`ASTCache`](../../ast_cache.md#ASTCache), [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`project_root`](base_tool.md#BaseMCPTool.project_root), [`apply_toon_format_to_response`](../utils/format_helper.md#apply_toon_format_to_response), [`close`](../../ast_cache.md#ASTCache.close), [`build_response`](_response_builder.md#build_response), [`_language_from_ext`](../../project_graph.md#_language_from_ext), [`analyze_project_heatmap`](../../complexity_heatmap.md#analyze_project_heatmap), [`__init__`](base_tool.md#BaseMCPTool.__init__), [`analyze_file_complexity`](../../complexity_heatmap.md#analyze_file_complexity), [`analyze_file_complexity_from_cache`](../../complexity_heatmap.md#analyze_file_complexity_from_cache), [`get_stats`](../../ast_cache.md#ASTCache.get_stats), [`build_error`](_response_builder.md#build_error), [`invalid_enum_error`](_validators.md#invalid_enum_error), [`_risk_band`](../../complexity_heatmap.md#_risk_band), [`RISK_BANDS`](../../complexity_heatmap.md#RISK_BANDS)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments), [`_on_project_root_changed`](base_tool.md#BaseMCPTool._on_project_root_changed), [`build_health_facade`](health_facade.md#build_health_facade)  (16 test-only)

## Module values
- `logger` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/complexity_heatmap_tool.py#L33)

