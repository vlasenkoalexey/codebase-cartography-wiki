---
title: 'Module: gitgalaxy/cobol_refractor_controller.py'
type: catalog
provenance: extracted
module: gitgalaxy/cobol_refractor_controller.py
status: fresh
symbol_base: scip-python python gitgalaxy 0.0.0 `gitgalaxy.cobol_refractor_controller`/
symbols:
  process_payload: process_payload().
  main: main().
  IRStateManager.conn: IRStateManager#conn.
  IRStateManager.get_orphaned_vars: IRStateManager#get_orphaned_vars().
  IRStateManager.record_dead_code: IRStateManager#record_dead_code().
  IRStateManager.get_dead_paras: IRStateManager#get_dead_paras().
  IRStateManager.db_file: IRStateManager#db_file.
  IRStateManager.mode: IRStateManager#mode.
  IRStateManager: IRStateManager#
  IRStateManager.close: IRStateManager#close().
  IRStateManager._init_sql_schema: IRStateManager#_init_sql_schema().
  calibrate_ir_medium: calibrate_ir_medium().
  IRStateManager.ram_ir: IRStateManager#ram_ir.
  IRStateManager.__init__: IRStateManager#__init__().
---
# Module: [`gitgalaxy/cobol_refractor_controller.py`](../../../../../raw/code/gitgalaxy/gitgalaxy/cobol_refractor_controller.py)

## Classes
### `IRStateManager`
- def: [`gitgalaxy/cobol_refractor_controller.py:58`](../../../../../raw/code/gitgalaxy/gitgalaxy/cobol_refractor_controller.py#L58) — documented in [gitgalaxy-cobol_refractor_controller](../../concepts/gitgalaxy-cobol_refractor_controller.md)
- doc: Abstracts the IR storage so the spoke tools don't have to care if it's RAM or SQL.
- signature: `class IRStateManager:`
- members:
  - `_init_sql_schema(self)` — [`L71`](../../../../../raw/code/gitgalaxy/gitgalaxy/cobol_refractor_controller.py#L71) — Sets up the relational structure for the massive codebase. (Maintains legacy schema names for downstream compatibility) — documented in [gitgalaxy-cobol_refractor_controller](../../concepts/gitgalaxy-cobol_refractor_controller.md)
  - `close(self)` — [`L126`](../../../../../raw/code/gitgalaxy/gitgalaxy/cobol_refractor_controller.py#L126)
  - `get_dead_paras(self, program_id: str)` — [`L104`](../../../../../raw/code/gitgalaxy/gitgalaxy/cobol_refractor_controller.py#L104) — documented in [gitgalaxy-cobol_refractor_controller](../../concepts/gitgalaxy-cobol_refractor_controller.md)
  - `get_orphaned_vars(self, program_id: str)` — [`L115`](../../../../../raw/code/gitgalaxy/gitgalaxy/cobol_refractor_controller.py#L115) — documented in [gitgalaxy-cobol_refractor_controller](../../concepts/gitgalaxy-cobol_refractor_controller.md)
  - `record_dead_code(self, program_id: str, dead_paras: set, orphaned_vars: set)` — [`L84`](../../../../../raw/code/gitgalaxy/gitgalaxy/cobol_refractor_controller.py#L84) — documented in [gitgalaxy-cobol_refractor_controller](../../concepts/gitgalaxy-cobol_refractor_controller.md)
  - `conn` — [`L64`](../../../../../raw/code/gitgalaxy/gitgalaxy/cobol_refractor_controller.py#L64) — documented in [gitgalaxy-cobol_refractor_controller](../../concepts/gitgalaxy-cobol_refractor_controller.md)
  - `db_file` — [`L67`](../../../../../raw/code/gitgalaxy/gitgalaxy/cobol_refractor_controller.py#L67) — documented in [gitgalaxy-cobol_refractor_controller](../../concepts/gitgalaxy-cobol_refractor_controller.md)
  - `mode` — [`L62`](../../../../../raw/code/gitgalaxy/gitgalaxy/cobol_refractor_controller.py#L62) — documented in [gitgalaxy-cobol_refractor_controller](../../concepts/gitgalaxy-cobol_refractor_controller.md)
  - `ram_ir` — [`L63`](../../../../../raw/code/gitgalaxy/gitgalaxy/cobol_refractor_controller.py#L63) — documented in [gitgalaxy-cobol_refractor_controller](../../concepts/gitgalaxy-cobol_refractor_controller.md)
- protocol/private: `__init__`[`L61`](../../../../../raw/code/gitgalaxy/gitgalaxy/cobol_refractor_controller.py#L61)
- used by: [`process_payload`](cobol_refractor_controller.md#process_payload), [`main`](cobol_refractor_controller.md#main)  (3 test-only)

## Functions
- `calibrate_ir_medium(target_path: Path, max_files=2000, max_mb=200)` — [`L38`](../../../../../raw/code/gitgalaxy/gitgalaxy/cobol_refractor_controller.py#L38) — Scouts the repository to determine the safest IR storage medium. — documented in [gitgalaxy-cobol_refractor_controller](../../concepts/gitgalaxy-cobol_refractor_controller.md)
- `main()` — [`L237`](../../../../../raw/code/gitgalaxy/gitgalaxy/cobol_refractor_controller.py#L237) — documented in [gitgalaxy-cobol_refractor_controller](../../concepts/gitgalaxy-cobol_refractor_controller.md)
- `process_payload(filepath: Path, state_manager: IRStateManager, target_var: str = None)` — [`L136`](../../../../../raw/code/gitgalaxy/gitgalaxy/cobol_refractor_controller.py#L136) — Processes a single COBOL payload through the enriched, shared-state pipeline. — documented in [gitgalaxy-cobol_refractor_controller](../../concepts/gitgalaxy-cobol_refractor_controller.md)

