---
title: 'Module: tests/unit/test_codegraph_class_hierarchy_tool.py'
type: catalog
provenance: extracted
module: tests/unit/test_codegraph_class_hierarchy_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_codegraph_class_hierarchy_tool`/
symbols:
  TestClassHierarchyEdgeStore.test_edge_store_metadata_fallbacks_and_empty_parent_map: TestClassHierarchyEdgeStore#test_edge_store_metadata_fallbacks_and_empty_parent_map().
  TestSameNameDifferentBaseCollision.test_same_name_children_different_bases_isolated: TestSameNameDifferentBaseCollision#test_same_name_children_different_bases_isolated().
  TestAgentSummaryPresence.tool_with_monkeypatched_hierarchy: TestAgentSummaryPresence#tool_with_monkeypatched_hierarchy().
  _stub_hierarchy: _stub_hierarchy().
  TestExecute.test_rebuild_marker_warns_without_phantom_subclass_count: TestExecute#test_rebuild_marker_warns_without_phantom_subclass_count().
  TestClassHierarchyEdgeStore.test_falls_back_to_symbol_parents_when_edge_store_unavailable: TestClassHierarchyEdgeStore#test_falls_back_to_symbol_parents_when_edge_store_unavailable().
  TestExecute.test_subclasses_mode_reads_edge_store_when_symbol_parents_missing: TestExecute#test_subclasses_mode_reads_edge_store_when_symbol_parents_missing().
  TestClassHierarchyEdgeStore.test_same_name_class_without_parents_not_listed_as_subclass: TestClassHierarchyEdgeStore#test_same_name_class_without_parents_not_listed_as_subclass().
  test_has_class_distinguishes_existence_from_emptiness: test_has_class_distinguishes_existence_from_emptiness().
  tool: tool().
  tool_with_root: tool_with_root().
  TestExecute.test_tree_leaf_class_is_found_not_notfound: TestExecute#test_tree_leaf_class_is_found_not_notfound().
  TestExecute.test_tree_unknown_class_is_notfound: TestExecute#test_tree_unknown_class_is_notfound().
  TestExecute.test_default_mode_named_class_is_class_scoped_not_global: TestExecute#test_default_mode_named_class_is_class_scoped_not_global().
  TestExecute.test_subclasses_existing_class_no_children_is_info: TestExecute#test_subclasses_existing_class_no_children_is_info().
  TestExecute.test_subclasses_unknown_class_is_notfound: TestExecute#test_subclasses_unknown_class_is_notfound().
  TestExecute.test_superclasses_root_class_is_info: TestExecute#test_superclasses_root_class_is_info().
  TestClassHierarchyEdgeStore.test_falls_back_to_symbol_parents_when_edge_store_unavailable.BrokenEdgeStore: TestClassHierarchyEdgeStore#test_falls_back_to_symbol_parents_when_edge_store_unavailable().BrokenEdgeStore#
  TestAgentSummaryPresence._has_class: TestAgentSummaryPresence#_has_class().
  TestAgentSummaryPresence._subclasses_of: TestAgentSummaryPresence#_subclasses_of().
  TestAgentSummaryPresence._superclasses_of: TestAgentSummaryPresence#_superclasses_of().
  TestAgentSummaryPresence._hierarchy_tree: TestAgentSummaryPresence#_hierarchy_tree().
  TestAgentSummaryPresence._all_classes: TestAgentSummaryPresence#_all_classes().
  TestAgentSummaryPresence._summary: TestAgentSummaryPresence#_summary().
  TestToolDefinition: TestToolDefinition#
  TestToolDefinition.test_tool_name: TestToolDefinition#test_tool_name().
  TestToolDefinition.test_description_mentions_no_other: TestToolDefinition#test_description_mentions_no_other().
  TestToolDefinition.test_schema_mode_enum: TestToolDefinition#test_schema_mode_enum().
  TestToolDefinition.test_schema_output_format_default_toon: TestToolDefinition#test_schema_output_format_default_toon().
  TestToolDefinition.test_annotations_readonly: TestToolDefinition#test_annotations_readonly().
  TestToolDefinition.test_mode_not_required: TestToolDefinition#test_mode_not_required().
  TestValidation: TestValidation#
  TestValidation.test_all_mode_no_class_required: TestValidation#test_all_mode_no_class_required().
  TestValidation.test_summary_mode_no_class_required: TestValidation#test_summary_mode_no_class_required().
  TestValidation.test_subclasses_requires_class_name: TestValidation#test_subclasses_requires_class_name().
  TestValidation.test_superclasses_requires_class_name: TestValidation#test_superclasses_requires_class_name().
  TestValidation.test_valid_subclasses_with_class_name: TestValidation#test_valid_subclasses_with_class_name().
  TestExecute: TestExecute#
  TestExecute.test_no_project_root_raises_or_returns_error: TestExecute#test_no_project_root_raises_or_returns_error().
  TestExecute.test_all_mode_on_project: TestExecute#test_all_mode_on_project().
  TestExecute.test_summary_mode_on_project: TestExecute#test_summary_mode_on_project().
  TestExecute.test_toon_format_default: TestExecute#test_toon_format_default().
  TestClassHierarchyEdgeStore: TestClassHierarchyEdgeStore#
  TestClassHierarchyEdgeStore.test_falls_back_to_symbol_parents_when_edge_store_unavailable.BrokenEdgeStore.__init__: TestClassHierarchyEdgeStore#test_falls_back_to_symbol_parents_when_edge_store_unavailable().BrokenEdgeStore#__init__().
  TestSameNameDifferentBaseCollision: TestSameNameDifferentBaseCollision#
  TestAgentSummaryPresence: TestAgentSummaryPresence#
  TestAgentSummaryPresence.test_subclasses_has_agent_summary: TestAgentSummaryPresence#test_subclasses_has_agent_summary().
  TestAgentSummaryPresence.test_superclasses_has_agent_summary: TestAgentSummaryPresence#test_superclasses_has_agent_summary().
  TestAgentSummaryPresence.test_tree_has_agent_summary: TestAgentSummaryPresence#test_tree_has_agent_summary().
  TestAgentSummaryPresence.test_all_has_agent_summary: TestAgentSummaryPresence#test_all_has_agent_summary().
  TestAgentSummaryPresence.test_summary_has_agent_summary: TestAgentSummaryPresence#test_summary_has_agent_summary().
  TestAgentSummaryPresence.test_unknown_mode_has_agent_summary: TestAgentSummaryPresence#test_unknown_mode_has_agent_summary().
---
# Module: [`tests/unit/test_codegraph_class_hierarchy_tool.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_class_hierarchy_tool.py)

## Classes
### `BrokenEdgeStore`
- def: [`tests/unit/test_codegraph_class_hierarchy_tool.py:317`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_class_hierarchy_tool.py#L317)
- signature: `class BrokenEdgeStore:`
- protocol/private: `__init__`[`L318`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_class_hierarchy_tool.py#L318)
- used by: (1 test-only callers)

### `TestAgentSummaryPresence`
- def: [`tests/unit/test_codegraph_class_hierarchy_tool.py:510`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_class_hierarchy_tool.py#L510)
- doc: #733: class_hierarchy must include agent_summary in every mode's response.
- signature: `class TestAgentSummaryPresence:`
- members:
  - `test_all_has_agent_summary(self, tool_with_monkeypatched_hierarchy)` — [`L610`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_class_hierarchy_tool.py#L610)
  - `test_subclasses_has_agent_summary(self, tool_with_monkeypatched_hierarchy)` — [`L585`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_class_hierarchy_tool.py#L585)
  - `test_summary_has_agent_summary(self, tool_with_monkeypatched_hierarchy)` — [`L616`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_class_hierarchy_tool.py#L616)
  - `test_superclasses_has_agent_summary(self, tool_with_monkeypatched_hierarchy)` — [`L596`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_class_hierarchy_tool.py#L596)
  - `test_tree_has_agent_summary(self, tool_with_monkeypatched_hierarchy)` — [`L604`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_class_hierarchy_tool.py#L604)
  - `test_unknown_mode_has_agent_summary(self, tool_with_monkeypatched_hierarchy)` — [`L622`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_class_hierarchy_tool.py#L622)
  - `tool_with_monkeypatched_hierarchy(self, tool, monkeypatch)` — [`L514`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_class_hierarchy_tool.py#L514)
- protocol/private: `_all_classes`[`L569`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_class_hierarchy_tool.py#L569), `_has_class`[`L547`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_class_hierarchy_tool.py#L547), `_hierarchy_tree`[`L566`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_class_hierarchy_tool.py#L566), `_subclasses_of`[`L550`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_class_hierarchy_tool.py#L550), `_summary`[`L572`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_class_hierarchy_tool.py#L572), `_superclasses_of`[`L561`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_class_hierarchy_tool.py#L561)
- uses (calls/refs, reference-scoped): [`ClassHierarchy`](../../tree_sitter_analyzer/class_hierarchy.md#ClassHierarchy), [`subclasses_of`](../../tree_sitter_analyzer/class_hierarchy.md#ClassHierarchy.subclasses_of), [`build`](../../tree_sitter_analyzer/class_hierarchy.md#ClassHierarchy.build), [`superclasses_of`](../../tree_sitter_analyzer/class_hierarchy.md#ClassHierarchy.superclasses_of), [`has_class`](../../tree_sitter_analyzer/class_hierarchy.md#ClassHierarchy.has_class), [`summary`](../../tree_sitter_analyzer/class_hierarchy.md#ClassHierarchy.summary), [`all_classes`](../../tree_sitter_analyzer/class_hierarchy.md#ClassHierarchy.all_classes), [`hierarchy_tree`](../../tree_sitter_analyzer/class_hierarchy.md#ClassHierarchy.hierarchy_tree), [`_built`](../../tree_sitter_analyzer/class_hierarchy.md#ClassHierarchy._built)

### `TestClassHierarchyEdgeStore`
- def: [`tests/unit/test_codegraph_class_hierarchy_tool.py:306`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_class_hierarchy_tool.py#L306)
- signature: `class TestClassHierarchyEdgeStore:`
- members:
  - `test_edge_store_metadata_fallbacks_and_empty_parent_map(self, tmp_path)` — [`L334`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_class_hierarchy_tool.py#L334)
  - `test_falls_back_to_symbol_parents_when_edge_store_unavailable(self, monkeypatch, tmp_path)` — [`L307`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_class_hierarchy_tool.py#L307)
  - `test_same_name_class_without_parents_not_listed_as_subclass(self, tmp_path)` — [`L404`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_class_hierarchy_tool.py#L404) — Regression: #659 — same-name collision must not create false subclass.
- uses (calls/refs, reference-scoped): [`ASTCache`](../../tree_sitter_analyzer/ast_cache.md#ASTCache), [`close`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.close), [`EdgeKind`](../../tree_sitter_analyzer/graph/edge_store.md#EdgeKind), [`get_conn`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.get_conn), [`symbol_node`](../../tree_sitter_analyzer/graph/edge_store.md#symbol_node), [`index_file`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.index_file), [`Edge`](../../tree_sitter_analyzer/graph/edge_store.md#Edge), [`ClassHierarchy`](../../tree_sitter_analyzer/class_hierarchy.md#ClassHierarchy), [`EdgeStore`](../../tree_sitter_analyzer/graph/edge_store.md#EdgeStore), [`upsert_edges`](../../tree_sitter_analyzer/graph/edge_store.md#EdgeStore.upsert_edges), [`_build_edges_from_edge_store`](../../tree_sitter_analyzer/class_hierarchy.md#ClassHierarchy._build_edges_from_edge_store), [`subclasses_of`](../../tree_sitter_analyzer/class_hierarchy.md#ClassHierarchy.subclasses_of), [`build`](../../tree_sitter_analyzer/class_hierarchy.md#ClassHierarchy.build), [`metadata`](../../tree_sitter_analyzer/graph/edge_store.md#Edge.metadata), [`EXTENDS`](../../tree_sitter_analyzer/graph/edge_store.md#EdgeKind.EXTENDS), [`file_node`](../../tree_sitter_analyzer/graph/edge_store.md#file_node), [`class_node`](../../tree_sitter_analyzer/graph/edge_store.md#class_node)  (1 test-only)

### `TestExecute`
- def: [`tests/unit/test_codegraph_class_hierarchy_tool.py:134`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_class_hierarchy_tool.py#L134)
- signature: `class TestExecute:`
- members:
  - `test_all_mode_on_project(self, tool_with_root)` — [`L142`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_class_hierarchy_tool.py#L142)
  - `test_default_mode_named_class_is_class_scoped_not_global(self, tool, monkeypatch)` — [`L181`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_class_hierarchy_tool.py#L181) — No explicit mode + a class_name → class-scoped 'tree', NOT the global
  - `test_no_project_root_raises_or_returns_error(self, tool)` — [`L135`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_class_hierarchy_tool.py#L135)
  - `test_rebuild_marker_warns_without_phantom_subclass_count(self, tmp_path)` — [`L223`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_class_hierarchy_tool.py#L223)
  - `test_subclasses_existing_class_no_children_is_info(self, tool, monkeypatch)` — [`L195`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_class_hierarchy_tool.py#L195) — Review issue 1: an existing class with zero subclasses is a valid
  - `test_subclasses_mode_reads_edge_store_when_symbol_parents_missing(self, tmp_path)` — [`L265`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_class_hierarchy_tool.py#L265)
  - `test_subclasses_unknown_class_is_notfound(self, tool, monkeypatch)` — [`L210`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_class_hierarchy_tool.py#L210)
  - `test_summary_mode_on_project(self, tool_with_root)` — [`L146`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_class_hierarchy_tool.py#L146)
  - `test_superclasses_root_class_is_info(self, tool, monkeypatch)` — [`L253`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_class_hierarchy_tool.py#L253) — Review issue 1: a root class with no parents exists → INFO, not
  - `test_toon_format_default(self, tool_with_root)` — [`L152`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_class_hierarchy_tool.py#L152)
  - `test_tree_leaf_class_is_found_not_notfound(self, tool, monkeypatch)` — [`L157`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_class_hierarchy_tool.py#L157) — Wave 1b (audit structure-01): a real leaf class (exists but has no
  - `test_tree_unknown_class_is_notfound(self, tool, monkeypatch)` — [`L172`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_class_hierarchy_tool.py#L172)
- uses (calls/refs, reference-scoped): [`ASTCache`](../../tree_sitter_analyzer/ast_cache.md#ASTCache), [`close`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.close), [`index_project`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.index_project), [`get_conn`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.get_conn), [`index_file`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.index_file), [`execute`](../../tree_sitter_analyzer/mcp/tools/class_hierarchy_tool.md#ClassHierarchyTool.execute), [`ClassHierarchyTool`](../../tree_sitter_analyzer/mcp/tools/class_hierarchy_tool.md#ClassHierarchyTool), [`mark_build_in_progress`](../../tree_sitter_analyzer/_ast_cache_build_state.md#mark_build_in_progress), [`clear_build_in_progress`](../../tree_sitter_analyzer/_ast_cache_build_state.md#clear_build_in_progress)  (1 test-only)

### `TestSameNameDifferentBaseCollision`
- def: [`tests/unit/test_codegraph_class_hierarchy_tool.py:456`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_class_hierarchy_tool.py#L456)
- doc: Codex P2 on #659: two same-named children inheriting DIFFERENT bases
- signature: `class TestSameNameDifferentBaseCollision:`
- members:
  - `test_same_name_children_different_bases_isolated(self, tmp_path)` — [`L460`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_class_hierarchy_tool.py#L460)
- uses (calls/refs, reference-scoped): [`ClassHierarchy`](../../tree_sitter_analyzer/class_hierarchy.md#ClassHierarchy), [`subclasses_of`](../../tree_sitter_analyzer/class_hierarchy.md#ClassHierarchy.subclasses_of), [`build`](../../tree_sitter_analyzer/class_hierarchy.md#ClassHierarchy.build), [`_classes`](../../tree_sitter_analyzer/class_hierarchy.md#ClassHierarchy._classes), [`_children`](../../tree_sitter_analyzer/class_hierarchy.md#ClassHierarchy._children), [`file`](../../tree_sitter_analyzer/class_hierarchy.md#ClassInfo.file), [`parents`](../../tree_sitter_analyzer/class_hierarchy.md#ClassInfo.parents), [`ClassInfo`](../../tree_sitter_analyzer/class_hierarchy.md#ClassInfo), [`_parent_map`](../../tree_sitter_analyzer/class_hierarchy.md#ClassHierarchy._parent_map), [`name`](../../tree_sitter_analyzer/class_hierarchy.md#ClassInfo.name), [`language`](../../tree_sitter_analyzer/class_hierarchy.md#ClassInfo.language), [`line`](../../tree_sitter_analyzer/class_hierarchy.md#ClassInfo.line), [`_built`](../../tree_sitter_analyzer/class_hierarchy.md#ClassHierarchy._built), [`end_line`](../../tree_sitter_analyzer/class_hierarchy.md#ClassInfo.end_line), [`_confirmed_child_files`](../../tree_sitter_analyzer/class_hierarchy.md#ClassHierarchy._confirmed_child_files)

### `TestToolDefinition`
- def: [`tests/unit/test_codegraph_class_hierarchy_tool.py:73`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_class_hierarchy_tool.py#L73)
- signature: `class TestToolDefinition:`
- members:
  - `test_annotations_readonly(self, tool)` — [`L99`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_class_hierarchy_tool.py#L99)
  - `test_description_mentions_no_other(self, tool)` — [`L77`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_class_hierarchy_tool.py#L77)
  - `test_mode_not_required(self, tool)` — [`L104`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_class_hierarchy_tool.py#L104) — Wave 1b (review issue 2): mode is resolved at runtime, so it must NOT
  - `test_schema_mode_enum(self, tool)` — [`L81`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_class_hierarchy_tool.py#L81)
  - `test_schema_output_format_default_toon(self, tool)` — [`L94`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_class_hierarchy_tool.py#L94)
  - `test_tool_name(self, tool)` — [`L74`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_class_hierarchy_tool.py#L74)

### `TestValidation`
- def: [`tests/unit/test_codegraph_class_hierarchy_tool.py:111`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_class_hierarchy_tool.py#L111)
- signature: `class TestValidation:`
- members:
  - `test_all_mode_no_class_required(self, tool)` — [`L112`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_class_hierarchy_tool.py#L112)
  - `test_subclasses_requires_class_name(self, tool)` — [`L118`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_class_hierarchy_tool.py#L118)
  - `test_summary_mode_no_class_required(self, tool)` — [`L115`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_class_hierarchy_tool.py#L115)
  - `test_superclasses_requires_class_name(self, tool)` — [`L122`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_class_hierarchy_tool.py#L122)
  - `test_valid_subclasses_with_class_name(self, tool)` — [`L126`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_class_hierarchy_tool.py#L126)

## Functions
- `_stub_hierarchy(names_with_parents: dict[str, list[str]])` — [`L24`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_class_hierarchy_tool.py#L24) — Build a pre-populated ClassHierarchy without touching an AST cache.
- `test_has_class_distinguishes_existence_from_emptiness()` — [`L52`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_class_hierarchy_tool.py#L52) — has_class is True for a defined leaf class (no subclasses) and False for
- `tool()` — [`L61`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_class_hierarchy_tool.py#L61)
- `tool_with_root(tmp_path)` — [`L66`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_class_hierarchy_tool.py#L66)

