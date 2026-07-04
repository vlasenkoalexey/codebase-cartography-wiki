---
title: 'Module: tests/unit/test_health_scorer.py'
type: catalog
provenance: extracted
module: tests/unit/test_health_scorer.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_health_scorer`/
symbols:
  TestHealthScore.test_health_score_to_dict: TestHealthScore#test_health_score_to_dict().
  TestScoreComplexityExtractorPath.test_java_switch_counts_construct_once_via_extractor: TestScoreComplexityExtractorPath#test_java_switch_counts_construct_once_via_extractor().
  TestHealthScorer.test_score_file_fast_dependencies_uses_fallback: TestHealthScorer#test_score_file_fast_dependencies_uses_fallback().
  TestHealthScore.test_health_score_creation: TestHealthScore#test_health_score_creation().
  TestScoreComplexityExtractorPath.test_java_switch_ternary_do_while_matches_extractor: TestScoreComplexityExtractorPath#test_java_switch_ternary_do_while_matches_extractor().
  TestScoreComplexityExtractorPath.test_javascript_ternary_scored_correctly: TestScoreComplexityExtractorPath#test_javascript_ternary_scored_correctly().
  TestScoreComplexityExtractorPath.test_extractor_aggregate_matches_scorer_for_multi_function_file: TestScoreComplexityExtractorPath#test_extractor_aggregate_matches_scorer_for_multi_function_file().
  HEALTH_PROJECT: HEALTH_PROJECT.
  TestHealthScorer.test_score_project_respects_custom_source_extensions: TestHealthScorer#test_score_project_respects_custom_source_extensions().
  TestHealthScorer.test_score_file_default_dependencies_uses_full_graph_score: TestHealthScorer#test_score_file_default_dependencies_uses_full_graph_score().
  TestHealthScorer.test_score_project_prunes_hidden_and_generated_dirs: TestHealthScorer#test_score_project_prunes_hidden_and_generated_dirs().
  TestHealthScorer.test_stale_coverage_json_is_ignored: TestHealthScorer#test_stale_coverage_json_is_ignored().
  TestHealthScorer.test_current_coverage_json_is_used: TestHealthScorer#test_current_coverage_json_is_used().
  TestHealthScorer.test_scala_avg_cc_includes_all_methods: TestHealthScorer#test_scala_avg_cc_includes_all_methods().
  TestScoreComplexityExtractorPath._write: TestScoreComplexityExtractorPath#_write().
  TestHealthScorer.test_is_excluded_falls_back_to_absolute_parts: TestHealthScorer#test_is_excluded_falls_back_to_absolute_parts().
  TestHealthScorer.test_iter_source_files_skips_hidden_filenames: TestHealthScorer#test_iter_source_files_skips_hidden_filenames().
  TestHealthScorer.test_score_project_counts_scoring_failures: TestHealthScorer#test_score_project_counts_scoring_failures().
  TestHealthScorer.test_score_project_counts_defensive_excluded_file: TestHealthScorer#test_score_project_counts_defensive_excluded_file().
  TestHealthScorer.test_bash_complexity_counts_decision_nodes: TestHealthScorer#test_bash_complexity_counts_decision_nodes().
  TestHealthScorer.test_bash_case_scores_decision_per_case: TestHealthScorer#test_bash_case_scores_decision_per_case().
  TestHealthScorer.test_git_hotspot_uses_repo_relative_pathspec: TestHealthScorer#test_git_hotspot_uses_repo_relative_pathspec().
  TestHealthScore.test_health_score_grade: TestHealthScore#test_health_score_grade().
  TestScoreComplexityExtractorPath.test_java_high_complexity_method_scored_correctly: TestScoreComplexityExtractorPath#test_java_high_complexity_method_scored_correctly().
  TestScoreComplexityExtractorPath.test_no_plugin_language_returns_neutral: TestScoreComplexityExtractorPath#test_no_plugin_language_returns_neutral().
  TestHealthScorer.scorer: TestHealthScorer#scorer().
  TestHealthScorer.test_healthy_file_scores_higher: TestHealthScorer#test_healthy_file_scores_higher().
  TestHealthScorer.test_score_is_between_0_and_100: TestHealthScorer#test_score_is_between_0_and_100().
  TestHealthScorer.test_score_has_breakdown: TestHealthScorer#test_score_has_breakdown().
  TestHealthScorer.test_score_project: TestHealthScorer#test_score_project().
  TestHealthScorer.test_score_project_includes_reported_source_extensions: TestHealthScorer#test_score_project_includes_reported_source_extensions().
  TestHealthScorer.test_weights_sum_to_100: TestHealthScorer#test_weights_sum_to_100().
  TestHealthScorer.test_dependencies_neutral_for_unanalyzable_languages: TestHealthScorer#test_dependencies_neutral_for_unanalyzable_languages().
  TestHealthScorer.test_fast_dependencies_neutral_for_unanalyzable_language: TestHealthScorer#test_fast_dependencies_neutral_for_unanalyzable_language().
  TestHealthScorer.test_seven_dimensions_in_weights: TestHealthScorer#test_seven_dimensions_in_weights().
  FIXTURES_DIR: FIXTURES_DIR.
  TestHealthScorer.fail_full_graph: TestHealthScorer#fail_full_graph().
  TestHealthScorer.fake_run: TestHealthScorer#fake_run().
  TestHealthScorer: TestHealthScorer#
  TestHealthScorer.test_score_empty_file: TestHealthScorer#test_score_empty_file().
  TestHealthScorer.test_score_nonexistent_file: TestHealthScorer#test_score_nonexistent_file().
  TestHealthScorer.test_large_file_gets_penalized: TestHealthScorer#test_large_file_gets_penalized().
  TestHealthScorer.test_cc_penalizes_branches: TestHealthScorer#test_cc_penalizes_branches().
  TestHealthScorer.test_deeply_nested_code_penalized: TestHealthScorer#test_deeply_nested_code_penalized().
  TestHealthScorer.test_coverage_none_without_data: TestHealthScorer#test_coverage_none_without_data().
  TestHealthScorer.test_duplication_penalizes_repeated_code: TestHealthScorer#test_duplication_penalizes_repeated_code().
  TestHealthScorer.test_git_hotspot_none_outside_git: TestHealthScorer#test_git_hotspot_none_outside_git().
  TestHealthScore: TestHealthScore#
  TestScoreComplexityExtractorPath: TestScoreComplexityExtractorPath#
---
# Module: [`tests/unit/test_health_scorer.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_scorer.py)

## Classes
### `TestHealthScore`
- def: [`tests/unit/test_health_scorer.py:533`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_scorer.py#L533)
- doc: Test the HealthScore data class.
- signature: `class TestHealthScore:`
- members:
  - `test_health_score_creation(self)` — [`L536`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_scorer.py#L536)
  - `test_health_score_grade(self)` — [`L566`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_scorer.py#L566)
  - `test_health_score_to_dict(self)` — [`L553`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_scorer.py#L553)
- uses (calls/refs, reference-scoped): [`HealthScore`](../../tree_sitter_analyzer/health_scorer.md#HealthScore), [`file_path`](../../tree_sitter_analyzer/health_scorer.md#HealthScore.file_path), [`total`](../../tree_sitter_analyzer/health_scorer.md#HealthScore.total), [`grade`](../../tree_sitter_analyzer/health_scorer.md#HealthScore.grade), [`dimensions`](../../tree_sitter_analyzer/health_scorer.md#HealthScore.dimensions), [`to_dict`](../../tree_sitter_analyzer/health_scorer.md#HealthScore.to_dict)

### `TestHealthScorer`
- def: [`tests/unit/test_health_scorer.py:19`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_scorer.py#L19)
- doc: Test file health scoring.
- signature: `class TestHealthScorer:`
- members:
  - `fail_full_graph(_file_path)` — [`L117`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_scorer.py#L117)
  - `fake_run(cmd, **kwargs)` — [`L498`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_scorer.py#L498)
  - `scorer(self)` — [`L23`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_scorer.py#L23)
  - `test_bash_case_scores_decision_per_case(self, tmp_path)` — [`L413`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_scorer.py#L413) — A K-arm bash ``case`` dispatch: the extractor (single source of
  - `test_bash_complexity_counts_decision_nodes(self, scorer, tmp_path)` — [`L359`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_scorer.py#L359) — A bash function with 4 if + 2 while + 2 for + 1 case + 1 elif
  - `test_cc_penalizes_branches(self, scorer, tmp_path)` — [`L246`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_scorer.py#L246) — Code with many branches should have lower complexity score.
  - `test_coverage_none_without_data(self, scorer, tmp_path)` — [`L284`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_scorer.py#L284) — Coverage should be None (excluded from total) when no coverage.json exists.
  - `test_current_coverage_json_is_used(self, monkeypatch, tmp_path)` — [`L324`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_scorer.py#L324) — Use JSON coverage when it is as current as the raw coverage data.
  - `test_deeply_nested_code_penalized(self, scorer, tmp_path)` — [`L267`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_scorer.py#L267) — Deeply nested code should have lower structure score.
  - `test_dependencies_neutral_for_unanalyzable_languages(self, tmp_path)` — [`L389`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_scorer.py#L389) — Languages DependencyGraph cannot resolve (bash/scala/swift) must
  - `test_duplication_penalizes_repeated_code(self, scorer, tmp_path)` — [`L459`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_scorer.py#L459) — Files with repeated code blocks should have lower duplication score.
  - `test_fast_dependencies_neutral_for_unanalyzable_language(self, tmp_path)` — [`L403`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_scorer.py#L403) — The ``fast_dependencies=True`` path (``_score_deps_fallback``) must
  - `test_git_hotspot_none_outside_git(self, scorer, tmp_path)` — [`L477`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_scorer.py#L477) — Git hotspot should be None for files outside git repo.
  - `test_git_hotspot_uses_repo_relative_pathspec(self, monkeypatch, tmp_path)` — [`L485`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_scorer.py#L485) — Git hotspot should query from repo root with a repo-relative path.
  - `test_healthy_file_scores_higher(self, scorer)` — [`L28`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_scorer.py#L28) — healthy.py should score higher than unhealthy.py.
  - `test_is_excluded_falls_back_to_absolute_parts(self, tmp_path)` — [`L151`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_scorer.py#L151) — Paths outside root still honor generated/hidden path parts.
  - `test_iter_source_files_skips_hidden_filenames(self, tmp_path)` — [`L159`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_scorer.py#L159) — Hidden filenames are not counted as project source files.
  - `test_large_file_gets_penalized(self, scorer, tmp_path)` — [`L236`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_scorer.py#L236) — Files over 500 lines should have lower size score.
  - `test_scala_avg_cc_includes_all_methods(self, tmp_path)` — [`L429`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_scorer.py#L429) — A Scala trait with abstract + concrete methods: the extractor
  - `test_score_empty_file(self, scorer, tmp_path)` — [`L54`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_scorer.py#L54) — Empty file gets a baseline score.
  - `test_score_file_default_dependencies_uses_full_graph_score(self, monkeypatch, tmp_path)` — [`L131`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_scorer.py#L131) — Default scoring keeps the full dependency graph dimension.
  - `test_score_file_fast_dependencies_uses_fallback(self, monkeypatch, tmp_path)` — [`L109`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_scorer.py#L109) — Latency-sensitive callers can bypass whole-project dependency graphing.
  - `test_score_has_breakdown(self, scorer)` — [`L44`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_scorer.py#L44) — Score should include per-dimension breakdown.
  - `test_score_is_between_0_and_100(self, scorer)` — [`L36`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_scorer.py#L36) — All scores should be in the 0-100 range.
  - `test_score_nonexistent_file(self, scorer)` — [`L61`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_scorer.py#L61) — Nonexistent file returns 0 score.
  - `test_score_project(self, scorer)` — [`L66`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_scorer.py#L66) — Can score an entire project directory.
  - `test_score_project_counts_defensive_excluded_file(self, monkeypatch, tmp_path)` — [`L190`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_scorer.py#L190) — A defensive _is_excluded hit is still reported in project stats.
  - `test_score_project_counts_scoring_failures(self, monkeypatch, tmp_path)` — [`L176`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_scorer.py#L176) — Stats should record files that were discovered but failed scoring.
  - `test_score_project_includes_reported_source_extensions(self, scorer, tmp_path)` — [`L73`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_scorer.py#L73) — Project scoring should include all configured reportable extensions.
  - `test_score_project_prunes_hidden_and_generated_dirs(self, tmp_path)` — [`L211`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_scorer.py#L211) — Project scoring should not descend into hidden/generated directories.
  - `test_score_project_respects_custom_source_extensions(self, tmp_path)` — [`L94`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_scorer.py#L94) — Health scorer should limit scan scope to caller-provided extensions.
  - `test_seven_dimensions_in_weights(self)` — [`L512`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_scorer.py#L512) — All 7 dimensions should be in DIMENSION_WEIGHTS.
  - `test_stale_coverage_json_is_ignored(self, monkeypatch, tmp_path)` — [`L294`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_scorer.py#L294) — Do not use stale JSON coverage when pytest-cov has newer raw data.
  - `test_weights_sum_to_100(self)` — [`L351`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_scorer.py#L351) — Default dimension weights must sum to 100.
- uses (calls/refs, reference-scoped): [`analyze_file_complexity`](../../tree_sitter_analyzer/complexity_heatmap.md#analyze_file_complexity), [`HealthScorer`](../../tree_sitter_analyzer/health_scorer.md#HealthScorer), [`score_file`](../../tree_sitter_analyzer/health_scorer.md#HealthScorer.score_file), [`complexity`](../../tree_sitter_analyzer/complexity_heatmap.md#FunctionComplexity.complexity), [`score_dependencies`](../../tree_sitter_analyzer/health_scorer.md#score_dependencies), [`score_complexity`](../../tree_sitter_analyzer/health_scorer.md#score_complexity), [`file_path`](../../tree_sitter_analyzer/health_scorer.md#HealthScore.file_path), [`score_project_with_stats`](../../tree_sitter_analyzer/health_scorer.md#HealthScorer.score_project_with_stats), [`PROJECT_HEALTH_SOURCE_EXTS`](../../tree_sitter_analyzer/health_scorer.md#PROJECT_HEALTH_SOURCE_EXTS), [`_score_deps_fallback`](../../tree_sitter_analyzer/health_scorer.md#_score_deps_fallback), [`dimensions`](../../tree_sitter_analyzer/health_scorer.md#HealthScore.dimensions), [`score_project`](../../tree_sitter_analyzer/health_scorer.md#HealthScorer.score_project), [`to_dict`](../../tree_sitter_analyzer/health_scorer.md#HealthScore.to_dict), [`score_git_hotspot`](../../tree_sitter_analyzer/health_scorer.md#score_git_hotspot), [`DIMENSION_WEIGHTS`](../../tree_sitter_analyzer/health_scorer.md#DIMENSION_WEIGHTS), [`_iter_source_files`](../../tree_sitter_analyzer/health_scorer.md#HealthScorer._iter_source_files), [`_is_excluded`](../../tree_sitter_analyzer/health_scorer.md#HealthScorer._is_excluded)  (1 test-only)

### `TestScoreComplexityExtractorPath`
- def: [`tests/unit/test_health_scorer.py:581`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_scorer.py#L581)
- doc: Verify score_complexity derives CC from the extractor (single
- signature: `class TestScoreComplexityExtractorPath:`
- members:
  - `test_extractor_aggregate_matches_scorer_for_multi_function_file(self, tmp_path)` — [`L766`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_scorer.py#L766) — For a Python file with >= 3 functions, score_complexity must use
  - `test_java_high_complexity_method_scored_correctly(self, tmp_path)` — [`L701`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_scorer.py#L701) — A single Java method with CC > 15 must be penalised.
  - `test_java_switch_counts_construct_once_via_extractor(self, tmp_path)` — [`L653`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_scorer.py#L653) — A Java ``switch`` contributes exactly ONE decision to cyclomatic
  - `test_java_switch_ternary_do_while_matches_extractor(self, tmp_path)` — [`L599`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_scorer.py#L599) — Java method with 3-case switch + ternary + do-while must yield
  - `test_javascript_ternary_scored_correctly(self, tmp_path)` — [`L736`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_scorer.py#L736) — JavaScript ternary_expression was mapped to ``conditional_expression``
  - `test_no_plugin_language_returns_neutral(self, tmp_path)` — [`L759`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_scorer.py#L759) — When language is None, score_complexity returns 50.0 (neutral).
- protocol/private: `_write`[`L594`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_scorer.py#L594)
- uses (calls/refs, reference-scoped): [`analyze_file_complexity`](../../tree_sitter_analyzer/complexity_heatmap.md#analyze_file_complexity), [`complexity`](../../tree_sitter_analyzer/complexity_heatmap.md#FunctionComplexity.complexity), [`score_complexity`](../../tree_sitter_analyzer/health_scorer.md#score_complexity), [`CC_IDEAL`](../../tree_sitter_analyzer/health_scorer.md#CC_IDEAL)

## Module values
- `FIXTURES_DIR` — [`L10`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_scorer.py#L10)
- `HEALTH_PROJECT` — [`L11`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_scorer.py#L11)

