---
title: 'Module: tests/integration/test_call_graph_cross_file.py'
type: catalog
provenance: extracted
module: tests/integration/test_call_graph_cross_file.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.test_call_graph_cross_file`/
symbols:
  TestCallGraphCrossFileJS.test_js_cross_file_calls: TestCallGraphCrossFileJS#test_js_cross_file_calls().
  graph: graph().
  python_project: python_project().
  TestCallGraphCrossFileBuild: TestCallGraphCrossFileBuild#
  TestCallGraphCrossFileBuild.test_builds_graph: TestCallGraphCrossFileBuild#test_builds_graph().
  TestCallGraphCrossFileBuild.test_finds_functions: TestCallGraphCrossFileBuild#test_finds_functions().
  TestCallGraphCrossFileBuild.test_finds_cross_file_edges: TestCallGraphCrossFileBuild#test_finds_cross_file_edges().
  TestCallGraphCrossFileBuild.test_summary: TestCallGraphCrossFileBuild#test_summary().
  TestCallGraphCrossFileResolution: TestCallGraphCrossFileResolution#
  TestCallGraphCrossFileResolution.test_main_calls_process: TestCallGraphCrossFileResolution#test_main_calls_process().
  TestCallGraphCrossFileResolution.test_service_calls_create_user: TestCallGraphCrossFileResolution#test_service_calls_create_user().
  TestCallGraphCrossFileResolution.test_create_user_is_called_by_process: TestCallGraphCrossFileResolution#test_create_user_is_called_by_process().
  TestCallGraphCrossFileResolution.test_process_is_called_by_run: TestCallGraphCrossFileResolution#test_process_is_called_by_run().
  TestCallGraphCrossFileResolution.test_import_resolution_prefers_imported_file: TestCallGraphCrossFileResolution#test_import_resolution_prefers_imported_file().
  TestCallGraphCrossFileNoResolution: TestCallGraphCrossFileNoResolution#
  TestCallGraphCrossFileNoResolution.test_dead_code_has_no_callers: TestCallGraphCrossFileNoResolution#test_dead_code_has_no_callers().
  TestCallGraphCrossFileNoResolution.test_entry_point_has_no_callers: TestCallGraphCrossFileNoResolution#test_entry_point_has_no_callers().
  TestCallGraphCrossFileJS: TestCallGraphCrossFileJS#
---
# Module: [`tests/integration/test_call_graph_cross_file.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_call_graph_cross_file.py)

## Classes
### `TestCallGraphCrossFileBuild`
- def: [`tests/integration/test_call_graph_cross_file.py:53`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_call_graph_cross_file.py#L53)
- signature: `class TestCallGraphCrossFileBuild:`
- members:
  - `test_builds_graph(self, graph)` — [`L54`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_call_graph_cross_file.py#L54)
  - `test_finds_cross_file_edges(self, graph)` — [`L64`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_call_graph_cross_file.py#L64)
  - `test_finds_functions(self, graph)` — [`L57`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_call_graph_cross_file.py#L57)
  - `test_summary(self, graph)` — [`L67`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_call_graph_cross_file.py#L67)

### `TestCallGraphCrossFileJS`
- def: [`tests/integration/test_call_graph_cross_file.py:113`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_call_graph_cross_file.py#L113)
- signature: `class TestCallGraphCrossFileJS:`
- members:
  - `test_js_cross_file_calls(self, tmp_path)` — [`L114`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_call_graph_cross_file.py#L114)
- uses (calls/refs, reference-scoped): [`CallGraph`](../../tree_sitter_analyzer/call_graph.md#CallGraph), [`build`](../../tree_sitter_analyzer/call_graph.md#CallGraph.build), [`callees_of`](../../tree_sitter_analyzer/call_graph.md#CallGraph.callees_of), [`_built`](../../tree_sitter_analyzer/call_graph.md#CallGraph._built)

### `TestCallGraphCrossFileNoResolution`
- def: [`tests/integration/test_call_graph_cross_file.py:103`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_call_graph_cross_file.py#L103)
- signature: `class TestCallGraphCrossFileNoResolution:`
- members:
  - `test_dead_code_has_no_callers(self, graph)` — [`L104`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_call_graph_cross_file.py#L104)
  - `test_entry_point_has_no_callers(self, graph)` — [`L108`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_call_graph_cross_file.py#L108)

### `TestCallGraphCrossFileResolution`
- def: [`tests/integration/test_call_graph_cross_file.py:76`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_call_graph_cross_file.py#L76)
- signature: `class TestCallGraphCrossFileResolution:`
- members:
  - `test_create_user_is_called_by_process(self, graph)` — [`L87`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_call_graph_cross_file.py#L87)
  - `test_import_resolution_prefers_imported_file(self, graph)` — [`L97`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_call_graph_cross_file.py#L97)
  - `test_main_calls_process(self, graph)` — [`L77`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_call_graph_cross_file.py#L77)
  - `test_process_is_called_by_run(self, graph)` — [`L92`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_call_graph_cross_file.py#L92)
  - `test_service_calls_create_user(self, graph)` — [`L82`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_call_graph_cross_file.py#L82)

## Functions
- `graph(python_project)` — [`L47`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_call_graph_cross_file.py#L47)
- `python_project(tmp_path)` — [`L11`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_call_graph_cross_file.py#L11)

