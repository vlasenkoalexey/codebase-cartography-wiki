---
title: 'Module: tests/unit/mcp/test_nav_impact_boundary.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_nav_impact_boundary.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_nav_impact_boundary`/
symbols:
  _make_ref: _make_ref().
  _capture_call_tool_handler: _capture_call_tool_handler().
  TestNavImpactBoundary.test_include_tests_false_tests_bucket_present_no_file_lists: TestNavImpactBoundary#test_include_tests_false_tests_bucket_present_no_file_lists().
  TestNavImpactBoundary.test_include_tests_true_adds_file_lists: TestNavImpactBoundary#test_include_tests_true_adds_file_lists().
  TestNavImpactBoundary.test_function_impact_mode_tests_bucket_in_risk: TestNavImpactBoundary#test_function_impact_mode_tests_bucket_in_risk().
  TestNavImpactBoundary.test_file_path_mismatch_gives_candidate_hint: TestNavImpactBoundary#test_file_path_mismatch_gives_candidate_hint().
  TestNavImpactBoundary.test_ambiguous_symbol_sets_flag_and_unknown_level: TestNavImpactBoundary#test_ambiguous_symbol_sets_flag_and_unknown_level().
  TestNavImpactBoundary.test_file_path_dot_prefix_does_not_false_positive: TestNavImpactBoundary#test_file_path_dot_prefix_does_not_false_positive().
  _make_mock_graph: _make_mock_graph().
  _capture_call_tool_handler.capture_decorator: _capture_call_tool_handler().capture_decorator().
  _capture_call_tool_handler.capture_decorator.decorator: _capture_call_tool_handler().capture_decorator().decorator().
  TestNavImpactBoundary.resolve_side_effect: TestNavImpactBoundary#resolve_side_effect().
  TestNavImpactBoundary: TestNavImpactBoundary#
---
# Module: [`tests/unit/mcp/test_nav_impact_boundary.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_nav_impact_boundary.py)

## Classes
### `TestNavImpactBoundary`
- def: [`tests/unit/mcp/test_nav_impact_boundary.py:69`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_nav_impact_boundary.py#L69)
- doc: RFC-0014 Phase A: boundary integration for nav action=impact.
- signature: `class TestNavImpactBoundary:`
- members:
  - `resolve_side_effect(name, fp=None)` — [`L287`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_nav_impact_boundary.py#L287)
  - `test_ambiguous_symbol_sets_flag_and_unknown_level(self, tmp_path)` — [`L224`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_nav_impact_boundary.py#L224) — #799: when resolve_targets returns >1 result with no file_path qualifier,
  - `test_file_path_dot_prefix_does_not_false_positive(self, tmp_path)` — [`L330`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_nav_impact_boundary.py#L330) — Codex P2 (#873): ./src/tool_a.py and src/tool_a.py are the same file.
  - `test_file_path_mismatch_gives_candidate_hint(self, tmp_path)` — [`L273`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_nav_impact_boundary.py#L273) — #867/#873: when file_path is set but doesn't match, warn with candidate files.
  - `test_function_impact_mode_tests_bucket_in_risk(self, tmp_path)` — [`L184`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_nav_impact_boundary.py#L184) — function_impact mode: tests bucket nested under result["risk"].
  - `test_include_tests_false_tests_bucket_present_no_file_lists(self, tmp_path)` — [`L81`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_nav_impact_boundary.py#L81) — include_tests=False (default): tests bucket always present, no file lists.
  - `test_include_tests_true_adds_file_lists(self, tmp_path)` — [`L129`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_nav_impact_boundary.py#L129) — include_tests=True: file lists appear in the tests bucket.
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerMCPServer`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer)  (3 test-only)

## Functions
- `_capture_call_tool_handler(server: TreeSitterAnalyzerMCPServer)` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_nav_impact_boundary.py#L33) — Capture the ``handle_call_tool`` closure registered by ``create_server``.
- `_make_mock_graph(func_ref: FunctionRef, callers=None, callees=None)` — [`L53`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_nav_impact_boundary.py#L53) — Build a minimal mock CallGraph for impact tests.
- `_make_ref(name: str, file: str)` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_nav_impact_boundary.py#L29)
- `capture_decorator(name)` — [`L40`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_nav_impact_boundary.py#L40)
- `decorator(func)` — [`L41`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_nav_impact_boundary.py#L41)

