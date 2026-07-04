---
title: 'Module: tests/unit/test_tool_registry.py'
type: catalog
provenance: extracted
module: tests/unit/test_tool_registry.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_tool_registry`/TestCreateToolRegistry#
symbols:
  TestCreateToolRegistry.test_returns_tools_and_dict: test_returns_tools_and_dict().
  TestCreateToolRegistry.test_tool_names_are_strings: test_tool_names_are_strings().
  TestCreateToolRegistry.test_dict_keys_match_tool_names: test_dict_keys_match_tool_names().
  TestCreateToolRegistry.test_expected_tool_count: test_expected_tool_count().
  TestCreateToolRegistry.test_specific_tools_present: test_specific_tools_present().
  TestCreateToolRegistry.test_tool_instances_have_execute: test_tool_instances_have_execute().
  TestCreateToolRegistry.test_project_root_passed_through: test_project_root_passed_through().
  TestCreateToolRegistry: ''
---
# Module: [`tests/unit/test_tool_registry.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_tool_registry.py)

## Classes
### `TestCreateToolRegistry`
- def: [`tests/unit/test_tool_registry.py:8`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_tool_registry.py#L8)
- signature: `class TestCreateToolRegistry:`
- members:
  - `test_dict_keys_match_tool_names(self)` — [`L21`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_tool_registry.py#L21)
  - `test_expected_tool_count(self)` — [`L26`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_tool_registry.py#L26)
  - `test_project_root_passed_through(self, tmp_path)` — [`L53`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_tool_registry.py#L53)
  - `test_returns_tools_and_dict(self)` — [`L9`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_tool_registry.py#L9)
  - `test_specific_tools_present(self)` — [`L31`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_tool_registry.py#L31)
  - `test_tool_instances_have_execute(self)` — [`L48`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_tool_registry.py#L48)
  - `test_tool_names_are_strings(self)` — [`L15`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_tool_registry.py#L15)
- uses (calls/refs, reference-scoped): [`create_tool_registry`](../../tree_sitter_analyzer/mcp/_tool_registry.md#create_tool_registry)

