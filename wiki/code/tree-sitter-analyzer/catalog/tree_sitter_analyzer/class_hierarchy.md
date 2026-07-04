---
title: 'Module: tree_sitter_analyzer/class_hierarchy.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/class_hierarchy.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.class_hierarchy`/
symbols:
  ClassHierarchy: ClassHierarchy#
  ClassHierarchy._build_edges_from_edge_store: ClassHierarchy#_build_edges_from_edge_store().
  ClassHierarchy.hierarchy_impact: ClassHierarchy#hierarchy_impact().
  ClassHierarchy.subclasses_of: ClassHierarchy#subclasses_of().
  ClassHierarchy.build: ClassHierarchy#build().
  ClassHierarchy._load_from_cache: ClassHierarchy#_load_from_cache().
  ClassHierarchy.superclasses_of: ClassHierarchy#superclasses_of().
  ClassHierarchy._classes: ClassHierarchy#_classes.
  ClassHierarchy._build_tree: ClassHierarchy#_build_tree().
  ClassInfo.to_dict: ClassInfo#to_dict().
  HierarchyImpact.to_dict: HierarchyImpact#to_dict().
  ClassHierarchy._children: ClassHierarchy#_children.
  ClassHierarchy.has_class: ClassHierarchy#has_class().
  ClassHierarchy.summary: ClassHierarchy#summary().
  ClassHierarchy.all_classes: ClassHierarchy#all_classes().
  ClassInfo.file: ClassInfo#file.
  ClassInfo.parents: ClassInfo#parents.
  ClassHierarchy._parent_map: ClassHierarchy#_parent_map.
  ClassInfo: ClassInfo#
  ClassHierarchy._build_edges: ClassHierarchy#_build_edges().
  ClassInfo.name: ClassInfo#name.
  ClassInfo.line: ClassInfo#line.
  ClassInfo.language: ClassInfo#language.
  ClassHierarchy.hierarchy_tree: ClassHierarchy#hierarchy_tree().
  ClassHierarchy._measure_depth: ClassHierarchy#_measure_depth().
  ClassHierarchy._built: ClassHierarchy#_built.
  ClassInfo.end_line: ClassInfo#end_line.
  HierarchyImpact.risk_level: HierarchyImpact#risk_level.
  ClassHierarchy._confirmed_child_files: ClassHierarchy#_confirmed_child_files.
  HierarchyImpact: HierarchyImpact#
  HierarchyImpact.target_class: HierarchyImpact#target_class.
  HierarchyImpact.direct_subclass_count: HierarchyImpact#direct_subclass_count.
  HierarchyImpact.total_subclass_count: HierarchyImpact#total_subclass_count.
  HierarchyImpact.affected_files: HierarchyImpact#affected_files.
  HierarchyImpact.risk_score: HierarchyImpact#risk_score.
  ClassHierarchy._cache: ClassHierarchy#_cache.
  logger: logger.
  ClassHierarchy.__init__: ClassHierarchy#__init__().
---
# Module: [`tree_sitter_analyzer/class_hierarchy.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/class_hierarchy.py)

## Classes
### `ClassHierarchy`
- def: [`tree_sitter_analyzer/class_hierarchy.py:69`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/class_hierarchy.py#L69) — documented in [tree_sitter_analyzer-uml_export](../../concepts/tree_sitter_analyzer-uml_export.md)
- doc: Cache-backed class inheritance hierarchy analysis.
- signature: `class ClassHierarchy:`
- members:
  - `all_classes(self)` — [`L379`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/class_hierarchy.py#L379) — Return all discovered class definitions.
  - `build(self)` — [`L101`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/class_hierarchy.py#L101) — documented in [tree_sitter_analyzer-uml_export](../../concepts/tree_sitter_analyzer-uml_export.md)
  - `has_class(self, class_name: str)` — [`L213`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/class_hierarchy.py#L213) — Whether ``class_name`` is a known, defined class in the project.
  - `hierarchy_impact(self, class_name: str)` — [`L329`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/class_hierarchy.py#L329) — Risk analysis for modifying a class.
  - `hierarchy_tree(self, class_name: str)` — [`L292`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/class_hierarchy.py#L292) — Get the full subtree rooted at ``class_name``.
  - `subclasses_of(self, class_name: str, max_depth: int = 10)` — [`L222`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/class_hierarchy.py#L222) — Find all classes that inherit from ``class_name`` (transitively).
  - `summary(self)` — [`L388`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/class_hierarchy.py#L388) — Return hierarchy summary statistics.
  - `superclasses_of(self, class_name: str)` — [`L265`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/class_hierarchy.py#L265) — Find the inheritance chain above ``class_name``.
- protocol/private: `__init__`[`L90`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/class_hierarchy.py#L90), `_build_edges`[`L144`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/class_hierarchy.py#L144), `_build_edges_from_edge_store`[`L157`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/class_hierarchy.py#L157), `_build_tree`[`L300`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/class_hierarchy.py#L300), `_built`[`L99`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/class_hierarchy.py#L99), `_cache`[`L91`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/class_hierarchy.py#L91), `_children`[`L93`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/class_hierarchy.py#L93), `_classes`[`L92`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/class_hierarchy.py#L92), `_confirmed_child_files`[`L98`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/class_hierarchy.py#L98), `_load_from_cache`[`L109`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/class_hierarchy.py#L109), `_measure_depth`[`L407`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/class_hierarchy.py#L407), `_parent_map`[`L94`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/class_hierarchy.py#L94)
- uses (calls/refs, reference-scoped): [`EdgeKind`](graph/edge_store.md#EdgeKind), [`EdgeStore`](graph/edge_store.md#EdgeStore), [`parse_node_id`](graph/edge_store.md#parse_node_id), [`name`](graph/edge_store.md#NodeRef.name), [`file_path`](graph/edge_store.md#NodeRef.file_path), [`to_dict`](class_hierarchy.md#ClassInfo.to_dict), [`EXTENDS`](graph/edge_store.md#EdgeKind.EXTENDS), [`conn`](graph/edge_store.md#EdgeStore.conn), [`file`](class_hierarchy.md#ClassInfo.file), [`parents`](class_hierarchy.md#ClassInfo.parents), [`ClassInfo`](class_hierarchy.md#ClassInfo), [`name`](class_hierarchy.md#ClassInfo.name), [`language`](class_hierarchy.md#ClassInfo.language), [`line`](class_hierarchy.md#ClassInfo.line), [`end_line`](class_hierarchy.md#ClassInfo.end_line), [`risk_level`](class_hierarchy.md#HierarchyImpact.risk_level), [`IMPLEMENTS`](graph/edge_store.md#EdgeKind.IMPLEMENTS), [`HierarchyImpact`](class_hierarchy.md#HierarchyImpact), [`affected_files`](class_hierarchy.md#HierarchyImpact.affected_files), [`direct_subclass_count`](class_hierarchy.md#HierarchyImpact.direct_subclass_count), [`risk_score`](class_hierarchy.md#HierarchyImpact.risk_score), [`target_class`](class_hierarchy.md#HierarchyImpact.target_class), [`total_subclass_count`](class_hierarchy.md#HierarchyImpact.total_subclass_count)
- used by: [`state_diagram`](uml_export.md#UMLExporter.state_diagram), [`class_diagram`](uml_export.md#UMLExporter.class_diagram), [`execute`](mcp/tools/class_inspect_tool.md#ClassInspectTool.execute), [`execute`](mcp/tools/class_hierarchy_tool.md#ClassHierarchyTool.execute), [`_hierarchy_for`](mcp/tools/symbol_lineage_tool.md#SymbolLineageTool._hierarchy_for), [`_collect_inherited_methods`](mcp/tools/class_inspect_tool.md#ClassInspectTool._collect_inherited_methods), [`_find_override_source`](mcp/tools/class_inspect_tool.md#ClassInspectTool._find_override_source), [`_parent_method_names`](mcp/tools/class_inspect_tool.md#ClassInspectTool._parent_method_names), [`_get_hierarchy`](mcp/tools/class_hierarchy_tool.md#ClassHierarchyTool._get_hierarchy), [`__init__`](mcp/tools/class_hierarchy_tool.md#ClassHierarchyTool.__init__)  (17 test-only)

### `ClassInfo`
- def: [`tree_sitter_analyzer/class_hierarchy.py:28`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/class_hierarchy.py#L28)
- signature: `class ClassInfo:`
- members:
  - `to_dict(self)` — [`L36`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/class_hierarchy.py#L36)
  - `end_line` — [`L32`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/class_hierarchy.py#L32)
  - `file` — [`L30`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/class_hierarchy.py#L30)
  - `language` — [`L33`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/class_hierarchy.py#L33)
  - `line` — [`L31`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/class_hierarchy.py#L31)
  - `name` — [`L29`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/class_hierarchy.py#L29)
  - `parents` — [`L34`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/class_hierarchy.py#L34)
- used by: [`hierarchy_impact`](class_hierarchy.md#ClassHierarchy.hierarchy_impact), [`subclasses_of`](class_hierarchy.md#ClassHierarchy.subclasses_of), [`_load_from_cache`](class_hierarchy.md#ClassHierarchy._load_from_cache), [`superclasses_of`](class_hierarchy.md#ClassHierarchy.superclasses_of), [`_classes`](class_hierarchy.md#ClassHierarchy._classes), [`_build_tree`](class_hierarchy.md#ClassHierarchy._build_tree), [`all_classes`](class_hierarchy.md#ClassHierarchy.all_classes)  (3 test-only)

### `HierarchyImpact`
- def: [`tree_sitter_analyzer/class_hierarchy.py:50`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/class_hierarchy.py#L50)
- signature: `class HierarchyImpact:`
- members:
  - `to_dict(self)` — [`L58`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/class_hierarchy.py#L58)
  - `affected_files` — [`L54`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/class_hierarchy.py#L54)
  - `direct_subclass_count` — [`L52`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/class_hierarchy.py#L52)
  - `risk_level` — [`L55`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/class_hierarchy.py#L55)
  - `risk_score` — [`L56`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/class_hierarchy.py#L56)
  - `target_class` — [`L51`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/class_hierarchy.py#L51)
  - `total_subclass_count` — [`L53`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/class_hierarchy.py#L53)
- used by: [`execute`](mcp/tools/class_hierarchy_tool.md#ClassHierarchyTool.execute), [`hierarchy_impact`](class_hierarchy.md#ClassHierarchy.hierarchy_impact)

## Module values
- `logger` — [`L24`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/class_hierarchy.py#L24)

