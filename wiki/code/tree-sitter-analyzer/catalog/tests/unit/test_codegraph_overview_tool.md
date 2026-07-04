---
title: 'Module: tests/unit/test_codegraph_overview_tool.py'
type: catalog
provenance: extracted
module: tests/unit/test_codegraph_overview_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_codegraph_overview_tool`/
symbols:
  _execute: _execute().
  TestCodeGraphOverviewToolInit.test_init_with_project_root: TestCodeGraphOverviewToolInit#test_init_with_project_root().
  PY_PROJECT: PY_PROJECT.
  tool: tool().
  TestCodeGraphOverviewToolInit.test_init_without_project_root: TestCodeGraphOverviewToolInit#test_init_without_project_root().
  TestCodeGraphOverviewToolInit.test_get_call_graph_raises_without_root: TestCodeGraphOverviewToolInit#test_get_call_graph_raises_without_root().
  TestCodeGraphOverviewToolExecute.test_execute_returns_success: TestCodeGraphOverviewToolExecute#test_execute_returns_success().
  TestCodeGraphOverviewToolExecute.test_execute_empty_project: TestCodeGraphOverviewToolExecute#test_execute_empty_project().
  TestFindHubFunctions.test_hub_caller_files_are_sampled: TestFindHubFunctions#test_hub_caller_files_are_sampled().
  TestComputeDepthDistribution.test_handles_cycles_without_recursive_explosion: TestComputeDepthDistribution#test_handles_cycles_without_recursive_explosion().
  TestComputeDepthDistribution.test_uses_function_references_not_ambiguous_names: TestComputeDepthDistribution#test_uses_function_references_not_ambiguous_names().
  TestComputeDepthDistribution.test_caps_deep_call_chains: TestComputeDepthDistribution#test_caps_deep_call_chains().
  TestCodeGraphOverviewToolInit.test_set_project_path_resets_graph: TestCodeGraphOverviewToolInit#test_set_project_path_resets_graph().
  TestCodeGraphOverviewToolExecute.test_execute_summary_fields: TestCodeGraphOverviewToolExecute#test_execute_summary_fields().
  TestCodeGraphOverviewToolExecute.test_execute_entry_points: TestCodeGraphOverviewToolExecute#test_execute_entry_points().
  TestCodeGraphOverviewToolExecute.test_execute_hub_functions: TestCodeGraphOverviewToolExecute#test_execute_hub_functions().
  TestCodeGraphOverviewToolExecute.test_execute_dead_code: TestCodeGraphOverviewToolExecute#test_execute_dead_code().
  TestCodeGraphOverviewToolExecute.test_execute_depth_distribution: TestCodeGraphOverviewToolExecute#test_execute_depth_distribution().
  TestCodeGraphOverviewToolExecute.test_execute_module_coupling: TestCodeGraphOverviewToolExecute#test_execute_module_coupling().
  TestCodeGraphOverviewToolExecute.test_execute_toon_format: TestCodeGraphOverviewToolExecute#test_execute_toon_format().
  TestCodeGraphOverviewToolExecute.test_execute_has_agent_summary_envelope: TestCodeGraphOverviewToolExecute#test_execute_has_agent_summary_envelope().
  TestFindEntryPoints.test_finds_entry_points: TestFindEntryPoints#test_finds_entry_points().
  TestFindEntryPoints.test_respects_limit: TestFindEntryPoints#test_respects_limit().
  TestFindHubFunctions.test_hubs_have_min_three_callers: TestFindHubFunctions#test_hubs_have_min_three_callers().
  TestFindDeadCode.test_dead_code_has_no_callers_or_callees: TestFindDeadCode#test_dead_code_has_no_callers_or_callees().
  TestComputeDepthDistribution.test_returns_expected_keys: TestComputeDepthDistribution#test_returns_expected_keys().
  TestComputeModuleCoupling.test_coupling_cross_file_only: TestComputeModuleCoupling#test_coupling_cross_file_only().
  FIXTURES_DIR: FIXTURES_DIR.
  TestCodeGraphOverviewToolInit: TestCodeGraphOverviewToolInit#
  TestCodeGraphOverviewToolInit.test_get_call_graph_caches: TestCodeGraphOverviewToolInit#test_get_call_graph_caches().
  TestCodeGraphOverviewToolDefinition: TestCodeGraphOverviewToolDefinition#
  TestCodeGraphOverviewToolDefinition.test_get_tool_definition: TestCodeGraphOverviewToolDefinition#test_get_tool_definition().
  TestCodeGraphOverviewToolDefinition.test_get_tool_schema_has_required_properties: TestCodeGraphOverviewToolDefinition#test_get_tool_schema_has_required_properties().
  TestCodeGraphOverviewToolDefinition.test_validate_arguments_always_true: TestCodeGraphOverviewToolDefinition#test_validate_arguments_always_true().
  TestCodeGraphOverviewToolExecute: TestCodeGraphOverviewToolExecute#
  TestFindEntryPoints: TestFindEntryPoints#
  TestFindHubFunctions: TestFindHubFunctions#
  TestFindDeadCode: TestFindDeadCode#
  TestComputeDepthDistribution: TestComputeDepthDistribution#
  TestComputeModuleCoupling: TestComputeModuleCoupling#
---
# Module: [`tests/unit/test_codegraph_overview_tool.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_overview_tool.py)

## Classes
### `TestCodeGraphOverviewToolDefinition`
- def: [`tests/unit/test_codegraph_overview_tool.py:68`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_overview_tool.py#L68)
- signature: `class TestCodeGraphOverviewToolDefinition:`
- members:
  - `test_get_tool_definition(self, tool)` — [`L69`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_overview_tool.py#L69)
  - `test_get_tool_schema_has_required_properties(self, tool)` — [`L76`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_overview_tool.py#L76)
  - `test_validate_arguments_always_true(self, tool)` — [`L85`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_overview_tool.py#L85)

### `TestCodeGraphOverviewToolExecute`
- def: [`tests/unit/test_codegraph_overview_tool.py:95`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_overview_tool.py#L95)
- signature: `class TestCodeGraphOverviewToolExecute:`
- members:
  - `test_execute_dead_code(self, tool)` — [`L135`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_overview_tool.py#L135)
  - `test_execute_depth_distribution(self, tool)` — [`L142`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_overview_tool.py#L142)
  - `test_execute_empty_project(self, tmp_path)` — [`L175`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_overview_tool.py#L175)
  - `test_execute_entry_points(self, tool)` — [`L115`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_overview_tool.py#L115)
  - `test_execute_has_agent_summary_envelope(self, tool)` — [`L162`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_overview_tool.py#L162) — #743: codegraph_overview must include agent_summary dict and summary_line.
  - `test_execute_hub_functions(self, tool)` — [`L128`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_overview_tool.py#L128)
  - `test_execute_module_coupling(self, tool)` — [`L150`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_overview_tool.py#L150)
  - `test_execute_returns_success(self, tool)` — [`L97`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_overview_tool.py#L97)
  - `test_execute_summary_fields(self, tool)` — [`L103`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_overview_tool.py#L103)
  - `test_execute_toon_format(self, tool)` — [`L157`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_overview_tool.py#L157)
- uses (calls/refs, reference-scoped): [`CodeGraphOverviewTool`](../../tree_sitter_analyzer/mcp/tools/codegraph_overview_tool.md#CodeGraphOverviewTool)  (2 test-only)

### `TestCodeGraphOverviewToolInit`
- def: [`tests/unit/test_codegraph_overview_tool.py:36`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_overview_tool.py#L36)
- signature: `class TestCodeGraphOverviewToolInit:`
- members:
  - `test_get_call_graph_caches(self, tool)` — [`L52`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_overview_tool.py#L52)
  - `test_get_call_graph_raises_without_root(self)` — [`L57`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_overview_tool.py#L57)
  - `test_init_with_project_root(self)` — [`L37`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_overview_tool.py#L37)
  - `test_init_without_project_root(self)` — [`L42`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_overview_tool.py#L42)
  - `test_set_project_path_resets_graph(self, tool)` — [`L46`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_overview_tool.py#L46)
- uses (calls/refs, reference-scoped): [`project_root`](../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.project_root), [`CodeGraphOverviewTool`](../../tree_sitter_analyzer/mcp/tools/codegraph_overview_tool.md#CodeGraphOverviewTool), [`get_call_graph`](../../tree_sitter_analyzer/mcp/tools/codegraph_overview_tool.md#CodeGraphOverviewTool.get_call_graph), [`call_graph_initialized`](../../tree_sitter_analyzer/mcp/tools/codegraph_overview_tool.md#CodeGraphOverviewTool.call_graph_initialized)  (1 test-only)

### `TestComputeDepthDistribution`
- def: [`tests/unit/test_codegraph_overview_tool.py:245`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_overview_tool.py#L245)
- signature: `class TestComputeDepthDistribution:`
- members:
  - `test_caps_deep_call_chains(self)` — [`L287`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_overview_tool.py#L287)
  - `test_handles_cycles_without_recursive_explosion(self)` — [`L255`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_overview_tool.py#L255)
  - `test_returns_expected_keys(self, tool)` — [`L246`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_overview_tool.py#L246)
  - `test_uses_function_references_not_ambiguous_names(self)` — [`L271`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_overview_tool.py#L271)
- uses (calls/refs, reference-scoped): [`FunctionRef`](../../tree_sitter_analyzer/call_graph.md#FunctionRef), [`_compute_depth_distribution`](../../tree_sitter_analyzer/mcp/tools/codegraph_overview_tool.md#_compute_depth_distribution)

### `TestComputeModuleCoupling`
- def: [`tests/unit/test_codegraph_overview_tool.py:301`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_overview_tool.py#L301)
- signature: `class TestComputeModuleCoupling:`
- members:
  - `test_coupling_cross_file_only(self, tool)` — [`L302`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_overview_tool.py#L302)
- uses (calls/refs, reference-scoped): [`_compute_module_coupling`](../../tree_sitter_analyzer/mcp/tools/codegraph_overview_tool.md#_compute_module_coupling)

### `TestFindDeadCode`
- def: [`tests/unit/test_codegraph_overview_tool.py:235`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_overview_tool.py#L235)
- signature: `class TestFindDeadCode:`
- members:
  - `test_dead_code_has_no_callers_or_callees(self, tool)` — [`L236`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_overview_tool.py#L236)
- uses (calls/refs, reference-scoped): [`_find_dead_code`](../../tree_sitter_analyzer/mcp/tools/codegraph_overview_tool.md#_find_dead_code)

### `TestFindEntryPoints`
- def: [`tests/unit/test_codegraph_overview_tool.py:191`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_overview_tool.py#L191)
- signature: `class TestFindEntryPoints:`
- members:
  - `test_finds_entry_points(self, tool)` — [`L192`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_overview_tool.py#L192)
  - `test_respects_limit(self, tool)` — [`L201`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_overview_tool.py#L201)
- uses (calls/refs, reference-scoped): [`_find_entry_points`](../../tree_sitter_analyzer/mcp/tools/codegraph_overview_tool.md#_find_entry_points)

### `TestFindHubFunctions`
- def: [`tests/unit/test_codegraph_overview_tool.py:208`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_overview_tool.py#L208)
- signature: `class TestFindHubFunctions:`
- members:
  - `test_hub_caller_files_are_sampled(self)` — [`L216`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_overview_tool.py#L216)
  - `test_hubs_have_min_three_callers(self, tool)` — [`L209`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_overview_tool.py#L209)
- uses (calls/refs, reference-scoped): [`FunctionRef`](../../tree_sitter_analyzer/call_graph.md#FunctionRef), [`_find_hub_functions`](../../tree_sitter_analyzer/mcp/tools/codegraph_overview_tool.md#_find_hub_functions)

## Functions
- `_execute(tool, args=None)` — [`L27`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_overview_tool.py#L27)
- `tool()` — [`L23`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_overview_tool.py#L23)

## Module values
- `FIXTURES_DIR` — [`L18`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_overview_tool.py#L18)
- `PY_PROJECT` — [`L19`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_overview_tool.py#L19)

