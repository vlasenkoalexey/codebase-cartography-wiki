---
title: 'Module: tests/cobol_mainframe/test_cobol_dag_architect.py'
type: catalog
provenance: extracted
module: tests/cobol_mainframe/test_cobol_dag_architect.py
status: fresh
symbol_base: scip-python python gitgalaxy 0.0.0 `tests.cobol_mainframe.test_cobol_dag_architect`/test_
symbols:
  test_ghost_deflector_lineage: ghost_deflector_lineage().
  test_dag_architect_topological_sort: dag_architect_topological_sort().
  test_dag_architect_cycle_detection: dag_architect_cycle_detection().
---
# Module: [`tests/cobol_mainframe/test_cobol_dag_architect.py`](../../../../../../raw/code/gitgalaxy/tests/cobol_mainframe/test_cobol_dag_architect.py)

## Functions
- `test_dag_architect_cycle_detection(tmp_path, capsys)` — [`L111`](../../../../../../raw/code/gitgalaxy/tests/cobol_mainframe/test_cobol_dag_architect.py#L111) — Proves the engine catches circular data dependencies and halts execution
- `test_dag_architect_topological_sort(tmp_path, capsys)` — [`L57`](../../../../../../raw/code/gitgalaxy/tests/cobol_mainframe/test_cobol_dag_architect.py#L57) — Proves Kahn's Algorithm perfectly calculates execution order by resolving
- `test_ghost_deflector_lineage(tmp_path)` — [`L12`](../../../../../../raw/code/gitgalaxy/tests/cobol_mainframe/test_cobol_dag_architect.py#L12) — Proves the lineage extractor correctly maps DD assignments, strips prefixes,

