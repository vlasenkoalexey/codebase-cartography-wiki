---
title: 'Module: tests/unit/formatters/test_sql_formatter_wrapper_extraction.py'
type: catalog
provenance: extracted
module: tests/unit/formatters/test_sql_formatter_wrapper_extraction.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.formatters.test_sql_formatter_wrapper_extraction`/
symbols:
  formatter: formatter().
  TestExtractTableColumns: TestExtractTableColumns#
  TestExtractTableColumns.test_extract_simple_columns: TestExtractTableColumns#test_extract_simple_columns().
  TestExtractTableColumns.test_extract_columns_with_constraints: TestExtractTableColumns#test_extract_columns_with_constraints().
  TestExtractTableColumns.test_extract_columns_skip_keywords: TestExtractTableColumns#test_extract_columns_skip_keywords().
  TestExtractViewInfo: TestExtractViewInfo#
  TestExtractViewInfo.test_extract_simple_view: TestExtractViewInfo#test_extract_simple_view().
  TestExtractViewInfo.test_extract_view_with_join: TestExtractViewInfo#test_extract_view_with_join().
  TestExtractProcedureInfo: TestExtractProcedureInfo#
  TestExtractProcedureInfo.test_extract_simple_procedure: TestExtractProcedureInfo#test_extract_simple_procedure().
  TestExtractProcedureInfo.test_extract_procedure_with_dependencies: TestExtractProcedureInfo#test_extract_procedure_with_dependencies().
  TestExtractFunctionInfo: TestExtractFunctionInfo#
  TestExtractFunctionInfo.test_extract_simple_function: TestExtractFunctionInfo#test_extract_simple_function().
  TestExtractFunctionInfo.test_extract_function_with_dependencies: TestExtractFunctionInfo#test_extract_function_with_dependencies().
  TestExtractTriggerInfo: TestExtractTriggerInfo#
  TestExtractTriggerInfo.test_extract_before_update_trigger: TestExtractTriggerInfo#test_extract_before_update_trigger().
  TestExtractTriggerInfo.test_extract_after_insert_trigger: TestExtractTriggerInfo#test_extract_after_insert_trigger().
  TestExtractTriggerInfo.test_extract_trigger_with_dependencies: TestExtractTriggerInfo#test_extract_trigger_with_dependencies().
  TestExtractIndexInfo: TestExtractIndexInfo#
  TestExtractIndexInfo.test_extract_simple_index: TestExtractIndexInfo#test_extract_simple_index().
  TestExtractIndexInfo.test_extract_unique_index: TestExtractIndexInfo#test_extract_unique_index().
  TestExtractIndexInfo.test_extract_composite_index: TestExtractIndexInfo#test_extract_composite_index().
---
# Module: [`tests/unit/formatters/test_sql_formatter_wrapper_extraction.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_extraction.py)

## Classes
### `TestExtractFunctionInfo`
- def: [`tests/unit/formatters/test_sql_formatter_wrapper_extraction.py:104`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_extraction.py#L104)
- doc: Test _extract_function_info method.
- signature: `class TestExtractFunctionInfo:`
- members:
  - `test_extract_function_with_dependencies(self, formatter)` — [`L119`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_extraction.py#L119) — Test extraction of function with table dependencies.
  - `test_extract_simple_function(self, formatter)` — [`L107`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_extraction.py#L107) — Test extraction of simple function info.

### `TestExtractIndexInfo`
- def: [`tests/unit/formatters/test_sql_formatter_wrapper_extraction.py:176`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_extraction.py#L176)
- doc: Test _extract_index_info method.
- signature: `class TestExtractIndexInfo:`
- members:
  - `test_extract_composite_index(self, formatter)` — [`L193`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_extraction.py#L193) — Test extraction of composite index info.
  - `test_extract_simple_index(self, formatter)` — [`L179`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_extraction.py#L179) — Test extraction of simple index info.
  - `test_extract_unique_index(self, formatter)` — [`L187`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_extraction.py#L187) — Test extraction of unique index info.

### `TestExtractProcedureInfo`
- def: [`tests/unit/formatters/test_sql_formatter_wrapper_extraction.py:76`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_extraction.py#L76)
- doc: Test _extract_procedure_info method.
- signature: `class TestExtractProcedureInfo:`
- members:
  - `test_extract_procedure_with_dependencies(self, formatter)` — [`L90`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_extraction.py#L90) — Test extraction of procedure with table dependencies.
  - `test_extract_simple_procedure(self, formatter)` — [`L79`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_extraction.py#L79) — Test extraction of simple procedure info.

### `TestExtractTableColumns`
- def: [`tests/unit/formatters/test_sql_formatter_wrapper_extraction.py:15`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_extraction.py#L15)
- doc: Test _extract_table_columns method.
- signature: `class TestExtractTableColumns:`
- members:
  - `test_extract_columns_skip_keywords(self, formatter)` — [`L43`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_extraction.py#L43) — Test that keywords are skipped.
  - `test_extract_columns_with_constraints(self, formatter)` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_extraction.py#L29) — Test extraction with constraints.
  - `test_extract_simple_columns(self, formatter)` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_extraction.py#L18) — Test extraction of simple columns.

### `TestExtractTriggerInfo`
- def: [`tests/unit/formatters/test_sql_formatter_wrapper_extraction.py:132`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_extraction.py#L132)
- doc: Test _extract_trigger_info method.
- signature: `class TestExtractTriggerInfo:`
- members:
  - `test_extract_after_insert_trigger(self, formatter)` — [`L148`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_extraction.py#L148) — Test extraction of AFTER INSERT trigger.
  - `test_extract_before_update_trigger(self, formatter)` — [`L135`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_extraction.py#L135) — Test extraction of BEFORE UPDATE trigger.
  - `test_extract_trigger_with_dependencies(self, formatter)` — [`L161`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_extraction.py#L161) — Test extraction of trigger with additional dependencies.

### `TestExtractViewInfo`
- def: [`tests/unit/formatters/test_sql_formatter_wrapper_extraction.py:55`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_extraction.py#L55)
- doc: Test _extract_view_info method.
- signature: `class TestExtractViewInfo:`
- members:
  - `test_extract_simple_view(self, formatter)` — [`L58`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_extraction.py#L58) — Test extraction of simple view info.
  - `test_extract_view_with_join(self, formatter)` — [`L64`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_extraction.py#L64) — Test extraction of view with JOIN.

## Functions
- `formatter()` — [`L11`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_extraction.py#L11)

