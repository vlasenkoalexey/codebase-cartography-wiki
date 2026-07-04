---
title: 'Module: tests/unit/test_codegraph_refactor_tool.py'
type: catalog
provenance: extracted
module: tests/unit/test_codegraph_refactor_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_codegraph_refactor_tool`/
symbols:
  tool: tool().
  tool_with_root: tool_with_root().
  TestToolDefinition: TestToolDefinition#
  TestToolDefinition.test_tool_name: TestToolDefinition#test_tool_name().
  TestToolDefinition.test_schema_required_fields: TestToolDefinition#test_schema_required_fields().
  TestToolDefinition.test_schema_mode_enum: TestToolDefinition#test_schema_mode_enum().
  TestToolDefinition.test_schema_output_format_default_toon: TestToolDefinition#test_schema_output_format_default_toon().
  TestToolDefinition.test_no_annotations_destructive_false: TestToolDefinition#test_no_annotations_destructive_false().
  TestValidation: TestValidation#
  TestValidation.test_valid_rename: TestValidation#test_valid_rename().
  TestValidation.test_requires_symbol: TestValidation#test_requires_symbol().
  TestValidation.test_requires_new_name: TestValidation#test_requires_new_name().
  TestValidation.test_same_name_rejected: TestValidation#test_same_name_rejected().
  TestValidation.test_invalid_chars_in_symbol: TestValidation#test_invalid_chars_in_symbol().
  TestValidation.test_invalid_chars_in_new_name: TestValidation#test_invalid_chars_in_new_name().
  TestValidation.test_dotted_symbol_allowed: TestValidation#test_dotted_symbol_allowed().
  TestExecutePreview: TestExecutePreview#
  TestExecutePreview.test_preview_no_project_root_returns_error: TestExecutePreview#test_preview_no_project_root_returns_error().
  TestExecutePreview.test_preview_on_empty_project: TestExecutePreview#test_preview_on_empty_project().
  TestExecutePreview.test_toon_format_default: TestExecutePreview#test_toon_format_default().
---
# Module: [`tests/unit/test_codegraph_refactor_tool.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_refactor_tool.py)

## Classes
### `TestExecutePreview`
- def: [`tests/unit/test_codegraph_refactor_tool.py:84`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_refactor_tool.py#L84)
- signature: `class TestExecutePreview:`
- members:
  - `test_preview_no_project_root_returns_error(self, tool)` — [`L85`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_refactor_tool.py#L85)
  - `test_preview_on_empty_project(self, tool_with_root)` — [`L91`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_refactor_tool.py#L91)
  - `test_toon_format_default(self, tool_with_root)` — [`L106`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_refactor_tool.py#L106)

### `TestToolDefinition`
- def: [`tests/unit/test_codegraph_refactor_tool.py:21`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_refactor_tool.py#L21)
- signature: `class TestToolDefinition:`
- members:
  - `test_no_annotations_destructive_false(self, tool)` — [`L39`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_refactor_tool.py#L39)
  - `test_schema_mode_enum(self, tool)` — [`L30`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_refactor_tool.py#L30)
  - `test_schema_output_format_default_toon(self, tool)` — [`L35`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_refactor_tool.py#L35)
  - `test_schema_required_fields(self, tool)` — [`L25`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_refactor_tool.py#L25)
  - `test_tool_name(self, tool)` — [`L22`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_refactor_tool.py#L22)

### `TestValidation`
- def: [`tests/unit/test_codegraph_refactor_tool.py:47`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_refactor_tool.py#L47)
- signature: `class TestValidation:`
- members:
  - `test_dotted_symbol_allowed(self, tool)` — [`L74`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_refactor_tool.py#L74)
  - `test_invalid_chars_in_new_name(self, tool)` — [`L70`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_refactor_tool.py#L70)
  - `test_invalid_chars_in_symbol(self, tool)` — [`L66`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_refactor_tool.py#L66)
  - `test_requires_new_name(self, tool)` — [`L58`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_refactor_tool.py#L58)
  - `test_requires_symbol(self, tool)` — [`L54`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_refactor_tool.py#L54)
  - `test_same_name_rejected(self, tool)` — [`L62`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_refactor_tool.py#L62)
  - `test_valid_rename(self, tool)` — [`L48`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_refactor_tool.py#L48)

## Functions
- `tool()` — [`L11`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_refactor_tool.py#L11)
- `tool_with_root(tmp_path)` — [`L16`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_refactor_tool.py#L16)

