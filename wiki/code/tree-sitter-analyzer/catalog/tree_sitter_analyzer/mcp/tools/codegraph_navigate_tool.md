---
title: 'Module: tree_sitter_analyzer/mcp/tools/codegraph_navigate_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/codegraph_navigate_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.codegraph_navigate_tool`/
symbols:
  CodeGraphNavigateTool._call_hierarchy: CodeGraphNavigateTool#_call_hierarchy().
  CodeGraphNavigateTool._resolve_definition: CodeGraphNavigateTool#_resolve_definition().
  CodeGraphNavigateTool._find_references: CodeGraphNavigateTool#_find_references().
  CodeGraphNavigateTool.execute: CodeGraphNavigateTool#execute().
  CodeGraphNavigateTool: CodeGraphNavigateTool#
  _MAX_LISTED: _MAX_LISTED.
  CodeGraphNavigateTool._get_call_graph: CodeGraphNavigateTool#_get_call_graph().
  CodeGraphNavigateTool._inline_definition_bodies: CodeGraphNavigateTool#_inline_definition_bodies().
  CodeGraphNavigateTool._try_get_cache: CodeGraphNavigateTool#_try_get_cache().
  _transitive_callers: _transitive_callers().
  _transitive_callees: _transitive_callees().
  CodeGraphNavigateTool._call_graph: CodeGraphNavigateTool#_call_graph.
  CodeGraphNavigateTool._cache: CodeGraphNavigateTool#_cache.
  CodeGraphNavigateTool._get_cache: CodeGraphNavigateTool#_get_cache().
  logger: logger.
  CodeGraphNavigateTool.get_call_graph: CodeGraphNavigateTool#get_call_graph().
  CodeGraphNavigateTool.get_cache: CodeGraphNavigateTool#get_cache().
  CodeGraphNavigateTool._on_project_root_changed: CodeGraphNavigateTool#_on_project_root_changed().
  CodeGraphNavigateTool.call_graph_initialized: CodeGraphNavigateTool#call_graph_initialized().
  CodeGraphNavigateTool.cache_initialized: CodeGraphNavigateTool#cache_initialized().
  CodeGraphNavigateTool.get_tool_definition: CodeGraphNavigateTool#get_tool_definition().
  _MAX_TRANSITIVE: _MAX_TRANSITIVE.
  CodeGraphNavigateTool.get_tool_schema: CodeGraphNavigateTool#get_tool_schema().
  CodeGraphNavigateTool.validate_arguments: CodeGraphNavigateTool#validate_arguments().
  CodeGraphNavigateTool.__init__: CodeGraphNavigateTool#__init__().
---
# Module: [`tree_sitter_analyzer/mcp/tools/codegraph_navigate_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_navigate_tool.py)

## Classes
### `CodeGraphNavigateTool`  ·  implements/extends BaseMCPTool
- def: [`tree_sitter_analyzer/mcp/tools/codegraph_navigate_tool.py:39`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_navigate_tool.py#L39)
- doc: MCP Tool for unified symbol navigation (CodeGraph parity).
- signature: `class CodeGraphNavigateTool(BaseMCPTool):`
- members:
  - `_inline_definition_bodies(self, result: dict[str, Any])` — [`L238`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_navigate_tool.py#L238) — P2: attach a verbatim source body to each definition record.
  - `cache_initialized(self)` — [`L96`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_navigate_tool.py#L96) — True if the AST cache has been lazily initialized (i.e. cached).
  - `call_graph_initialized(self)` — [`L91`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_navigate_tool.py#L91) — True if the call graph has been lazily initialized (i.e. cached).
  - `execute(self, arguments: dict[str, Any])` — [`L168`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_navigate_tool.py#L168)
  - `get_cache(self)` — [`L86`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_navigate_tool.py#L86) — Public alias for _get_cache() — use this instead of replacing _get_cache.
  - `get_call_graph(self)` — [`L82`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_navigate_tool.py#L82) — Public alias for _get_call_graph() — use this instead of accessing _call_graph.
  - `get_tool_definition(self)` — [`L100`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_navigate_tool.py#L100)
  - `get_tool_schema(self)` — [`L123`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_navigate_tool.py#L123)
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L163`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_navigate_tool.py#L163)
- protocol/private: `__init__`[`L42`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_navigate_tool.py#L42), `_cache`[`L44`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_navigate_tool.py#L44), `_call_graph`[`L43`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_navigate_tool.py#L43), `_call_hierarchy`[`L312`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_navigate_tool.py#L312), `_find_references`[`L293`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_navigate_tool.py#L293), `_get_cache`[`L66`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_navigate_tool.py#L66), `_get_call_graph`[`L71`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_navigate_tool.py#L71), `_on_project_root_changed`[`L47`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_navigate_tool.py#L47), `_resolve_definition`[`L273`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_navigate_tool.py#L273), `_try_get_cache`[`L51`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_navigate_tool.py#L51)
- uses (calls/refs, reference-scoped): [`ASTCache`](../../ast_cache.md#ASTCache), [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`project_root`](base_tool.md#BaseMCPTool.project_root), [`apply_toon_format_to_response`](../utils/format_helper.md#apply_toon_format_to_response), [`close`](../../ast_cache.md#ASTCache.close), [`CallGraph`](../../call_graph.md#CallGraph), [`build`](../../call_graph.md#CallGraph.build), [`CachedCallGraph`](../../call_graph.md#CachedCallGraph), [`__init__`](base_tool.md#BaseMCPTool.__init__), [`get_stats`](../../ast_cache.md#ASTCache.get_stats), [`callees_of`](../../call_graph.md#CallGraph.callees_of), [`definitions`](../../symbol_resolver.md#ResolveResult.definitions), [`callers_of`](../../call_graph.md#CallGraph.callers_of), [`to_dict`](../../symbol_resolver.md#DefinitionLocation.to_dict), [`SymbolResolver`](../../symbol_resolver.md#SymbolResolver), [`resolve`](../../symbol_resolver.md#SymbolResolver.resolve), [`find_references`](../../symbol_resolver.md#SymbolResolver.find_references), [`to_dict`](../../symbol_resolver.md#ReferenceLocation.to_dict), [`_MAX_LISTED`](codegraph_navigate_tool.md#_MAX_LISTED), [`inline_symbol_body`](symbol_body_inline.md#inline_symbol_body), [`references`](../../symbol_resolver.md#ResolveResult.references), [`_transitive_callees`](codegraph_navigate_tool.md#_transitive_callees), [`_transitive_callers`](codegraph_navigate_tool.md#_transitive_callers), [`logger`](codegraph_navigate_tool.md#logger), [`resolved_via`](../../symbol_resolver.md#ResolveResult.resolved_via), [`NAVIGATE_DETERRENT`](symbol_body_inline.md#NAVIGATE_DETERRENT)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments), [`build_nav_facade`](nav_facade.md#build_nav_facade), [`_on_project_root_changed`](base_tool.md#BaseMCPTool._on_project_root_changed)  (6 test-only)

## Functions
- `_transitive_callees(graph: CallGraph, symbol: str, file_path: str | None, max_depth: int)` — [`L413`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_navigate_tool.py#L413)
- `_transitive_callers(graph: CallGraph, symbol: str, file_path: str | None, max_depth: int)` — [`L380`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_navigate_tool.py#L380)

## Module values
- `_MAX_LISTED` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_navigate_tool.py#L36)
- `_MAX_TRANSITIVE` — [`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_navigate_tool.py#L31)
- `logger` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_navigate_tool.py#L29)

