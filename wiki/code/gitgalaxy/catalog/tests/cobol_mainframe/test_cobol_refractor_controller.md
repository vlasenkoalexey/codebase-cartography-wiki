---
title: 'Module: tests/cobol_mainframe/test_cobol_refractor_controller.py'
type: catalog
provenance: extracted
module: tests/cobol_mainframe/test_cobol_refractor_controller.py
status: fresh
symbol_base: scip-python python gitgalaxy 0.0.0 `tests.cobol_mainframe.test_cobol_refractor_controller`/test_
symbols:
  test_ir_state_manager_parity: ir_state_manager_parity().
  test_process_payload_integration: process_payload_integration().
  test_process_payload_corporate_header_and_exception: process_payload_corporate_header_and_exception().
  test_scale_sensor_calibration: scale_sensor_calibration().
  test_main_missing_target: main_missing_target().
  test_main_empty_target: main_empty_target().
  test_main_full_orchestration: main_full_orchestration().
---
# Module: [`tests/cobol_mainframe/test_cobol_refractor_controller.py`](../../../../../../raw/code/gitgalaxy/tests/cobol_mainframe/test_cobol_refractor_controller.py)

## Functions
- `test_ir_state_manager_parity(tmp_path)` — [`L42`](../../../../../../raw/code/gitgalaxy/tests/cobol_mainframe/test_cobol_refractor_controller.py#L42) — Proves that the IR abstraction layer perfectly mirrors data retrieval — documented in [gitgalaxy-cobol_refractor_controller](../../../concepts/gitgalaxy-cobol_refractor_controller.md)
- `test_main_empty_target(tmp_path, capsys)` — [`L157`](../../../../../../raw/code/gitgalaxy/tests/cobol_mainframe/test_cobol_refractor_controller.py#L157) — Proves the CLI safely exits (code 0) if no COBOL code is found to refract. — documented in [gitgalaxy-cobol_refractor_controller](../../../concepts/gitgalaxy-cobol_refractor_controller.md)
- `test_main_full_orchestration(tmp_path, capsys)` — [`L173`](../../../../../../raw/code/gitgalaxy/tests/cobol_mainframe/test_cobol_refractor_controller.py#L173) — Proves the orchestrator successfully creates the Clean Room environment,
- `test_main_missing_target(capsys)` — [`L144`](../../../../../../raw/code/gitgalaxy/tests/cobol_mainframe/test_cobol_refractor_controller.py#L144) — Proves the CLI gracefully aborts if the legacy directory doesn't exist.
- `test_process_payload_corporate_header_and_exception(tmp_path)` — [`L112`](../../../../../../raw/code/gitgalaxy/tests/cobol_mainframe/test_cobol_refractor_controller.py#L112) — Proves the payload processor injects corporate headers and survives locked files. — documented in [gitgalaxy-cobol_refractor_controller](../../../concepts/gitgalaxy-cobol_refractor_controller.md)
- `test_process_payload_integration(tmp_path)` — [`L73`](../../../../../../raw/code/gitgalaxy/tests/cobol_mainframe/test_cobol_refractor_controller.py#L73) — Proves the orchestrator successfully routes a file through the sub-tools — documented in [gitgalaxy-cobol_refractor_controller](../../../concepts/gitgalaxy-cobol_refractor_controller.md)
- `test_scale_sensor_calibration(tmp_path)` — [`L11`](../../../../../../raw/code/gitgalaxy/tests/cobol_mainframe/test_cobol_refractor_controller.py#L11) — Proves the orchestrator accurately calculates repository mass and dynamically

