---
title: 'Module: tree_sitter_analyzer/mcp/tools/class_hierarchy_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/class_hierarchy_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.class_hierarchy_tool`/
symbols:
  ClassHierarchyTool.execute: ClassHierarchyTool#execute().
  ClassHierarchyTool: ClassHierarchyTool#
  ClassHierarchyTool._get_hierarchy: ClassHierarchyTool#_get_hierarchy().
  ClassHierarchyTool._resolve_mode: ClassHierarchyTool#_resolve_mode().
  ClassHierarchyTool.validate_arguments: ClassHierarchyTool#validate_arguments().
  ClassHierarchyTool._normalize_mode: ClassHierarchyTool#_normalize_mode().
  ClassHierarchyTool._hierarchy: ClassHierarchyTool#_hierarchy.
  ClassHierarchyTool.__init__: ClassHierarchyTool#__init__().
  logger: logger.
  ClassHierarchyTool._on_project_root_changed: ClassHierarchyTool#_on_project_root_changed().
  ClassHierarchyTool.get_tool_definition: ClassHierarchyTool#get_tool_definition().
  ClassHierarchyTool.get_tool_schema: ClassHierarchyTool#get_tool_schema().
  ClassHierarchyTool._MODE_ALIASES: ClassHierarchyTool#_MODE_ALIASES.
  ClassHierarchyTool._VALID_MODES: ClassHierarchyTool#_VALID_MODES.
---
# Module: [`tree_sitter_analyzer/mcp/tools/class_hierarchy_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/class_hierarchy_tool.py)

## Classes
### `ClassHierarchyTool`  ·  implements/extends BaseMCPTool
- def: [`tree_sitter_analyzer/mcp/tools/class_hierarchy_tool.py:30`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/class_hierarchy_tool.py#L30)
- doc: MCP Tool for class inheritance hierarchy analysis (CodeGraph parity).
- signature: `class ClassHierarchyTool(BaseMCPTool):`
- members:
  - `_normalize_mode(mode: str)` — [`L154`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/class_hierarchy_tool.py#L154) — Resolve mode aliases to their canonical form.
  - `_resolve_mode(cls, arguments: dict[str, Any])` — [`L133`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/class_hierarchy_tool.py#L133) — Effective query mode.
  - `execute(self, arguments: dict[str, Any])` — [`L170`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/class_hierarchy_tool.py#L170)
  - `get_tool_definition(self)` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/class_hierarchy_tool.py#L48)
  - `get_tool_schema(self)` — [`L71`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/class_hierarchy_tool.py#L71)
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L163`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/class_hierarchy_tool.py#L163)
- protocol/private: `_MODE_ALIASES`[`L118`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/class_hierarchy_tool.py#L118), `_VALID_MODES`[`L123`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/class_hierarchy_tool.py#L123), `__init__`[`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/class_hierarchy_tool.py#L33), `_get_hierarchy`[`L40`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/class_hierarchy_tool.py#L40), `_hierarchy`[`L34`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/class_hierarchy_tool.py#L34), `_on_project_root_changed`[`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/class_hierarchy_tool.py#L37)
- uses (calls/refs, reference-scoped): [`ASTCache`](../../ast_cache.md#ASTCache), [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`project_root`](base_tool.md#BaseMCPTool.project_root), [`apply_toon_format_to_response`](../utils/format_helper.md#apply_toon_format_to_response), [`__init__`](base_tool.md#BaseMCPTool.__init__), [`ClassHierarchy`](../../class_hierarchy.md#ClassHierarchy), [`mirror_summary_line`](base_tool.md#mirror_summary_line), [`hierarchy_impact`](../../class_hierarchy.md#ClassHierarchy.hierarchy_impact), [`subclasses_of`](../../class_hierarchy.md#ClassHierarchy.subclasses_of), [`build`](../../class_hierarchy.md#ClassHierarchy.build), [`superclasses_of`](../../class_hierarchy.md#ClassHierarchy.superclasses_of), [`to_dict`](../../class_hierarchy.md#HierarchyImpact.to_dict), [`has_class`](../../class_hierarchy.md#ClassHierarchy.has_class), [`summary`](../../class_hierarchy.md#ClassHierarchy.summary), [`all_classes`](../../class_hierarchy.md#ClassHierarchy.all_classes), [`is_index_rebuilding`](index_rebuild_signal.md#is_index_rebuilding), [`hierarchy_tree`](../../class_hierarchy.md#ClassHierarchy.hierarchy_tree), [`rebuild_in_progress_next_step`](index_rebuild_signal.md#rebuild_in_progress_next_step), [`risk_level`](../../class_hierarchy.md#HierarchyImpact.risk_level)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments), [`_on_project_root_changed`](base_tool.md#BaseMCPTool._on_project_root_changed), [`build_structure_facade`](structure_facade.md#build_structure_facade)  (20 test-only)

## Module values
- `logger` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/class_hierarchy_tool.py#L27)

