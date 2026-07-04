---
title: 'Module: tests/security_auditing/test_binary_anomaly_detector.py'
type: catalog
provenance: extracted
module: tests/security_auditing/test_binary_anomaly_detector.py
status: fresh
symbol_base: scip-python python gitgalaxy 0.0.0 `tests.security_auditing.test_binary_anomaly_detector`/test_
symbols:
  test_xray_deep_scan_threats: xray_deep_scan_threats().
  test_main_clean_run: main_clean_run().
  test_xray_import_fallback: xray_import_fallback().
  test_xray_routing_matrix: xray_routing_matrix().
  test_xray_shebang_shield: xray_shebang_shield().
  test_xray_run_audit_exception: xray_run_audit_exception().
  test_main_missing_target: main_missing_target().
  test_main_anomaly_detected: main_anomaly_detected().
  test_main_file_read_exception: main_file_read_exception().
  test_xray_test_folder_bypass: xray_test_folder_bypass().
  test_xray_deep_scan_threats.mock_scan_binary: xray_deep_scan_threats().mock_scan_binary().
  test_xray_deep_scan_threats.mock_scan_content: xray_deep_scan_threats().mock_scan_content().
  test_main_clean_run.mock_scan_content: main_clean_run().mock_scan_content().
---
# Module: [`tests/security_auditing/test_binary_anomaly_detector.py`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_binary_anomaly_detector.py)

## Functions
- `mock_scan_binary(head_bytes, ext)` — [`L70`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_binary_anomaly_detector.py#L70)
- `mock_scan_content(content, limit)` — [`L77`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_binary_anomaly_detector.py#L77)
- `mock_scan_content(content, limit)` — [`L170`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_binary_anomaly_detector.py#L170)
- `test_main_anomaly_detected(mock_aperture_class, mock_security_class, tmp_path, monkeypatch, capsys)` — [`L201`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_binary_anomaly_detector.py#L201) — Proves the CLI detects active anomalies, blocks the commit, and logs the blocking action.
- `test_main_clean_run(mock_aperture_class, mock_security_class, tmp_path, monkeypatch, capsys)` — [`L158`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_binary_anomaly_detector.py#L158) — Proves a clean repository successfully logs completion without raising SystemExit.
- `test_main_file_read_exception(mock_aperture_class, mock_security_class, tmp_path)` — [`L239`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_binary_anomaly_detector.py#L239) — Triggers the generic 'except Exception: pass' inside the deep scan loop of main().
- `test_main_missing_target(capsys)` — [`L142`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_binary_anomaly_detector.py#L142) — Proves the CLI catches invalid directories and exits safely.
- `test_xray_deep_scan_threats(mock_aperture_class, mock_security_class, tmp_path)` — [`L55`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_binary_anomaly_detector.py#L55)
- `test_xray_import_fallback()` — [`L256`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_binary_anomaly_detector.py#L256) — Proves the module gracefully degrades if custom bypass arrays are missing from config. — documented in [gitgalaxy-standards-gitgalaxy_config](../../../concepts/gitgalaxy-standards-gitgalaxy_config.md)
- `test_xray_routing_matrix(mock_aperture_class, mock_security_class, tmp_path, monkeypatch)` — [`L14`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_binary_anomaly_detector.py#L14)
- `test_xray_run_audit_exception(mock_aperture_class, mock_security_class, tmp_path)` — [`L123`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_binary_anomaly_detector.py#L123)
- `test_xray_shebang_shield(mock_aperture_class, mock_security_class, tmp_path)` — [`L96`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_binary_anomaly_detector.py#L96)
- `test_xray_test_folder_bypass(mock_aperture_class, mock_security_class, tmp_path, capsys)` — [`L287`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_binary_anomaly_detector.py#L287) — Proves that high entropy mock files placed within test directories are safely ignored.

