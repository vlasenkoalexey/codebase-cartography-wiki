---
title: 'Module: tests/unit/test_codegraph_xref_tool.py'
type: catalog
provenance: extracted
module: tests/unit/test_codegraph_xref_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_codegraph_xref_tool`/
symbols:
  tool: tool().
  tool_with_root: tool_with_root().
  TestToolDefinition: TestToolDefinition#
  TestToolDefinition.test_tool_name: TestToolDefinition#test_tool_name().
  TestToolDefinition.test_description_mentions_codegraph_parity: TestToolDefinition#test_description_mentions_codegraph_parity().
  TestToolDefinition.test_annotations_readonly: TestToolDefinition#test_annotations_readonly().
  TestToolDefinition.test_schema_mode_default_symbol: TestToolDefinition#test_schema_mode_default_symbol().
  TestToolDefinition.test_schema_output_format_default_toon: TestToolDefinition#test_schema_output_format_default_toon().
  TestValidation: TestValidation#
  TestValidation.test_symbol_mode_requires_symbol: TestValidation#test_symbol_mode_requires_symbol().
  TestValidation.test_file_mode_requires_file_path: TestValidation#test_file_mode_requires_file_path().
  TestValidation.test_invalid_mode_rejected: TestValidation#test_invalid_mode_rejected().
  TestValidation.test_valid_symbol_mode: TestValidation#test_valid_symbol_mode().
  TestValidation.test_valid_file_mode: TestValidation#test_valid_file_mode().
  TestExecute: TestExecute#
  TestExecute.test_symbol_not_found_returns_not_found_verdict: TestExecute#test_symbol_not_found_returns_not_found_verdict().
  TestExecute.test_toon_format_default: TestExecute#test_toon_format_default().
  TestExecute.test_symbol_mode_field_in_response: TestExecute#test_symbol_mode_field_in_response().
  TestExecute.test_file_mode_field_in_response: TestExecute#test_file_mode_field_in_response().
  TestXRefFileModeAgentSummary: TestXRefFileModeAgentSummary#
  TestXRefFileModeAgentSummary.test_file_mode_response_has_agent_summary: TestXRefFileModeAgentSummary#test_file_mode_response_has_agent_summary().
  TestXRefFileModeAgentSummary.test_file_mode_agent_summary_has_count_semantics: TestXRefFileModeAgentSummary#test_file_mode_agent_summary_has_count_semantics().
  TestXRefFileModeAgentSummary.test_file_mode_agent_summary_carries_canonical_fields: TestXRefFileModeAgentSummary#test_file_mode_agent_summary_carries_canonical_fields().
  TestXRefFileModeAgentSummary.test_file_mode_top_level_summary_line_on_direct_path: TestXRefFileModeAgentSummary#test_file_mode_top_level_summary_line_on_direct_path().
  TestXRefFileModeAgentSummary.test_file_mode_count_semantics_mentions_callers: TestXRefFileModeAgentSummary#test_file_mode_count_semantics_mentions_callers().
  TestXRefFileModeAgentSummary.test_file_mode_count_semantics_mentions_import_dependents: TestXRefFileModeAgentSummary#test_file_mode_count_semantics_mentions_import_dependents().
  TestXRefFileModeAgentSummary.test_file_mode_count_semantics_mentions_file_dependents: TestXRefFileModeAgentSummary#test_file_mode_count_semantics_mentions_file_dependents().
---
# Module: [`tests/unit/test_codegraph_xref_tool.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_xref_tool.py)

## Classes
### `TestExecute`
- def: [`tests/unit/test_codegraph_xref_tool.py:65`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_xref_tool.py#L65)
- signature: `class TestExecute:`
- members:
  - `test_file_mode_field_in_response(self, tool_with_root, tmp_path)` — [`L85`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_xref_tool.py#L85)
  - `test_symbol_mode_field_in_response(self, tool_with_root)` — [`L79`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_xref_tool.py#L79)
  - `test_symbol_not_found_returns_not_found_verdict(self, tool_with_root)` — [`L66`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_xref_tool.py#L66)
  - `test_toon_format_default(self, tool_with_root)` — [`L72`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_xref_tool.py#L72)

### `TestToolDefinition`
- def: [`tests/unit/test_codegraph_xref_tool.py:20`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_xref_tool.py#L20)
- signature: `class TestToolDefinition:`
- members:
  - `test_annotations_readonly(self, tool)` — [`L28`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_xref_tool.py#L28)
  - `test_description_mentions_codegraph_parity(self, tool)` — [`L24`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_xref_tool.py#L24)
  - `test_schema_mode_default_symbol(self, tool)` — [`L33`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_xref_tool.py#L33)
  - `test_schema_output_format_default_toon(self, tool)` — [`L38`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_xref_tool.py#L38)
  - `test_tool_name(self, tool)` — [`L21`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_xref_tool.py#L21)

### `TestValidation`
- def: [`tests/unit/test_codegraph_xref_tool.py:44`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_xref_tool.py#L44)
- signature: `class TestValidation:`
- members:
  - `test_file_mode_requires_file_path(self, tool)` — [`L49`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_xref_tool.py#L49)
  - `test_invalid_mode_rejected(self, tool)` — [`L53`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_xref_tool.py#L53)
  - `test_symbol_mode_requires_symbol(self, tool)` — [`L45`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_xref_tool.py#L45)
  - `test_valid_file_mode(self, tool)` — [`L60`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_xref_tool.py#L60)
  - `test_valid_symbol_mode(self, tool)` — [`L57`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_xref_tool.py#L57)

### `TestXRefFileModeAgentSummary`
- def: [`tests/unit/test_codegraph_xref_tool.py:99`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_xref_tool.py#L99)
- doc: #669: nav action=xref mode=file must include an agent_summary that
- signature: `class TestXRefFileModeAgentSummary:`
- members:
  - `test_file_mode_agent_summary_carries_canonical_fields(self, tool_with_root, tmp_path)` — [`L127`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_xref_tool.py#L127)
  - `test_file_mode_agent_summary_has_count_semantics(self, tool_with_root, tmp_path)` — [`L116`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_xref_tool.py#L116) — agent_summary.count_semantics must be present and explain the three counts.
  - `test_file_mode_count_semantics_mentions_callers(self, tool_with_root, tmp_path)` — [`L157`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_xref_tool.py#L157) — count_semantics must explain caller_count (function-level call sites).
  - `test_file_mode_count_semantics_mentions_file_dependents(self, tool_with_root, tmp_path)` — [`L179`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_xref_tool.py#L179) — count_semantics must explain file_dependent_count (files with call edges).
  - `test_file_mode_count_semantics_mentions_import_dependents(self, tool_with_root, tmp_path)` — [`L168`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_xref_tool.py#L168) — count_semantics must explain import_dependent_count (files importing this module).
  - `test_file_mode_response_has_agent_summary(self, tool_with_root, tmp_path)` — [`L108`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_xref_tool.py#L108) — agent_summary must be present in file mode response.
  - `test_file_mode_top_level_summary_line_on_direct_path(self, tool_with_root, tmp_path)` — [`L143`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_xref_tool.py#L143)

## Functions
- `tool()` — [`L11`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_xref_tool.py#L11)
- `tool_with_root(tmp_path)` — [`L16`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_xref_tool.py#L16)

