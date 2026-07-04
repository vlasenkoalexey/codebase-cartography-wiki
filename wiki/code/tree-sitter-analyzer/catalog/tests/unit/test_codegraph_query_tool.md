---
title: 'Module: tests/unit/test_codegraph_query_tool.py'
type: catalog
provenance: extracted
module: tests/unit/test_codegraph_query_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_codegraph_query_tool`/
symbols:
  TestParseChain.test_sort_all_valid_fields_parse: TestParseChain#test_sort_all_valid_fields_parse().
  TestParseChain.test_sort_path_alias_for_file_parses: TestParseChain#test_sort_path_alias_for_file_parses().
  TestParseChain.test_plain_string_expands: TestParseChain#test_plain_string_expands().
  TestParseChain.test_dotted_chain_parsed: TestParseChain#test_dotted_chain_parsed().
  tool: tool().
  tool_with_root: tool_with_root().
  TestToolDefinition: TestToolDefinition#
  TestToolDefinition.test_tool_name: TestToolDefinition#test_tool_name().
  TestToolDefinition.test_description_mentions_confidence: TestToolDefinition#test_description_mentions_confidence().
  TestToolDefinition.test_description_mentions_bm25: TestToolDefinition#test_description_mentions_bm25().
  TestToolDefinition.test_annotations_readonly: TestToolDefinition#test_annotations_readonly().
  TestToolDefinition.test_schema_requires_query: TestToolDefinition#test_schema_requires_query().
  TestToolDefinition.test_schema_output_format_default_toon: TestToolDefinition#test_schema_output_format_default_toon().
  TestValidation: TestValidation#
  TestValidation.test_requires_query: TestValidation#test_requires_query().
  TestValidation.test_empty_query_rejected: TestValidation#test_empty_query_rejected().
  TestValidation.test_valid_query: TestValidation#test_valid_query().
  TestParseChain: TestParseChain#
  TestExecute: TestExecute#
  TestExecute.test_toon_format_default: TestExecute#test_toon_format_default().
  TestExecute.test_json_format: TestExecute#test_json_format().
  TestExecute.test_plain_query_returns_results: TestExecute#test_plain_query_returns_results().
  TestExecute.test_invalid_chain_step_returns_error: TestExecute#test_invalid_chain_step_returns_error().
---
# Module: [`tests/unit/test_codegraph_query_tool.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_tool.py)

## Classes
### `TestExecute`
- def: [`tests/unit/test_codegraph_query_tool.py:99`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_tool.py#L99)
- signature: `class TestExecute:`
- members:
  - `test_invalid_chain_step_returns_error(self, tool_with_root)` — [`L118`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_tool.py#L118)
  - `test_json_format(self, tool_with_root)` — [`L105`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_tool.py#L105)
  - `test_plain_query_returns_results(self, tool_with_root)` — [`L112`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_tool.py#L112)
  - `test_toon_format_default(self, tool_with_root)` — [`L100`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_tool.py#L100)

### `TestParseChain`
- def: [`tests/unit/test_codegraph_query_tool.py:65`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_tool.py#L65)
- signature: `class TestParseChain:`
- members:
  - `test_dotted_chain_parsed(self)` — [`L70`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_tool.py#L70)
  - `test_plain_string_expands(self)` — [`L66`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_tool.py#L66)
  - `test_sort_all_valid_fields_parse(self)` — [`L76`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_tool.py#L76) — All 7 sort fields in the README must parse without error.
  - `test_sort_path_alias_for_file_parses(self)` — [`L91`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_tool.py#L91) — 'path' is documented as an alias for 'file' in sort().
- uses (calls/refs, reference-scoped): [`parse_chain`](../../tree_sitter_analyzer/mcp/tools/_codegraph_query_dsl.md#parse_chain), [`kwargs`](../../tree_sitter_analyzer/mcp/tools/_codegraph_query_dsl.md#_ChainStep.kwargs), [`name`](../../tree_sitter_analyzer/mcp/tools/_codegraph_query_dsl.md#_ChainStep.name)

### `TestToolDefinition`
- def: [`tests/unit/test_codegraph_query_tool.py:26`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_tool.py#L26)
- signature: `class TestToolDefinition:`
- members:
  - `test_annotations_readonly(self, tool)` — [`L38`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_tool.py#L38)
  - `test_description_mentions_bm25(self, tool)` — [`L34`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_tool.py#L34)
  - `test_description_mentions_confidence(self, tool)` — [`L30`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_tool.py#L30)
  - `test_schema_output_format_default_toon(self, tool)` — [`L46`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_tool.py#L46)
  - `test_schema_requires_query(self, tool)` — [`L43`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_tool.py#L43)
  - `test_tool_name(self, tool)` — [`L27`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_tool.py#L27)

### `TestValidation`
- def: [`tests/unit/test_codegraph_query_tool.py:52`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_tool.py#L52)
- signature: `class TestValidation:`
- members:
  - `test_empty_query_rejected(self, tool)` — [`L57`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_tool.py#L57)
  - `test_requires_query(self, tool)` — [`L53`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_tool.py#L53)
  - `test_valid_query(self, tool)` — [`L61`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_tool.py#L61)

## Functions
- `tool()` — [`L14`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_tool.py#L14)
- `tool_with_root(tmp_path)` — [`L19`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_tool.py#L19)

