---
title: 'Module: tests/unit/mcp/test_batch_search_tool.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_batch_search_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_batch_search_tool`/
symbols:
  TestBatchSearchToolExecution.test_matches_truncated_at_20: TestBatchSearchToolExecution#test_matches_truncated_at_20().
  TestBatchSearchToolDefinition.test_tool_definition_description_contains_when_to_use: TestBatchSearchToolDefinition#test_tool_definition_description_contains_when_to_use().
  TestBatchSearchToolDefinition.test_tool_definition_description_contains_when_not_to_use: TestBatchSearchToolDefinition#test_tool_definition_description_contains_when_not_to_use().
  TestBatchSearchToolDefinition.test_queries_required_field: TestBatchSearchToolDefinition#test_queries_required_field().
  TestBatchSearchToolDefinition.test_queries_min_max_items: TestBatchSearchToolDefinition#test_queries_min_max_items().
  TestBatchSearchToolValidation.test_minimum_queries_enforced: TestBatchSearchToolValidation#test_minimum_queries_enforced().
  TestBatchSearchToolValidation.test_maximum_queries_enforced: TestBatchSearchToolValidation#test_maximum_queries_enforced().
  TestBatchSearchToolValidation.test_queries_not_a_list_raises: TestBatchSearchToolValidation#test_queries_not_a_list_raises().
  TestBatchSearchToolValidation.test_valid_two_queries_passes: TestBatchSearchToolValidation#test_valid_two_queries_passes().
  TestBatchSearchToolValidation.test_missing_pattern_raises: TestBatchSearchToolValidation#test_missing_pattern_raises().
  TestBatchSearchToolExecution.test_execute_parallel_searches: TestBatchSearchToolExecution#test_execute_parallel_searches().
  TestBatchSearchToolExecution.test_results_aggregated: TestBatchSearchToolExecution#test_results_aggregated().
  TestBatchSearchToolExecution.test_empty_results: TestBatchSearchToolExecution#test_empty_results().
  TestBatchSearchToolExecution.test_label_defaults_to_pattern: TestBatchSearchToolExecution#test_label_defaults_to_pattern().
  TestBatchSearchToolExecution.test_custom_label_used: TestBatchSearchToolExecution#test_custom_label_used().
  TestBatchSearchToolExecution.test_execution_note_mentions_count: TestBatchSearchToolExecution#test_execution_note_mentions_count().
  tool: tool().
  TestBatchSearchToolInitialization.test_init_creates_tool: TestBatchSearchToolInitialization#test_init_creates_tool().
  _make_fake_match: _make_fake_match().
  TestBatchSearchToolInitialization: TestBatchSearchToolInitialization#
  TestBatchSearchToolDefinition: TestBatchSearchToolDefinition#
  TestBatchSearchToolValidation: TestBatchSearchToolValidation#
  TestBatchSearchToolExecution: TestBatchSearchToolExecution#
---
# Module: [`tests/unit/mcp/test_batch_search_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_batch_search_tool.py)

## Classes
### `TestBatchSearchToolDefinition`
- def: [`tests/unit/mcp/test_batch_search_tool.py:48`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_batch_search_tool.py#L48)
- doc: Tests for get_tool_definition().
- signature: `class TestBatchSearchToolDefinition:`
- members:
  - `test_queries_min_max_items(self, tool: BatchSearchTool)` — [`L71`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_batch_search_tool.py#L71) — Test that queries schema enforces minItems=2 and maxItems=10.
  - `test_queries_required_field(self, tool: BatchSearchTool)` — [`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_batch_search_tool.py#L65) — Test that queries is in the required array.
  - `test_tool_definition_description_contains_when_not_to_use(self, tool: BatchSearchTool)` — [`L58`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_batch_search_tool.py#L58) — Test that the description contains WHEN NOT TO USE section.
  - `test_tool_definition_description_contains_when_to_use(self, tool: BatchSearchTool)` — [`L51`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_batch_search_tool.py#L51) — Test that the description contains WHEN TO USE section.
- uses (calls/refs, reference-scoped): [`BatchSearchTool`](../../../tree_sitter_analyzer/mcp/tools/batch_search_tool.md#BatchSearchTool), [`get_tool_definition`](../../../tree_sitter_analyzer/mcp/tools/batch_search_tool.md#BatchSearchTool.get_tool_definition)

### `TestBatchSearchToolExecution`
- def: [`tests/unit/mcp/test_batch_search_tool.py:113`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_batch_search_tool.py#L113)
- doc: Tests for execute() — core test class.
- signature: `class TestBatchSearchToolExecution:`
- members:
  - `test_custom_label_used(self, tool: BatchSearchTool)` — [`L282`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_batch_search_tool.py#L282) — Test that a provided label is used in the result.
  - `test_empty_results(self, tool: BatchSearchTool)` — [`L235`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_batch_search_tool.py#L235) — Test that a ripgrep no-match return code produces match_count=0.
  - `test_execute_parallel_searches(self, tool: BatchSearchTool)` — [`L117`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_batch_search_tool.py#L117) — Test that execute runs searches in parallel and returns results for each query.
  - `test_execution_note_mentions_count(self, tool: BatchSearchTool)` — [`L303`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_batch_search_tool.py#L303) — Test that execution_note mentions the number of searches run.
  - `test_label_defaults_to_pattern(self, tool: BatchSearchTool)` — [`L261`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_batch_search_tool.py#L261) — Test that when no label is provided, the pattern is used as the label.
  - `test_matches_truncated_at_20(self, tool: BatchSearchTool)` — [`L194`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_batch_search_tool.py#L194) — Test that matches are truncated at _BATCH_MAX_MATCHES_PER_QUERY (20).
  - `test_results_aggregated(self, tool: BatchSearchTool)` — [`L142`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_batch_search_tool.py#L142) — Test that total_matches is the sum of all individual match counts.
- uses (calls/refs, reference-scoped): [`execute`](../../../tree_sitter_analyzer/mcp/tools/batch_search_tool.md#BatchSearchTool.execute), [`BatchSearchTool`](../../../tree_sitter_analyzer/mcp/tools/batch_search_tool.md#BatchSearchTool), [`_BATCH_MAX_MATCHES_PER_QUERY`](../../../tree_sitter_analyzer/mcp/tools/batch_search_tool.md#_BATCH_MAX_MATCHES_PER_QUERY)

### `TestBatchSearchToolInitialization`
- def: [`tests/unit/mcp/test_batch_search_tool.py:40`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_batch_search_tool.py#L40)
- doc: Tests for tool initialization.
- signature: `class TestBatchSearchToolInitialization:`
- members:
  - `test_init_creates_tool(self, tool: BatchSearchTool)` — [`L43`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_batch_search_tool.py#L43) — Test that initialization creates a tool instance.
- uses (calls/refs, reference-scoped): [`BatchSearchTool`](../../../tree_sitter_analyzer/mcp/tools/batch_search_tool.md#BatchSearchTool)

### `TestBatchSearchToolValidation`
- def: [`tests/unit/mcp/test_batch_search_tool.py:79`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_batch_search_tool.py#L79)
- doc: Tests for validate_arguments().
- signature: `class TestBatchSearchToolValidation:`
- members:
  - `test_maximum_queries_enforced(self, tool: BatchSearchTool)` — [`L87`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_batch_search_tool.py#L87) — Test that more than 10 queries raises a ValueError.
  - `test_minimum_queries_enforced(self, tool: BatchSearchTool)` — [`L82`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_batch_search_tool.py#L82) — Test that fewer than 2 queries raises a ValueError.
  - `test_missing_pattern_raises(self, tool: BatchSearchTool)` — [`L105`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_batch_search_tool.py#L105) — Test that a query missing pattern raises ValueError.
  - `test_queries_not_a_list_raises(self, tool: BatchSearchTool)` — [`L93`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_batch_search_tool.py#L93) — Test that non-list queries raises ValueError.
  - `test_valid_two_queries_passes(self, tool: BatchSearchTool)` — [`L98`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_batch_search_tool.py#L98) — Test that exactly two valid queries passes validation.
- uses (calls/refs, reference-scoped): [`BatchSearchTool`](../../../tree_sitter_analyzer/mcp/tools/batch_search_tool.md#BatchSearchTool), [`validate_arguments`](../../../tree_sitter_analyzer/mcp/tools/batch_search_tool.md#BatchSearchTool.validate_arguments)

## Functions
- `_make_fake_match(path: str = "src/foo.py", line: int = 1)` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_batch_search_tool.py#L27) — Build a minimal fake rg match dict.
- `tool()` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_batch_search_tool.py#L22) — Create a fresh BatchSearchTool instance for each test.

