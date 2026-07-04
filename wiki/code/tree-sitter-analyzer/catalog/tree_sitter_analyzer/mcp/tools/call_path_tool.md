---
title: 'Module: tree_sitter_analyzer/mcp/tools/call_path_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/call_path_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.call_path_tool`/
symbols:
  CodeGraphCallPathTool.execute: CodeGraphCallPathTool#execute().
  CodeGraphCallPathTool: CodeGraphCallPathTool#
  CodeGraphCallPathTool._enrich_with_bodies: CodeGraphCallPathTool#_enrich_with_bodies().
  CodeGraphCallPathTool._get_finder: CodeGraphCallPathTool#_get_finder().
  CodeGraphCallPathTool._finder: CodeGraphCallPathTool#_finder.
  CodeGraphCallPathTool.__init__: CodeGraphCallPathTool#__init__().
  CodeGraphCallPathTool.get_tool_definition: CodeGraphCallPathTool#get_tool_definition().
  CodeGraphCallPathTool.validate_arguments: CodeGraphCallPathTool#validate_arguments().
  logger: logger.
  CodeGraphCallPathTool._on_project_root_changed: CodeGraphCallPathTool#_on_project_root_changed().
  CodeGraphCallPathTool.get_tool_schema: CodeGraphCallPathTool#get_tool_schema().
---
# Module: [`tree_sitter_analyzer/mcp/tools/call_path_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/call_path_tool.py)

## Classes
### `CodeGraphCallPathTool`  ·  implements/extends BaseMCPTool
- def: [`tree_sitter_analyzer/mcp/tools/call_path_tool.py:28`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/call_path_tool.py#L28)
- doc: MCP Tool for finding execution paths between two functions.
- signature: `class CodeGraphCallPathTool(BaseMCPTool):`
- members:
  - `_enrich_with_bodies(self, result_dict: dict[str, Any], paths: list[dict[str, Any]], source_function: str, target_function: str, source_file: str | None, target_file: str | None)` — [`L178`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/call_path_tool.py#L178) — Inline source bodies + a deterrent ``next_step`` into the envelope.
  - `execute(self, arguments: dict[str, Any])` — [`L125`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/call_path_tool.py#L125)
  - `get_tool_definition(self)` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/call_path_tool.py#L45)
  - `get_tool_schema(self)` — [`L63`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/call_path_tool.py#L63)
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L118`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/call_path_tool.py#L118)
- protocol/private: `__init__`[`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/call_path_tool.py#L31), `_finder`[`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/call_path_tool.py#L32), `_get_finder`[`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/call_path_tool.py#L38), `_on_project_root_changed`[`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/call_path_tool.py#L35)
- uses (calls/refs, reference-scoped): [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`project_root`](base_tool.md#BaseMCPTool.project_root), [`apply_toon_format_to_response`](../utils/format_helper.md#apply_toon_format_to_response), [`__init__`](base_tool.md#BaseMCPTool.__init__), [`paths`](../../call_path.md#CallPathResult.paths), [`find_path`](../../call_path.md#CallPathFinder.find_path), [`CallPathFinder`](../../call_path.md#CallPathFinder), [`inline_path_bodies`](call_path_enrich.md#inline_path_bodies), [`_try_get_cache`](../../call_path.md#CallPathFinder._try_get_cache), [`data_source`](../../call_path.md#CallPathResult.data_source), [`to_dict`](../../call_path.md#CallChain.to_dict), [`build_dead_end`](call_path_enrich.md#build_dead_end), [`truncated`](../../call_path.md#CallPathResult.truncated)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments), [`build_nav_facade`](nav_facade.md#build_nav_facade), [`_on_project_root_changed`](base_tool.md#BaseMCPTool._on_project_root_changed)  (4 test-only)

## Module values
- `logger` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/call_path_tool.py#L25)

