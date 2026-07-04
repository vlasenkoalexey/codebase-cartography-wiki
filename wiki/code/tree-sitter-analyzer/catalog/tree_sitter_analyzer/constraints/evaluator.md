---
title: 'Module: tree_sitter_analyzer/constraints/evaluator.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/constraints/evaluator.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.constraints.evaluator`/
symbols:
  _iter_violations: _iter_violations().
  evaluate: evaluate().
  _is_excepted: _is_excepted().
  _build_import_index: _build_import_index().
  _callee_is_imported: _callee_is_imported().
  _build_select_sql: _build_select_sql().
  logger: logger.
---
# Module: [`tree_sitter_analyzer/constraints/evaluator.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/constraints/evaluator.py)

## Functions
- `_build_import_index(db_conn: sqlite3.Connection)` — [`L157`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/constraints/evaluator.py#L157) — Build a lookup of {file_path: set(module_path_suffixes)} from ast_imports.
- `_build_select_sql(db_conn: sqlite3.Connection)` — [`L226`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/constraints/evaluator.py#L226) — Build the per-DB SELECT statement over the unified ``edges`` table.
- `_callee_is_imported(caller_file: str, callee_file: str, import_index: dict[str, set[str]])` — [`L193`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/constraints/evaluator.py#L193) — Return True when the caller's import set covers the callee's module.
- `_is_excepted(caller_file: str, compiled: _CompiledConstraint)` — [`L145`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/constraints/evaluator.py#L145) — Return True when the caller is on the rule's exception list.
- `_iter_violations(compiled: list[_CompiledConstraint], db_conn: sqlite3.Connection, detected_at: int)` — [`L74`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/constraints/evaluator.py#L74) — Stream edges from the DB and yield matching violations.
- `evaluate(constraints: list[Constraint], db_conn: sqlite3.Connection)` — [`L45`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/constraints/evaluator.py#L45) — Evaluate constraints against the unified ``edges`` table (CALLS rows).

## Module values
- `logger` — [`L42`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/constraints/evaluator.py#L42)

