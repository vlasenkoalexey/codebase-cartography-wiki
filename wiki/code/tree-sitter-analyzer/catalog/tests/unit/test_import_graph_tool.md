---
title: 'Module: tests/unit/test_import_graph_tool.py'
type: catalog
provenance: extracted
module: tests/unit/test_import_graph_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_import_graph_tool`/
symbols:
  TestSummaryMode.test_summary_success: TestSummaryMode#test_summary_success().
  TestCyclesMode.test_no_cycles: TestCyclesMode#test_no_cycles().
  TestCyclesMode.test_with_cycles: TestCyclesMode#test_with_cycles().
  TestCouplingMode.test_coupling: TestCouplingMode#test_coupling().
  TestToonFormat.test_toon_output: TestToonFormat#test_toon_output().
  TestModeInferenceFromFilePath.test_file_path_infers_deps: TestModeInferenceFromFilePath#test_file_path_infers_deps().
  TestModeInferenceFromFilePath.test_no_file_path_is_summary: TestModeInferenceFromFilePath#test_no_file_path_is_summary().
  TestModeInferenceFromFilePath.test_explicit_mode_wins_over_inference: TestModeInferenceFromFilePath#test_explicit_mode_wins_over_inference().
  TestModeInferenceFromFilePath.test_mode_not_required_in_schema: TestModeInferenceFromFilePath#test_mode_not_required_in_schema().
  tool: tool().
  mock_graph: mock_graph().
  TestToolDefinition: TestToolDefinition#
  TestToolDefinition.test_name: TestToolDefinition#test_name().
  TestToolDefinition.test_schema_modes: TestToolDefinition#test_schema_modes().
  TestValidation: TestValidation#
  TestValidation.test_deps_requires_file_path: TestValidation#test_deps_requires_file_path().
  TestValidation.test_dependents_requires_file_path: TestValidation#test_dependents_requires_file_path().
  TestValidation.test_blast_radius_requires_file_path: TestValidation#test_blast_radius_requires_file_path().
  TestValidation.test_invalid_mode: TestValidation#test_invalid_mode().
  TestSummaryMode: TestSummaryMode#
  TestDepsMode: TestDepsMode#
  TestDepsMode.test_deps_with_results: TestDepsMode#test_deps_with_results().
  TestDepsMode.test_deps_no_results: TestDepsMode#test_deps_no_results().
  TestDependentsMode: TestDependentsMode#
  TestDependentsMode.test_dependents_with_results: TestDependentsMode#test_dependents_with_results().
  TestBlastRadiusMode: TestBlastRadiusMode#
  TestBlastRadiusMode.test_blast_radius_small: TestBlastRadiusMode#test_blast_radius_small().
  TestBlastRadiusMode.test_blast_radius_large: TestBlastRadiusMode#test_blast_radius_large().
  TestCyclesMode: TestCyclesMode#
  TestCouplingMode: TestCouplingMode#
  TestToonFormat: TestToonFormat#
  TestModeInferenceFromFilePath: TestModeInferenceFromFilePath#
---
# Module: [`tests/unit/test_import_graph_tool.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_graph_tool.py)

## Classes
### `TestBlastRadiusMode`
- def: [`tests/unit/test_import_graph_tool.py:126`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_graph_tool.py#L126)
- signature: `class TestBlastRadiusMode:`
- members:
  - `test_blast_radius_large(self, tool, mock_graph, tmp_path)` — [`L150`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_graph_tool.py#L150)
  - `test_blast_radius_small(self, tool, mock_graph, tmp_path)` — [`L128`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_graph_tool.py#L128)

### `TestCouplingMode`
- def: [`tests/unit/test_import_graph_tool.py:192`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_graph_tool.py#L192)
- signature: `class TestCouplingMode:`
- members:
  - `test_coupling(self, tool, mock_graph)` — [`L194`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_graph_tool.py#L194)
- uses (calls/refs, reference-scoped): [`edges`](../../tree_sitter_analyzer/import_graph.md#ImportGraphResult.edges), [`ImportGraphResult`](../../tree_sitter_analyzer/import_graph.md#ImportGraphResult), [`cycles`](../../tree_sitter_analyzer/import_graph.md#ImportGraphResult.cycles), [`edge_count`](../../tree_sitter_analyzer/import_graph.md#ImportGraphResult.edge_count), [`file_count`](../../tree_sitter_analyzer/import_graph.md#ImportGraphResult.file_count)

### `TestCyclesMode`
- def: [`tests/unit/test_import_graph_tool.py:166`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_graph_tool.py#L166)
- signature: `class TestCyclesMode:`
- members:
  - `test_no_cycles(self, tool, mock_graph)` — [`L168`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_graph_tool.py#L168)
  - `test_with_cycles(self, tool, mock_graph)` — [`L179`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_graph_tool.py#L179)
- uses (calls/refs, reference-scoped): [`edges`](../../tree_sitter_analyzer/import_graph.md#ImportGraphResult.edges), [`ImportGraphResult`](../../tree_sitter_analyzer/import_graph.md#ImportGraphResult), [`cycles`](../../tree_sitter_analyzer/import_graph.md#ImportGraphResult.cycles), [`edge_count`](../../tree_sitter_analyzer/import_graph.md#ImportGraphResult.edge_count), [`file_count`](../../tree_sitter_analyzer/import_graph.md#ImportGraphResult.file_count)

### `TestDependentsMode`
- def: [`tests/unit/test_import_graph_tool.py:110`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_graph_tool.py#L110)
- signature: `class TestDependentsMode:`
- members:
  - `test_dependents_with_results(self, tool, mock_graph, tmp_path)` — [`L112`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_graph_tool.py#L112)

### `TestDepsMode`
- def: [`tests/unit/test_import_graph_tool.py:86`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_graph_tool.py#L86)
- signature: `class TestDepsMode:`
- members:
  - `test_deps_no_results(self, tool, mock_graph, tmp_path)` — [`L101`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_graph_tool.py#L101)
  - `test_deps_with_results(self, tool, mock_graph, tmp_path)` — [`L88`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_graph_tool.py#L88)

### `TestModeInferenceFromFilePath`
- def: [`tests/unit/test_import_graph_tool.py:226`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_graph_tool.py#L226)
- doc: #575: `imports file_path=X` without mode= must infer 'deps' (what that
- signature: `class TestModeInferenceFromFilePath:`
- members:
  - `test_explicit_mode_wins_over_inference(self)` — [`L237`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_graph_tool.py#L237)
  - `test_file_path_infers_deps(self)` — [`L231`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_graph_tool.py#L231)
  - `test_mode_not_required_in_schema(self)` — [`L245`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_graph_tool.py#L245)
  - `test_no_file_path_is_summary(self)` — [`L234`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_graph_tool.py#L234)
- uses (calls/refs, reference-scoped): [`CodeGraphImportGraphTool`](../../tree_sitter_analyzer/mcp/tools/import_graph_tool.md#CodeGraphImportGraphTool), [`_effective_mode`](../../tree_sitter_analyzer/mcp/tools/import_graph_tool.md#CodeGraphImportGraphTool._effective_mode), [`get_tool_definition`](../../tree_sitter_analyzer/mcp/tools/import_graph_tool.md#CodeGraphImportGraphTool.get_tool_definition)

### `TestSummaryMode`
- def: [`tests/unit/test_import_graph_tool.py:63`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_graph_tool.py#L63)
- signature: `class TestSummaryMode:`
- members:
  - `test_summary_success(self, tool, mock_graph)` — [`L65`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_graph_tool.py#L65)
- uses (calls/refs, reference-scoped): [`edges`](../../tree_sitter_analyzer/import_graph.md#ImportGraphResult.edges), [`ImportGraphResult`](../../tree_sitter_analyzer/import_graph.md#ImportGraphResult), [`cycles`](../../tree_sitter_analyzer/import_graph.md#ImportGraphResult.cycles), [`edge_count`](../../tree_sitter_analyzer/import_graph.md#ImportGraphResult.edge_count), [`file_count`](../../tree_sitter_analyzer/import_graph.md#ImportGraphResult.file_count)

### `TestToolDefinition`
- def: [`tests/unit/test_import_graph_tool.py:25`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_graph_tool.py#L25)
- signature: `class TestToolDefinition:`
- members:
  - `test_name(self, tool)` — [`L26`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_graph_tool.py#L26)
  - `test_schema_modes(self, tool)` — [`L30`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_graph_tool.py#L30)

### `TestToonFormat`
- def: [`tests/unit/test_import_graph_tool.py:209`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_graph_tool.py#L209)
- signature: `class TestToonFormat:`
- members:
  - `test_toon_output(self, tool, mock_graph)` — [`L211`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_graph_tool.py#L211)
- uses (calls/refs, reference-scoped): [`edges`](../../tree_sitter_analyzer/import_graph.md#ImportGraphResult.edges), [`ImportGraphResult`](../../tree_sitter_analyzer/import_graph.md#ImportGraphResult), [`cycles`](../../tree_sitter_analyzer/import_graph.md#ImportGraphResult.cycles), [`edge_count`](../../tree_sitter_analyzer/import_graph.md#ImportGraphResult.edge_count), [`file_count`](../../tree_sitter_analyzer/import_graph.md#ImportGraphResult.file_count)

### `TestValidation`
- def: [`tests/unit/test_import_graph_tool.py:41`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_graph_tool.py#L41)
- signature: `class TestValidation:`
- members:
  - `test_blast_radius_requires_file_path(self, tool)` — [`L53`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_graph_tool.py#L53)
  - `test_dependents_requires_file_path(self, tool)` — [`L48`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_graph_tool.py#L48)
  - `test_deps_requires_file_path(self, tool)` — [`L43`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_graph_tool.py#L43)
  - `test_invalid_mode(self, tool)` — [`L58`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_graph_tool.py#L58)

## Functions
- `mock_graph()` — [`L19`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_graph_tool.py#L19)
- `tool(tmp_path)` — [`L14`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_graph_tool.py#L14)

