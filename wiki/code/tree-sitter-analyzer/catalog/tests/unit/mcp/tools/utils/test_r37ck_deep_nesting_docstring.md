---
title: 'Module: tests/unit/mcp/tools/utils/test_r37ck_deep_nesting_docstring.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/tools/utils/test_r37ck_deep_nesting_docstring.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.tools.utils.test_r37ck_deep_nesting_docstring`/TestDeepNestingDocstringSuppression#
symbols:
  TestDeepNestingDocstringSuppression.test_indented_docstring_continuation_does_not_count: test_indented_docstring_continuation_does_not_count().
  TestDeepNestingDocstringSuppression.test_real_nesting_still_detected: test_real_nesting_still_detected().
  TestDeepNestingDocstringSuppression.test_module_docstring_indented_arg_table_does_not_count: test_module_docstring_indented_arg_table_does_not_count().
  TestDeepNestingDocstringSuppression: ''
---
# Module: [`tests/unit/mcp/tools/utils/test_r37ck_deep_nesting_docstring.py`](../../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/utils/test_r37ck_deep_nesting_docstring.py)

## Classes
### `TestDeepNestingDocstringSuppression`
- def: [`tests/unit/mcp/tools/utils/test_r37ck_deep_nesting_docstring.py:16`](../../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/utils/test_r37ck_deep_nesting_docstring.py#L16)
- doc: Indented continuation lines inside docstrings must not inflate depth.
- signature: `class TestDeepNestingDocstringSuppression:`
- members:
  - `test_indented_docstring_continuation_does_not_count(self)` — [`L19`](../../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/utils/test_r37ck_deep_nesting_docstring.py#L19)
  - `test_module_docstring_indented_arg_table_does_not_count(self)` — [`L55`](../../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/utils/test_r37ck_deep_nesting_docstring.py#L55) — The bug seen in health_scorer.py:321 — argument table inside docstring.
  - `test_real_nesting_still_detected(self)` — [`L39`](../../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/utils/test_r37ck_deep_nesting_docstring.py#L39) — Sanity — the docstring skip must not blind us to actual indents.
- uses (calls/refs, reference-scoped): [`deepest_nesting_location`](../../../../../tree_sitter_analyzer/mcp/tools/utils/file_health_locations.md#deepest_nesting_location)

