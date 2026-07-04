---
title: 'Module: tests/security_auditing/test_supply_chain_firewall.py'
type: catalog
provenance: extracted
module: tests/security_auditing/test_supply_chain_firewall.py
status: fresh
symbol_base: scip-python python gitgalaxy 0.0.0 `tests.security_auditing.test_supply_chain_firewall`/test_
symbols:
  test_zero_trust_import_verification: zero_trust_import_verification().
  test_import_truncation_and_local_shield: import_truncation_and_local_shield().
  test_alias_spoofing_detection: alias_spoofing_detection().
  test_strict_mode_enforcement: strict_mode_enforcement().
  test_behavioral_threat_evaluation: behavioral_threat_evaluation().
  test_build_time_execution_multiplier: build_time_execution_multiplier().
  test_main_missing_target: main_missing_target().
  test_main_corrupted_json: main_corrupted_json().
---
# Module: [`tests/security_auditing/test_supply_chain_firewall.py`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_supply_chain_firewall.py)

## Functions
- `test_alias_spoofing_detection(monkeypatch, capsys)` — [`L70`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_supply_chain_firewall.py#L70) — Validates that the firewall correctly detects when a safe alias is mapped
- `test_behavioral_threat_evaluation(tmp_path, monkeypatch)` — [`L127`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_supply_chain_firewall.py#L127) — Validates that artifacts exhibiting high-density threat indicators
- `test_build_time_execution_multiplier(monkeypatch)` — [`L159`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_supply_chain_firewall.py#L159) — Ensures that critical build files (like setup.py) have their risk equations
- `test_import_truncation_and_local_shield(monkeypatch)` — [`L45`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_supply_chain_firewall.py#L45) — Ensures that local relative imports are ignored, and deeply nested
- `test_main_corrupted_json(tmp_path, capsys)` — [`L207`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_supply_chain_firewall.py#L207) — Ensures the firewall gracefully exits if the input graph is malformed.
- `test_main_missing_target(capsys)` — [`L194`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_supply_chain_firewall.py#L194) — Proves the CLI catches invalid directories and exits safely.
- `test_strict_mode_enforcement(tmp_path, monkeypatch)` — [`L100`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_supply_chain_firewall.py#L100) — Ensures that when STRICT_IMPORT_MODE is enabled, any unknown dependency
- `test_zero_trust_import_verification(monkeypatch)` — [`L11`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_supply_chain_firewall.py#L11) — Validates that the firewall correctly segregates imports into approved,

