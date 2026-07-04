---
title: 'Module: tests/unit/mcp/test_tools/test_check_scale_output_cap_755.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_tools/test_check_scale_output_cap_755.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_tools.test_check_scale_output_cap_755`/
symbols:
  TestUniversalOverviewMethodCap._make_n_methods: TestUniversalOverviewMethodCap#_make_n_methods().
  _make_analysis_result_universal: _make_analysis_result_universal().
  TestUniversalOverviewMethodCap.test_under_cap_no_truncation_metadata: TestUniversalOverviewMethodCap#test_under_cap_no_truncation_metadata().
  TestUniversalOverviewMethodCap.test_exactly_cap_no_truncation: TestUniversalOverviewMethodCap#test_exactly_cap_no_truncation().
  TestUniversalOverviewMethodCap.test_over_cap_truncates_to_cap: TestUniversalOverviewMethodCap#test_over_cap_truncates_to_cap().
  TestUniversalOverviewMethodCap.test_large_method_count_capped_exactly: TestUniversalOverviewMethodCap#test_large_method_count_capped_exactly().
  TestUniversalOverviewMethodCap.test_cap_preserves_first_n_entries_by_line: TestUniversalOverviewMethodCap#test_cap_preserves_first_n_entries_by_line().
  TestUniversalOverviewMethodCap.test_custom_cap_via_kwarg: TestUniversalOverviewMethodCap#test_custom_cap_via_kwarg().
  TestUniversalOverviewMethodCap.test_complexity_hotspots_are_capped_with_metadata: TestUniversalOverviewMethodCap#test_complexity_hotspots_are_capped_with_metadata().
  TestJavaOverviewMethodCap.test_under_cap_no_truncation: TestJavaOverviewMethodCap#test_under_cap_no_truncation().
  TestJavaOverviewMethodCap.test_over_cap_truncates: TestJavaOverviewMethodCap#test_over_cap_truncates().
  TestJavaOverviewMethodCap.test_exactly_cap_no_truncation: TestJavaOverviewMethodCap#test_exactly_cap_no_truncation().
  TestJavaOverviewMethodCap.test_complexity_hotspots_are_capped_with_metadata: TestJavaOverviewMethodCap#test_complexity_hotspots_are_capped_with_metadata().
  TestJavaOverviewMethodCap._make_n_java_methods: TestJavaOverviewMethodCap#_make_n_java_methods().
  TestUniversalOverviewMethodCap.test_zero_methods_no_truncation_metadata: TestUniversalOverviewMethodCap#test_zero_methods_no_truncation_metadata().
  _make_java_fn_element: _make_java_fn_element().
  TestJavaOverviewMethodCap._make_result: TestJavaOverviewMethodCap#_make_result().
  TestMethodsOutputCap.test_cap_constant_is_fifty: TestMethodsOutputCap#test_cap_constant_is_fifty().
  TestMethodsOutputCap.test_cap_constant_is_int: TestMethodsOutputCap#test_cap_constant_is_int().
  _make_fn_element: _make_fn_element().
  _make_analysis_result_java: _make_analysis_result_java().
  TestMethodsOutputCap: TestMethodsOutputCap#
  TestUniversalOverviewMethodCap: TestUniversalOverviewMethodCap#
  TestJavaOverviewMethodCap: TestJavaOverviewMethodCap#
---
# Module: [`tests/unit/mcp/test_tools/test_check_scale_output_cap_755.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_check_scale_output_cap_755.py)

## Classes
### `TestJavaOverviewMethodCap`
- def: [`tests/unit/mcp/test_tools/test_check_scale_output_cap_755.py:234`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_check_scale_output_cap_755.py#L234)
- doc: The Java/Python extract_structural_overview path must enforce the same cap.
- signature: `class TestJavaOverviewMethodCap:`
- members:
  - `test_complexity_hotspots_are_capped_with_metadata(self)` — [`L281`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_check_scale_output_cap_755.py#L281)
  - `test_exactly_cap_no_truncation(self)` — [`L269`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_check_scale_output_cap_755.py#L269)
  - `test_over_cap_truncates(self)` — [`L260`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_check_scale_output_cap_755.py#L260)
  - `test_under_cap_no_truncation(self)` — [`L248`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_check_scale_output_cap_755.py#L248)
- protocol/private: `_make_n_java_methods`[`L237`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_check_scale_output_cap_755.py#L237), `_make_result`[`L242`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_check_scale_output_cap_755.py#L242)
- uses (calls/refs, reference-scoped): [`extract_structural_overview`](../../../../tree_sitter_analyzer/mcp/tools/analyze_scale_helpers.md#extract_structural_overview)  (1 test-only)

### `TestMethodsOutputCap`
- def: [`tests/unit/mcp/test_tools/test_check_scale_output_cap_755.py:100`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_check_scale_output_cap_755.py#L100)
- signature: `class TestMethodsOutputCap:`
- members:
  - `test_cap_constant_is_fifty(self)` — [`L101`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_check_scale_output_cap_755.py#L101) — Default cap must be exactly 50.
  - `test_cap_constant_is_int(self)` — [`L105`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_check_scale_output_cap_755.py#L105)
- uses (calls/refs, reference-scoped): [`METHODS_OUTPUT_CAP`](../../../../tree_sitter_analyzer/mcp/tools/analyze_scale_helpers.md#METHODS_OUTPUT_CAP)

### `TestUniversalOverviewMethodCap`
- def: [`tests/unit/mcp/test_tools/test_check_scale_output_cap_755.py:114`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_check_scale_output_cap_755.py#L114)
- signature: `class TestUniversalOverviewMethodCap:`
- members:
  - `test_cap_preserves_first_n_entries_by_line(self)` — [`L174`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_check_scale_output_cap_755.py#L174) — The kept entries should be the first N by line order (insertion order).
  - `test_complexity_hotspots_are_capped_with_metadata(self)` — [`L207`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_check_scale_output_cap_755.py#L207) — #960: hotspots must be capped separately from the methods list.
  - `test_custom_cap_via_kwarg(self)` — [`L186`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_check_scale_output_cap_755.py#L186) — method_cap keyword argument overrides the default cap.
  - `test_exactly_cap_no_truncation(self)` — [`L134`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_check_scale_output_cap_755.py#L134) — Exactly 50 methods: no truncation.
  - `test_large_method_count_capped_exactly(self)` — [`L164`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_check_scale_output_cap_755.py#L164) — 20 000 methods: list stays at 50, total_methods = 20 000.
  - `test_over_cap_truncates_to_cap(self)` — [`L147`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_check_scale_output_cap_755.py#L147) — 51 methods: list is capped at 50, truncation flag set.
  - `test_under_cap_no_truncation_metadata(self)` — [`L121`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_check_scale_output_cap_755.py#L121) — Fewer than CAP methods: no truncation flag, total_methods == len(methods).
  - `test_zero_methods_no_truncation_metadata(self)` — [`L196`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_check_scale_output_cap_755.py#L196) — Empty method list: total_methods == 0, no truncation flag.
- protocol/private: `_make_n_methods`[`L115`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_check_scale_output_cap_755.py#L115)
- uses (calls/refs, reference-scoped): [`extract_structural_overview_universal`](../../../../tree_sitter_analyzer/mcp/tools/analyze_scale_helpers.md#extract_structural_overview_universal)  (2 test-only)

## Functions
- `_make_analysis_result_java(elements)` — [`L89`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_check_scale_output_cap_755.py#L89)
- `_make_analysis_result_universal(elements)` — [`L83`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_check_scale_output_cap_755.py#L83)
- `_make_fn_element(name: str, start_line: int = 1, end_line: int = 5, complexity: int = 0)` — [`L34`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_check_scale_output_cap_755.py#L34) — Minimal mock function element for universal overview.
- `_make_java_fn_element(name: str, start_line: int = 1, end_line: int = 5, complexity_score: int = 0, visibility: str = "public", return_type: str = "void", parameters: list | None = None, is_constructor: bool = False, is_static: bool = False, annotations: list | None = None)` — [`L47`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_check_scale_output_cap_755.py#L47) — Minimal mock for the Java/Python extract_structural_overview path.

