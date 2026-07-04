---
title: 'Module: tree_sitter_analyzer/mcp/tools/parser_readiness_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/parser_readiness_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.parser_readiness_tool`/
symbols:
  ParserReadinessTool.execute: ParserReadinessTool#execute().
  ParserReadinessTool: ParserReadinessTool#
  ParserReadinessTool.validate_arguments: ParserReadinessTool#validate_arguments().
  ParserReadinessTool.get_tool_definition: ParserReadinessTool#get_tool_definition().
  ParserReadinessTool.get_tool_schema: ParserReadinessTool#get_tool_schema().
  TOOL_SCHEMA.TOOL_SCHEMA: TOOL_SCHEMA.TOOL_SCHEMA.
  _LANG_NAME_RE: _LANG_NAME_RE.
  _build_toon_response: _build_toon_response().
---
# Module: [`tree_sitter_analyzer/mcp/tools/parser_readiness_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/parser_readiness_tool.py)

## Classes
### `ParserReadinessTool`  ·  implements/extends BaseMCPTool
- def: [`tree_sitter_analyzer/mcp/tools/parser_readiness_tool.py:41`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/parser_readiness_tool.py#L41)
- doc: MCP tool that ranks language parser/plugin readiness.
- signature: `class ParserReadinessTool(BaseMCPTool):`
- members:
  - `execute(self, arguments: dict[str, Any])` — [`L98`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/parser_readiness_tool.py#L98) — Build parser readiness advice from local project metadata.
  - `get_tool_definition(self)` — [`L44`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/parser_readiness_tool.py#L44) — Return the MCP tool name, description, and input schema.
  - `get_tool_schema(self)` — [`L67`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/parser_readiness_tool.py#L67) — Return the JSON schema for tool input validation.
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L71`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/parser_readiness_tool.py#L71) — Validate optional language, include flag, and output format.
- uses (calls/refs, reference-scoped): [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`project_root`](base_tool.md#BaseMCPTool.project_root), [`build_parser_readiness_advice`](../../cli/parser_readiness.md#build_parser_readiness_advice), [`TOOL_SCHEMA`](parser_readiness_tool.md#TOOL_SCHEMA.TOOL_SCHEMA), [`_LANG_NAME_RE`](parser_readiness_tool.md#_LANG_NAME_RE), [`_build_toon_response`](parser_readiness_tool.md#_build_toon_response)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments), [`build_project_facade`](project_facade.md#build_project_facade), [`attach_tool_aliases`](../_server_helpers.md#attach_tool_aliases)  (13 test-only)

## Functions
- `_build_toon_response(result: dict[str, Any])` — [`L118`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/parser_readiness_tool.py#L118) — Return a compact MCP response when callers request TOON output.

## Module values
- `TOOL_SCHEMA` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/parser_readiness_tool.py#L18)
- `_LANG_NAME_RE` — [`L16`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/parser_readiness_tool.py#L16)

