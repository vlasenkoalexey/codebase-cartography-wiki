---
title: 'Module: tree_sitter_analyzer/mcp/tools/codegraph_sitemap_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/codegraph_sitemap_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.codegraph_sitemap_tool`/
symbols:
  CodeGraphSitemapTool.execute: CodeGraphSitemapTool#execute().
  CodeGraphSitemapTool: CodeGraphSitemapTool#
  CodeGraphSitemapTool.validate_arguments: CodeGraphSitemapTool#validate_arguments().
  CodeGraphSitemapTool._build_full_map: CodeGraphSitemapTool#_build_full_map().
  CodeGraphSitemapTool._get_cache: CodeGraphSitemapTool#_get_cache().
  DEFAULT_MAX_SYMBOLS: DEFAULT_MAX_SYMBOLS.
  CodeGraphSitemapTool._clean_tree: CodeGraphSitemapTool#_clean_tree().
  CodeGraphSitemapTool._build_module_metrics: CodeGraphSitemapTool#_build_module_metrics().
  CodeGraphSitemapTool._cache: CodeGraphSitemapTool#_cache.
  CodeGraphSitemapTool.get_tool_definition: CodeGraphSitemapTool#get_tool_definition().
  CodeGraphSitemapTool.get_tool_schema: CodeGraphSitemapTool#get_tool_schema().
  CodeGraphSitemapTool._build_api_surface: CodeGraphSitemapTool#_build_api_surface().
  CodeGraphSitemapTool._build_flat: CodeGraphSitemapTool#_build_flat().
  logger: logger.
  CodeGraphSitemapTool.__init__: CodeGraphSitemapTool#__init__().
  CodeGraphSitemapTool._on_project_root_changed: CodeGraphSitemapTool#_on_project_root_changed().
  _path_parts: _path_parts().
  CodeGraphSitemapTool._load_indexed_files: CodeGraphSitemapTool#_load_indexed_files().
  CodeGraphSitemapTool._class_members: CodeGraphSitemapTool#_class_members().
---
# Module: [`tree_sitter_analyzer/mcp/tools/codegraph_sitemap_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_sitemap_tool.py)

## Classes
### `CodeGraphSitemapTool`  ·  implements/extends BaseMCPTool
- def: [`tree_sitter_analyzer/mcp/tools/codegraph_sitemap_tool.py:45`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_sitemap_tool.py#L45)
- doc: MCP Tool for hierarchical project code map (CodeGraph parity).
- signature: `class CodeGraphSitemapTool(BaseMCPTool):`
- members:
  - `execute(self, arguments: dict[str, Any])` — [`L146`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_sitemap_tool.py#L146)
  - `get_tool_definition(self)` — [`L64`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_sitemap_tool.py#L64)
  - `get_tool_schema(self)` — [`L85`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_sitemap_tool.py#L85)
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L132`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_sitemap_tool.py#L132)
- protocol/private: `__init__`[`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_sitemap_tool.py#L48), `_build_api_surface`[`L347`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_sitemap_tool.py#L347), `_build_flat`[`L436`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_sitemap_tool.py#L436), `_build_full_map`[`L287`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_sitemap_tool.py#L287), `_build_module_metrics`[`L395`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_sitemap_tool.py#L395), `_cache`[`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_sitemap_tool.py#L49), `_class_members`[`L331`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_sitemap_tool.py#L331), `_clean_tree`[`L336`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_sitemap_tool.py#L336), `_get_cache`[`L55`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_sitemap_tool.py#L55), `_load_indexed_files`[`L228`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_sitemap_tool.py#L228), `_on_project_root_changed`[`L52`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_sitemap_tool.py#L52)
- uses (calls/refs, reference-scoped): [`ASTCache`](../../ast_cache.md#ASTCache), [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`project_root`](base_tool.md#BaseMCPTool.project_root), [`apply_toon_format_to_response`](../utils/format_helper.md#apply_toon_format_to_response), [`build_response`](_response_builder.md#build_response), [`__init__`](base_tool.md#BaseMCPTool.__init__), [`invalid_enum_error`](_validators.md#invalid_enum_error), [`_validate_positive_int`](_validators.md#_validate_positive_int), [`DEFAULT_MAX_SYMBOLS`](codegraph_sitemap_tool.md#DEFAULT_MAX_SYMBOLS), [`_path_parts`](codegraph_sitemap_tool.md#_path_parts)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments), [`_on_project_root_changed`](base_tool.md#BaseMCPTool._on_project_root_changed), [`build_structure_facade`](structure_facade.md#build_structure_facade)  (25 test-only)

## Functions
- `_path_parts(file_path: str)` — [`L41`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_sitemap_tool.py#L41)

## Module values
- `DEFAULT_MAX_SYMBOLS` — [`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_sitemap_tool.py#L38)
- `logger` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_sitemap_tool.py#L32)

