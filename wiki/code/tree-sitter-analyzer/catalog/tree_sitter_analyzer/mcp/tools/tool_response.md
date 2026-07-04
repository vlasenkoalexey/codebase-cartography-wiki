---
title: 'Module: tree_sitter_analyzer/mcp/tools/tool_response.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/tool_response.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.tool_response`/
symbols:
  validate_tool_response: validate_tool_response().
  CANONICAL_VERDICTS.CANONICAL_VERDICTS: CANONICAL_VERDICTS.CANONICAL_VERDICTS.
  ToolResponse: ToolResponse#
  ToolResponse.success: ToolResponse#success.
  ToolResponse.verdict: ToolResponse#verdict.
  ToolResponse.error: ToolResponse#error.
  ToolResponse.mode: ToolResponse#mode.
  ToolResponse.toon_content: ToolResponse#toon_content.
  __all__: __all__.
---
# Module: [`tree_sitter_analyzer/mcp/tools/tool_response.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/tool_response.py)

## Classes
### `ToolResponse`  ·  implements/extends _TypedDict
- def: [`tree_sitter_analyzer/mcp/tools/tool_response.py:60`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/tool_response.py#L60)
- doc: The shape every MCP tool response should follow.
- signature: `class ToolResponse(TypedDict, total=False):`
- members:
  - `error` — [`L77`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/tool_response.py#L77) — ---
  - `mode` — [`L81`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/tool_response.py#L81) — ---
  - `success` — [`L68`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/tool_response.py#L68) — ---
  - `toon_content` — [`L85`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/tool_response.py#L85) — ---
  - `verdict` — [`L71`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/tool_response.py#L71) — ---

## Functions
- `validate_tool_response(payload: Any, tool_name: str = "<unknown>")` — [`L91`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/tool_response.py#L91) — Raise ``AssertionError`` if ``payload`` doesn't honour the

## Module values
- `CANONICAL_VERDICTS` — [`L46`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/tool_response.py#L46)
- `__all__` — [`L134`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/tool_response.py#L134)

