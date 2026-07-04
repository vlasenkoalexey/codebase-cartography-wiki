---
title: 'Module: tests/unit/test_codegraph_exclusive_tools.py'
type: catalog
provenance: extracted
module: tests/unit/test_codegraph_exclusive_tools.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_codegraph_exclusive_tools`/
symbols:
  TestDeadCodeToolExecute.test_issues_branch_next_step_has_count_and_guard: TestDeadCodeToolExecute#test_issues_branch_next_step_has_count_and_guard().
  TestDeadCodeToolExecute.test_no_issues_branch_next_step: TestDeadCodeToolExecute#test_no_issues_branch_next_step().
  TestDeadCodeToolDefinition.test_tool_name: TestDeadCodeToolDefinition#test_tool_name().
  TestDeadCodeToolDefinition.test_schema_mode_enum: TestDeadCodeToolDefinition#test_schema_mode_enum().
  TestDeadCodeToolDefinition.test_toon_default: TestDeadCodeToolDefinition#test_toon_default().
  TestDeadCodeToolExecute.test_runs_on_project: TestDeadCodeToolExecute#test_runs_on_project().
  TestDeadCodeToolExecute.test_toon_format_default: TestDeadCodeToolExecute#test_toon_format_default().
  TestDeadCodeToolExecute.test_emits_actionable_next_step: TestDeadCodeToolExecute#test_emits_actionable_next_step().
  TestDependencyMatrixToolDefinition.test_tool_name: TestDependencyMatrixToolDefinition#test_tool_name().
  TestDependencyMatrixToolDefinition.test_schema_mode_enum: TestDependencyMatrixToolDefinition#test_schema_mode_enum().
  TestDependencyMatrixToolDefinition.test_toon_default: TestDependencyMatrixToolDefinition#test_toon_default().
  TestDependencyMatrixToolExecute.test_runs_on_project: TestDependencyMatrixToolExecute#test_runs_on_project().
  TestDependencyMatrixToolExecute.test_toon_format_default: TestDependencyMatrixToolExecute#test_toon_format_default().
  TestComplexityHeatmapToolDefinition.test_tool_name: TestComplexityHeatmapToolDefinition#test_tool_name().
  TestComplexityHeatmapToolDefinition.test_toon_default: TestComplexityHeatmapToolDefinition#test_toon_default().
  TestComplexityHeatmapToolExecute.test_runs_on_project: TestComplexityHeatmapToolExecute#test_runs_on_project().
  TestComplexityHeatmapToolExecute.test_toon_format_default: TestComplexityHeatmapToolExecute#test_toon_format_default().
  project: project().
  TestDeadCodeToolDefinition: TestDeadCodeToolDefinition#
  TestDeadCodeToolExecute: TestDeadCodeToolExecute#
  TestDependencyMatrixToolDefinition: TestDependencyMatrixToolDefinition#
  TestDependencyMatrixToolExecute: TestDependencyMatrixToolExecute#
  TestComplexityHeatmapToolDefinition: TestComplexityHeatmapToolDefinition#
  TestComplexityHeatmapToolExecute: TestComplexityHeatmapToolExecute#
---
# Module: [`tests/unit/test_codegraph_exclusive_tools.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_exclusive_tools.py)

## Classes
### `TestComplexityHeatmapToolDefinition`
- def: [`tests/unit/test_codegraph_exclusive_tools.py:154`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_exclusive_tools.py#L154)
- signature: `class TestComplexityHeatmapToolDefinition:`
- members:
  - `test_tool_name(self)` — [`L155`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_exclusive_tools.py#L155)
  - `test_toon_default(self)` — [`L161`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_exclusive_tools.py#L161)
- uses (calls/refs, reference-scoped): [`CodeGraphComplexityHeatmapTool`](../../tree_sitter_analyzer/mcp/tools/complexity_heatmap_tool.md#CodeGraphComplexityHeatmapTool), [`get_tool_definition`](../../tree_sitter_analyzer/mcp/tools/complexity_heatmap_tool.md#CodeGraphComplexityHeatmapTool.get_tool_definition), [`get_tool_schema`](../../tree_sitter_analyzer/mcp/tools/complexity_heatmap_tool.md#CodeGraphComplexityHeatmapTool.get_tool_schema)

### `TestComplexityHeatmapToolExecute`
- def: [`tests/unit/test_codegraph_exclusive_tools.py:167`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_exclusive_tools.py#L167)
- signature: `class TestComplexityHeatmapToolExecute:`
- members:
  - `test_runs_on_project(self, project)` — [`L168`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_exclusive_tools.py#L168)
  - `test_toon_format_default(self, project)` — [`L173`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_exclusive_tools.py#L173)
- uses (calls/refs, reference-scoped): [`execute`](../../tree_sitter_analyzer/mcp/tools/complexity_heatmap_tool.md#CodeGraphComplexityHeatmapTool.execute), [`CodeGraphComplexityHeatmapTool`](../../tree_sitter_analyzer/mcp/tools/complexity_heatmap_tool.md#CodeGraphComplexityHeatmapTool)

### `TestDeadCodeToolDefinition`
- def: [`tests/unit/test_codegraph_exclusive_tools.py:31`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_exclusive_tools.py#L31)
- signature: `class TestDeadCodeToolDefinition:`
- members:
  - `test_schema_mode_enum(self)` — [`L35`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_exclusive_tools.py#L35)
  - `test_tool_name(self)` — [`L32`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_exclusive_tools.py#L32)
  - `test_toon_default(self)` — [`L40`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_exclusive_tools.py#L40)
- uses (calls/refs, reference-scoped): [`CodeGraphDeadCodeTool`](../../tree_sitter_analyzer/mcp/tools/dead_code_tool.md#CodeGraphDeadCodeTool), [`get_tool_definition`](../../tree_sitter_analyzer/mcp/tools/dead_code_tool.md#CodeGraphDeadCodeTool.get_tool_definition), [`get_tool_schema`](../../tree_sitter_analyzer/mcp/tools/dead_code_tool.md#CodeGraphDeadCodeTool.get_tool_schema)

### `TestDeadCodeToolExecute`
- def: [`tests/unit/test_codegraph_exclusive_tools.py:46`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_exclusive_tools.py#L46)
- signature: `class TestDeadCodeToolExecute:`
- members:
  - `test_emits_actionable_next_step(self, project)` — [`L58`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_exclusive_tools.py#L58)
  - `test_issues_branch_next_step_has_count_and_guard(self, project, monkeypatch)` — [`L66`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_exclusive_tools.py#L66)
  - `test_no_issues_branch_next_step(self, project, monkeypatch)` — [`L94`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_exclusive_tools.py#L94)
  - `test_runs_on_project(self, project)` — [`L47`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_exclusive_tools.py#L47)
  - `test_toon_format_default(self, project)` — [`L52`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_exclusive_tools.py#L52)
- uses (calls/refs, reference-scoped): [`execute`](../../tree_sitter_analyzer/mcp/tools/dead_code_tool.md#CodeGraphDeadCodeTool.execute), [`CodeGraphDeadCodeTool`](../../tree_sitter_analyzer/mcp/tools/dead_code_tool.md#CodeGraphDeadCodeTool), [`dead_functions`](../../tree_sitter_analyzer/dead_code_analyzer.md#DeadCodeResult.dead_functions), [`DeadCodeResult`](../../tree_sitter_analyzer/dead_code_analyzer.md#DeadCodeResult), [`stats`](../../tree_sitter_analyzer/dead_code_analyzer.md#DeadCodeResult.stats), [`unreferenced_variables`](../../tree_sitter_analyzer/dead_code_analyzer.md#DeadCodeResult.unreferenced_variables), [`unused_imports`](../../tree_sitter_analyzer/dead_code_analyzer.md#DeadCodeResult.unused_imports), [`UnusedImport`](../../tree_sitter_analyzer/dead_code_analyzer.md#UnusedImport), [`file`](../../tree_sitter_analyzer/dead_code_analyzer.md#UnusedImport.file), [`line`](../../tree_sitter_analyzer/dead_code_analyzer.md#UnusedImport.line), [`unused_names`](../../tree_sitter_analyzer/dead_code_analyzer.md#UnusedImport.unused_names), [`import_text`](../../tree_sitter_analyzer/dead_code_analyzer.md#UnusedImport.import_text)

### `TestDependencyMatrixToolDefinition`
- def: [`tests/unit/test_codegraph_exclusive_tools.py:118`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_exclusive_tools.py#L118)
- signature: `class TestDependencyMatrixToolDefinition:`
- members:
  - `test_schema_mode_enum(self)` — [`L125`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_exclusive_tools.py#L125)
  - `test_tool_name(self)` — [`L119`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_exclusive_tools.py#L119)
  - `test_toon_default(self)` — [`L130`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_exclusive_tools.py#L130)
- uses (calls/refs, reference-scoped): [`CodeGraphDependencyMatrixTool`](../../tree_sitter_analyzer/mcp/tools/dependency_matrix_tool.md#CodeGraphDependencyMatrixTool), [`get_tool_definition`](../../tree_sitter_analyzer/mcp/tools/dependency_matrix_tool.md#CodeGraphDependencyMatrixTool.get_tool_definition), [`get_tool_schema`](../../tree_sitter_analyzer/mcp/tools/dependency_matrix_tool.md#CodeGraphDependencyMatrixTool.get_tool_schema)

### `TestDependencyMatrixToolExecute`
- def: [`tests/unit/test_codegraph_exclusive_tools.py:136`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_exclusive_tools.py#L136)
- signature: `class TestDependencyMatrixToolExecute:`
- members:
  - `test_runs_on_project(self, project)` — [`L137`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_exclusive_tools.py#L137)
  - `test_toon_format_default(self, project)` — [`L142`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_exclusive_tools.py#L142)
- uses (calls/refs, reference-scoped): [`execute`](../../tree_sitter_analyzer/mcp/tools/dependency_matrix_tool.md#CodeGraphDependencyMatrixTool.execute), [`CodeGraphDependencyMatrixTool`](../../tree_sitter_analyzer/mcp/tools/dependency_matrix_tool.md#CodeGraphDependencyMatrixTool)

## Functions
- `project(tmp_path)` — [`L19`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_exclusive_tools.py#L19)

