---
title: 'Module: tests/security_auditing/test_vault_sentinel.py'
type: catalog
provenance: extracted
module: tests/security_auditing/test_vault_sentinel.py
status: fresh
symbol_base: scip-python python gitgalaxy 0.0.0 `tests.security_auditing.test_vault_sentinel`/test_
symbols:
  test_ignore_rules_traversal: ignore_rules_traversal().
  test_sentinel_denylist_blocking: sentinel_denylist_blocking().
  test_sentinel_content_breach: sentinel_content_breach().
  test_sentinel_allowlist_bypass: sentinel_allowlist_bypass().
  test_unreadable_file_handling: unreadable_file_handling().
  test_main_missing_target: main_missing_target().
  test_ignore_rules_traversal.mock_check_ignore: ignore_rules_traversal().mock_check_ignore().
---
# Module: [`tests/security_auditing/test_vault_sentinel.py`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_vault_sentinel.py)

## Functions
- `mock_check_ignore(rel_path)` — [`L140`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_vault_sentinel.py#L140)
- `test_ignore_rules_traversal(mock_aperture_class, mock_security_class, tmp_path, monkeypatch, capsys)` — [`L127`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_vault_sentinel.py#L127) — Ensures that os.walk is properly mutated to completely skip directories
- `test_main_missing_target(capsys)` — [`L206`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_vault_sentinel.py#L206) — Proves the CLI catches invalid directories and exits safely.
- `test_sentinel_allowlist_bypass(mock_aperture_class, mock_security_class, tmp_path, monkeypatch, capsys)` — [`L80`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_vault_sentinel.py#L80) — Proves that if a file resides explicitly inside an ALLOWLIST_PATH, it completely
- `test_sentinel_content_breach(mock_aperture_class, mock_security_class, tmp_path, monkeypatch)` — [`L40`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_vault_sentinel.py#L40) — Proves that seemingly benign files are deeply scanned, and if the SAST engine
- `test_sentinel_denylist_blocking(mock_aperture_class, mock_security_class, tmp_path, monkeypatch)` — [`L12`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_vault_sentinel.py#L12) — Proves that files matching the DENYLIST_PATTERNS are instantly blocked
- `test_unreadable_file_handling(mock_aperture_class, mock_security_class, tmp_path, monkeypatch)` — [`L176`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_vault_sentinel.py#L176) — Validates that a file generating an I/O or Permission error during reading

