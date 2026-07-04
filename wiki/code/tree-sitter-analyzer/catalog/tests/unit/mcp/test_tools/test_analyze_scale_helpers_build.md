---
title: 'Module: tests/unit/mcp/test_tools/test_analyze_scale_helpers_build.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_tools/test_analyze_scale_helpers_build.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_tools.test_analyze_scale_helpers_build`/
symbols:
  _make_analysis_result: _make_analysis_result().
  TestCreateJsonFileAnalysis._base_metrics: TestCreateJsonFileAnalysis#_base_metrics().
  TestBuildAnalysisResult.test_with_elements_summary: TestBuildAnalysisResult#test_with_elements_summary().
  _make_element: _make_element().
  TestBuildAnalysisResult.test_basic_result_structure: TestBuildAnalysisResult#test_basic_result_structure().
  TestBuildAnalysisResult.test_package_included_when_present: TestBuildAnalysisResult#test_package_included_when_present().
  TestBuildAnalysisResult.test_package_none_when_absent: TestBuildAnalysisResult#test_package_none_when_absent().
  TestBuildDetailedAnalysis.test_detailed_class_extraction: TestBuildDetailedAnalysis#test_detailed_class_extraction().
  TestBuildDetailedAnalysis.test_detailed_method_extraction: TestBuildDetailedAnalysis#test_detailed_method_extraction().
  TestBuildDetailedAnalysis.test_detailed_field_extraction: TestBuildDetailedAnalysis#test_detailed_field_extraction().
  TestBuildDetailedAnalysis.test_mixed_elements_in_detailed: TestBuildDetailedAnalysis#test_mixed_elements_in_detailed().
  TestCreateJsonFileAnalysis.test_basic_analysis_structure: TestCreateJsonFileAnalysis#test_basic_analysis_structure().
  TestCreateJsonFileAnalysis.test_small_scale_category: TestCreateJsonFileAnalysis#test_small_scale_category().
  TestCreateJsonFileAnalysis.test_medium_scale_category: TestCreateJsonFileAnalysis#test_medium_scale_category().
  TestCreateJsonFileAnalysis.test_large_scale_category: TestCreateJsonFileAnalysis#test_large_scale_category().
  TestCreateJsonFileAnalysis.test_without_guidance: TestCreateJsonFileAnalysis#test_without_guidance().
  TestCreateJsonFileAnalysis.test_with_guidance: TestCreateJsonFileAnalysis#test_with_guidance().
  TestCreateJsonFileAnalysis.test_complexity_metrics_zeros: TestCreateJsonFileAnalysis#test_complexity_metrics_zeros().
  TestCreateJsonFileAnalysis.test_structural_overview_empty: TestCreateJsonFileAnalysis#test_structural_overview_empty().
  TestCreateJsonFileAnalysis.test_suitable_for_full_analysis_under_1000_lines: TestCreateJsonFileAnalysis#test_suitable_for_full_analysis_under_1000_lines().
  TestCreateJsonFileAnalysis.test_not_suitable_for_full_analysis_over_1000_lines: TestCreateJsonFileAnalysis#test_not_suitable_for_full_analysis_over_1000_lines().
  TestBuildAnalysisResult._mock_count_fn: TestBuildAnalysisResult#_mock_count_fn().
  TestBuildAnalysisResult.test_none_analysis_result: TestBuildAnalysisResult#test_none_analysis_result().
  TestBuildDetailedAnalysis.test_empty_analysis: TestBuildDetailedAnalysis#test_empty_analysis().
  TestBuildDetailedAnalysis.test_statistics_from_analysis_result: TestBuildDetailedAnalysis#test_statistics_from_analysis_result().
  TestF12FormatKeyConsistency.test_create_json_file_analysis_exposes_output_format_in_json: TestF12FormatKeyConsistency#test_create_json_file_analysis_exposes_output_format_in_json().
  TestF12FormatKeyConsistency.test_create_json_file_analysis_exposes_output_format_in_toon: TestF12FormatKeyConsistency#test_create_json_file_analysis_exposes_output_format_in_toon().
  TestF12FormatKeyConsistency.test_format_alias_matches_output_format_for_both_paths: TestF12FormatKeyConsistency#test_format_alias_matches_output_format_for_both_paths().
  TestF12FormatKeyConsistency._metrics: TestF12FormatKeyConsistency#_metrics().
  TestBuildDetailedAnalysis.test_none_analysis_result: TestBuildDetailedAnalysis#test_none_analysis_result().
  TestCreateJsonFileAnalysis: TestCreateJsonFileAnalysis#
  TestBuildAnalysisResult: TestBuildAnalysisResult#
  TestBuildDetailedAnalysis: TestBuildDetailedAnalysis#
  TestF12FormatKeyConsistency: TestF12FormatKeyConsistency#
---
# Module: [`tests/unit/mcp/test_tools/test_analyze_scale_helpers_build.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_build.py)

## Classes
### `TestBuildAnalysisResult`
- def: [`tests/unit/mcp/test_tools/test_analyze_scale_helpers_build.py:157`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_build.py#L157)
- signature: `class TestBuildAnalysisResult:`
- members:
  - `test_basic_result_structure(self)` — [`L161`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_build.py#L161)
  - `test_none_analysis_result(self)` — [`L191`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_build.py#L191)
  - `test_package_included_when_present(self)` — [`L203`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_build.py#L203)
  - `test_package_none_when_absent(self)` — [`L216`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_build.py#L216)
  - `test_with_elements_summary(self)` — [`L175`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_build.py#L175)
- protocol/private: `_mock_count_fn`[`L158`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_build.py#L158)
- uses (calls/refs, reference-scoped): [`build_analysis_result`](../../../../tree_sitter_analyzer/mcp/tools/analyze_scale_helpers.md#build_analysis_result)  (2 test-only)

### `TestBuildDetailedAnalysis`
- def: [`tests/unit/mcp/test_tools/test_analyze_scale_helpers_build.py:228`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_build.py#L228)
- signature: `class TestBuildDetailedAnalysis:`
- members:
  - `test_detailed_class_extraction(self)` — [`L243`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_build.py#L243)
  - `test_detailed_field_extraction(self)` — [`L291`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_build.py#L291)
  - `test_detailed_method_extraction(self)` — [`L266`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_build.py#L266)
  - `test_empty_analysis(self)` — [`L229`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_build.py#L229)
  - `test_mixed_elements_in_detailed(self)` — [`L318`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_build.py#L318)
  - `test_none_analysis_result(self)` — [`L238`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_build.py#L238)
  - `test_statistics_from_analysis_result(self)` — [`L312`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_build.py#L312)
- uses (calls/refs, reference-scoped): [`build_detailed_analysis`](../../../../tree_sitter_analyzer/mcp/tools/analyze_scale_helpers.md#build_detailed_analysis)  (2 test-only)

### `TestCreateJsonFileAnalysis`
- def: [`tests/unit/mcp/test_tools/test_analyze_scale_helpers_build.py:78`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_build.py#L78)
- signature: `class TestCreateJsonFileAnalysis:`
- members:
  - `test_basic_analysis_structure(self)` — [`L87`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_build.py#L87)
  - `test_complexity_metrics_zeros(self)` — [`L126`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_build.py#L126)
  - `test_large_scale_category(self)` — [`L107`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_build.py#L107)
  - `test_medium_scale_category(self)` — [`L101`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_build.py#L101)
  - `test_not_suitable_for_full_analysis_over_1000_lines(self)` — [`L150`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_build.py#L150)
  - `test_small_scale_category(self)` — [`L95`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_build.py#L95)
  - `test_structural_overview_empty(self)` — [`L135`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_build.py#L135)
  - `test_suitable_for_full_analysis_under_1000_lines(self)` — [`L144`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_build.py#L144)
  - `test_with_guidance(self)` — [`L117`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_build.py#L117)
  - `test_without_guidance(self)` — [`L113`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_build.py#L113)
- protocol/private: `_base_metrics`[`L79`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_build.py#L79)
- uses (calls/refs, reference-scoped): [`create_json_file_analysis`](../../../../tree_sitter_analyzer/mcp/tools/analyze_scale_helpers.md#create_json_file_analysis)

### `TestF12FormatKeyConsistency`
- def: [`tests/unit/mcp/test_tools/test_analyze_scale_helpers_build.py:331`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_build.py#L331)
- doc: Regression tests for F12 — round-16b dogfood found that the JSON
- signature: `class TestF12FormatKeyConsistency:`
- members:
  - `test_create_json_file_analysis_exposes_output_format_in_json(self)` — [`L350`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_build.py#L350) — JSON-file path on JSON output must expose ``output_format`` and
  - `test_create_json_file_analysis_exposes_output_format_in_toon(self)` — [`L361`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_build.py#L361) — JSON-file path on TOON output must still expose ``output_format``
  - `test_format_alias_matches_output_format_for_both_paths(self)` — [`L373`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_build.py#L373) — Whichever format the caller asks for, ``format`` and
- protocol/private: `_metrics`[`L340`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_build.py#L340)
- uses (calls/refs, reference-scoped): [`create_json_file_analysis`](../../../../tree_sitter_analyzer/mcp/tools/analyze_scale_helpers.md#create_json_file_analysis)

## Functions
- `_make_analysis_result(elements=None, package=None, annotations=None)` — [`L70`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_build.py#L70)
- `_make_element(element_type="class", name="TestElement", start_line=1, end_line=10, class_type="class", visibility="public", extends_class=None, implements_interfaces=None, annotations=None, return_type="void", parameters=None, complexity_score=0, is_constructor=False, is_static=False, field_type="Object", is_final=False, imported_name="TestImport", import_statement="import TestImport", line_number=1, is_static_import=False, is_wildcard=False, file_path="test.py")` — [`L14`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_build.py#L14)

