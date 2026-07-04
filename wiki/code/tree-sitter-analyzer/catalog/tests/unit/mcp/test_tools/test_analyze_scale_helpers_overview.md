---
title: 'Module: tests/unit/mcp/test_tools/test_analyze_scale_helpers_overview.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_tools/test_analyze_scale_helpers_overview.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_tools.test_analyze_scale_helpers_overview`/
symbols:
  _make_analysis_result: _make_analysis_result().
  _make_element: _make_element().
  TestExtractStructuralOverview.test_extracts_class_with_all_fields: TestExtractStructuralOverview#test_extracts_class_with_all_fields().
  TestExtractStructuralOverview.test_extracts_method_with_all_fields: TestExtractStructuralOverview#test_extracts_method_with_all_fields().
  TestExtractStructuralOverview.test_high_complexity_method_creates_hotspot: TestExtractStructuralOverview#test_high_complexity_method_creates_hotspot().
  TestExtractStructuralOverview.test_low_complexity_method_no_hotspot: TestExtractStructuralOverview#test_low_complexity_method_no_hotspot().
  TestExtractStructuralOverview.test_extracts_field_with_all_fields: TestExtractStructuralOverview#test_extracts_field_with_all_fields().
  TestExtractStructuralOverview.test_extracts_import_with_all_fields: TestExtractStructuralOverview#test_extracts_import_with_all_fields().
  TestExtractStructuralOverview.test_mixed_elements_all_extracted: TestExtractStructuralOverview#test_mixed_elements_all_extracted().
  TestExtractStructuralOverview.test_boundary_complexity_7_no_hotspot: TestExtractStructuralOverview#test_boundary_complexity_7_no_hotspot().
  TestExtractStructuralOverview.test_boundary_complexity_8_creates_hotspot: TestExtractStructuralOverview#test_boundary_complexity_8_creates_hotspot().
  TestExtractStructuralOverview.test_empty_elements_returns_empty_overview: TestExtractStructuralOverview#test_empty_elements_returns_empty_overview().
  TestExtractStructuralOverviewUniversal.test_empty_elements_returns_empty: TestExtractStructuralOverviewUniversal#test_empty_elements_returns_empty().
  TestExtractStructuralOverviewUniversal.test_extracts_class_element: TestExtractStructuralOverviewUniversal#test_extracts_class_element().
  TestExtractStructuralOverviewUniversal.test_extracts_function_element: TestExtractStructuralOverviewUniversal#test_extracts_function_element().
  TestExtractStructuralOverviewUniversal.test_extracts_method_element: TestExtractStructuralOverviewUniversal#test_extracts_method_element().
  TestExtractStructuralOverviewUniversal.test_extracts_variable_element: TestExtractStructuralOverviewUniversal#test_extracts_variable_element().
  TestExtractStructuralOverviewUniversal.test_extracts_import_element: TestExtractStructuralOverviewUniversal#test_extracts_import_element().
  TestExtractStructuralOverviewUniversal.test_high_complexity_creates_hotspot: TestExtractStructuralOverviewUniversal#test_high_complexity_creates_hotspot().
  TestExtractStructuralOverviewUniversal.test_missing_attr_uses_defaults: TestExtractStructuralOverviewUniversal#test_missing_attr_uses_defaults().
  TestExtractStructuralOverviewUniversal.test_none_analysis_result_returns_empty: TestExtractStructuralOverviewUniversal#test_none_analysis_result_returns_empty().
  TestExtractStructuralOverviewUniversal.test_no_elements_attr_returns_empty: TestExtractStructuralOverviewUniversal#test_no_elements_attr_returns_empty().
  TestExtractStructuralOverview: TestExtractStructuralOverview#
  TestExtractStructuralOverviewUniversal: TestExtractStructuralOverviewUniversal#
---
# Module: [`tests/unit/mcp/test_tools/test_analyze_scale_helpers_overview.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_overview.py)

## Classes
### `TestExtractStructuralOverview`
- def: [`tests/unit/mcp/test_tools/test_analyze_scale_helpers_overview.py:77`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_overview.py#L77)
- signature: `class TestExtractStructuralOverview:`
- members:
  - `test_boundary_complexity_7_no_hotspot(self)` — [`L220`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_overview.py#L220)
  - `test_boundary_complexity_8_creates_hotspot(self)` — [`L228`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_overview.py#L228)
  - `test_empty_elements_returns_empty_overview(self)` — [`L78`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_overview.py#L78)
  - `test_extracts_class_with_all_fields(self)` — [`L87`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_overview.py#L87)
  - `test_extracts_field_with_all_fields(self)` — [`L163`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_overview.py#L163)
  - `test_extracts_import_with_all_fields(self)` — [`L186`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_overview.py#L186)
  - `test_extracts_method_with_all_fields(self)` — [`L112`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_overview.py#L112)
  - `test_high_complexity_method_creates_hotspot(self)` — [`L137`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_overview.py#L137)
  - `test_low_complexity_method_no_hotspot(self)` — [`L153`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_overview.py#L153)
  - `test_mixed_elements_all_extracted(self)` — [`L206`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_overview.py#L206)
- uses (calls/refs, reference-scoped): [`extract_structural_overview`](../../../../tree_sitter_analyzer/mcp/tools/analyze_scale_helpers.md#extract_structural_overview)  (2 test-only)

### `TestExtractStructuralOverviewUniversal`
- def: [`tests/unit/mcp/test_tools/test_analyze_scale_helpers_overview.py:237`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_overview.py#L237)
- signature: `class TestExtractStructuralOverviewUniversal:`
- members:
  - `test_empty_elements_returns_empty(self)` — [`L247`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_overview.py#L247)
  - `test_extracts_class_element(self)` — [`L252`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_overview.py#L252)
  - `test_extracts_function_element(self)` — [`L264`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_overview.py#L264)
  - `test_extracts_import_element(self)` — [`L298`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_overview.py#L298)
  - `test_extracts_method_element(self)` — [`L276`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_overview.py#L276)
  - `test_extracts_variable_element(self)` — [`L287`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_overview.py#L287)
  - `test_high_complexity_creates_hotspot(self)` — [`L309`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_overview.py#L309)
  - `test_missing_attr_uses_defaults(self)` — [`L321`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_overview.py#L321)
  - `test_no_elements_attr_returns_empty(self)` — [`L243`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_overview.py#L243)
  - `test_none_analysis_result_returns_empty(self)` — [`L238`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_overview.py#L238)
- uses (calls/refs, reference-scoped): [`extract_structural_overview_universal`](../../../../tree_sitter_analyzer/mcp/tools/analyze_scale_helpers.md#extract_structural_overview_universal)  (1 test-only)

## Functions
- `_make_analysis_result(elements=None, package=None, annotations=None)` — [`L69`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_overview.py#L69)
- `_make_element(element_type="class", name="TestElement", start_line=1, end_line=10, class_type="class", visibility="public", extends_class=None, implements_interfaces=None, annotations=None, return_type="void", parameters=None, complexity_score=0, is_constructor=False, is_static=False, field_type="Object", is_final=False, imported_name="TestImport", import_statement="import TestImport", line_number=1, is_static_import=False, is_wildcard=False, file_path="test.py")` — [`L13`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_overview.py#L13)

