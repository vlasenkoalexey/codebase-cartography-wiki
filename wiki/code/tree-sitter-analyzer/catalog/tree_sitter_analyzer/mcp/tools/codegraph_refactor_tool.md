---
title: 'Module: tree_sitter_analyzer/mcp/tools/codegraph_refactor_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/codegraph_refactor_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.codegraph_refactor_tool`/
symbols:
  CodeGraphRefactorTool.execute: CodeGraphRefactorTool#execute().
  CodeGraphRefactorTool._get_cache: CodeGraphRefactorTool#_get_cache().
  CodeGraphRefactorTool: CodeGraphRefactorTool#
  CodeGraphRefactorTool._cache: CodeGraphRefactorTool#_cache.
  logger: logger.
  CodeGraphRefactorTool.__init__: CodeGraphRefactorTool#__init__().
  CodeGraphRefactorTool._on_project_root_changed: CodeGraphRefactorTool#_on_project_root_changed().
  CodeGraphRefactorTool.get_tool_definition: CodeGraphRefactorTool#get_tool_definition().
  CodeGraphRefactorTool.get_tool_schema: CodeGraphRefactorTool#get_tool_schema().
  CodeGraphRefactorTool.validate_arguments: CodeGraphRefactorTool#validate_arguments().
---
# Module: [`tree_sitter_analyzer/mcp/tools/codegraph_refactor_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_refactor_tool.py)

## Classes
### `CodeGraphRefactorTool`  ·  implements/extends BaseMCPTool
- def: [`tree_sitter_analyzer/mcp/tools/codegraph_refactor_tool.py:29`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_refactor_tool.py#L29)
- doc: MCP Tool for AST-aware symbol renaming (CodeGraph parity).
- signature: `class CodeGraphRefactorTool(BaseMCPTool):`
- members:
  - `execute(self, arguments: dict[str, Any])` — [`L112`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_refactor_tool.py#L112)
  - `get_tool_definition(self)` — [`L47`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_refactor_tool.py#L47)
  - `get_tool_schema(self)` — [`L61`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_refactor_tool.py#L61)
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L93`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_refactor_tool.py#L93)
- protocol/private: `__init__`[`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_refactor_tool.py#L32), `_cache`[`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_refactor_tool.py#L33), `_get_cache`[`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_refactor_tool.py#L39), `_on_project_root_changed`[`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_refactor_tool.py#L36)
- uses (calls/refs, reference-scoped): [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`project_root`](base_tool.md#BaseMCPTool.project_root), [`apply_toon_format_to_response`](../utils/format_helper.md#apply_toon_format_to_response), [`__init__`](base_tool.md#BaseMCPTool.__init__), [`rename_symbol`](../../rename_symbol.md#rename_symbol), [`ensure_indexed`](../utils/auto_index_guard.md#ensure_indexed), [`file`](../../rename_symbol.md#RenameSite.file), [`to_dict`](../../rename_symbol.md#RenameResult.to_dict), [`sites`](../../rename_symbol.md#RenameResult.sites), [`files_changed`](../../rename_symbol.md#RenameResult.files_changed), [`errors`](../../rename_symbol.md#RenameResult.errors), [`sites_renamed`](../../rename_symbol.md#RenameResult.sites_renamed)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments), [`_on_project_root_changed`](base_tool.md#BaseMCPTool._on_project_root_changed)  (2 test-only)

## Module values
- `logger` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_refactor_tool.py#L26)

