---
title: 'Module: tests/unit/grammar_coverage/test_auto_discovery.py'
type: catalog
provenance: extracted
module: tests/unit/grammar_coverage/test_auto_discovery.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.grammar_coverage.test_auto_discovery`/
symbols:
  test_coverage_gap_report_not_ok: test_coverage_gap_report_not_ok().
  test_coverage_gap_report_is_ok: test_coverage_gap_report_is_ok().
  test_analyze_coverage_gap_has_required_keys: test_analyze_coverage_gap_has_required_keys().
  test_score_wrapper_node_with_definition_field: test_score_wrapper_node_with_definition_field().
  test_node_stats_avg_children_computed: test_node_stats_avg_children_computed().
  test_analyze_coverage_gap_custom_corpus: test_analyze_coverage_gap_custom_corpus().
  test_analyze_coverage_gap_unavailable_language: test_analyze_coverage_gap_unavailable_language().
  python_report: python_report().
  test_detect_wrapper_nodes_python_decorated_definition: test_detect_wrapper_nodes_python_decorated_definition().
  test_detect_wrapper_nodes_sorted_by_score: test_detect_wrapper_nodes_sorted_by_score().
  test_detect_wrapper_nodes_typescript: test_detect_wrapper_nodes_typescript().
  test_analyze_coverage_gap_is_ok: test_analyze_coverage_gap_is_ok().
  test_analyze_all_languages_at_least_half_ok: test_analyze_all_languages_at_least_half_ok().
  test_generate_report_not_empty: test_generate_report_not_empty().
  test_generate_report_contains_language: test_generate_report_contains_language().
  test_generate_report_markdown_structure: test_generate_report_markdown_structure().
  test_score_wrapper_node_empty_stats: test_score_wrapper_node_empty_stats().
  test_score_wrapper_node_name_pattern: test_score_wrapper_node_name_pattern().
  test_node_stats_avg_children_zero_samples: test_node_stats_avg_children_zero_samples().
  test_get_all_node_types_python: test_get_all_node_types_python().
  test_get_all_node_types_is_sorted: test_get_all_node_types_is_sorted().
  test_get_all_node_types_returns_named_only: test_get_all_node_types_returns_named_only().
  test_get_all_node_types_contains_known_types: test_get_all_node_types_contains_known_types().
  test_get_all_node_types_unsupported_language: test_get_all_node_types_unsupported_language().
  test_get_all_node_types_typescript: test_get_all_node_types_typescript().
  test_get_all_field_names_python: test_get_all_field_names_python().
  test_get_all_field_names_unavailable_language: test_get_all_field_names_unavailable_language().
  test_detect_wrapper_nodes_python_has_results: test_detect_wrapper_nodes_python_has_results().
  test_detect_wrapper_nodes_threshold_effect: test_detect_wrapper_nodes_threshold_effect().
  test_detect_wrapper_nodes_empty_code: test_detect_wrapper_nodes_empty_code().
  test_enumerate_syntax_paths_returns_list: test_enumerate_syntax_paths_returns_list().
  test_enumerate_syntax_paths_format: test_enumerate_syntax_paths_format().
  test_enumerate_syntax_paths_no_duplicates: test_enumerate_syntax_paths_no_duplicates().
  test_enumerate_syntax_paths_max_depth: test_enumerate_syntax_paths_max_depth().
  test_analyze_coverage_gap_coverage_positive: test_analyze_coverage_gap_coverage_positive().
  test_analyze_coverage_gap_total_types_positive: test_analyze_coverage_gap_total_types_positive().
  test_analyze_coverage_gap_consistency: test_analyze_coverage_gap_consistency().
  test_analyze_coverage_gap_elapsed_ms: test_analyze_coverage_gap_elapsed_ms().
  test_analyze_all_languages_no_crash: test_analyze_all_languages_no_crash().
  test_analyze_all_languages_contains_python: test_analyze_all_languages_contains_python().
  test_analyze_all_languages_custom_list: test_analyze_all_languages_custom_list().
  engine: engine().
  python_corpus: python_corpus().
---
# Module: [`tests/unit/grammar_coverage/test_auto_discovery.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_auto_discovery.py)

## Functions
- `engine()` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_auto_discovery.py#L21)
- `python_corpus()` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_auto_discovery.py#L26)
- `python_report(engine: AutoDiscoveryEngine, python_corpus: str)` — [`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_auto_discovery.py#L31)
- `test_analyze_all_languages_at_least_half_ok(engine: AutoDiscoveryEngine)` — [`L298`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_auto_discovery.py#L298)
- `test_analyze_all_languages_contains_python(engine: AutoDiscoveryEngine)` — [`L288`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_auto_discovery.py#L288)
- `test_analyze_all_languages_custom_list(engine: AutoDiscoveryEngine)` — [`L293`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_auto_discovery.py#L293)
- `test_analyze_all_languages_no_crash(engine: AutoDiscoveryEngine)` — [`L265`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_auto_discovery.py#L265)
- `test_analyze_coverage_gap_consistency(python_report: CoverageGapReport)` — [`L228`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_auto_discovery.py#L228)
- `test_analyze_coverage_gap_coverage_positive(python_report: CoverageGapReport)` — [`L213`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_auto_discovery.py#L213)
- `test_analyze_coverage_gap_custom_corpus(engine: AutoDiscoveryEngine)` — [`L241`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_auto_discovery.py#L241)
- `test_analyze_coverage_gap_elapsed_ms(python_report: CoverageGapReport)` — [`L254`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_auto_discovery.py#L254)
- `test_analyze_coverage_gap_has_required_keys(python_report: CoverageGapReport)` — [`L201`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_auto_discovery.py#L201)
- `test_analyze_coverage_gap_is_ok(python_report: CoverageGapReport)` — [`L236`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_auto_discovery.py#L236)
- `test_analyze_coverage_gap_total_types_positive(python_report: CoverageGapReport)` — [`L220`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_auto_discovery.py#L220)
- `test_analyze_coverage_gap_unavailable_language(engine: AutoDiscoveryEngine)` — [`L248`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_auto_discovery.py#L248)
- `test_coverage_gap_report_is_ok()` — [`L385`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_auto_discovery.py#L385)
- `test_coverage_gap_report_not_ok()` — [`L398`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_auto_discovery.py#L398)
- `test_detect_wrapper_nodes_empty_code(engine: AutoDiscoveryEngine)` — [`L151`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_auto_discovery.py#L151)
- `test_detect_wrapper_nodes_python_decorated_definition(engine: AutoDiscoveryEngine, python_corpus: str)` — [`L115`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_auto_discovery.py#L115)
- `test_detect_wrapper_nodes_python_has_results(engine: AutoDiscoveryEngine, python_corpus: str)` — [`L108`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_auto_discovery.py#L108)
- `test_detect_wrapper_nodes_sorted_by_score(engine: AutoDiscoveryEngine, python_corpus: str)` — [`L125`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_auto_discovery.py#L125)
- `test_detect_wrapper_nodes_threshold_effect(engine: AutoDiscoveryEngine, python_corpus: str)` — [`L133`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_auto_discovery.py#L133)
- `test_detect_wrapper_nodes_typescript(engine: AutoDiscoveryEngine)` — [`L143`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_auto_discovery.py#L143)
- `test_enumerate_syntax_paths_format(engine: AutoDiscoveryEngine, python_corpus: str)` — [`L172`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_auto_discovery.py#L172)
- `test_enumerate_syntax_paths_max_depth(engine: AutoDiscoveryEngine, python_corpus: str)` — [`L187`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_auto_discovery.py#L187)
- `test_enumerate_syntax_paths_no_duplicates(engine: AutoDiscoveryEngine, python_corpus: str)` — [`L180`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_auto_discovery.py#L180)
- `test_enumerate_syntax_paths_returns_list(engine: AutoDiscoveryEngine, python_corpus: str)` — [`L162`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_auto_discovery.py#L162)
- `test_generate_report_contains_language(engine: AutoDiscoveryEngine)` — [`L321`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_auto_discovery.py#L321)
- `test_generate_report_markdown_structure(engine: AutoDiscoveryEngine)` — [`L327`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_auto_discovery.py#L327)
- `test_generate_report_not_empty(engine: AutoDiscoveryEngine)` — [`L311`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_auto_discovery.py#L311)
- `test_get_all_field_names_python(engine: AutoDiscoveryEngine)` — [`L86`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_auto_discovery.py#L86)
- `test_get_all_field_names_unavailable_language(engine: AutoDiscoveryEngine)` — [`L97`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_auto_discovery.py#L97)
- `test_get_all_node_types_contains_known_types(engine: AutoDiscoveryEngine)` — [`L61`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_auto_discovery.py#L61)
- `test_get_all_node_types_is_sorted(engine: AutoDiscoveryEngine)` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_auto_discovery.py#L48)
- `test_get_all_node_types_python(engine: AutoDiscoveryEngine)` — [`L40`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_auto_discovery.py#L40)
- `test_get_all_node_types_returns_named_only(engine: AutoDiscoveryEngine)` — [`L53`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_auto_discovery.py#L53)
- `test_get_all_node_types_typescript(engine: AutoDiscoveryEngine)` — [`L74`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_auto_discovery.py#L74)
- `test_get_all_node_types_unsupported_language(engine: AutoDiscoveryEngine)` — [`L69`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_auto_discovery.py#L69)
- `test_node_stats_avg_children_computed()` — [`L375`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_auto_discovery.py#L375)
- `test_node_stats_avg_children_zero_samples()` — [`L370`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_auto_discovery.py#L370)
- `test_score_wrapper_node_empty_stats()` — [`L340`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_auto_discovery.py#L340)
- `test_score_wrapper_node_name_pattern()` — [`L359`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_auto_discovery.py#L359)
- `test_score_wrapper_node_with_definition_field()` — [`L347`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_auto_discovery.py#L347)

