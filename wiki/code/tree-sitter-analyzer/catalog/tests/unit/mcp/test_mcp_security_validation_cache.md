---
title: 'Module: tests/unit/mcp/test_mcp_security_validation_cache.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_mcp_security_validation_cache.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_mcp_security_validation_cache`/
symbols:
  test_security_validation_is_cached_within_same_project_root: test_security_validation_is_cached_within_same_project_root().
  test_cache_is_invalidated_on_project_root_change: test_cache_is_invalidated_on_project_root_change().
  _DummyFileTool.execute: _DummyFileTool#execute().
  _DummyFileTool: _DummyFileTool#
  _DummyFileTool.get_tool_definition: _DummyFileTool#get_tool_definition().
  _DummyFileTool.get_tool_schema: _DummyFileTool#get_tool_schema().
  _DummyFileTool.validate_arguments: _DummyFileTool#validate_arguments().
  test_security_validation_is_cached_within_same_project_root._validate_spy: test_security_validation_is_cached_within_same_project_root()._validate_spy().
  test_security_validation_is_cached_within_same_project_root._resolve_spy: test_security_validation_is_cached_within_same_project_root()._resolve_spy().
  test_cache_is_invalidated_on_project_root_change._validate_spy: test_cache_is_invalidated_on_project_root_change()._validate_spy().
---
# Module: [`tests/unit/mcp/test_mcp_security_validation_cache.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_security_validation_cache.py)

## Classes
### `_DummyFileTool`  ·  implements/extends BaseMCPTool
- def: [`tests/unit/mcp/test_mcp_security_validation_cache.py:9`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_security_validation_cache.py#L9)
- signature: `class _DummyFileTool(BaseMCPTool):`
- members:
  - `execute(self, arguments)` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_security_validation_cache.py#L20)
  - `get_tool_definition(self)` — [`L13`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_security_validation_cache.py#L13)
  - `get_tool_schema(self)` — [`L10`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_security_validation_cache.py#L10)
  - `validate_arguments(self, arguments)` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_security_validation_cache.py#L25)
- uses (calls/refs, reference-scoped): [`BaseMCPTool`](../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool), [`resolve_and_validate_file_path`](../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.resolve_and_validate_file_path)
- used by: [`BaseMCPTool`](../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool), [`execute`](../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.validate_arguments)  (2 test-only)

## Functions
- `_resolve_spy(self, file_path)` — [`L54`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_security_validation_cache.py#L54)
- `_validate_spy(self, file_path, base_path=None)` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_security_validation_cache.py#L49)
- `_validate_spy(self, file_path, base_path=None)` — [`L91`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_security_validation_cache.py#L91)
- `test_cache_is_invalidated_on_project_root_change(tmp_path, monkeypatch)` — [`L76`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_security_validation_cache.py#L76) — documented in [tree_sitter_analyzer-security-validator](../../../../concepts/tree_sitter_analyzer-security-validator.md)
- `test_security_validation_is_cached_within_same_project_root(tmp_path, monkeypatch)` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_security_validation_cache.py#L33) — documented in [tree_sitter_analyzer-security-validator](../../../../concepts/tree_sitter_analyzer-security-validator.md)

