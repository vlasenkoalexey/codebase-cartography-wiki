---
title: 'Module: tests/unit/test_call_tree_primitives.py'
type: catalog
provenance: extracted
module: tests/unit/test_call_tree_primitives.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_call_tree_primitives`/
symbols:
  _graph_expander: _graph_expander().
  TestBuildCallTree.test_direct_children_appear_at_level_one: TestBuildCallTree#test_direct_children_appear_at_level_one().
  TestBuildCallTree.test_transitive_children_appear_at_depth_two: TestBuildCallTree#test_transitive_children_appear_at_depth_two().
  TestBuildCallTree.test_max_depth_limits_traversal: TestBuildCallTree#test_max_depth_limits_traversal().
  TestBuildCallTree.test_cycle_produces_leaf_not_infinite_recursion: TestBuildCallTree#test_cycle_produces_leaf_not_infinite_recursion().
  TestBuildCallTree.test_node_cap_truncates_and_flags: TestBuildCallTree#test_node_cap_truncates_and_flags().
  TestBuildCallTree.test_no_truncation_flag_when_under_cap: TestBuildCallTree#test_no_truncation_flag_when_under_cap().
  TestBuildCallTree.test_node_shape_has_name_file_line_children: TestBuildCallTree#test_node_shape_has_name_file_line_children().
  TestCalleeTreeTool.test_returns_nested_tree_one_call: TestCalleeTreeTool#test_returns_nested_tree_one_call().
  TestCalleeTreeTool.test_deterrent_next_step: TestCalleeTreeTool#test_deterrent_next_step().
  TestCalleeTreeTool.test_symbol_required: TestCalleeTreeTool#test_symbol_required().
  TestCalleeTreeTool.test_toon_format: TestCalleeTreeTool#test_toon_format().
  TestCalleeTreeTool.test_no_project_root_raises: TestCalleeTreeTool#test_no_project_root_raises().
  TestCallerTreeTool.test_returns_nested_caller_tree: TestCallerTreeTool#test_returns_nested_caller_tree().
  TestCallerTreeTool.test_symbol_required: TestCallerTreeTool#test_symbol_required().
  TestNavFacadeTreeActions.test_callee_tree_action: TestNavFacadeTreeActions#test_callee_tree_action().
  TestNavFacadeTreeActions.test_caller_tree_action: TestNavFacadeTreeActions#test_caller_tree_action().
  TestNavFacadeTreeActions.test_facade_exposes_tree_actions_in_enum: TestNavFacadeTreeActions#test_facade_exposes_tree_actions_in_enum().
  _graph_expander.expand: _graph_expander().expand().
  _PROJECT_ROOT: _PROJECT_ROOT.
  TestBuildCallTree: TestBuildCallTree#
  chain_project_root: chain_project_root().
  TestCalleeTreeTool: TestCalleeTreeTool#
  TestCallerTreeTool: TestCallerTreeTool#
  TestNavFacadeTreeActions: TestNavFacadeTreeActions#
---
# Module: [`tests/unit/test_call_tree_primitives.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_tree_primitives.py)

## Classes
### `TestBuildCallTree`
- def: [`tests/unit/test_call_tree_primitives.py:38`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_tree_primitives.py#L38)
- signature: `class TestBuildCallTree:`
- members:
  - `test_cycle_produces_leaf_not_infinite_recursion(self)` — [`L74`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_tree_primitives.py#L74)
  - `test_direct_children_appear_at_level_one(self)` — [`L39`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_tree_primitives.py#L39)
  - `test_max_depth_limits_traversal(self)` — [`L62`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_tree_primitives.py#L62)
  - `test_no_truncation_flag_when_under_cap(self)` — [`L97`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_tree_primitives.py#L97)
  - `test_node_cap_truncates_and_flags(self)` — [`L87`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_tree_primitives.py#L87)
  - `test_node_shape_has_name_file_line_children(self)` — [`L104`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_tree_primitives.py#L104)
  - `test_transitive_children_appear_at_depth_two(self)` — [`L52`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_tree_primitives.py#L52)
- uses (calls/refs, reference-scoped): [`build_call_tree`](../../tree_sitter_analyzer/mcp/tools/_call_tree.md#build_call_tree)  (1 test-only)

### `TestCalleeTreeTool`
- def: [`tests/unit/test_call_tree_primitives.py:126`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_tree_primitives.py#L126)
- signature: `class TestCalleeTreeTool:`
- members:
  - `test_deterrent_next_step(self, chain_project_root)` — [`L148`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_tree_primitives.py#L148)
  - `test_no_project_root_raises(self)` — [`L182`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_tree_primitives.py#L182)
  - `test_returns_nested_tree_one_call(self, chain_project_root)` — [`L128`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_tree_primitives.py#L128)
  - `test_symbol_required(self, chain_project_root)` — [`L162`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_tree_primitives.py#L162)
  - `test_toon_format(self, chain_project_root)` — [`L172`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_tree_primitives.py#L172)
- uses (calls/refs, reference-scoped): [`execute`](../../tree_sitter_analyzer/mcp/tools/_call_tree_tool.md#_CallTreeBase.execute), [`CodeGraphCalleeTreeTool`](../../tree_sitter_analyzer/mcp/tools/_call_tree_tool.md#CodeGraphCalleeTreeTool), [`validate_arguments`](../../tree_sitter_analyzer/mcp/tools/_call_tree_tool.md#_CallTreeBase.validate_arguments)

### `TestCallerTreeTool`
- def: [`tests/unit/test_call_tree_primitives.py:192`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_tree_primitives.py#L192)
- signature: `class TestCallerTreeTool:`
- members:
  - `test_returns_nested_caller_tree(self, chain_project_root)` — [`L194`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_tree_primitives.py#L194)
  - `test_symbol_required(self, chain_project_root)` — [`L214`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_tree_primitives.py#L214)
- uses (calls/refs, reference-scoped): [`execute`](../../tree_sitter_analyzer/mcp/tools/_call_tree_tool.md#_CallTreeBase.execute), [`CodeGraphCallerTreeTool`](../../tree_sitter_analyzer/mcp/tools/_call_tree_tool.md#CodeGraphCallerTreeTool), [`validate_arguments`](../../tree_sitter_analyzer/mcp/tools/_call_tree_tool.md#_CallTreeBase.validate_arguments)

### `TestNavFacadeTreeActions`
- def: [`tests/unit/test_call_tree_primitives.py:224`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_tree_primitives.py#L224)
- signature: `class TestNavFacadeTreeActions:`
- members:
  - `test_callee_tree_action(self, chain_project_root)` — [`L226`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_tree_primitives.py#L226)
  - `test_caller_tree_action(self, chain_project_root)` — [`L241`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_tree_primitives.py#L241)
  - `test_facade_exposes_tree_actions_in_enum(self, chain_project_root)` — [`L255`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_tree_primitives.py#L255)
- uses (calls/refs, reference-scoped): [`execute`](../../tree_sitter_analyzer/mcp/tools/facade_tool.md#FacadeTool.execute), [`build_nav_facade`](../../tree_sitter_analyzer/mcp/tools/nav_facade.md#build_nav_facade), [`get_tool_definition`](../../tree_sitter_analyzer/mcp/tools/facade_tool.md#FacadeTool.get_tool_definition)

## Functions
- `_graph_expander(graph: dict[str, list[dict]])` — [`L29`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_tree_primitives.py#L29) — Return an expand(name, file) callback backed by an in-memory dict.
- `chain_project_root(tmp_path)` — [`L117`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_tree_primitives.py#L117) — foo -> bar -> baz chain so the tree has real depth.
- `expand(name: str, _file: str | None)` — [`L32`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_tree_primitives.py#L32)

## Module values
- `_PROJECT_ROOT` — [`L21`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_tree_primitives.py#L21)

