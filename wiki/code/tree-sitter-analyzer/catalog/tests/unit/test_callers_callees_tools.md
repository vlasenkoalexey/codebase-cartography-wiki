---
title: 'Module: tests/unit/test_callers_callees_tools.py'
type: catalog
provenance: extracted
module: tests/unit/test_callers_callees_tools.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_callers_callees_tools`/
symbols:
  TestEmptyIndexHint.test_callers_rebuild_marker_warns_without_phantom_count: TestEmptyIndexHint#test_callers_rebuild_marker_warns_without_phantom_count().
  TestEmptyIndexHint.test_callees_rebuild_marker_warns_without_phantom_count: TestEmptyIndexHint#test_callees_rebuild_marker_warns_without_phantom_count().
  TestEmptyIndexHint.test_callers_non_empty_index_no_spurious_hint: TestEmptyIndexHint#test_callers_non_empty_index_no_spurious_hint().
  TestEmptyIndexHint.test_callers_built_index_zero_edges_no_hint: TestEmptyIndexHint#test_callers_built_index_zero_edges_no_hint().
  TestEmptyIndexHint.test_callees_built_index_zero_edges_no_hint: TestEmptyIndexHint#test_callees_built_index_zero_edges_no_hint().
  TestCodeGraphCallersTool.test_project_root_change_resets_cache: TestCodeGraphCallersTool#test_project_root_change_resets_cache().
  TestCodeGraphCalleesTool.test_project_root_change_resets_cache: TestCodeGraphCalleesTool#test_project_root_change_resets_cache().
  TestCallerCalleeIntegration.test_unknown_function_returns_empty: TestCallerCalleeIntegration#test_unknown_function_returns_empty().
  TestCallerCalleeIntegration.test_callers_and_callees_share_relation_bootstrap: TestCallerCalleeIntegration#test_callers_and_callees_share_relation_bootstrap().
  callers_tool: callers_tool().
  callees_tool: callees_tool().
  TestCodeGraphCallersTool.test_execute_returns_callers: TestCodeGraphCallersTool#test_execute_returns_callers().
  TestCodeGraphCallersTool.test_execute_with_file_path: TestCodeGraphCallersTool#test_execute_with_file_path().
  TestCodeGraphCallersTool.test_execute_toon_format: TestCodeGraphCallersTool#test_execute_toon_format().
  TestCodeGraphCallersTool.test_caller_inlines_source_body: TestCodeGraphCallersTool#test_caller_inlines_source_body().
  TestCodeGraphCallersTool.test_no_project_root_raises: TestCodeGraphCallersTool#test_no_project_root_raises().
  TestCodeGraphCalleesTool.test_execute_returns_callees: TestCodeGraphCalleesTool#test_execute_returns_callees().
  TestCodeGraphCalleesTool.test_execute_with_file_path: TestCodeGraphCalleesTool#test_execute_with_file_path().
  TestCodeGraphCalleesTool.test_callee_inlines_source_body: TestCodeGraphCalleesTool#test_callee_inlines_source_body().
  TestCodeGraphCalleesTool.test_execute_toon_format: TestCodeGraphCalleesTool#test_execute_toon_format().
  TestCodeGraphCalleesTool.test_no_project_root_raises: TestCodeGraphCalleesTool#test_no_project_root_raises().
  TestHonestTruncationCallers.test_default_limit_caps_at_50: TestHonestTruncationCallers#test_default_limit_caps_at_50().
  TestHonestTruncationCallers.test_raised_limit_shows_all: TestHonestTruncationCallers#test_raised_limit_shows_all().
  TestHonestTruncationCallers.test_no_truncation_when_few_callers: TestHonestTruncationCallers#test_no_truncation_when_few_callers().
  TestHonestTruncationCallers.test_truncated_next_step_present: TestHonestTruncationCallers#test_truncated_next_step_present().
  TestHonestTruncationCallers.test_schema_declares_limit_param: TestHonestTruncationCallers#test_schema_declares_limit_param().
  TestHonestTruncationCallers.test_zero_callers_not_truncated: TestHonestTruncationCallers#test_zero_callers_not_truncated().
  TestHonestTruncationCallees.test_default_limit_caps_at_50: TestHonestTruncationCallees#test_default_limit_caps_at_50().
  TestHonestTruncationCallees.test_raised_limit_shows_all: TestHonestTruncationCallees#test_raised_limit_shows_all().
  TestHonestTruncationCallees.test_no_truncation_when_few_callees: TestHonestTruncationCallees#test_no_truncation_when_few_callees().
  TestHonestTruncationCallees.test_schema_declares_limit_param: TestHonestTruncationCallees#test_schema_declares_limit_param().
  TestHonestTruncationCallees.test_zero_callees_not_truncated: TestHonestTruncationCallees#test_zero_callees_not_truncated().
  TestStaleCacheWarning.test_callees_warning_omitted_when_callees_empty: TestStaleCacheWarning#test_callees_warning_omitted_when_callees_empty().
  TestStaleCacheWarning.test_callers_warning_omitted_when_callers_empty: TestStaleCacheWarning#test_callers_warning_omitted_when_callers_empty().
  TestEmptyIndexHint.test_callers_empty_index_hint_mentions_full_index: TestEmptyIndexHint#test_callers_empty_index_hint_mentions_full_index().
  TestEmptyIndexHint.test_callees_empty_index_hint_mentions_full_index: TestEmptyIndexHint#test_callees_empty_index_hint_mentions_full_index().
  TestAgentSummaryCallers.test_callers_has_agent_summary_found: TestAgentSummaryCallers#test_callers_has_agent_summary_found().
  TestAgentSummaryCallers.test_callers_has_agent_summary_not_found: TestAgentSummaryCallers#test_callers_has_agent_summary_not_found().
  TestAgentSummaryCallers.test_callers_verdict_mirrors_agent_summary: TestAgentSummaryCallers#test_callers_verdict_mirrors_agent_summary().
  TestAgentSummaryCallees.test_callees_has_agent_summary_found: TestAgentSummaryCallees#test_callees_has_agent_summary_found().
  TestAgentSummaryCallees.test_callees_has_agent_summary_not_found: TestAgentSummaryCallees#test_callees_has_agent_summary_not_found().
  TestAgentSummaryCallees.test_callees_verdict_mirrors_agent_summary: TestAgentSummaryCallees#test_callees_verdict_mirrors_agent_summary().
  TestStaleCacheWarning.test_helper_is_false_for_empty: TestStaleCacheWarning#test_helper_is_false_for_empty().
  TestStaleCacheWarning.test_helper_is_true_when_all_unknown: TestStaleCacheWarning#test_helper_is_true_when_all_unknown().
  TestStaleCacheWarning.test_helper_is_false_when_majority_resolved: TestStaleCacheWarning#test_helper_is_false_when_majority_resolved().
  TestStaleCacheWarning.test_helper_trips_at_exactly_80_percent: TestStaleCacheWarning#test_helper_trips_at_exactly_80_percent().
  TestStaleCacheWarning.test_warning_message_recommends_valid_rebuild_command: TestStaleCacheWarning#test_warning_message_recommends_valid_rebuild_command().
  test_cli_call_limit_flag_parity: test_cli_call_limit_flag_parity().
  _PROJECT_ROOT: _PROJECT_ROOT.
  tiny_project_root: tiny_project_root().
  TestCodeGraphCallersTool: TestCodeGraphCallersTool#
  TestCodeGraphCallersTool.test_tool_definition: TestCodeGraphCallersTool#test_tool_definition().
  TestCodeGraphCallersTool.test_validate_missing_function_name: TestCodeGraphCallersTool#test_validate_missing_function_name().
  TestCodeGraphCallersTool.test_validate_with_function_name: TestCodeGraphCallersTool#test_validate_with_function_name().
  TestCodeGraphCalleesTool: TestCodeGraphCalleesTool#
  TestCodeGraphCalleesTool.test_tool_definition: TestCodeGraphCalleesTool#test_tool_definition().
  TestCodeGraphCalleesTool.test_validate_missing_function_name: TestCodeGraphCalleesTool#test_validate_missing_function_name().
  TestCodeGraphCalleesTool.test_validate_with_function_name: TestCodeGraphCalleesTool#test_validate_with_function_name().
  TestCallerCalleeIntegration: TestCallerCalleeIntegration#
  TestHonestTruncationCallers: TestHonestTruncationCallers#
  TestHonestTruncationCallers.many_callers_root: TestHonestTruncationCallers#many_callers_root().
  TestHonestTruncationCallees: TestHonestTruncationCallees#
  TestHonestTruncationCallees.many_callees_root: TestHonestTruncationCallees#many_callees_root().
  TestStaleCacheWarning: TestStaleCacheWarning#
  TestEmptyIndexHint: TestEmptyIndexHint#
  TestAgentSummaryCallers: TestAgentSummaryCallers#
  TestAgentSummaryCallees: TestAgentSummaryCallees#
---
# Module: [`tests/unit/test_callers_callees_tools.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_callees_tools.py)

## Classes
### `TestAgentSummaryCallees`
- def: [`tests/unit/test_callers_callees_tools.py:720`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_callees_tools.py#L720)
- doc: #546 seam 3 / #577 leftover: callees must emit agent_summary with
- signature: `class TestAgentSummaryCallees:`
- members:
  - `test_callees_has_agent_summary_found(self, tiny_project_root)` — [`L725`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_callees_tools.py#L725) — INFO case: foo calls bar → foo has 1 callee (bar).
  - `test_callees_has_agent_summary_not_found(self, tiny_project_root)` — [`L763`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_callees_tools.py#L763) — NOT_FOUND case: unknown symbol → agent_summary present, verdict NOT_FOUND.
  - `test_callees_verdict_mirrors_agent_summary(self, tiny_project_root)` — [`L780`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_callees_tools.py#L780) — Top-level verdict must always equal agent_summary.verdict (N4/r37u pattern).
- uses (calls/refs, reference-scoped): [`execute`](../../tree_sitter_analyzer/mcp/tools/callees_tool.md#CodeGraphCalleesTool.execute), [`CodeGraphCalleesTool`](../../tree_sitter_analyzer/mcp/tools/callees_tool.md#CodeGraphCalleesTool)

### `TestAgentSummaryCallers`
- def: [`tests/unit/test_callers_callees_tools.py:646`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_callees_tools.py#L646)
- doc: #546 seam 3 / #577 leftover: callers must emit agent_summary with
- signature: `class TestAgentSummaryCallers:`
- members:
  - `test_callers_has_agent_summary_found(self, tiny_project_root)` — [`L651`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_callees_tools.py#L651) — INFO case: foo calls bar → bar has 1 caller (foo).
  - `test_callers_has_agent_summary_not_found(self, tiny_project_root)` — [`L689`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_callees_tools.py#L689) — NOT_FOUND case: unknown symbol → agent_summary present, verdict NOT_FOUND.
  - `test_callers_verdict_mirrors_agent_summary(self, tiny_project_root)` — [`L706`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_callees_tools.py#L706) — Top-level verdict must always equal agent_summary.verdict (N4/r37u pattern).
- uses (calls/refs, reference-scoped): [`execute`](../../tree_sitter_analyzer/mcp/tools/callers_tool.md#CodeGraphCallersTool.execute), [`CodeGraphCallersTool`](../../tree_sitter_analyzer/mcp/tools/callers_tool.md#CodeGraphCallersTool)

### `TestCallerCalleeIntegration`
- def: [`tests/unit/test_callers_callees_tools.py:188`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_callees_tools.py#L188)
- signature: `class TestCallerCalleeIntegration:`
- members:
  - `test_callers_and_callees_share_relation_bootstrap(self)` — [`L189`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_callees_tools.py#L189)
  - `test_unknown_function_returns_empty(self, tiny_project_root)` — [`L194`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_callees_tools.py#L194)
- uses (calls/refs, reference-scoped): [`execute`](../../tree_sitter_analyzer/mcp/tools/callers_tool.md#CodeGraphCallersTool.execute), [`execute`](../../tree_sitter_analyzer/mcp/tools/callees_tool.md#CodeGraphCalleesTool.execute), [`CodeGraphCallersTool`](../../tree_sitter_analyzer/mcp/tools/callers_tool.md#CodeGraphCallersTool), [`CodeGraphCalleesTool`](../../tree_sitter_analyzer/mcp/tools/callees_tool.md#CodeGraphCalleesTool), [`CodeGraphRelationToolMixin`](../../tree_sitter_analyzer/mcp/tools/codegraph_relation_tool.md#CodeGraphRelationToolMixin)

### `TestCodeGraphCalleesTool`
- def: [`tests/unit/test_callers_callees_tools.py:113`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_callees_tools.py#L113)
- signature: `class TestCodeGraphCalleesTool:`
- members:
  - `test_callee_inlines_source_body(self, tiny_project_root)` — [`L153`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_callees_tools.py#L153) — P2: each callee carries its inlined verbatim source body (no Read).
  - `test_execute_returns_callees(self, tiny_project_root)` — [`L129`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_callees_tools.py#L129)
  - `test_execute_toon_format(self, tiny_project_root)` — [`L167`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_callees_tools.py#L167)
  - `test_execute_with_file_path(self, tiny_project_root)` — [`L141`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_callees_tools.py#L141)
  - `test_no_project_root_raises(self)` — [`L182`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_callees_tools.py#L182)
  - `test_project_root_change_resets_cache(self, tiny_project_root)` — [`L174`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_callees_tools.py#L174)
  - `test_tool_definition(self, callees_tool)` — [`L114`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_callees_tools.py#L114)
  - `test_validate_missing_function_name(self, callees_tool)` — [`L121`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_callees_tools.py#L121)
  - `test_validate_with_function_name(self, callees_tool)` — [`L125`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_callees_tools.py#L125)
- uses (calls/refs, reference-scoped): [`execute`](../../tree_sitter_analyzer/mcp/tools/callees_tool.md#CodeGraphCalleesTool.execute), [`CodeGraphCalleesTool`](../../tree_sitter_analyzer/mcp/tools/callees_tool.md#CodeGraphCalleesTool), [`get_call_graph`](../../tree_sitter_analyzer/mcp/tools/codegraph_relation_tool.md#CodeGraphRelationToolMixin.get_call_graph), [`call_graph_initialized`](../../tree_sitter_analyzer/mcp/tools/codegraph_relation_tool.md#CodeGraphRelationToolMixin.call_graph_initialized), [`_on_project_root_changed`](../../tree_sitter_analyzer/mcp/tools/callees_tool.md#CodeGraphCalleesTool._on_project_root_changed)

### `TestCodeGraphCallersTool`
- def: [`tests/unit/test_callers_callees_tools.py:38`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_callees_tools.py#L38)
- signature: `class TestCodeGraphCallersTool:`
- members:
  - `test_caller_inlines_source_body(self, tiny_project_root)` — [`L87`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_callees_tools.py#L87) — P2: each caller carries its inlined verbatim source body (no Read).
  - `test_execute_returns_callers(self, tiny_project_root)` — [`L54`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_callees_tools.py#L54)
  - `test_execute_toon_format(self, tiny_project_root)` — [`L79`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_callees_tools.py#L79)
  - `test_execute_with_file_path(self, tiny_project_root)` — [`L66`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_callees_tools.py#L66)
  - `test_no_project_root_raises(self)` — [`L107`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_callees_tools.py#L107)
  - `test_project_root_change_resets_cache(self, tiny_project_root)` — [`L99`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_callees_tools.py#L99)
  - `test_tool_definition(self, callers_tool)` — [`L39`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_callees_tools.py#L39)
  - `test_validate_missing_function_name(self, callers_tool)` — [`L46`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_callees_tools.py#L46)
  - `test_validate_with_function_name(self, callers_tool)` — [`L50`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_callees_tools.py#L50)
- uses (calls/refs, reference-scoped): [`execute`](../../tree_sitter_analyzer/mcp/tools/callers_tool.md#CodeGraphCallersTool.execute), [`CodeGraphCallersTool`](../../tree_sitter_analyzer/mcp/tools/callers_tool.md#CodeGraphCallersTool), [`get_call_graph`](../../tree_sitter_analyzer/mcp/tools/codegraph_relation_tool.md#CodeGraphRelationToolMixin.get_call_graph), [`call_graph_initialized`](../../tree_sitter_analyzer/mcp/tools/codegraph_relation_tool.md#CodeGraphRelationToolMixin.call_graph_initialized), [`_on_project_root_changed`](../../tree_sitter_analyzer/mcp/tools/callers_tool.md#CodeGraphCallersTool._on_project_root_changed)

### `TestEmptyIndexHint`
- def: [`tests/unit/test_callers_callees_tools.py:473`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_callees_tools.py#L473)
- doc: #548: callers/callees on an empty/partial call-graph index must surface
- signature: `class TestEmptyIndexHint:`
- members:
  - `test_callees_built_index_zero_edges_no_hint(self, tmp_path)` — [`L623`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_callees_tools.py#L623) — #705 follow-up: same zero-edge scenario for callees.
  - `test_callees_empty_index_hint_mentions_full_index(self, tmp_path)` — [`L498`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_callees_tools.py#L498) — Callees NOT_FOUND on empty index carries --full-index hint.
  - `test_callees_rebuild_marker_warns_without_phantom_count(self, tmp_path)` — [`L541`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_callees_tools.py#L541)
  - `test_callers_built_index_zero_edges_no_hint(self, tmp_path)` — [`L597`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_callees_tools.py#L597) — #705 follow-up: index IS built (total_files > 0) but the project has
  - `test_callers_empty_index_hint_mentions_full_index(self, tmp_path)` — [`L484`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_callees_tools.py#L484) — Callers NOT_FOUND on empty index carries --full-index hint.
  - `test_callers_non_empty_index_no_spurious_hint(self, tiny_project_root)` — [`L570`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_callees_tools.py#L570) — When a built index has call edges, an unknown symbol gets no hint.
  - `test_callers_rebuild_marker_warns_without_phantom_count(self, tmp_path)` — [`L512`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_callees_tools.py#L512)
- uses (calls/refs, reference-scoped): [`ASTCache`](../../tree_sitter_analyzer/ast_cache.md#ASTCache), [`close`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.close), [`index_project`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.index_project), [`get_conn`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.get_conn), [`execute`](../../tree_sitter_analyzer/mcp/tools/callers_tool.md#CodeGraphCallersTool.execute), [`execute`](../../tree_sitter_analyzer/mcp/tools/callees_tool.md#CodeGraphCalleesTool.execute), [`CodeGraphCallersTool`](../../tree_sitter_analyzer/mcp/tools/callers_tool.md#CodeGraphCallersTool), [`CodeGraphCalleesTool`](../../tree_sitter_analyzer/mcp/tools/callees_tool.md#CodeGraphCalleesTool), [`get_stats`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.get_stats), [`call_graph_built`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.call_graph_built), [`has_call_edges`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.has_call_edges), [`mark_build_in_progress`](../../tree_sitter_analyzer/_ast_cache_build_state.md#mark_build_in_progress), [`clear_build_in_progress`](../../tree_sitter_analyzer/_ast_cache_build_state.md#clear_build_in_progress)

### `TestHonestTruncationCallees`
- def: [`tests/unit/test_callers_callees_tools.py:312`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_callees_tools.py#L312)
- doc: Symmetric to TestHonestTruncationCallers — callees_tool must apply the
- signature: `class TestHonestTruncationCallees:`
- members:
  - `many_callees_root(self, tmp_path)` — [`L317`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_callees_tools.py#L317) — One source function ``hub()`` calling 60 distinct helpers.
  - `test_default_limit_caps_at_50(self, many_callees_root)` — [`L336`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_callees_tools.py#L336) — With 60 callees and default limit=50, listed == 50, total == 60.
  - `test_no_truncation_when_few_callees(self, tiny_project_root)` — [`L360`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_callees_tools.py#L360) — 1 callee (foo→bar) → truncated=False.
  - `test_raised_limit_shows_all(self, many_callees_root)` — [`L348`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_callees_tools.py#L348) — limit=100 > 60 callees → no truncation.
  - `test_schema_declares_limit_param(self)` — [`L368`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_callees_tools.py#L368)
  - `test_zero_callees_not_truncated(self, tiny_project_root)` — [`L376`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_callees_tools.py#L376) — 0 callees → truncated=False, callees_listed==0.
- uses (calls/refs, reference-scoped): [`execute`](../../tree_sitter_analyzer/mcp/tools/callees_tool.md#CodeGraphCalleesTool.execute), [`CodeGraphCalleesTool`](../../tree_sitter_analyzer/mcp/tools/callees_tool.md#CodeGraphCalleesTool), [`get_tool_schema`](../../tree_sitter_analyzer/mcp/tools/callees_tool.md#CodeGraphCalleesTool.get_tool_schema)

### `TestHonestTruncationCallers`
- def: [`tests/unit/test_callers_callees_tools.py:220`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_callees_tools.py#L220)
- doc: DF-13: default limit=50 caps high-fan-in callers; response carries
- signature: `class TestHonestTruncationCallers:`
- members:
  - `many_callers_root(self, tmp_path)` — [`L225`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_callees_tools.py#L225) — Tiny project with one target function called by 60 callers.
  - `test_default_limit_caps_at_50(self, many_callers_root)` — [`L245`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_callees_tools.py#L245) — With 60 callers and default limit=50, listed == 50, total == 60.
  - `test_no_truncation_when_few_callers(self, tiny_project_root)` — [`L274`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_callees_tools.py#L274) — 1 caller (foo→bar) → truncated=False, callers_listed == caller_count.
  - `test_raised_limit_shows_all(self, many_callers_root)` — [`L261`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_callees_tools.py#L261) — limit=100 > 60 callers → no truncation, all listed.
  - `test_schema_declares_limit_param(self)` — [`L293`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_callees_tools.py#L293)
  - `test_truncated_next_step_present(self, many_callers_root)` — [`L283`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_callees_tools.py#L283) — When truncated, next_step must mention the counts and suggest narrowing.
  - `test_zero_callers_not_truncated(self, tiny_project_root)` — [`L301`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_callees_tools.py#L301) — 0 callers → truncated=False, callers_listed==0.
- uses (calls/refs, reference-scoped): [`execute`](../../tree_sitter_analyzer/mcp/tools/callers_tool.md#CodeGraphCallersTool.execute), [`CodeGraphCallersTool`](../../tree_sitter_analyzer/mcp/tools/callers_tool.md#CodeGraphCallersTool), [`get_tool_schema`](../../tree_sitter_analyzer/mcp/tools/callers_tool.md#CodeGraphCallersTool.get_tool_schema)

### `TestStaleCacheWarning`
- def: [`tests/unit/test_callers_callees_tools.py:387`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_callees_tools.py#L387)
- doc: Stale-cache hint surfaces in callees/callers when ≥80% of edges
- signature: `class TestStaleCacheWarning:`
- members:
  - `test_callees_warning_omitted_when_callees_empty(self, tiny_project_root)` — [`L438`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_callees_tools.py#L438)
  - `test_callers_warning_omitted_when_callers_empty(self, tiny_project_root)` — [`L450`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_callees_tools.py#L450)
  - `test_helper_is_false_for_empty(self)` — [`L392`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_callees_tools.py#L392)
  - `test_helper_is_false_when_majority_resolved(self)` — [`L403`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_callees_tools.py#L403)
  - `test_helper_is_true_when_all_unknown(self)` — [`L397`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_callees_tools.py#L397)
  - `test_helper_trips_at_exactly_80_percent(self)` — [`L412`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_callees_tools.py#L412)
  - `test_warning_message_recommends_valid_rebuild_command(self)` — [`L421`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_callees_tools.py#L421)
- uses (calls/refs, reference-scoped): [`execute`](../../tree_sitter_analyzer/mcp/tools/callers_tool.md#CodeGraphCallersTool.execute), [`execute`](../../tree_sitter_analyzer/mcp/tools/callees_tool.md#CodeGraphCalleesTool.execute), [`CodeGraphCallersTool`](../../tree_sitter_analyzer/mcp/tools/callers_tool.md#CodeGraphCallersTool), [`CodeGraphCalleesTool`](../../tree_sitter_analyzer/mcp/tools/callees_tool.md#CodeGraphCalleesTool), [`_is_stale_resolution`](../../tree_sitter_analyzer/mcp/tools/codegraph_relation_tool.md#_is_stale_resolution), [`_STALE_CACHE_WARNING`](../../tree_sitter_analyzer/mcp/tools/codegraph_relation_tool.md#_STALE_CACHE_WARNING)

## Functions
- `callees_tool()` — [`L25`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_callees_tools.py#L25)
- `callers_tool()` — [`L20`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_callees_tools.py#L20)
- `test_cli_call_limit_flag_parity()` — [`L461`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_callees_tools.py#L461) — Codex P2 (#500): CLI must be able to raise the new limit (MCP/CLI parity).
- `tiny_project_root(tmp_path)` — [`L30`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_callees_tools.py#L30)

## Module values
- `_PROJECT_ROOT` — [`L16`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_callers_callees_tools.py#L16)

