---
title: 'Module: tree_sitter_analyzer/mcp/tools/symbol_resolve_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/symbol_resolve_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.symbol_resolve_tool`/
symbols:
  CodeGraphSymbolResolveTool.execute: CodeGraphSymbolResolveTool#execute().
  CodeGraphSymbolResolveTool: CodeGraphSymbolResolveTool#
  CodeGraphSymbolResolveTool._get_cache: CodeGraphSymbolResolveTool#_get_cache().
  CodeGraphSymbolResolveTool.get_tool_schema: CodeGraphSymbolResolveTool#get_tool_schema().
  CodeGraphSymbolResolveTool._cache: CodeGraphSymbolResolveTool#_cache.
  CodeGraphSymbolResolveTool.get_tool_definition: CodeGraphSymbolResolveTool#get_tool_definition().
  CodeGraphSymbolResolveTool.validate_arguments: CodeGraphSymbolResolveTool#validate_arguments().
  logger: logger.
  CodeGraphSymbolResolveTool.__init__: CodeGraphSymbolResolveTool#__init__().
  CodeGraphSymbolResolveTool._on_project_root_changed: CodeGraphSymbolResolveTool#_on_project_root_changed().
  TOOL_SCHEMA.TOOL_SCHEMA: TOOL_SCHEMA.TOOL_SCHEMA.
---
# Module: [`tree_sitter_analyzer/mcp/tools/symbol_resolve_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_resolve_tool.py)

## Classes
### `CodeGraphSymbolResolveTool`  ·  implements/extends BaseMCPTool
- def: [`tree_sitter_analyzer/mcp/tools/symbol_resolve_tool.py:54`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_resolve_tool.py#L54)
- doc: MCP Tool for CodeGraph go-to-definition and find-all-references.
- signature: `class CodeGraphSymbolResolveTool(BaseMCPTool):`
- members:
  - `execute(self, arguments: dict[str, Any])` — [`L102`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_resolve_tool.py#L102)
  - `get_tool_definition(self)` — [`L73`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_resolve_tool.py#L73)
  - `get_tool_schema(self)` — [`L94`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_resolve_tool.py#L94)
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L97`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_resolve_tool.py#L97)
- protocol/private: `__init__`[`L57`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_resolve_tool.py#L57), `_cache`[`L58`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_resolve_tool.py#L58), `_get_cache`[`L64`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_resolve_tool.py#L64), `_on_project_root_changed`[`L61`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_resolve_tool.py#L61)
- uses (calls/refs, reference-scoped): [`ASTCache`](../../ast_cache.md#ASTCache), [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`project_root`](base_tool.md#BaseMCPTool.project_root), [`apply_toon_format_to_response`](../utils/format_helper.md#apply_toon_format_to_response), [`__init__`](base_tool.md#BaseMCPTool.__init__), [`definitions`](../../symbol_resolver.md#ResolveResult.definitions), [`to_dict`](../../symbol_resolver.md#DefinitionLocation.to_dict), [`SymbolResolver`](../../symbol_resolver.md#SymbolResolver), [`resolve`](../../symbol_resolver.md#SymbolResolver.resolve), [`find_references`](../../symbol_resolver.md#SymbolResolver.find_references), [`to_dict`](../../symbol_resolver.md#ReferenceLocation.to_dict), [`references`](../../symbol_resolver.md#ResolveResult.references), [`symbol`](../../symbol_resolver.md#ResolveResult.symbol), [`resolved_via`](../../symbol_resolver.md#ResolveResult.resolved_via), [`TOOL_SCHEMA`](symbol_resolve_tool.md#TOOL_SCHEMA.TOOL_SCHEMA)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments), [`build_nav_facade`](nav_facade.md#build_nav_facade), [`_on_project_root_changed`](base_tool.md#BaseMCPTool._on_project_root_changed)  (12 test-only)

## Module values
- `TOOL_SCHEMA` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_resolve_tool.py#L23)
- `logger` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_resolve_tool.py#L21)

