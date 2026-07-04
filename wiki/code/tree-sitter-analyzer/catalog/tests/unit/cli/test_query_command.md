---
title: 'Module: tests/unit/cli/test_query_command.py'
type: catalog
provenance: extracted
module: tests/unit/cli/test_query_command.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.cli.test_query_command`/
symbols:
  TestQueryCommandInit.test_init_with_args: TestQueryCommandInit#test_init_with_args().
  command: command().
  TestQueryCommandInit.test_init: TestQueryCommandInit#test_init().
  mock_args: mock_args().
  TestQueryCommandInit: TestQueryCommandInit#
  TestQueryCommandExecuteQuery: TestQueryCommandExecuteQuery#
  TestQueryCommandExecuteQuery.test_execute_query_with_query_key: TestQueryCommandExecuteQuery#test_execute_query_with_query_key().
  TestQueryCommandExecuteQuery.test_execute_query_with_custom_query: TestQueryCommandExecuteQuery#test_execute_query_with_custom_query().
  TestQueryCommandExecuteQuery.test_execute_query_with_filter: TestQueryCommandExecuteQuery#test_execute_query_with_filter().
  TestQueryCommandExecuteQuery.test_execute_query_failure: TestQueryCommandExecuteQuery#test_execute_query_failure().
  TestQueryCommandExecuteAsync: TestQueryCommandExecuteAsync#
  TestQueryCommandExecuteAsync.test_execute_async_with_query_key: TestQueryCommandExecuteAsync#test_execute_async_with_query_key().
  TestQueryCommandExecuteAsync.test_execute_async_with_query_string: TestQueryCommandExecuteAsync#test_execute_async_with_query_string().
  TestQueryCommandExecuteAsync.test_execute_async_no_query: TestQueryCommandExecuteAsync#test_execute_async_no_query().
  TestQueryCommandExecuteAsync.test_execute_async_invalid_query_key: TestQueryCommandExecuteAsync#test_execute_async_invalid_query_key().
  TestQueryCommandExecuteAsync.test_execute_async_unsafe_query_string: TestQueryCommandExecuteAsync#test_execute_async_unsafe_query_string().
  TestQueryCommandOutput: TestQueryCommandOutput#
  TestQueryCommandOutput.test_execute_async_outputs_json: TestQueryCommandOutput#test_execute_async_outputs_json().
  TestQueryCommandOutput.test_execute_async_outputs_toon: TestQueryCommandOutput#test_execute_async_outputs_toon().
  TestQueryCommandOutput.test_execute_async_outputs_text: TestQueryCommandOutput#test_execute_async_outputs_text().
  TestQueryCommandOutput.test_execute_async_no_results: TestQueryCommandOutput#test_execute_async_no_results().
  TestQueryCommandBehavior: TestQueryCommandBehavior#
  TestQueryCommandBehavior.test_execute_query_sanitizes_input: TestQueryCommandBehavior#test_execute_query_sanitizes_input().
  TestQueryCommandBehavior.test_execute_async_query_failure_returns_1: TestQueryCommandBehavior#test_execute_async_query_failure_returns_1().
  TestQueryCommandBehavior.test_execute_async_multiple_results: TestQueryCommandBehavior#test_execute_async_multiple_results().
  TestR37acQueryCanonicalEnvelope: TestR37acQueryCanonicalEnvelope#
  TestR37acQueryCanonicalEnvelope.test_query_json_returns_envelope_dict: TestR37acQueryCanonicalEnvelope#test_query_json_returns_envelope_dict().
  TestR37acQueryCanonicalEnvelope.test_query_json_zero_matches_still_envelope: TestR37acQueryCanonicalEnvelope#test_query_json_zero_matches_still_envelope().
---
# Module: [`tests/unit/cli/test_query_command.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_query_command.py)

## Classes
### `TestQueryCommandBehavior`
- def: [`tests/unit/cli/test_query_command.py:297`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_query_command.py#L297)
- doc: Tests for QueryCommand behavior.
- signature: `class TestQueryCommandBehavior:`
- members:
  - `test_execute_async_multiple_results(self, command)` — [`L338`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_query_command.py#L338) — Test execute_async handles multiple results.
  - `test_execute_async_query_failure_returns_1(self, command)` — [`L327`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_query_command.py#L327) — Test execute_async returns 1 when query fails.
  - `test_execute_query_sanitizes_input(self, command)` — [`L301`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_query_command.py#L301) — Test execute_query sanitizes query key input.

### `TestQueryCommandExecuteAsync`
- def: [`tests/unit/cli/test_query_command.py:138`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_query_command.py#L138)
- doc: Tests for QueryCommand.execute_async method.
- signature: `class TestQueryCommandExecuteAsync:`
- members:
  - `test_execute_async_invalid_query_key(self, command)` — [`L194`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_query_command.py#L194) — Test execute_async with invalid query key.
  - `test_execute_async_no_query(self, command)` — [`L184`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_query_command.py#L184) — Test execute_async with no query specified.
  - `test_execute_async_unsafe_query_string(self, command)` — [`L209`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_query_command.py#L209) — Test execute_async with unsafe query string.
  - `test_execute_async_with_query_key(self, command)` — [`L142`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_query_command.py#L142) — Test execute_async with query_key parameter.
  - `test_execute_async_with_query_string(self, command)` — [`L163`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_query_command.py#L163) — Test execute_async with query_string parameter.

### `TestQueryCommandExecuteQuery`
- def: [`tests/unit/cli/test_query_command.py:71`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_query_command.py#L71)
- doc: Tests for QueryCommand.execute_query method.
- signature: `class TestQueryCommandExecuteQuery:`
- members:
  - `test_execute_query_failure(self, command)` — [`L124`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_query_command.py#L124) — Test execute_query handles exceptions.
  - `test_execute_query_with_custom_query(self, command)` — [`L91`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_query_command.py#L91) — Test execute_query with custom query string.
  - `test_execute_query_with_filter(self, command)` — [`L107`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_query_command.py#L107) — Test execute_query with filter expression.
  - `test_execute_query_with_query_key(self, command)` — [`L75`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_query_command.py#L75) — Test execute_query with predefined query key.

### `TestQueryCommandInit`
- def: [`tests/unit/cli/test_query_command.py:54`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_query_command.py#L54)
- doc: Tests for QueryCommand initialization.
- signature: `class TestQueryCommandInit:`
- members:
  - `test_init(self, command)` — [`L57`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_query_command.py#L57) — Test QueryCommand initialization.
  - `test_init_with_args(self, mock_args)` — [`L64`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_query_command.py#L64) — Test QueryCommand initialization with args.
- uses (calls/refs, reference-scoped): [`args`](../../../tree_sitter_analyzer/cli/commands/base_command.md#BaseCommand.args), [`QueryCommand`](../../../tree_sitter_analyzer/cli/commands/query_command.md#QueryCommand), [`query_service`](../../../tree_sitter_analyzer/cli/commands/query_command.md#QueryCommand.query_service)

### `TestQueryCommandOutput`
- def: [`tests/unit/cli/test_query_command.py:224`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_query_command.py#L224)
- doc: Tests for QueryCommand output.
- signature: `class TestQueryCommandOutput:`
- members:
  - `test_execute_async_no_results(self, command)` — [`L282`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_query_command.py#L282) — Test execute_async with no results.
  - `test_execute_async_outputs_json(self, command)` — [`L228`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_query_command.py#L228) — Test execute_async outputs JSON format.
  - `test_execute_async_outputs_text(self, command)` — [`L258`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_query_command.py#L258) — Test execute_async outputs text format.
  - `test_execute_async_outputs_toon(self, command)` — [`L244`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_query_command.py#L244) — Test execute_async outputs TOON format.

### `TestR37acQueryCanonicalEnvelope`
- def: [`tests/unit/cli/test_query_command.py:369`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_query_command.py#L369)
- doc: r37ac (dogfood): CLI `--query-key X` previously emitted a bare
- signature: `class TestR37acQueryCanonicalEnvelope:`
- members:
  - `test_query_json_returns_envelope_dict(self, command)` — [`L377`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_query_command.py#L377) — ``--query-key methods --format json`` must emit a dict envelope.
  - `test_query_json_zero_matches_still_envelope(self, command)` — [`L428`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_query_command.py#L428) — No matches must also return a dict envelope with match_count=0.

## Functions
- `command(mock_args)` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_query_command.py#L49) — Create QueryCommand instance for testing.
- `mock_args()` — [`L15`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_query_command.py#L15) — Create mock args for BaseCommand initialization.

