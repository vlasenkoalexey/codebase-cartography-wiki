---
title: 'Module: tree_sitter_analyzer/mcp/tools/class_inspect_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/class_inspect_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.class_inspect_tool`/
symbols:
  ClassInspectTool.execute: ClassInspectTool#execute().
  ClassInspectTool: ClassInspectTool#
  ClassInspectTool._find_override_source: ClassInspectTool#_find_override_source().
  ClassInspectTool._collect_inherited_methods: ClassInspectTool#_collect_inherited_methods().
  ClassInspectTool._parent_method_names: ClassInspectTool#_parent_method_names().
  _is_method_abstract: _is_method_abstract().
  ClassInspectTool._collect_fields: ClassInspectTool#_collect_fields().
  _extract_fields_from_source: _extract_fields_from_source().
  ClassInspectTool._get_cache: ClassInspectTool#_get_cache().
  ClassInspectTool._collect_class_info: ClassInspectTool#_collect_class_info().
  ClassInspectTool._collect_raw_methods: ClassInspectTool#_collect_raw_methods().
  _compute_visibility: _compute_visibility().
  _read_source_lines: _read_source_lines().
  logger: logger.
  ClassInspectTool.get_tool_definition: ClassInspectTool#get_tool_definition().
  ClassInspectTool.get_tool_schema: ClassInspectTool#get_tool_schema().
  ClassInspectTool.validate_arguments: ClassInspectTool#validate_arguments().
  _filter_closures: _filter_closures().
  _ABSTRACTMETHOD_PATTERN: _ABSTRACTMETHOD_PATTERN.
  _CLS_ATTR_RE: _CLS_ATTR_RE.
  _SELF_ATTR_RE: _SELF_ATTR_RE.
---
# Module: [`tree_sitter_analyzer/mcp/tools/class_inspect_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/class_inspect_tool.py)

## Classes
### `ClassInspectTool`  ·  implements/extends BaseMCPTool
- def: [`tree_sitter_analyzer/mcp/tools/class_inspect_tool.py:225`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/class_inspect_tool.py#L225)
- doc: Inspect a single class: fields, methods (no closures), visibility, extends.
- signature: `class ClassInspectTool(BaseMCPTool):`
- members:
  - `_collect_class_info(self, cache: ASTCache, class_name: str)` — [`L276`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/class_inspect_tool.py#L276) — Return the raw class symbol dict for class_name (first match).
  - `_collect_fields(self, cache: ASTCache, class_info: dict[str, Any])` — [`L417`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/class_inspect_tool.py#L417) — Extract class-level and instance fields by scanning source.
  - `_collect_inherited_methods(self, hierarchy: ClassHierarchy, class_name: str, cache: ASTCache)` — [`L447`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/class_inspect_tool.py#L447) — Collect inherited methods from the nearest in-project ancestor.
  - `_collect_raw_methods(self, cache: ASTCache, class_name: str, file_path: str | None = None)` — [`L303`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/class_inspect_tool.py#L303) — Return method/function symbols whose enclosing class is class_name.
  - `_find_override_source(self, hierarchy: ClassHierarchy, class_name: str, method_name: str, cache: ASTCache)` — [`L379`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/class_inspect_tool.py#L379) — Return the name of the ancestor class that first defines method_name.
  - `_parent_method_names(self, hierarchy: ClassHierarchy, class_name: str, cache: ASTCache)` — [`L351`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/class_inspect_tool.py#L351) — Collect method names defined in any ancestor of class_name.
  - `execute(self, arguments: dict[str, Any])` — [`L501`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/class_inspect_tool.py#L501)
  - `get_tool_definition(self)` — [`L228`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/class_inspect_tool.py#L228)
  - `get_tool_schema(self)` — [`L247`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/class_inspect_tool.py#L247)
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L266`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/class_inspect_tool.py#L266)
- protocol/private: `_get_cache`[`L271`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/class_inspect_tool.py#L271)
- uses (calls/refs, reference-scoped): [`ASTCache`](../../ast_cache.md#ASTCache), [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`project_root`](base_tool.md#BaseMCPTool.project_root), [`apply_toon_format_to_response`](../utils/format_helper.md#apply_toon_format_to_response), [`get_conn`](../../ast_cache.md#ASTCache.get_conn), [`ClassHierarchy`](../../class_hierarchy.md#ClassHierarchy), [`build`](../../class_hierarchy.md#ClassHierarchy.build), [`superclasses_of`](../../class_hierarchy.md#ClassHierarchy.superclasses_of), [`_classes`](../../class_hierarchy.md#ClassHierarchy._classes), [`_is_method_abstract`](class_inspect_tool.md#_is_method_abstract), [`_extract_fields_from_source`](class_inspect_tool.md#_extract_fields_from_source), [`_compute_visibility`](class_inspect_tool.md#_compute_visibility), [`_read_source_lines`](class_inspect_tool.md#_read_source_lines), [`_filter_closures`](class_inspect_tool.md#_filter_closures)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments), [`build_structure_facade`](structure_facade.md#build_structure_facade), [`_class_detail_route`](structure_facade.md#build_structure_facade._class_detail_route)  (32 test-only)

## Functions
- `_compute_visibility(name: str)` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/class_inspect_tool.py#L45) — Derive Python visibility from name convention.
- `_extract_fields_from_source(source: str, class_name: str, class_start: int, class_end: int)` — [`L97`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/class_inspect_tool.py#L97) — Extract class-level and instance attributes from source text.
- `_filter_closures(raw_methods: list[dict[str, Any]])` — [`L67`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/class_inspect_tool.py#L67) — Remove closures — functions whose line range is fully contained within
- `_is_method_abstract(source_lines: list[str], def_line_1indexed: int)` — [`L180`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/class_inspect_tool.py#L180) — Return True if the line immediately before *def_line_1indexed* is ``@abstractmethod``.
- `_read_source_lines(file_path: str, project_root: str)` — [`L210`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/class_inspect_tool.py#L210) — Read and return source lines for *file_path*, resolved against *project_root*.

## Module values
- `_ABSTRACTMETHOD_PATTERN` — [`L177`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/class_inspect_tool.py#L177)
- `_CLS_ATTR_RE` — [`L34`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/class_inspect_tool.py#L34)
- `_SELF_ATTR_RE` — [`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/class_inspect_tool.py#L39)
- `logger` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/class_inspect_tool.py#L30)

