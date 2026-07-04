---
title: 'Module: tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.utils.change_impact_analysis`/
symbols:
  _build_change_impact_result: _build_change_impact_result().
  _build_test_only_change_impact_result: _build_test_only_change_impact_result().
  _build_verification_strategy: _build_verification_strategy().
  _attach_doc_drift_hints: _attach_doc_drift_hints().
  _find_test_files: _find_test_files().
  ChangeImpactRequest.changed_files: ChangeImpactRequest#changed_files.
  _ensure_ast_cache: _ensure_ast_cache().
  _classify_changed_files: _classify_changed_files().
  ChangeImpactRequest.project_root: ChangeImpactRequest#project_root.
  _attach_constraint_violations: _attach_constraint_violations().
  ChangeImpactRequest: ChangeImpactRequest#
  _build_file_impacts: _build_file_impacts().
  _attach_hot_zone_risk: _attach_hot_zone_risk().
  _low_impact_pytest_command: _low_impact_pytest_command().
  ChangeImpactRequest.mode: ChangeImpactRequest#mode.
  ChangeImpactRequest.include_tests: ChangeImpactRequest#include_tests.
  _test_file_matches_change: _test_file_matches_change().
  _load_dependency_graph: _load_dependency_graph().
  _build_test_plan: _build_test_plan().
  _is_runnable_test_change: _is_runnable_test_change().
  _is_test_only_change_set: _is_test_only_change_set().
  ChangeImpactRequest.diff_stat: ChangeImpactRequest#diff_stat.
  _enrich_with_cache_symbols: _enrich_with_cache_symbols().
  _find_affected_symbols: _find_affected_symbols().
  _is_runnable_test_file: _is_runnable_test_file().
  ChangeImpactRequest.resource_profile: ChangeImpactRequest#resource_profile.
  _append_large_dirty_hint: _append_large_dirty_hint().
  ChangeImpactRequest.scope_paths: ChangeImpactRequest#scope_paths.
  ChangeImpactRequest.agent_summary_only: ChangeImpactRequest#agent_summary_only.
  _with_local_low_impact_profile: _with_local_low_impact_profile().
  _hot_zone_symbols_for_files: _hot_zone_symbols_for_files().
  _assess_risk: _assess_risk().
  _select_verification_path: _select_verification_path().
  _file_symbol_dict: _file_symbol_dict().
  _build_no_changes_result: _build_no_changes_result.
  _build_agent_summary: _build_agent_summary.
  logger: logger.
  FOCUSED_TEST_COMMAND_LIMIT: FOCUSED_TEST_COMMAND_LIMIT.
  _build_change_impact_response: _build_change_impact_response.
  TESTS_TO_RUN_DISPLAY_LIMIT: TESTS_TO_RUN_DISPLAY_LIMIT.
  RESOURCE_PROFILE_DEFAULT: RESOURCE_PROFILE_DEFAULT.
  RESOURCE_PROFILE_LOCAL_LOW_IMPACT: RESOURCE_PROFILE_LOCAL_LOW_IMPACT.
  TEST_DIRS: TEST_DIRS.
  TEST_SUFFIXES: TEST_SUFFIXES.
  _file_impact_dict: _file_impact_dict().
  _drop_pytest_quiet_and_worker_flags: _drop_pytest_quiet_and_worker_flags().
  _symbol_dict: _symbol_dict().
  _affected_symbol_dict: _affected_symbol_dict().
  _inject_cs_into_impact: _inject_cs_into_impact().
  _hot_zone_factor: _hot_zone_factor().
  _class_result_dict: _class_result_dict().
  _HOT_ZONE_THRESHOLD: _HOT_ZONE_THRESHOLD.
  _CLI_SURFACE_FILES: _CLI_SURFACE_FILES.
  _CLI_SURFACE_PREFIXES: _CLI_SURFACE_PREFIXES.
  _FACADE_DOC_FILES: _FACADE_DOC_FILES.
  _FACADE_TOOL_PREFIX: _FACADE_TOOL_PREFIX.
  _FACADE_TOOL_EXCLUDE: _FACADE_TOOL_EXCLUDE.
---
# Module: [`tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.py)

## Classes
### `ChangeImpactRequest`
- def: [`tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.py:65`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.py#L65)
- doc: Inputs needed to build a change-impact response.
- signature: `class ChangeImpactRequest:`
- members:
  - `agent_summary_only` — [`L74`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.py#L74)
  - `changed_files` — [`L69`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.py#L69)
  - `diff_stat` — [`L70`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.py#L70)
  - `include_tests` — [`L72`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.py#L72)
  - `mode` — [`L68`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.py#L68)
  - `project_root` — [`L71`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.py#L71)
  - `resource_profile` — [`L75`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.py#L75)
  - `scope_paths` — [`L73`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.py#L73)
- uses (calls/refs, reference-scoped): [`RESOURCE_PROFILE_DEFAULT`](change_impact_analysis.md#RESOURCE_PROFILE_DEFAULT)
- used by: [`_build_change_impact_result`](change_impact_analysis.md#_build_change_impact_result), [`execute`](../change_impact_tool.md#ChangeImpactTool.execute), [`_build_test_only_change_impact_result`](change_impact_analysis.md#_build_test_only_change_impact_result), [`_execute_pr_analysis`](../change_impact_tool.md#ChangeImpactTool._execute_pr_analysis), [`_attach_constraint_violations`](change_impact_analysis.md#_attach_constraint_violations), [`_attach_hot_zone_risk`](change_impact_analysis.md#_attach_hot_zone_risk)  (6 test-only)

## Functions
- `_affected_symbol_dict(rel: str, s: dict[str, Any])` — [`L504`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.py#L504) — Build one result entry for _find_affected_symbols.
- `_append_large_dirty_hint(hint: str, changed_count: int)` — [`L447`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.py#L447) — Append large-diff guidance without obscuring the primary hint.
- `_assess_risk(changed_files: list[str], affected: set[str], graph: Any)` — [`L139`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.py#L139) — Assess change risk level based on blast radius size.
- `_attach_constraint_violations(result: dict[str, Any], request: ChangeImpactRequest, affected: set[str])` — [`L906`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.py#L906) — Decorate the change-impact result with persisted constraint violations.
- `_attach_doc_drift_hints(result: dict[str, Any], changed_files: list[str])` — [`L857`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.py#L857) — Append deterministic doc-drift verification steps for known CLI/MCP surfaces.
- `_attach_hot_zone_risk(result: dict[str, Any], request: ChangeImpactRequest)` — [`L743`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.py#L743) — Decorate the change-impact result with temporal hot-zone risk factors.
- `_build_change_impact_result(request: ChangeImpactRequest)` — [`L634`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.py#L634) — Build the full change-impact response for changed files. — documented in [tree_sitter_analyzer-mcp-tools-base_tool](../../../../../concepts/tree_sitter_analyzer-mcp-tools-base_tool.md)
- `_build_file_impacts(changed_files: list[str], graph: Any | None)` — [`L164`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.py#L164) — Build per-file impact rows and the total affected file set.
- `_build_test_only_change_impact_result(request: ChangeImpactRequest)` — [`L227`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.py#L227) — Build a fast change-impact response for test-only edits.
- `_build_test_plan(changed_files: list[str], graph: Any | None, include_tests: bool)` — [`L183`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.py#L183) — Build changed-file-to-test mapping and a sorted runnable test list.
- `_build_verification_strategy(*, changed_count: int, tests_to_run: list[str], verification: dict[str, Any], resource_profile: str = RESOURCE_PROFILE_DEFAULT)` — [`L288`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.py#L288) — Build an action-oriented verification strategy for agents.
- `_class_result_dict(file_path: str, language: str, class_dict: dict[str, Any])` — [`L543`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.py#L543) — Build one semantic-classification result entry.
- `_classify_changed_files(changed_files: list[str], project_root: str | None)` — [`L949`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.py#L949) — Run semantic_classify over a list of changed files; best-effort. — documented in [tree_sitter_analyzer-ast_diff](../../../../../concepts/tree_sitter_analyzer-ast_diff.md)
- `_drop_pytest_quiet_and_worker_flags(parts: list[str])` — [`L391`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.py#L391) — Remove command-level pytest quiet/xdist flags before applying local caps.
- `_enrich_with_cache_symbols(changed_files: list[str], cache: Any)` — [`L555`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.py#L555) — Enrich changed files with symbol-level detail from the AST cache.
- `_ensure_ast_cache(project_root: str | None, changed_files: list[str])` — [`L457`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.py#L457) — Return an open ASTCache, auto-indexing if the cache is empty or stale. — documented in [tree_sitter_analyzer-ast_cache](../../../../../concepts/tree_sitter_analyzer-ast_cache.md)
- `_file_impact_dict(changed_file: str, graph: Any, fwd: set[str])` — [`L155`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.py#L155) — Build one file-impact row for _build_file_impacts.
- `_file_symbol_dict(rel: str, symbols: list[dict[str, Any]])` — [`L494`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.py#L494) — Build the enriched file entry for _enrich_with_cache_symbols.
- `_find_affected_symbols(affected_files: set[str], cache: Any)` — [`L591`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.py#L591) — Look up top-level symbols in affected (dependent) files.
- `_find_test_files(changed_files: list[str], graph_nodes: set[str])` — [`L78`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.py#L78) — Map changed files to related test files using stem matching.
- `_hot_zone_factor(row: Any)` — [`L527`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.py#L527) — Build one hot-zone risk-factor dict from a hot-rows query result.
- `_hot_zone_symbols_for_files(project_root: str, changed_files: list[str])` — [`L786`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.py#L786) — Return per-symbol activation rows above the hot-zone threshold.
- `_inject_cs_into_impact(fi: dict[str, Any], changed_symbols: list[dict[str, Any]])` — [`L515`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.py#L515) — Inject changed-symbol metadata into a file-impact row (in-place).
- `_is_runnable_test_change(path: str)` — [`L204`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.py#L204) — Return True when a changed path is itself a direct test target.
- `_is_runnable_test_file(path: str, test_dirs: set[str], test_suffixes: tuple[str, ...])` — [`L118`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.py#L118) — Return True for files that are intended to be direct pytest targets.
- `_is_test_only_change_set(changed_files: list[str])` — [`L209`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.py#L209) — Return True when every changed file is a runnable test file.
- `_load_dependency_graph(project_root: str | None)` — [`L216`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.py#L216) — Build the dependency graph, returning None when analysis is unavailable.
- `_low_impact_pytest_command(command: str)` — [`L367`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.py#L367) — Rewrite a pytest command so it is friendlier to an interactive machine.
- `_select_verification_path(*, verification: dict[str, Any], focused_command: str, final_command: str, tests_to_run_count: int, default_command: str)` — [`L410`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.py#L410) — Choose verification steps, strategy label, and hint text.
- `_symbol_dict(s: dict[str, Any])` — [`L488`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.py#L488) — Build a compact symbol dict for cache-enrichment output.
- `_test_file_matches_change(test_file: str, changed_file: str)` — [`L105`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.py#L105) — Return True when a test filename appears related to a changed file.
- `_with_local_low_impact_profile(strategy: dict[str, Any], *, verification: dict[str, Any], focused_command: str, final_command: str)` — [`L333`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.py#L333) — Attach local low-impact pytest commands while preserving CI intent.

## Module values
- `FOCUSED_TEST_COMMAND_LIMIT` — [`L47`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.py#L47)
- `RESOURCE_PROFILE_DEFAULT` — [`L48`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.py#L48)
- `RESOURCE_PROFILE_LOCAL_LOW_IMPACT` — [`L49`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.py#L49)
- `TESTS_TO_RUN_DISPLAY_LIMIT` — [`L46`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.py#L46)
- `TEST_DIRS` — [`L50`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.py#L50)
- `TEST_SUFFIXES` — [`L51`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.py#L51)
- `_CLI_SURFACE_FILES` — [`L832`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.py#L832)
- `_CLI_SURFACE_PREFIXES` — [`L840`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.py#L840)
- `_FACADE_DOC_FILES` — [`L842`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.py#L842)
- `_FACADE_TOOL_EXCLUDE` — [`L849`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.py#L849)
- `_FACADE_TOOL_PREFIX` — [`L848`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.py#L848)
- `_HOT_ZONE_THRESHOLD` — [`L740`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.py#L740)
- `_build_agent_summary` — [`L945`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.py#L945)
- `_build_change_impact_response` — [`L946`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.py#L946)
- `_build_no_changes_result` — [`L944`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.py#L944)
- `logger` — [`L44`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/change_impact_analysis.py#L44)

