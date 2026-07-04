---
title: 'Module: tests/cobol_mainframe/test_cobol_microservice_slicer.py'
type: catalog
provenance: extracted
module: tests/cobol_mainframe/test_cobol_microservice_slicer.py
status: fresh
symbol_base: scip-python python gitgalaxy 0.0.0 `tests.cobol_mainframe.test_cobol_microservice_slicer`/test_slicer_
symbols:
  test_slicer_recursive_tainting: recursive_tainting().
  test_slicer_ghost_deflector: ghost_deflector().
  test_slicer_orphaned_memory_abort: orphaned_memory_abort().
  test_slicer_cli_e2e: cli_e2e().
---
# Module: [`tests/cobol_mainframe/test_cobol_microservice_slicer.py`](../../../../../../raw/code/gitgalaxy/tests/cobol_mainframe/test_cobol_microservice_slicer.py)

## Functions
- `test_slicer_cli_e2e(tmp_path, capsys)` — [`L107`](../../../../../../raw/code/gitgalaxy/tests/cobol_mainframe/test_cobol_microservice_slicer.py#L107) — Proves the CLI wrapper correctly formats the extracted slice into terminal output.
- `test_slicer_ghost_deflector(tmp_path)` — [`L47`](../../../../../../raw/code/gitgalaxy/tests/cobol_mainframe/test_cobol_microservice_slicer.py#L47) — Proves that the slicer uses the IR RAM (dead_paras) to mathematically blind
- `test_slicer_orphaned_memory_abort(tmp_path)` — [`L82`](../../../../../../raw/code/gitgalaxy/tests/cobol_mainframe/test_cobol_microservice_slicer.py#L82) — Proves that if the Graveyard Reaper identifies the variable as dead memory,
- `test_slicer_recursive_tainting(tmp_path)` — [`L11`](../../../../../../raw/code/gitgalaxy/tests/cobol_mainframe/test_cobol_microservice_slicer.py#L11) — Proves that the engine successfully chains taints across multiple operations

