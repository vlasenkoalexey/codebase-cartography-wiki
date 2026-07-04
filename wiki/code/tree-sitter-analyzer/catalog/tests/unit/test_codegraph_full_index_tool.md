---
title: 'Module: tests/unit/test_codegraph_full_index_tool.py'
type: catalog
provenance: extracted
module: tests/unit/test_codegraph_full_index_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_codegraph_full_index_tool`/
symbols:
  TestExecute.test_verdict_is_warn_when_incremental_sync_has_errors: TestExecute#test_verdict_is_warn_when_incremental_sync_has_errors().
  tool: tool().
  tool_with_root: tool_with_root().
  TestToolDefinition: TestToolDefinition#
  TestToolDefinition.test_tool_name: TestToolDefinition#test_tool_name().
  TestToolDefinition.test_description_mentions_no_other: TestToolDefinition#test_description_mentions_no_other().
  TestToolDefinition.test_schema_mode_enum: TestToolDefinition#test_schema_mode_enum().
  TestToolDefinition.test_schema_output_format_default_toon: TestToolDefinition#test_schema_output_format_default_toon().
  TestToolDefinition.test_annotations_destructive: TestToolDefinition#test_annotations_destructive().
  TestValidation: TestValidation#
  TestValidation.test_valid_incremental: TestValidation#test_valid_incremental().
  TestValidation.test_valid_full: TestValidation#test_valid_full().
  TestValidation.test_invalid_mode_rejected: TestValidation#test_invalid_mode_rejected().
  TestExecute: TestExecute#
  TestExecute.test_no_project_root_returns_error: TestExecute#test_no_project_root_returns_error().
  TestExecute.test_incremental_on_empty_project: TestExecute#test_incremental_on_empty_project().
  TestExecute.test_toon_format_default: TestExecute#test_toon_format_default().
---
# Module: [`tests/unit/test_codegraph_full_index_tool.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_full_index_tool.py)

## Classes
### `TestExecute`
- def: [`tests/unit/test_codegraph_full_index_tool.py:58`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_full_index_tool.py#L58)
- signature: `class TestExecute:`
- members:
  - `test_incremental_on_empty_project(self, tool_with_root)` — [`L63`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_full_index_tool.py#L63)
  - `test_no_project_root_returns_error(self, tool)` — [`L59`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_full_index_tool.py#L59)
  - `test_toon_format_default(self, tool_with_root)` — [`L69`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_full_index_tool.py#L69)
  - `test_verdict_is_warn_when_incremental_sync_has_errors(self, tool_with_root)` — [`L74`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_full_index_tool.py#L74) — #860: DB flush errors in incremental_sync must escalate verdict to WARN.
- uses (calls/refs, reference-scoped): [`errors`](../../tree_sitter_analyzer/incremental_sync.md#SyncResult.errors), [`SyncResult`](../../tree_sitter_analyzer/incremental_sync.md#SyncResult), [`deleted_files`](../../tree_sitter_analyzer/incremental_sync.md#SyncResult.deleted_files), [`new_files`](../../tree_sitter_analyzer/incremental_sync.md#SyncResult.new_files), [`updated_files`](../../tree_sitter_analyzer/incremental_sync.md#SyncResult.updated_files), [`scanned`](../../tree_sitter_analyzer/incremental_sync.md#SyncResult.scanned), [`unchanged_files`](../../tree_sitter_analyzer/incremental_sync.md#SyncResult.unchanged_files)

### `TestToolDefinition`
- def: [`tests/unit/test_codegraph_full_index_tool.py:21`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_full_index_tool.py#L21)
- signature: `class TestToolDefinition:`
- members:
  - `test_annotations_destructive(self, tool)` — [`L39`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_full_index_tool.py#L39)
  - `test_description_mentions_no_other(self, tool)` — [`L25`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_full_index_tool.py#L25)
  - `test_schema_mode_enum(self, tool)` — [`L29`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_full_index_tool.py#L29)
  - `test_schema_output_format_default_toon(self, tool)` — [`L34`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_full_index_tool.py#L34)
  - `test_tool_name(self, tool)` — [`L22`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_full_index_tool.py#L22)

### `TestValidation`
- def: [`tests/unit/test_codegraph_full_index_tool.py:45`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_full_index_tool.py#L45)
- signature: `class TestValidation:`
- members:
  - `test_invalid_mode_rejected(self, tool)` — [`L52`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_full_index_tool.py#L52)
  - `test_valid_full(self, tool)` — [`L49`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_full_index_tool.py#L49)
  - `test_valid_incremental(self, tool)` — [`L46`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_full_index_tool.py#L46)

## Functions
- `tool()` — [`L11`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_full_index_tool.py#L11)
- `tool_with_root(tmp_path)` — [`L16`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_full_index_tool.py#L16)

