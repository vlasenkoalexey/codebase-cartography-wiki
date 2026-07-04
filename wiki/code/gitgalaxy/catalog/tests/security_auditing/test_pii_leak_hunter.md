---
title: 'Module: tests/security_auditing/test_pii_leak_hunter.py'
type: catalog
provenance: extracted
module: tests/security_auditing/test_pii_leak_hunter.py
status: fresh
symbol_base: scip-python python gitgalaxy 0.0.0 `tests.security_auditing.test_pii_leak_hunter`/test_
symbols:
  test_pii_masking_engine: pii_masking_engine().
  test_pii_leak_hunter_e2e: pii_leak_hunter_e2e().
  test_missing_target_argument: missing_target_argument().
  test_invalid_target_path: invalid_target_path().
  test_custom_output_directory: custom_output_directory().
  test_clean_log_processing: clean_log_processing().
  test_output_directory_permission_error: output_directory_permission_error().
---
# Module: [`tests/security_auditing/test_pii_leak_hunter.py`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_pii_leak_hunter.py)

## Functions
- `test_clean_log_processing(tmp_path, capsys)` — [`L147`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_pii_leak_hunter.py#L147) — Proves the tool processes safe logs without generating false evidence data.
- `test_custom_output_directory(tmp_path)` — [`L125`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_pii_leak_hunter.py#L125) — Verifies that the --out argument redirects the evidence log successfully.
- `test_invalid_target_path(tmp_path, capsys)` — [`L108`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_pii_leak_hunter.py#L108) — Ensures the tool exits cleanly when provided a non-existent file.
- `test_missing_target_argument(capsys)` — [`L93`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_pii_leak_hunter.py#L93) — Ensures the CLI gracefully exits when no target is provided.
- `test_output_directory_permission_error(tmp_path, capsys)` — [`L169`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_pii_leak_hunter.py#L169) — Simulates a scenario where the application lacks rights to create the output folder.
- `test_pii_leak_hunter_e2e(tmp_path)` — [`L39`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_pii_leak_hunter.py#L39) — End-to-End test simulating a live log stream.
- `test_pii_masking_engine()` — [`L12`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_pii_leak_hunter.py#L12) — Mathematically verifies that the regex engine correctly intercepts and

