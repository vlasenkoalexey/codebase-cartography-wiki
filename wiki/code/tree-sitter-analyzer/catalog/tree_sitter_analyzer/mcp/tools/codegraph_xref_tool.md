---
title: 'Module: tree_sitter_analyzer/mcp/tools/codegraph_xref_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/codegraph_xref_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.codegraph_xref_tool`/
symbols:
  CodeGraphXRefTool.execute: CodeGraphXRefTool#execute().
  CodeGraphXRefTool: CodeGraphXRefTool#
  CodeGraphXRefTool._get_cache: CodeGraphXRefTool#_get_cache().
  CodeGraphXRefTool._cache: CodeGraphXRefTool#_cache.
  logger: logger.
  CodeGraphXRefTool.__init__: CodeGraphXRefTool#__init__().
  CodeGraphXRefTool._on_project_root_changed: CodeGraphXRefTool#_on_project_root_changed().
  CodeGraphXRefTool.get_tool_definition: CodeGraphXRefTool#get_tool_definition().
  CodeGraphXRefTool.get_tool_schema: CodeGraphXRefTool#get_tool_schema().
  CodeGraphXRefTool.validate_arguments: CodeGraphXRefTool#validate_arguments().
---
# Module: [`tree_sitter_analyzer/mcp/tools/codegraph_xref_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_xref_tool.py)

## Classes
### `CodeGraphXRefTool`  ·  implements/extends BaseMCPTool
- def: [`tree_sitter_analyzer/mcp/tools/codegraph_xref_tool.py:29`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_xref_tool.py#L29)
- doc: MCP Tool for instant cross-reference queries (CodeGraph parity).
- signature: `class CodeGraphXRefTool(BaseMCPTool):`
- members:
  - `execute(self, arguments: dict[str, Any])` — [`L129`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_xref_tool.py#L129)
  - `get_tool_definition(self)` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_xref_tool.py#L48)
  - `get_tool_schema(self)` — [`L67`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_xref_tool.py#L67)
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L119`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_xref_tool.py#L119)
- protocol/private: `__init__`[`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_xref_tool.py#L32), `_cache`[`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_xref_tool.py#L33), `_get_cache`[`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_xref_tool.py#L39), `_on_project_root_changed`[`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_xref_tool.py#L36)
- uses (calls/refs, reference-scoped): [`ASTCache`](../../ast_cache.md#ASTCache), [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`project_root`](base_tool.md#BaseMCPTool.project_root), [`apply_toon_format_to_response`](../utils/format_helper.md#apply_toon_format_to_response), [`build_response`](_response_builder.md#build_response), [`__init__`](base_tool.md#BaseMCPTool.__init__), [`xref`](../../xref.md#XRefEngine.xref), [`file_xref`](../../xref.md#XRefEngine.file_xref), [`XRefEngine`](../../xref.md#XRefEngine), [`to_dict`](../../xref.md#XRefResult.to_dict), [`definitions`](../../xref.md#XRefResult.definitions), [`callees`](../../xref.md#XRefResult.callees), [`callers`](../../xref.md#XRefResult.callers)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments), [`build_nav_facade`](nav_facade.md#build_nav_facade), [`_on_project_root_changed`](base_tool.md#BaseMCPTool._on_project_root_changed)  (2 test-only)

## Module values
- `logger` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_xref_tool.py#L26)

