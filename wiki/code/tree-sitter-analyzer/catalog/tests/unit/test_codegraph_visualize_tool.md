---
title: 'Module: tests/unit/test_codegraph_visualize_tool.py'
type: catalog
provenance: extracted
module: tests/unit/test_codegraph_visualize_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_codegraph_visualize_tool`/
symbols:
  TestVisualizeToolNoProject.test_mocked_function_mode: TestVisualizeToolNoProject#test_mocked_function_mode().
  TestVisualizeToolNoProject.test_mocked_function_mode_sigma_payload: TestVisualizeToolNoProject#test_mocked_function_mode_sigma_payload().
  TestVisualizeToolNoProject.test_mocked_file_mode: TestVisualizeToolNoProject#test_mocked_file_mode().
  TestBug786TruncatedFlag.test_mocked_full_mode_truncated_flag: TestBug786TruncatedFlag#test_mocked_full_mode_truncated_flag().
  TestBug786TruncatedFlag.test_function_mode_no_truncation_flag_on_small_graph: TestBug786TruncatedFlag#test_function_mode_no_truncation_flag_on_small_graph().
  tiny_call_project: tiny_call_project().
  TestVisualizeToolNoProject.test_mocked_full_mode: TestVisualizeToolNoProject#test_mocked_full_mode().
  _PROJECT_ROOT: _PROJECT_ROOT.
  TestVisualizeToolSchema.test_tool_definition_has_name: TestVisualizeToolSchema#test_tool_definition_has_name().
  TestVisualizeToolSchema.test_schema_modes: TestVisualizeToolSchema#test_schema_modes().
  TestVisualizeToolSchema.test_schema_visualization_formats: TestVisualizeToolSchema#test_schema_visualization_formats().
  TestVisualizeToolSchema.test_validate_file_mode_requires_path: TestVisualizeToolSchema#test_validate_file_mode_requires_path().
  TestVisualizeToolSchema.test_validate_function_mode_requires_name: TestVisualizeToolSchema#test_validate_function_mode_requires_name().
  TestVisualizeToolSchema.test_validate_full_mode_ok: TestVisualizeToolSchema#test_validate_full_mode_ok().
  TestVisualizeToolSchema.test_validate_bad_max_edges: TestVisualizeToolSchema#test_validate_bad_max_edges().
  TestVisualizeToolSchema.test_validate_bad_depth: TestVisualizeToolSchema#test_validate_bad_depth().
  TestVisualizeToolSchema.test_validate_bad_visualization_format: TestVisualizeToolSchema#test_validate_bad_visualization_format().
  TestVisualizeToolNoProject.test_no_project_root: TestVisualizeToolNoProject#test_no_project_root().
  TestVisualizeIndexedProject.test_full_mode_on_indexed_project: TestVisualizeIndexedProject#test_full_mode_on_indexed_project().
  TestVisualizeIndexedProject.test_full_mode_stops_at_edge_limit: TestVisualizeIndexedProject#test_full_mode_stops_at_edge_limit().
  TestVisualizeIndexedProject.test_function_mode_on_indexed_project: TestVisualizeIndexedProject#test_function_mode_on_indexed_project().
  TestBug786TruncatedFlag.test_full_mode_truncated_flag_set_when_cap_hit: TestBug786TruncatedFlag#test_full_mode_truncated_flag_set_when_cap_hit().
  TestBug786TruncatedFlag.test_full_mode_no_truncated_flag_when_all_edges_fit: TestBug786TruncatedFlag#test_full_mode_no_truncated_flag_when_all_edges_fit().
  TestMermaidRenderer.test_empty_edges: TestMermaidRenderer#test_empty_edges().
  TestMermaidRenderer.test_single_edge: TestMermaidRenderer#test_single_edge().
  TestMermaidRenderer.test_direction_lr: TestMermaidRenderer#test_direction_lr().
  TestMermaidRenderer.test_deduplication: TestMermaidRenderer#test_deduplication().
  TestMermaidRenderer.test_node_label_escaping: TestMermaidRenderer#test_node_label_escaping().
  TestSafeNodeId.test_simple: TestSafeNodeId#test_simple().
  TestSafeNodeId.test_special_chars: TestSafeNodeId#test_special_chars().
  TestSafeNodeId.test_consistent: TestSafeNodeId#test_consistent().
  TestShortLabel.test_basename: TestShortLabel#test_basename().
  TestShortLabel.test_nested: TestShortLabel#test_nested().
  TestMermaidRenderer: TestMermaidRenderer#
  TestSafeNodeId: TestSafeNodeId#
  TestShortLabel: TestShortLabel#
  TestVisualizeToolSchema: TestVisualizeToolSchema#
  TestVisualizeToolNoProject: TestVisualizeToolNoProject#
  TestVisualizeIndexedProject: TestVisualizeIndexedProject#
  TestBug786TruncatedFlag: TestBug786TruncatedFlag#
---
# Module: [`tests/unit/test_codegraph_visualize_tool.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_visualize_tool.py)

## Classes
### `TestBug786TruncatedFlag`
- def: [`tests/unit/test_codegraph_visualize_tool.py:346`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_visualize_tool.py#L346)
- doc: Bug #786: when edge collection is capped at max_edges, the response
- signature: `class TestBug786TruncatedFlag:`
- members:
  - `test_full_mode_no_truncated_flag_when_all_edges_fit(self, tiny_call_project: str)` — [`L375`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_visualize_tool.py#L375) — When max_edges is large enough to hold the whole graph, truncated
  - `test_full_mode_truncated_flag_set_when_cap_hit(self, tiny_call_project: str)` — [`L356`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_visualize_tool.py#L356) — Requesting max_edges=1 on a project with more than 1 edge must
  - `test_function_mode_no_truncation_flag_on_small_graph(self)` — [`L417`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_visualize_tool.py#L417) — mode=function on a small graph (fewer edges than max_edges) must
  - `test_mocked_full_mode_truncated_flag(self)` — [`L392`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_visualize_tool.py#L392) — Mock-based test so we can force exactly max_edges edges out of a
- uses (calls/refs, reference-scoped): [`FunctionRef`](../../tree_sitter_analyzer/call_graph.md#FunctionRef), [`execute`](../../tree_sitter_analyzer/mcp/tools/codegraph_visualize_tool.md#CodeGraphVisualizeTool.execute), [`CodeGraphVisualizeTool`](../../tree_sitter_analyzer/mcp/tools/codegraph_visualize_tool.md#CodeGraphVisualizeTool)  (1 test-only)

### `TestMermaidRenderer`
- def: [`tests/unit/test_codegraph_visualize_tool.py:46`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_visualize_tool.py#L46)
- signature: `class TestMermaidRenderer:`
- members:
  - `test_deduplication(self)` — [`L65`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_visualize_tool.py#L65)
  - `test_direction_lr(self)` — [`L60`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_visualize_tool.py#L60)
  - `test_empty_edges(self)` — [`L47`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_visualize_tool.py#L47)
  - `test_node_label_escaping(self)` — [`L73`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_visualize_tool.py#L73)
  - `test_single_edge(self)` — [`L52`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_visualize_tool.py#L52)
- uses (calls/refs, reference-scoped): [`render_call_flowchart`](../../tree_sitter_analyzer/mcp/tools/codegraph_visualization_hub.md#render_call_flowchart)

### `TestSafeNodeId`
- def: [`tests/unit/test_codegraph_visualize_tool.py:79`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_visualize_tool.py#L79)
- signature: `class TestSafeNodeId:`
- members:
  - `test_consistent(self)` — [`L87`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_visualize_tool.py#L87)
  - `test_simple(self)` — [`L80`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_visualize_tool.py#L80)
  - `test_special_chars(self)` — [`L83`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_visualize_tool.py#L83)
- uses (calls/refs, reference-scoped): [`safe_node_id`](../../tree_sitter_analyzer/mcp/tools/codegraph_visualization_hub.md#safe_node_id)

### `TestShortLabel`
- def: [`tests/unit/test_codegraph_visualize_tool.py:93`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_visualize_tool.py#L93)
- signature: `class TestShortLabel:`
- members:
  - `test_basename(self)` — [`L94`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_visualize_tool.py#L94)
  - `test_nested(self)` — [`L97`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_visualize_tool.py#L97)
- uses (calls/refs, reference-scoped): [`short_label`](../../tree_sitter_analyzer/mcp/tools/codegraph_visualization_hub.md#short_label)

### `TestVisualizeIndexedProject`
- def: [`tests/unit/test_codegraph_visualize_tool.py:298`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_visualize_tool.py#L298)
- signature: `class TestVisualizeIndexedProject:`
- members:
  - `test_full_mode_on_indexed_project(self, tiny_call_project: str)` — [`L300`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_visualize_tool.py#L300)
  - `test_full_mode_stops_at_edge_limit(self, tiny_call_project: str)` — [`L315`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_visualize_tool.py#L315)
  - `test_function_mode_on_indexed_project(self, tiny_call_project: str)` — [`L328`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_visualize_tool.py#L328)
- uses (calls/refs, reference-scoped): [`execute`](../../tree_sitter_analyzer/mcp/tools/codegraph_visualize_tool.md#CodeGraphVisualizeTool.execute), [`CodeGraphVisualizeTool`](../../tree_sitter_analyzer/mcp/tools/codegraph_visualize_tool.md#CodeGraphVisualizeTool)

### `TestVisualizeToolNoProject`
- def: [`tests/unit/test_codegraph_visualize_tool.py:158`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_visualize_tool.py#L158)
- signature: `class TestVisualizeToolNoProject:`
- members:
  - `test_mocked_file_mode(self)` — [`L273`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_visualize_tool.py#L273)
  - `test_mocked_full_mode(self)` — [`L167`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_visualize_tool.py#L167)
  - `test_mocked_function_mode(self)` — [`L182`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_visualize_tool.py#L182)
  - `test_mocked_function_mode_sigma_payload(self)` — [`L209`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_visualize_tool.py#L209)
  - `test_no_project_root(self)` — [`L160`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_visualize_tool.py#L160)
- uses (calls/refs, reference-scoped): [`FunctionRef`](../../tree_sitter_analyzer/call_graph.md#FunctionRef), [`execute`](../../tree_sitter_analyzer/mcp/tools/codegraph_visualize_tool.md#CodeGraphVisualizeTool.execute), [`CodeGraphVisualizeTool`](../../tree_sitter_analyzer/mcp/tools/codegraph_visualize_tool.md#CodeGraphVisualizeTool)  (1 test-only)

### `TestVisualizeToolSchema`
- def: [`tests/unit/test_codegraph_visualize_tool.py:101`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_visualize_tool.py#L101)
- signature: `class TestVisualizeToolSchema:`
- members:
  - `test_schema_modes(self)` — [`L108`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_visualize_tool.py#L108)
  - `test_schema_visualization_formats(self)` — [`L116`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_visualize_tool.py#L116)
  - `test_tool_definition_has_name(self)` — [`L102`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_visualize_tool.py#L102)
  - `test_validate_bad_depth(self)` — [`L143`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_visualize_tool.py#L143)
  - `test_validate_bad_max_edges(self)` — [`L138`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_visualize_tool.py#L138)
  - `test_validate_bad_visualization_format(self)` — [`L150`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_visualize_tool.py#L150)
  - `test_validate_file_mode_requires_path(self)` — [`L124`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_visualize_tool.py#L124)
  - `test_validate_full_mode_ok(self)` — [`L134`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_visualize_tool.py#L134)
  - `test_validate_function_mode_requires_name(self)` — [`L129`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_visualize_tool.py#L129)
- uses (calls/refs, reference-scoped): [`CodeGraphVisualizeTool`](../../tree_sitter_analyzer/mcp/tools/codegraph_visualize_tool.md#CodeGraphVisualizeTool), [`validate_arguments`](../../tree_sitter_analyzer/mcp/tools/codegraph_visualize_tool.md#CodeGraphVisualizeTool.validate_arguments), [`get_tool_schema`](../../tree_sitter_analyzer/mcp/tools/codegraph_visualize_tool.md#CodeGraphVisualizeTool.get_tool_schema), [`get_tool_definition`](../../tree_sitter_analyzer/mcp/tools/codegraph_visualize_tool.md#CodeGraphVisualizeTool.get_tool_definition)

## Functions
- `tiny_call_project(tmp_path: Path)` — [`L21`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_visualize_tool.py#L21)

## Module values
- `_PROJECT_ROOT` — [`L17`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_visualize_tool.py#L17)

