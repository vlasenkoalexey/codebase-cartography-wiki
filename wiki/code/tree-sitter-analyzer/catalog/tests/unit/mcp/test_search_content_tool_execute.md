---
title: 'Module: tests/unit/mcp/test_search_content_tool_execute.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_search_content_tool_execute.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_search_content_tool_execute`/
symbols:
  TestApplyLimits.test_default_cap_applied_when_no_user_max: TestApplyLimits#test_default_cap_applied_when_no_user_max().
  TestExecute.test_execute_with_cache_disabled: TestExecute#test_execute_with_cache_disabled().
  TestApplyLimits.test_no_truncation_when_below_default_cap: TestApplyLimits#test_no_truncation_when_below_default_cap().
  TestApplyLimits.test_user_max_overrides_default_cap: TestApplyLimits#test_user_max_overrides_default_cap().
  TestApplyLimits.test_user_max_no_truncation_when_below: TestApplyLimits#test_user_max_no_truncation_when_below().
  TestApplyLimits._make_matches: TestApplyLimits#_make_matches().
  TestApplyLimits._make_mock_fd: TestApplyLimits#_make_mock_fd().
  tool: tool().
  test_apply_limits_aggregate_modes_uncapped: test_apply_limits_aggregate_modes_uncapped().
  sample_project_structure: sample_project_structure().
  TestExecute: TestExecute#
  TestExecute.test_execute_rg_not_found: TestExecute#test_execute_rg_not_found().
  TestExecute.test_execute_total_only_mode: TestExecute#test_execute_total_only_mode().
  TestExecute.test_execute_count_only_matches_mode: TestExecute#test_execute_count_only_matches_mode().
  TestExecute.test_execute_summary_only_mode: TestExecute#test_execute_summary_only_mode().
  TestExecute.test_execute_group_by_file_mode: TestExecute#test_execute_group_by_file_mode().
  TestExecute.test_execute_with_file_output: TestExecute#test_execute_with_file_output().
  TestExecute.test_execute_with_suppress_output: TestExecute#test_execute_with_suppress_output().
  TestExecute.test_execute_with_toon_format: TestExecute#test_execute_with_toon_format().
  TestExecute.test_execute_rg_failure: TestExecute#test_execute_rg_failure().
  TestExecute.test_execute_with_cache_hit: TestExecute#test_execute_with_cache_hit().
  TestExecute.test_execute_with_parallel_processing: TestExecute#test_execute_with_parallel_processing().
  TestExecute.test_execute_with_files_parameter: TestExecute#test_execute_with_files_parameter().
  TestExecute.test_execute_with_optimize_paths: TestExecute#test_execute_with_optimize_paths().
  TestExecute.test_execute_file_save_error: TestExecute#test_execute_file_save_error().
  TestExecute.test_execute_with_timeout: TestExecute#test_execute_with_timeout().
  TestExecute.test_execute_with_max_count: TestExecute#test_execute_with_max_count().
  TestApplyLimits: TestApplyLimits#
---
# Module: [`tests/unit/mcp/test_search_content_tool_execute.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_execute.py)

## Classes
### `TestApplyLimits`
- def: [`tests/unit/mcp/test_search_content_tool_execute.py:533`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_execute.py#L533)
- doc: Unit tests for apply_limits — DF-1 default cap and explicit max_count.
- signature: `class TestApplyLimits:`
- members:
  - `test_default_cap_applied_when_no_user_max(self)` — [`L547`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_execute.py#L547) — DF-1: when max_count absent, DEFAULT_CONTENT_LISTED_CAP=50 caps matches.
  - `test_no_truncation_when_below_default_cap(self)` — [`L560`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_execute.py#L560) — DF-1: 30 matches with no user max → no truncation.
  - `test_user_max_no_truncation_when_below(self)` — [`L580`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_execute.py#L580) — DF-1 backward compat: user max_count=100 with 30 matches → no truncation.
  - `test_user_max_overrides_default_cap(self)` — [`L569`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_execute.py#L569) — DF-1 backward compat: explicit max_count always wins over default.
- protocol/private: `_make_matches`[`L536`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_execute.py#L536), `_make_mock_fd`[`L542`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_execute.py#L542)
- uses (calls/refs, reference-scoped): [`apply_limits`](../../../tree_sitter_analyzer/mcp/tools/search_content_response.md#apply_limits), [`DEFAULT_CONTENT_LISTED_CAP`](../../../tree_sitter_analyzer/mcp/tools/search_content_response.md#DEFAULT_CONTENT_LISTED_CAP)

### `TestExecute`
- def: [`tests/unit/mcp/test_search_content_tool_execute.py:41`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_execute.py#L41)
- doc: Tests for execute method.
- signature: `class TestExecute:`
- members:
  - `test_execute_count_only_matches_mode(self, tool, sample_project_structure)` — [`L85`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_execute.py#L85) — Test execute in count_only_matches mode.
  - `test_execute_file_save_error(self, tool, sample_project_structure)` — [`L453`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_execute.py#L453) — Test execute when file save fails.
  - `test_execute_group_by_file_mode(self, tool, sample_project_structure)` — [`L150`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_execute.py#L150) — Test execute in group_by_file mode.
  - `test_execute_rg_failure(self, tool, sample_project_structure)` — [`L289`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_execute.py#L289) — Test execute when ripgrep command fails.
  - `test_execute_rg_not_found(self, tool)` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_execute.py#L45) — Test execute fails when rg command is not found.
  - `test_execute_summary_only_mode(self, tool, sample_project_structure)` — [`L117`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_execute.py#L117) — Test execute in summary_only mode.
  - `test_execute_total_only_mode(self, tool, sample_project_structure)` — [`L57`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_execute.py#L57) — Test execute in total_only mode.
  - `test_execute_with_cache_disabled(self, tool, sample_project_structure)` — [`L332`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_execute.py#L332) — Test execute with cache disabled.
  - `test_execute_with_cache_hit(self, tool, sample_project_structure)` — [`L312`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_execute.py#L312) — Test execute with cache hit.
  - `test_execute_with_file_output(self, tool, sample_project_structure)` — [`L186`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_execute.py#L186) — Test execute with file output.
  - `test_execute_with_files_parameter(self, tool, sample_project_structure)` — [`L396`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_execute.py#L396) — Test execute with files parameter instead of roots.
  - `test_execute_with_max_count(self, tool, sample_project_structure)` — [`L510`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_execute.py#L510) — Test execute with max_count parameter.
  - `test_execute_with_optimize_paths(self, tool, sample_project_structure)` — [`L418`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_execute.py#L418) — Test execute with optimize_paths.
  - `test_execute_with_parallel_processing(self, tool, sample_project_structure)` — [`L357`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_execute.py#L357) — Test execute with parallel processing enabled.
  - `test_execute_with_suppress_output(self, tool, sample_project_structure)` — [`L219`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_execute.py#L219) — Test execute with suppress_output.
  - `test_execute_with_timeout(self, tool, sample_project_structure)` — [`L487`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_execute.py#L487) — Test execute with timeout parameter.
  - `test_execute_with_toon_format(self, tool, sample_project_structure)` — [`L256`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_execute.py#L256) — Test execute with toon output format.
- uses (calls/refs, reference-scoped): [`SearchContentTool`](../../../tree_sitter_analyzer/mcp/tools/search_content_tool.md#SearchContentTool), [`execute`](../../../tree_sitter_analyzer/mcp/tools/search_content_tool.md#SearchContentTool.execute), [`cache`](../../../tree_sitter_analyzer/mcp/tools/search_content_tool.md#SearchContentTool.cache)

## Functions
- `sample_project_structure(tmp_path: Path)` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_execute.py#L26) — Create a sample project structure for testing.
- `test_apply_limits_aggregate_modes_uncapped()` — [`L592`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_execute.py#L592) — Codex P2 (#505): summary/group_by_file must see ALL matches —
- `tool()` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_execute.py#L20) — Create a fresh tool instance for each test.

