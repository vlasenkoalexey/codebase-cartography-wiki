---
title: 'Module: tests/unit/mcp/tools/test_dead_code_counts_consistency.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/tools/test_dead_code_counts_consistency.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.tools.test_dead_code_counts_consistency`/
symbols:
  _fake_result: _fake_result().
  _mixed_path_result: _mixed_path_result().
  _run: _run().
  _make_dead: _make_dead().
  _make_import: _make_import().
  _make_var: _make_var().
  TestDeadCodeCountsConsistency.test_no_truncation_listed_equals_total: TestDeadCodeCountsConsistency#test_no_truncation_listed_equals_total().
  TestDeadCodeCountsConsistency.test_truncated_flag_set_when_dead_exceeds_cap: TestDeadCodeCountsConsistency#test_truncated_flag_set_when_dead_exceeds_cap().
  TestDeadCodeCountsConsistency.test_truncated_flag_set_when_imports_exceeds_cap: TestDeadCodeCountsConsistency#test_truncated_flag_set_when_imports_exceeds_cap().
  TestDeadCodeCountsConsistency.test_truncated_flag_set_when_vars_exceed_cap: TestDeadCodeCountsConsistency#test_truncated_flag_set_when_vars_exceed_cap().
  TestDeadCodeCountsConsistency.test_no_hidden_third_number_in_response: TestDeadCodeCountsConsistency#test_no_hidden_third_number_in_response().
  TestDeadCodeCountsConsistency.test_narrative_uses_same_count_as_listed_total: TestDeadCodeCountsConsistency#test_narrative_uses_same_count_as_listed_total().
  TestDeadCodeCountsConsistency.test_truncated_next_step_mentions_totals: TestDeadCodeCountsConsistency#test_truncated_next_step_mentions_totals().
  TestDeadCodeCountsConsistency.test_candidates_lte_total: TestDeadCodeCountsConsistency#test_candidates_lte_total().
  TestDeadCodeCountsConsistency.test_empty_result_truncated_false: TestDeadCodeCountsConsistency#test_empty_result_truncated_false().
  TestDeadCodeCountsConsistency.test_listed_equals_min_total_cap_parametric: TestDeadCodeCountsConsistency#test_listed_equals_min_total_cap_parametric().
  TestDeadCodePathScoping.test_no_path_returns_everything: TestDeadCodePathScoping#test_no_path_returns_everything().
  TestDeadCodePathScoping.test_path_scopes_to_product_package: TestDeadCodePathScoping#test_path_scopes_to_product_package().
  TestDeadCodePathScoping.test_path_excludes_corpus_and_benchmarks: TestDeadCodePathScoping#test_path_excludes_corpus_and_benchmarks().
  TestDeadCodePathScoping.test_path_matches_single_subtree: TestDeadCodePathScoping#test_path_matches_single_subtree().
  TestDeadCodePathScoping.test_path_trailing_slash_normalized: TestDeadCodePathScoping#test_path_trailing_slash_normalized().
  TestDeadCodePathScoping.test_path_respects_segment_boundary: TestDeadCodePathScoping#test_path_respects_segment_boundary().
  TestDeadCodePathScoping.test_path_dot_means_whole_project: TestDeadCodePathScoping#test_path_dot_means_whole_project().
  TestDeadCodePathScoping.test_path_leading_dot_slash_normalized: TestDeadCodePathScoping#test_path_leading_dot_slash_normalized().
  TestDeadCodePathScoping.test_path_no_match_is_empty_not_error: TestDeadCodePathScoping#test_path_no_match_is_empty_not_error().
  TestDeadCodeToolEdgeCases.test_mode_dead_functions_omits_imports_and_vars: TestDeadCodeToolEdgeCases#test_mode_dead_functions_omits_imports_and_vars().
  TestDeadCodeToolEdgeCases.test_mode_unused_imports_omits_dead_and_vars: TestDeadCodeToolEdgeCases#test_mode_unused_imports_omits_dead_and_vars().
  TestDeadCodeToolEdgeCases.test_mode_variables_omits_dead_and_imports: TestDeadCodeToolEdgeCases#test_mode_variables_omits_dead_and_imports().
  test_scoped_mode_ignores_hidden_category_truncation: test_scoped_mode_ignores_hidden_category_truncation().
  TestDeadCodeToolEdgeCases.test_no_project_root_returns_error: TestDeadCodeToolEdgeCases#test_no_project_root_returns_error().
  TestDeadCodeToolEdgeCases.test_invalid_mode_raises_value_error: TestDeadCodeToolEdgeCases#test_invalid_mode_raises_value_error().
  TestDeadCodeToolEdgeCases.test_invalid_mode_enumerates_valid_values: TestDeadCodeToolEdgeCases#test_invalid_mode_enumerates_valid_values().
  TestDeadCodeToolEdgeCases.test_analyze_dead_code_exception_returns_error: TestDeadCodeToolEdgeCases#test_analyze_dead_code_exception_returns_error().
  _make_func_ref: _make_func_ref().
  fake_root: fake_root().
  TestDeadCodeCountsConsistency: TestDeadCodeCountsConsistency#
  TestDeadCodeToolEdgeCases: TestDeadCodeToolEdgeCases#
  TestDeadCodePathScoping: TestDeadCodePathScoping#
---
# Module: [`tests/unit/mcp/tools/test_dead_code_counts_consistency.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_dead_code_counts_consistency.py)

## Classes
### `TestDeadCodeCountsConsistency`
- def: [`tests/unit/mcp/tools/test_dead_code_counts_consistency.py:104`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_dead_code_counts_consistency.py#L104)
- doc: Invariant: every count in the response must label what it counts,
- signature: `class TestDeadCodeCountsConsistency:`
- members:
  - `test_candidates_lte_total(self, fake_root, monkeypatch)` — [`L232`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_dead_code_counts_consistency.py#L232) — candidates_after_filters <= total_dead_functions_transitive (they're equal here;
  - `test_empty_result_truncated_false(self, fake_root, monkeypatch)` — [`L245`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_dead_code_counts_consistency.py#L245) — A clean result must report truncated=False and zero listed counts.
  - `test_listed_equals_min_total_cap_parametric(self, fake_root, monkeypatch)` — [`L257`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_dead_code_counts_consistency.py#L257) — Parametric: for several (total, cap) combos, listed == min(total, cap).
  - `test_narrative_uses_same_count_as_listed_total(self, fake_root, monkeypatch)` — [`L194`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_dead_code_counts_consistency.py#L194) — next_step must cite the same count as listed_total, not a third number.
  - `test_no_hidden_third_number_in_response(self, fake_root, monkeypatch)` — [`L178`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_dead_code_counts_consistency.py#L178) — The old stats["dead_functions"] raw total must NOT appear in the tool
  - `test_no_truncation_listed_equals_total(self, fake_root, monkeypatch)` — [`L108`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_dead_code_counts_consistency.py#L108) — When total < cap, listed == total and truncated is False.
  - `test_truncated_flag_set_when_dead_exceeds_cap(self, fake_root, monkeypatch)` — [`L131`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_dead_code_counts_consistency.py#L131) — listed == cap when total > cap, truncated is True.
  - `test_truncated_flag_set_when_imports_exceeds_cap(self, fake_root, monkeypatch)` — [`L148`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_dead_code_counts_consistency.py#L148)
  - `test_truncated_flag_set_when_vars_exceed_cap(self, fake_root, monkeypatch)` — [`L163`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_dead_code_counts_consistency.py#L163)
  - `test_truncated_next_step_mentions_totals(self, fake_root, monkeypatch)` — [`L213`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_dead_code_counts_consistency.py#L213) — When truncated, next_step must cite both the listed and total counts.
- uses (calls/refs, reference-scoped): [`execute`](../../../../tree_sitter_analyzer/mcp/tools/dead_code_tool.md#CodeGraphDeadCodeTool.execute), [`CodeGraphDeadCodeTool`](../../../../tree_sitter_analyzer/mcp/tools/dead_code_tool.md#CodeGraphDeadCodeTool)  (2 test-only)

### `TestDeadCodePathScoping`
- def: [`tests/unit/mcp/tools/test_dead_code_counts_consistency.py:397`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_dead_code_counts_consistency.py#L397)
- doc: #1084: `path` scopes results to items defined under a path prefix
- signature: `class TestDeadCodePathScoping:`
- members:
  - `test_no_path_returns_everything(self, fake_root, monkeypatch)` — [`L401`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_dead_code_counts_consistency.py#L401)
  - `test_path_dot_means_whole_project(self, fake_root, monkeypatch)` — [`L474`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_dead_code_counts_consistency.py#L474) — Codex P2: ``path='.'`` is the root scope — must match everything,
  - `test_path_excludes_corpus_and_benchmarks(self, fake_root, monkeypatch)` — [`L430`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_dead_code_counts_consistency.py#L430)
  - `test_path_leading_dot_slash_normalized(self, fake_root, monkeypatch)` — [`L484`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_dead_code_counts_consistency.py#L484) — Codex P2: a copy-pasted ``./pkg`` prefix must behave like ``pkg``.
  - `test_path_matches_single_subtree(self, fake_root, monkeypatch)` — [`L443`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_dead_code_counts_consistency.py#L443)
  - `test_path_no_match_is_empty_not_error(self, fake_root, monkeypatch)` — [`L497`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_dead_code_counts_consistency.py#L497)
  - `test_path_respects_segment_boundary(self, fake_root, monkeypatch)` — [`L462`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_dead_code_counts_consistency.py#L462) — A partial segment ('.../m') must NOT match '.../mcp/...' — the
  - `test_path_scopes_to_product_package(self, fake_root, monkeypatch)` — [`L411`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_dead_code_counts_consistency.py#L411)
  - `test_path_trailing_slash_normalized(self, fake_root, monkeypatch)` — [`L452`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_dead_code_counts_consistency.py#L452)
- uses (calls/refs, reference-scoped): [`execute`](../../../../tree_sitter_analyzer/mcp/tools/dead_code_tool.md#CodeGraphDeadCodeTool.execute), [`CodeGraphDeadCodeTool`](../../../../tree_sitter_analyzer/mcp/tools/dead_code_tool.md#CodeGraphDeadCodeTool)  (2 test-only)

### `TestDeadCodeToolEdgeCases`
- def: [`tests/unit/mcp/tools/test_dead_code_counts_consistency.py:279`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_dead_code_counts_consistency.py#L279)
- doc: Coverage for error paths and mode-filter branches.
- signature: `class TestDeadCodeToolEdgeCases:`
- members:
  - `test_analyze_dead_code_exception_returns_error(self, fake_root, monkeypatch)` — [`L312`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_dead_code_counts_consistency.py#L312) — If analyze_dead_code raises, tool must return success=False.
  - `test_invalid_mode_enumerates_valid_values(self, fake_root)` — [`L295`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_dead_code_counts_consistency.py#L295) — Error message must list all valid mode values (issue #449).
  - `test_invalid_mode_raises_value_error(self, fake_root)` — [`L289`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_dead_code_counts_consistency.py#L289) — validate_arguments must raise ValueError for unknown mode.
  - `test_mode_dead_functions_omits_imports_and_vars(self, fake_root, monkeypatch)` — [`L326`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_dead_code_counts_consistency.py#L326) — mode=dead_functions must drop unused_imports and unreferenced_variables.
  - `test_mode_unused_imports_omits_dead_and_vars(self, fake_root, monkeypatch)` — [`L340`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_dead_code_counts_consistency.py#L340) — mode=unused_imports must drop dead_functions and unreferenced_variables.
  - `test_mode_variables_omits_dead_and_imports(self, fake_root, monkeypatch)` — [`L354`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_dead_code_counts_consistency.py#L354) — mode=variables must drop dead_functions and unused_imports.
  - `test_no_project_root_returns_error(self)` — [`L282`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_dead_code_counts_consistency.py#L282) — Tool with no project_root must return success=False, not raise.
- uses (calls/refs, reference-scoped): [`execute`](../../../../tree_sitter_analyzer/mcp/tools/dead_code_tool.md#CodeGraphDeadCodeTool.execute), [`CodeGraphDeadCodeTool`](../../../../tree_sitter_analyzer/mcp/tools/dead_code_tool.md#CodeGraphDeadCodeTool), [`validate_arguments`](../../../../tree_sitter_analyzer/mcp/tools/dead_code_tool.md#CodeGraphDeadCodeTool.validate_arguments)  (1 test-only)

## Functions
- `_fake_result(n_dead: int = 0, n_imports: int = 0, n_vars: int = 0)` — [`L65`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_dead_code_counts_consistency.py#L65)
- `_make_dead(name: str, file: str = "a.py", line: int = 1)` — [`L47`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_dead_code_counts_consistency.py#L47)
- `_make_func_ref(name: str, file: str = "a.py", line: int = 1)` — [`L36`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_dead_code_counts_consistency.py#L36) — Create a minimal FunctionRef (no tree-sitter node needed for serialization).
- `_make_import(name: str, file: str = "a.py")` — [`L55`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_dead_code_counts_consistency.py#L55)
- `_make_var(name: str, file: str = "a.py")` — [`L61`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_dead_code_counts_consistency.py#L61)
- `_mixed_path_result()` — [`L369`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_dead_code_counts_consistency.py#L369) — Dead items spread across product / corpus / benchmarks paths (#1084).
- `_run(coro: Any)` — [`L84`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_dead_code_counts_consistency.py#L84)
- `fake_root(tmp_path)` — [`L94`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_dead_code_counts_consistency.py#L94)
- `test_scoped_mode_ignores_hidden_category_truncation(tmp_path)` — [`L510`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_dead_code_counts_consistency.py#L510) — Codex P2 (#486): mode=unused_imports strips dead_functions from the

