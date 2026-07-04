---
title: 'Module: tests/unit/test_codegraph_autoindex_tool.py'
type: catalog
provenance: extracted
module: tests/unit/test_codegraph_autoindex_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_codegraph_autoindex_tool`/
symbols:
  TestExecute.test_status_indexed_matches_actual_row_count: TestExecute#test_status_indexed_matches_actual_row_count().
  warm_cache_root: warm_cache_root().
  TestExecute.test_status_warm_cache_reports_indexed_true: TestExecute#test_status_warm_cache_reports_indexed_true().
  TestExecute.test_status_built_marker_distinct_from_indexed: TestExecute#test_status_built_marker_distinct_from_indexed().
  tool: tool().
  tool_with_root: tool_with_root().
  TestToolDefinition: TestToolDefinition#
  TestToolDefinition.test_tool_name: TestToolDefinition#test_tool_name().
  TestToolDefinition.test_schema_mode_enum: TestToolDefinition#test_schema_mode_enum().
  TestToolDefinition.test_schema_output_format_default_toon: TestToolDefinition#test_schema_output_format_default_toon().
  TestToolDefinition.test_annotations_not_readonly: TestToolDefinition#test_annotations_not_readonly().
  TestValidation: TestValidation#
  TestValidation.test_valid_status: TestValidation#test_valid_status().
  TestValidation.test_valid_warm: TestValidation#test_valid_warm().
  TestValidation.test_valid_reset: TestValidation#test_valid_reset().
  TestValidation.test_invalid_mode_rejected: TestValidation#test_invalid_mode_rejected().
  TestExecute: TestExecute#
  TestExecute.test_status_no_project_root_returns_warn: TestExecute#test_status_no_project_root_returns_warn().
  TestExecute.test_status_empty_project_returns_info: TestExecute#test_status_empty_project_returns_info().
  TestExecute.test_toon_format_default: TestExecute#test_toon_format_default().
  TestExecute.test_reset_mode_runs_without_error: TestExecute#test_reset_mode_runs_without_error().
  TestExecute.test_warm_mode_returns_indexed_true: TestExecute#test_warm_mode_returns_indexed_true().
  TestExecute.test_status_empty_cache_reports_indexed_false: TestExecute#test_status_empty_cache_reports_indexed_false().
---
# Module: [`tests/unit/test_codegraph_autoindex_tool.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_autoindex_tool.py)

## Classes
### `TestExecute`
- def: [`tests/unit/test_codegraph_autoindex_tool.py:80`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_autoindex_tool.py#L80)
- signature: `class TestExecute:`
- members:
  - `test_reset_mode_runs_without_error(self, tool_with_root)` — [`L98`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_autoindex_tool.py#L98)
  - `test_status_built_marker_distinct_from_indexed(self, warm_cache_root)` — [`L136`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_autoindex_tool.py#L136)
  - `test_status_empty_cache_reports_indexed_false(self, tool_with_root)` — [`L146`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_autoindex_tool.py#L146)
  - `test_status_empty_project_returns_info(self, tool_with_root)` — [`L86`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_autoindex_tool.py#L86)
  - `test_status_indexed_matches_actual_row_count(self, warm_cache_root)` — [`L124`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_autoindex_tool.py#L124)
  - `test_status_no_project_root_returns_warn(self, tool)` — [`L81`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_autoindex_tool.py#L81)
  - `test_status_warm_cache_reports_indexed_true(self, warm_cache_root)` — [`L114`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_autoindex_tool.py#L114)
  - `test_toon_format_default(self, tool_with_root)` — [`L93`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_autoindex_tool.py#L93)
  - `test_warm_mode_returns_indexed_true(self, tool_with_root)` — [`L104`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_autoindex_tool.py#L104)
- uses (calls/refs, reference-scoped): [`ASTCache`](../../tree_sitter_analyzer/ast_cache.md#ASTCache), [`close`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.close), [`get_stats`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.get_stats), [`CodeGraphAutoIndexTool`](../../tree_sitter_analyzer/mcp/tools/auto_index_tool.md#CodeGraphAutoIndexTool), [`execute`](../../tree_sitter_analyzer/mcp/tools/auto_index_tool.md#CodeGraphAutoIndexTool.execute)

### `TestToolDefinition`
- def: [`tests/unit/test_codegraph_autoindex_tool.py:44`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_autoindex_tool.py#L44)
- signature: `class TestToolDefinition:`
- members:
  - `test_annotations_not_readonly(self, tool)` — [`L58`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_autoindex_tool.py#L58)
  - `test_schema_mode_enum(self, tool)` — [`L48`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_autoindex_tool.py#L48)
  - `test_schema_output_format_default_toon(self, tool)` — [`L53`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_autoindex_tool.py#L53)
  - `test_tool_name(self, tool)` — [`L45`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_autoindex_tool.py#L45)

### `TestValidation`
- def: [`tests/unit/test_codegraph_autoindex_tool.py:64`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_autoindex_tool.py#L64)
- signature: `class TestValidation:`
- members:
  - `test_invalid_mode_rejected(self, tool)` — [`L74`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_autoindex_tool.py#L74)
  - `test_valid_reset(self, tool)` — [`L71`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_autoindex_tool.py#L71)
  - `test_valid_status(self, tool)` — [`L65`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_autoindex_tool.py#L65)
  - `test_valid_warm(self, tool)` — [`L68`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_autoindex_tool.py#L68)

## Functions
- `tool()` — [`L13`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_autoindex_tool.py#L13)
- `tool_with_root(tmp_path)` — [`L18`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_autoindex_tool.py#L18)
- `warm_cache_root(tmp_path)` — [`L23`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_autoindex_tool.py#L23) — A project whose on-disk cache is fully populated, but whose

