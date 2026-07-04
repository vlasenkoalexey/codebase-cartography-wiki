---
title: 'Module: tests/unit/mcp/test_dependency_analysis_tool.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_dependency_analysis_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_dependency_analysis_tool`/
symbols:
  _run: _run().
  _write: _write().
  TestFileDepsMode.test_file_deps_isolated_file: TestFileDepsMode#test_file_deps_isolated_file().
  TestBlastRadiusMode.test_blast_radius_isolated_file: TestBlastRadiusMode#test_blast_radius_isolated_file().
  TestCyclesMode.test_cycles_with_cycle: TestCyclesMode#test_cycles_with_cycle().
  TestCyclesMode.test_cycles_clean_project: TestCyclesMode#test_cycles_clean_project().
  TestBug784CyclesScope.test_cycles_response_has_scope_field: TestBug784CyclesScope#test_cycles_response_has_scope_field().
  TestBug784CyclesScope.test_cycles_response_has_scope_note: TestBug784CyclesScope#test_cycles_response_has_scope_note().
  TestBug784CyclesScope.test_summary_response_has_scope_field: TestBug784CyclesScope#test_summary_response_has_scope_field().
  TestBug784CyclesScope.test_summary_response_has_scope_note: TestBug784CyclesScope#test_summary_response_has_scope_note().
  TestSummaryMode.test_summary_empty_project: TestSummaryMode#test_summary_empty_project().
  TestCyclesHelper.test_cycles_helper_with_cycle: TestCyclesHelper#test_cycles_helper_with_cycle().
  TestNoProjectRoot.test_execute_without_project_root_raises: TestNoProjectRoot#test_execute_without_project_root_raises().
  TestBug784CyclesScope.test_cycles_helper_has_scope: TestBug784CyclesScope#test_cycles_helper_has_scope().
  tool: tool().
  TestValidation.test_blast_is_alias_for_blast_radius: TestValidation#test_blast_is_alias_for_blast_radius().
  TestSummaryHelper.test_summary_populates_hubs: TestSummaryHelper#test_summary_populates_hubs().
  TestSummaryHelper.test_summary_empty_graph: TestSummaryHelper#test_summary_empty_graph().
  TestCyclesHelper.test_cycles_helper_no_cycles: TestCyclesHelper#test_cycles_helper_no_cycles().
  TestFileDepsHelper.test_file_deps_helper: TestFileDepsHelper#test_file_deps_helper().
  TestFileDepsHelper.test_file_deps_helper_counts: TestFileDepsHelper#test_file_deps_helper_counts().
  TestNoProjectRoot.test_get_graph_without_root_raises: TestNoProjectRoot#test_get_graph_without_root_raises().
  project: project().
  TestSummaryMode.test_summary_returns_node_and_edge_count: TestSummaryMode#test_summary_returns_node_and_edge_count().
  TestSummaryMode.test_summary_with_toon_format: TestSummaryMode#test_summary_with_toon_format().
  TestSummaryMode.test_summary_identifies_hub_files: TestSummaryMode#test_summary_identifies_hub_files().
  TestFileDepsMode.test_file_deps_returns_dependencies: TestFileDepsMode#test_file_deps_returns_dependencies().
  TestFileDepsMode.test_file_deps_with_toon: TestFileDepsMode#test_file_deps_with_toon().
  TestFileDepsMode.test_file_deps_file_not_found: TestFileDepsMode#test_file_deps_file_not_found().
  TestFileDepsMode.test_file_deps_absolute_path: TestFileDepsMode#test_file_deps_absolute_path().
  TestBlastRadiusMode.test_blast_radius_returns_impact: TestBlastRadiusMode#test_blast_radius_returns_impact().
  TestBlastRadiusMode.test_blast_radius_file_not_found: TestBlastRadiusMode#test_blast_radius_file_not_found().
  TestBlastRadiusMode.test_blast_radius_with_toon: TestBlastRadiusMode#test_blast_radius_with_toon().
  TestCyclesMode.test_cycles_no_cycles: TestCyclesMode#test_cycles_no_cycles().
  TestCyclesMode.test_cycles_with_toon: TestCyclesMode#test_cycles_with_toon().
  TestBlastRecommendation.test_isolated_file: TestBlastRecommendation#test_isolated_file().
  TestBlastRecommendation.test_high_impact: TestBlastRecommendation#test_high_impact().
  TestBlastRecommendation.test_moderate_impact: TestBlastRecommendation#test_moderate_impact().
  TestBlastRecommendation.test_low_impact: TestBlastRecommendation#test_low_impact().
  TestBlastRecommendation.test_no_downstream: TestBlastRecommendation#test_no_downstream().
  TestGraphResetOnPathChange.test_set_project_path_resets_graph: TestGraphResetOnPathChange#test_set_project_path_resets_graph().
  TestGraphResetOnPathChange.test_graph_rebuilt_after_reset: TestGraphResetOnPathChange#test_graph_rebuilt_after_reset().
  TestDefaultArguments.test_default_mode_is_summary: TestDefaultArguments#test_default_mode_is_summary().
  TestDefaultArguments.test_default_format_is_toon: TestDefaultArguments#test_default_format_is_toon().
  TestUnknownMode.test_unknown_mode_raises: TestUnknownMode#test_unknown_mode_raises().
  TestToolDefinition: TestToolDefinition#
  TestToolDefinition.test_definition_has_name: TestToolDefinition#test_definition_has_name().
  TestToolDefinition.test_schema_has_mode: TestToolDefinition#test_schema_has_mode().
  TestToolDefinition.test_schema_modes_include_required: TestToolDefinition#test_schema_modes_include_required().
  TestValidation: TestValidation#
  TestValidation.test_summary_needs_no_file_path: TestValidation#test_summary_needs_no_file_path().
  TestValidation.test_cycles_needs_no_file_path: TestValidation#test_cycles_needs_no_file_path().
  TestValidation.test_blast_radius_requires_file_path: TestValidation#test_blast_radius_requires_file_path().
  TestValidation.test_file_deps_requires_file_path: TestValidation#test_file_deps_requires_file_path().
  TestValidation.test_blast_radius_passes_with_file_path: TestValidation#test_blast_radius_passes_with_file_path().
  TestValidation.test_file_deps_passes_with_file_path: TestValidation#test_file_deps_passes_with_file_path().
  TestValidation.test_default_mode_is_summary: TestValidation#test_default_mode_is_summary().
  TestSummaryMode: TestSummaryMode#
  TestFileDepsMode: TestFileDepsMode#
  TestBlastRadiusMode: TestBlastRadiusMode#
  TestCyclesMode: TestCyclesMode#
  TestResolveFile: TestResolveFile#
  TestResolveFile.test_resolves_by_filename_fuzzy: TestResolveFile#test_resolves_by_filename_fuzzy().
  TestResolveFile.test_resolves_relative_path: TestResolveFile#test_resolves_relative_path().
  TestResolveFile.test_raises_on_missing: TestResolveFile#test_raises_on_missing().
  TestBlastRecommendation: TestBlastRecommendation#
  TestSummaryHelper: TestSummaryHelper#
  TestCyclesHelper: TestCyclesHelper#
  TestFileDepsHelper: TestFileDepsHelper#
  TestGraphResetOnPathChange: TestGraphResetOnPathChange#
  TestNoProjectRoot: TestNoProjectRoot#
  TestDefaultArguments: TestDefaultArguments#
  TestUnknownMode: TestUnknownMode#
  TestBug784CyclesScope: TestBug784CyclesScope#
---
# Module: [`tests/unit/mcp/test_dependency_analysis_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py)

## Classes
### `TestBlastRadiusMode`
- def: [`tests/unit/mcp/test_dependency_analysis_tool.py:207`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py#L207)
- signature: `class TestBlastRadiusMode:`
- members:
  - `test_blast_radius_file_not_found(self, tool, project)` — [`L242`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py#L242)
  - `test_blast_radius_isolated_file(self, tool, tmp_path)` — [`L226`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py#L226)
  - `test_blast_radius_returns_impact(self, tool, project)` — [`L208`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py#L208)
  - `test_blast_radius_with_toon(self, tool, project)` — [`L254`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py#L254)
- uses (calls/refs, reference-scoped): [`execute`](../../../tree_sitter_analyzer/mcp/tools/dependency_analysis_tool.md#DependencyAnalysisTool.execute), [`set_project_path`](../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.set_project_path), [`DependencyAnalysisTool`](../../../tree_sitter_analyzer/mcp/tools/dependency_analysis_tool.md#DependencyAnalysisTool)  (2 test-only)

### `TestBlastRecommendation`
- def: [`tests/unit/mcp/test_dependency_analysis_tool.py:314`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py#L314)
- signature: `class TestBlastRecommendation:`
- members:
  - `test_high_impact(self)` — [`L319`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py#L319)
  - `test_isolated_file(self)` — [`L315`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py#L315)
  - `test_low_impact(self)` — [`L327`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py#L327)
  - `test_moderate_impact(self)` — [`L323`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py#L323)
  - `test_no_downstream(self)` — [`L331`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py#L331)
- uses (calls/refs, reference-scoped): [`_blast_recommendation`](../../../tree_sitter_analyzer/mcp/tools/dependency_analysis_tool.md#_blast_recommendation)

### `TestBug784CyclesScope`
- def: [`tests/unit/mcp/test_dependency_analysis_tool.py:421`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py#L421)
- doc: Bug #784: cycles mode must include a scope label explaining that its
- signature: `class TestBug784CyclesScope:`
- members:
  - `test_cycles_helper_has_scope(self, tmp_path)` — [`L446`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py#L446) — _cycles() helper must include scope at the dict level.
  - `test_cycles_response_has_scope_field(self, tmp_path)` — [`L430`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py#L430)
  - `test_cycles_response_has_scope_note(self, tmp_path)` — [`L438`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py#L438)
  - `test_summary_response_has_scope_field(self, tmp_path)` — [`L454`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py#L454) — summary mode must also include scope so a consumer comparing
  - `test_summary_response_has_scope_note(self, tmp_path)` — [`L464`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py#L464) — summary mode scope_note must reference the import-graph alternative.
- uses (calls/refs, reference-scoped): [`DependencyGraph`](../../../tree_sitter_analyzer/project_graph.md#DependencyGraph), [`execute`](../../../tree_sitter_analyzer/mcp/tools/dependency_analysis_tool.md#DependencyAnalysisTool.execute), [`set_project_path`](../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.set_project_path), [`DependencyAnalysisTool`](../../../tree_sitter_analyzer/mcp/tools/dependency_analysis_tool.md#DependencyAnalysisTool), [`_cycles`](../../../tree_sitter_analyzer/mcp/tools/dependency_analysis_tool.md#_cycles)  (2 test-only)

### `TestCyclesHelper`
- def: [`tests/unit/mcp/test_dependency_analysis_tool.py:351`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py#L351)
- signature: `class TestCyclesHelper:`
- members:
  - `test_cycles_helper_no_cycles(self, project)` — [`L352`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py#L352)
  - `test_cycles_helper_with_cycle(self, tmp_path)` — [`L358`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py#L358)
- uses (calls/refs, reference-scoped): [`DependencyGraph`](../../../tree_sitter_analyzer/project_graph.md#DependencyGraph), [`_cycles`](../../../tree_sitter_analyzer/mcp/tools/dependency_analysis_tool.md#_cycles)  (1 test-only)

### `TestCyclesMode`
- def: [`tests/unit/mcp/test_dependency_analysis_tool.py:268`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py#L268)
- signature: `class TestCyclesMode:`
- members:
  - `test_cycles_clean_project(self, tmp_path)` — [`L290`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py#L290)
  - `test_cycles_no_cycles(self, tool, project)` — [`L269`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py#L269)
  - `test_cycles_with_cycle(self, tmp_path)` — [`L276`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py#L276)
  - `test_cycles_with_toon(self, tool, project)` — [`L285`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py#L285)
- uses (calls/refs, reference-scoped): [`execute`](../../../tree_sitter_analyzer/mcp/tools/dependency_analysis_tool.md#DependencyAnalysisTool.execute), [`set_project_path`](../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.set_project_path), [`DependencyAnalysisTool`](../../../tree_sitter_analyzer/mcp/tools/dependency_analysis_tool.md#DependencyAnalysisTool)  (2 test-only)

### `TestDefaultArguments`
- def: [`tests/unit/mcp/test_dependency_analysis_tool.py:405`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py#L405)
- signature: `class TestDefaultArguments:`
- members:
  - `test_default_format_is_toon(self, tool, project)` — [`L410`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py#L410)
  - `test_default_mode_is_summary(self, tool, project)` — [`L406`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py#L406)
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `TestFileDepsHelper`
- def: [`tests/unit/mcp/test_dependency_analysis_tool.py:366`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py#L366)
- signature: `class TestFileDepsHelper:`
- members:
  - `test_file_deps_helper(self, project)` — [`L367`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py#L367)
  - `test_file_deps_helper_counts(self, project)` — [`L373`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py#L373)
- uses (calls/refs, reference-scoped): [`DependencyGraph`](../../../tree_sitter_analyzer/project_graph.md#DependencyGraph), [`_file_deps`](../../../tree_sitter_analyzer/mcp/tools/dependency_analysis_tool.md#_file_deps)

### `TestFileDepsMode`
- def: [`tests/unit/mcp/test_dependency_analysis_tool.py:140`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py#L140)
- signature: `class TestFileDepsMode:`
- members:
  - `test_file_deps_absolute_path(self, tool, project)` — [`L180`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py#L180)
  - `test_file_deps_file_not_found(self, tool, project)` — [`L168`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py#L168)
  - `test_file_deps_isolated_file(self, tool, tmp_path)` — [`L189`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py#L189)
  - `test_file_deps_returns_dependencies(self, tool, project)` — [`L141`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py#L141)
  - `test_file_deps_with_toon(self, tool, project)` — [`L155`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py#L155)
- uses (calls/refs, reference-scoped): [`execute`](../../../tree_sitter_analyzer/mcp/tools/dependency_analysis_tool.md#DependencyAnalysisTool.execute), [`set_project_path`](../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.set_project_path), [`DependencyAnalysisTool`](../../../tree_sitter_analyzer/mcp/tools/dependency_analysis_tool.md#DependencyAnalysisTool)  (2 test-only)

### `TestGraphResetOnPathChange`
- def: [`tests/unit/mcp/test_dependency_analysis_tool.py:380`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py#L380)
- signature: `class TestGraphResetOnPathChange:`
- members:
  - `test_graph_rebuilt_after_reset(self, tool, project)` — [`L386`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py#L386)
  - `test_set_project_path_resets_graph(self, tool, project)` — [`L381`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py#L381)
- uses (calls/refs, reference-scoped): [`DependencyGraph`](../../../tree_sitter_analyzer/project_graph.md#DependencyGraph)

### `TestNoProjectRoot`
- def: [`tests/unit/mcp/test_dependency_analysis_tool.py:393`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py#L393)
- signature: `class TestNoProjectRoot:`
- members:
  - `test_execute_without_project_root_raises(self)` — [`L394`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py#L394)
  - `test_get_graph_without_root_raises(self)` — [`L399`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py#L399)
- uses (calls/refs, reference-scoped): [`execute`](../../../tree_sitter_analyzer/mcp/tools/dependency_analysis_tool.md#DependencyAnalysisTool.execute), [`DependencyAnalysisTool`](../../../tree_sitter_analyzer/mcp/tools/dependency_analysis_tool.md#DependencyAnalysisTool), [`_get_graph`](../../../tree_sitter_analyzer/mcp/tools/dependency_analysis_tool.md#DependencyAnalysisTool._get_graph)  (1 test-only)

### `TestResolveFile`
- def: [`tests/unit/mcp/test_dependency_analysis_tool.py:300`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py#L300)
- signature: `class TestResolveFile:`
- members:
  - `test_raises_on_missing(self, tool, project)` — [`L309`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py#L309)
  - `test_resolves_by_filename_fuzzy(self, tool, project)` — [`L301`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py#L301)
  - `test_resolves_relative_path(self, tool, project)` — [`L305`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py#L305)

### `TestSummaryHelper`
- def: [`tests/unit/mcp/test_dependency_analysis_tool.py:336`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py#L336)
- signature: `class TestSummaryHelper:`
- members:
  - `test_summary_empty_graph(self, tmp_path)` — [`L344`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py#L344)
  - `test_summary_populates_hubs(self, project)` — [`L337`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py#L337)
- uses (calls/refs, reference-scoped): [`DependencyGraph`](../../../tree_sitter_analyzer/project_graph.md#DependencyGraph), [`_summary`](../../../tree_sitter_analyzer/mcp/tools/dependency_analysis_tool.md#_summary)

### `TestSummaryMode`
- def: [`tests/unit/mcp/test_dependency_analysis_tool.py:110`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py#L110)
- signature: `class TestSummaryMode:`
- members:
  - `test_summary_empty_project(self, tmp_path)` — [`L125`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py#L125)
  - `test_summary_identifies_hub_files(self, tool, project)` — [`L132`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py#L132)
  - `test_summary_returns_node_and_edge_count(self, tool, project)` — [`L111`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py#L111)
  - `test_summary_with_toon_format(self, tool, project)` — [`L120`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py#L120)
- uses (calls/refs, reference-scoped): [`execute`](../../../tree_sitter_analyzer/mcp/tools/dependency_analysis_tool.md#DependencyAnalysisTool.execute), [`set_project_path`](../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.set_project_path), [`DependencyAnalysisTool`](../../../tree_sitter_analyzer/mcp/tools/dependency_analysis_tool.md#DependencyAnalysisTool)  (1 test-only)

### `TestToolDefinition`
- def: [`tests/unit/mcp/test_dependency_analysis_tool.py:49`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py#L49)
- signature: `class TestToolDefinition:`
- members:
  - `test_definition_has_name(self, tool)` — [`L50`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py#L50)
  - `test_schema_has_mode(self, tool)` — [`L55`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py#L55)
  - `test_schema_modes_include_required(self, tool)` — [`L61`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py#L61)

### `TestUnknownMode`
- def: [`tests/unit/mcp/test_dependency_analysis_tool.py:415`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py#L415)
- signature: `class TestUnknownMode:`
- members:
  - `test_unknown_mode_raises(self, tool, project)` — [`L416`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py#L416)
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `TestValidation`
- def: [`tests/unit/mcp/test_dependency_analysis_tool.py:70`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py#L70)
- signature: `class TestValidation:`
- members:
  - `test_blast_is_alias_for_blast_radius(self, tool)` — [`L100`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py#L100)
  - `test_blast_radius_passes_with_file_path(self, tool)` — [`L85`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py#L85)
  - `test_blast_radius_requires_file_path(self, tool)` — [`L77`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py#L77)
  - `test_cycles_needs_no_file_path(self, tool)` — [`L74`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py#L74)
  - `test_default_mode_is_summary(self, tool)` — [`L97`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py#L97)
  - `test_file_deps_passes_with_file_path(self, tool)` — [`L91`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py#L91)
  - `test_file_deps_requires_file_path(self, tool)` — [`L81`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py#L81)
  - `test_summary_needs_no_file_path(self, tool)` — [`L71`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py#L71)
- uses (calls/refs, reference-scoped): [`DependencyAnalysisTool`](../../../tree_sitter_analyzer/mcp/tools/dependency_analysis_tool.md#DependencyAnalysisTool), [`_normalize_mode`](../../../tree_sitter_analyzer/mcp/tools/dependency_analysis_tool.md#DependencyAnalysisTool._normalize_mode)

## Functions
- `_run(coro)` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py#L20)
- `_write(tmp_path: Path, rel: str, content: str)` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py#L24)
- `project(tmp_path)` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py#L32)
- `tool(project)` — [`L43`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_dependency_analysis_tool.py#L43)

