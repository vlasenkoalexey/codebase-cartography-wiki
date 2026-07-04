---
title: 'Module: tests/unit/test_codegraph_incremental_sync_tool.py'
type: catalog
provenance: extracted
module: tests/unit/test_codegraph_incremental_sync_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_codegraph_incremental_sync_tool`/
symbols:
  tool: tool().
  tool_with_root: tool_with_root().
  TestToolDefinition: TestToolDefinition#
  TestToolDefinition.test_tool_name: TestToolDefinition#test_tool_name().
  TestToolDefinition.test_description_mentions_no_other: TestToolDefinition#test_description_mentions_no_other().
  TestToolDefinition.test_schema_mode_enum: TestToolDefinition#test_schema_mode_enum().
  TestToolDefinition.test_schema_output_format_default_toon: TestToolDefinition#test_schema_output_format_default_toon().
  TestToolDefinition.test_annotations_destructive: TestToolDefinition#test_annotations_destructive().
  TestValidation: TestValidation#
  TestValidation.test_valid_sync: TestValidation#test_valid_sync().
  TestValidation.test_valid_changes: TestValidation#test_valid_changes().
  TestValidation.test_valid_status: TestValidation#test_valid_status().
  TestValidation.test_invalid_mode_rejected: TestValidation#test_invalid_mode_rejected().
  TestExecute: TestExecute#
  TestExecute.test_status_no_project_root_returns_error: TestExecute#test_status_no_project_root_returns_error().
  TestExecute.test_status_on_empty_project: TestExecute#test_status_on_empty_project().
  TestExecute.test_changes_mode_preview: TestExecute#test_changes_mode_preview().
  TestExecute.test_toon_format_default: TestExecute#test_toon_format_default().
---
# Module: [`tests/unit/test_codegraph_incremental_sync_tool.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_incremental_sync_tool.py)

## Classes
### `TestExecute`
- def: [`tests/unit/test_codegraph_incremental_sync_tool.py:62`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_incremental_sync_tool.py#L62)
- signature: `class TestExecute:`
- members:
  - `test_changes_mode_preview(self, tool_with_root)` — [`L73`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_incremental_sync_tool.py#L73)
  - `test_status_no_project_root_returns_error(self, tool)` — [`L63`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_incremental_sync_tool.py#L63)
  - `test_status_on_empty_project(self, tool_with_root)` — [`L67`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_incremental_sync_tool.py#L67)
  - `test_toon_format_default(self, tool_with_root)` — [`L79`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_incremental_sync_tool.py#L79)

### `TestToolDefinition`
- def: [`tests/unit/test_codegraph_incremental_sync_tool.py:23`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_incremental_sync_tool.py#L23)
- signature: `class TestToolDefinition:`
- members:
  - `test_annotations_destructive(self, tool)` — [`L40`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_incremental_sync_tool.py#L40)
  - `test_description_mentions_no_other(self, tool)` — [`L27`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_incremental_sync_tool.py#L27)
  - `test_schema_mode_enum(self, tool)` — [`L31`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_incremental_sync_tool.py#L31)
  - `test_schema_output_format_default_toon(self, tool)` — [`L35`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_incremental_sync_tool.py#L35)
  - `test_tool_name(self, tool)` — [`L24`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_incremental_sync_tool.py#L24)

### `TestValidation`
- def: [`tests/unit/test_codegraph_incremental_sync_tool.py:46`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_incremental_sync_tool.py#L46)
- signature: `class TestValidation:`
- members:
  - `test_invalid_mode_rejected(self, tool)` — [`L56`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_incremental_sync_tool.py#L56)
  - `test_valid_changes(self, tool)` — [`L50`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_incremental_sync_tool.py#L50)
  - `test_valid_status(self, tool)` — [`L53`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_incremental_sync_tool.py#L53)
  - `test_valid_sync(self, tool)` — [`L47`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_incremental_sync_tool.py#L47)

## Functions
- `tool()` — [`L13`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_incremental_sync_tool.py#L13)
- `tool_with_root(tmp_path)` — [`L18`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_incremental_sync_tool.py#L18)

