---
title: 'Module: tree_sitter_analyzer/mcp/tools/build_project_index_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/build_project_index_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.build_project_index_tool`/
symbols:
  BuildProjectIndexTool: BuildProjectIndexTool#
  BuildProjectIndexTool._do_execute: BuildProjectIndexTool#_do_execute().
  BuildProjectIndexTool.execute: BuildProjectIndexTool#execute().
  BuildProjectIndexTool.validate_arguments: BuildProjectIndexTool#validate_arguments().
  BuildProjectIndexTool.get_tool_definition: BuildProjectIndexTool#get_tool_definition().
  _validate_one_root: _validate_one_root().
  BuildProjectIndexTool.get_tool_schema: BuildProjectIndexTool#get_tool_schema().
  _boundary_error_msg: _boundary_error_msg().
  _security_error_response: _security_error_response().
  _internal_error_response: _internal_error_response().
  _make_abs_root: _make_abs_root().
  _INPUT_SCHEMA._INPUT_SCHEMA: _INPUT_SCHEMA._INPUT_SCHEMA.
---
# Module: [`tree_sitter_analyzer/mcp/tools/build_project_index_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/build_project_index_tool.py)

## Classes
### `BuildProjectIndexTool`  ·  implements/extends BaseMCPTool
- def: [`tree_sitter_analyzer/mcp/tools/build_project_index_tool.py:114`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/build_project_index_tool.py#L114)
- doc: MCP tool that rebuilds and persists the project structure index.
- signature: `class BuildProjectIndexTool(BaseMCPTool):`
- members:
  - `_do_execute(self, arguments: dict[str, Any])` — [`L209`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/build_project_index_tool.py#L209) — Core build logic — called only after validate_arguments passes.
  - `execute(self, arguments: dict[str, Any])` — [`L197`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/build_project_index_tool.py#L197) — Build a fresh project index, persist it, and return a build report.
  - `get_tool_definition(self)` — [`L120`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/build_project_index_tool.py#L120)
  - `get_tool_schema(self)` — [`L117`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/build_project_index_tool.py#L117)
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L153`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/build_project_index_tool.py#L153) — Validate roots against project boundary before any filesystem traversal.
- uses (calls/refs, reference-scoped): [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`project_root`](base_tool.md#BaseMCPTool.project_root), [`ProjectIndexManager`](../utils/project_index/_manager.md#ProjectIndexManager), [`build`](../utils/project_index/_manager.md#ProjectIndexManager.build), [`load`](../utils/project_index/_manager.md#ProjectIndexManager.load), [`mirror_summary_line`](base_tool.md#mirror_summary_line), [`ProjectIndex`](../utils/project_index/_models.md#ProjectIndex), [`resolve_and_validate_directory_path`](base_tool.md#BaseMCPTool.resolve_and_validate_directory_path), [`save`](../utils/project_index/_manager.md#ProjectIndexManager.save), [`custom_notes`](../utils/project_index/_models.md#ProjectIndex.custom_notes), [`language_distribution`](../utils/project_index/_models.md#ProjectIndex.language_distribution), [`_make_quick_start`](get_project_summary_tool.md#_make_quick_start), [`file_count`](../utils/project_index/_models.md#ProjectIndex.file_count), [`_validate_one_root`](build_project_index_tool.md#_validate_one_root), [`CACHE_FILE`](../utils/project_index/_manager.md#ProjectIndexManager.CACHE_FILE), [`_INPUT_SCHEMA`](build_project_index_tool.md#_INPUT_SCHEMA._INPUT_SCHEMA), [`_internal_error_response`](build_project_index_tool.md#_internal_error_response), [`_make_abs_root`](build_project_index_tool.md#_make_abs_root), [`_security_error_response`](build_project_index_tool.md#_security_error_response)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments), [`build_index_facade`](index_facade.md#build_index_facade)  (33 test-only)

## Functions
- `_boundary_error_msg(root: str, resolved: Path, project_abs: Path)` — [`L42`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/build_project_index_tool.py#L42)
- `_internal_error_response(exc: Exception)` — [`L92`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/build_project_index_tool.py#L92)
- `_make_abs_root(r: str, project_root: str)` — [`L108`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/build_project_index_tool.py#L108)
- `_security_error_response(exc: Exception)` — [`L76`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/build_project_index_tool.py#L76)
- `_validate_one_root(root: str, project_root: str | None, resolve_fn: Any)` — [`L50`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/build_project_index_tool.py#L50)

## Module values
- `_INPUT_SCHEMA` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/build_project_index_tool.py#L19)

