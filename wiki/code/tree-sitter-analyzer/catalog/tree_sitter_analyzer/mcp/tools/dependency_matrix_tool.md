---
title: 'Module: tree_sitter_analyzer/mcp/tools/dependency_matrix_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/dependency_matrix_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.dependency_matrix_tool`/
symbols:
  CodeGraphDependencyMatrixTool.execute: CodeGraphDependencyMatrixTool#execute().
  CodeGraphDependencyMatrixTool: CodeGraphDependencyMatrixTool#
  CodeGraphDependencyMatrixTool._get_matrix: CodeGraphDependencyMatrixTool#_get_matrix().
  CodeGraphDependencyMatrixTool.__init__: CodeGraphDependencyMatrixTool#__init__().
  CodeGraphDependencyMatrixTool._dm: CodeGraphDependencyMatrixTool#_dm.
  CodeGraphDependencyMatrixTool.get_tool_definition: CodeGraphDependencyMatrixTool#get_tool_definition().
  CodeGraphDependencyMatrixTool.validate_arguments: CodeGraphDependencyMatrixTool#validate_arguments().
  CodeGraphDependencyMatrixTool.get_tool_schema: CodeGraphDependencyMatrixTool#get_tool_schema().
  logger: logger.
  CodeGraphDependencyMatrixTool._on_project_root_changed: CodeGraphDependencyMatrixTool#_on_project_root_changed().
---
# Module: [`tree_sitter_analyzer/mcp/tools/dependency_matrix_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/dependency_matrix_tool.py)

## Classes
### `CodeGraphDependencyMatrixTool`  ·  implements/extends BaseMCPTool
- def: [`tree_sitter_analyzer/mcp/tools/dependency_matrix_tool.py:29`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/dependency_matrix_tool.py#L29)
- doc: MCP Tool for module coupling analysis via dependency matrix.
- signature: `class CodeGraphDependencyMatrixTool(BaseMCPTool):`
- members:
  - `execute(self, arguments: dict[str, Any])` — [`L115`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/dependency_matrix_tool.py#L115)
  - `get_tool_definition(self)` — [`L46`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/dependency_matrix_tool.py#L46)
  - `get_tool_schema(self)` — [`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/dependency_matrix_tool.py#L65)
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L106`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/dependency_matrix_tool.py#L106)
- protocol/private: `__init__`[`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/dependency_matrix_tool.py#L32), `_dm`[`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/dependency_matrix_tool.py#L33), `_get_matrix`[`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/dependency_matrix_tool.py#L39), `_on_project_root_changed`[`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/dependency_matrix_tool.py#L36)
- uses (calls/refs, reference-scoped): [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`project_root`](base_tool.md#BaseMCPTool.project_root), [`apply_toon_format_to_response`](../utils/format_helper.md#apply_toon_format_to_response), [`resolve_and_validate_file_path`](base_tool.md#BaseMCPTool.resolve_and_validate_file_path), [`__init__`](base_tool.md#BaseMCPTool.__init__), [`build`](../../dependency_matrix.md#DependencyMatrix.build), [`invalid_enum_error`](_validators.md#invalid_enum_error), [`summary`](../../dependency_matrix.md#DependencyMatrix.summary), [`coupling_pairs`](../../dependency_matrix.md#DependencyMatrixResult.coupling_pairs), [`DependencyMatrix`](../../dependency_matrix.md#DependencyMatrix), [`unstable_modules`](../../dependency_matrix.md#DependencyMatrix.unstable_modules), [`to_dict`](../../dependency_matrix.md#CouplingEntry.to_dict), [`most_coupled`](../../dependency_matrix.md#DependencyMatrix.most_coupled), [`to_dict`](../../dependency_matrix.md#ModuleStats.to_dict), [`score`](../../dependency_matrix.md#CouplingEntry.score), [`file_a`](../../dependency_matrix.md#CouplingEntry.file_a), [`file_b`](../../dependency_matrix.md#CouplingEntry.file_b), [`modules`](../../dependency_matrix.md#DependencyMatrixResult.modules), [`call_count`](../../dependency_matrix.md#CouplingEntry.call_count), [`import_count`](../../dependency_matrix.md#CouplingEntry.import_count)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments), [`_on_project_root_changed`](base_tool.md#BaseMCPTool._on_project_root_changed), [`build_health_facade`](health_facade.md#build_health_facade)  (6 test-only)

## Module values
- `logger` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/dependency_matrix_tool.py#L26)

