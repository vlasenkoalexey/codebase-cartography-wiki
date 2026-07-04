---
title: 'Module: tests/unit/cli/test_query_exception_propagation.py'
type: catalog
provenance: extracted
module: tests/unit/cli/test_query_exception_propagation.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `tests.unit.cli.test_query_exception_propagation`/
symbols:
  _services: _services().
  TestCypherHelperExceptionPropagation.test_exits_nonzero_on_query_error: TestCypherHelperExceptionPropagation#test_exits_nonzero_on_query_error().
  TestCypherHelperExceptionPropagation.test_print_query_exception_called_with_correct_query: TestCypherHelperExceptionPropagation#test_print_query_exception_called_with_correct_query().
  TestCypherHelperVisualExceptionPropagation.test_visual_exits_nonzero_on_query_error: TestCypherHelperVisualExceptionPropagation#test_visual_exits_nonzero_on_query_error().
  TestPrintQueryException: TestPrintQueryException#
  TestPrintQueryException.test_kuzu_parser_error_no_traceback: TestPrintQueryException#test_kuzu_parser_error_no_traceback().
  TestPrintQueryException.test_kuzu_parser_error_shows_message: TestPrintQueryException#test_kuzu_parser_error_shows_message().
  TestPrintQueryException.test_neo4j_error_shows_code_and_message: TestPrintQueryException#test_neo4j_error_shows_code_and_message().
  TestPrintQueryException.test_falkordb_error_shows_message: TestPrintQueryException#test_falkordb_error_shows_message().
  TestCypherHelperExceptionPropagation: TestCypherHelperExceptionPropagation#
  TestCypherHelperVisualExceptionPropagation: TestCypherHelperVisualExceptionPropagation#
---
# Module: [`tests/unit/cli/test_query_exception_propagation.py`](../../../../../../../raw/code/codegraphcontext/tests/unit/cli/test_query_exception_propagation.py)

## Classes
### `TestCypherHelperExceptionPropagation`
- def: [`tests/unit/cli/test_query_exception_propagation.py:106`](../../../../../../../raw/code/codegraphcontext/tests/unit/cli/test_query_exception_propagation.py#L106)
- doc: Verify cypher_helper calls _print_query_exception on failure.
- signature: `class TestCypherHelperExceptionPropagation:`
- members:
  - `test_exits_nonzero_on_query_error(self, tmp_path)` — [`L109`](../../../../../../../raw/code/codegraphcontext/tests/unit/cli/test_query_exception_propagation.py#L109) — cypher_helper must exit with code 1 when query raises.
  - `test_print_query_exception_called_with_correct_query(self, tmp_path)` — [`L132`](../../../../../../../raw/code/codegraphcontext/tests/unit/cli/test_query_exception_propagation.py#L132) — _print_query_exception must receive the original query string.
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `TestCypherHelperVisualExceptionPropagation`
- def: [`tests/unit/cli/test_query_exception_propagation.py:156`](../../../../../../../raw/code/codegraphcontext/tests/unit/cli/test_query_exception_propagation.py#L156)
- doc: Verify cypher_helper_visual also calls _print_query_exception.
- signature: `class TestCypherHelperVisualExceptionPropagation:`
- members:
  - `test_visual_exits_nonzero_on_query_error(self, tmp_path)` — [`L159`](../../../../../../../raw/code/codegraphcontext/tests/unit/cli/test_query_exception_propagation.py#L159)
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `TestPrintQueryException`
- def: [`tests/unit/cli/test_query_exception_propagation.py:21`](../../../../../../../raw/code/codegraphcontext/tests/unit/cli/test_query_exception_propagation.py#L21)
- doc: Verify _print_query_exception surfaces the right message per backend.
- signature: `class TestPrintQueryException:`
- members:
  - `test_falkordb_error_shows_message(self)` — [`L77`](../../../../../../../raw/code/codegraphcontext/tests/unit/cli/test_query_exception_propagation.py#L77) — FalkorDB exceptions should show the database message.
  - `test_kuzu_parser_error_no_traceback(self, capsys)` — [`L24`](../../../../../../../raw/code/codegraphcontext/tests/unit/cli/test_query_exception_propagation.py#L24) — KuzuDB RuntimeError with 'Parser exception' should print cleanly.
  - `test_kuzu_parser_error_shows_message(self, capsys)` — [`L33`](../../../../../../../raw/code/codegraphcontext/tests/unit/cli/test_query_exception_propagation.py#L33) — Output must contain the raw parser exception text.
  - `test_neo4j_error_shows_code_and_message(self)` — [`L50`](../../../../../../../raw/code/codegraphcontext/tests/unit/cli/test_query_exception_propagation.py#L50) — Neo4j exceptions should show .code and .message attributes.

## Functions
- `_services()` — [`L10`](../../../../../../../raw/code/codegraphcontext/tests/unit/cli/test_query_exception_propagation.py#L10)

