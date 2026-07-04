---
title: 'Module: tests/core_engine/test_licensing.py'
type: catalog
provenance: extracted
module: tests/core_engine/test_licensing.py
status: fresh
symbol_base: scip-python python gitgalaxy 0.0.0 `tests.core_engine.test_licensing`/test_
symbols:
  test_licensing_pytest_bypass: licensing_pytest_bypass().
  test_licensing_env_loader: licensing_env_loader().
  test_licensing_env_loader_exception: licensing_env_loader_exception().
  test_validate_key_missing_or_malformed: validate_key_missing_or_malformed().
  test_validate_key_cryptographic_authenticity: validate_key_cryptographic_authenticity().
  test_routing_community_tier: routing_community_tier().
  test_routing_valid_enterprise_tier: routing_valid_enterprise_tier().
  test_routing_forgery_hammer: routing_forgery_hammer().
---
# Module: [`tests/core_engine/test_licensing.py`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_licensing.py)

## Functions
- `test_licensing_env_loader(mock_exists, monkeypatch)` — [`L28`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_licensing.py#L28) — Proves the custom .env loader parses variables without overriding existing ones.
- `test_licensing_env_loader_exception(mock_exists, monkeypatch)` — [`L56`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_licensing.py#L56) — Proves OS permission errors on the .env file are swallowed gracefully.
- `test_licensing_pytest_bypass(monkeypatch, capsys)` — [`L10`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_licensing.py#L10) — Proves the Pytest bypass was successfully removed and strict compliance is enforced. — documented in [gitgalaxy-licensing](../../../concepts/gitgalaxy-licensing.md)
- `test_routing_community_tier(monkeypatch, capsys)` — [`L138`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_licensing.py#L138) — Proves the Community tier logs the audit tripwire with NO sleep penalty. — documented in [gitgalaxy-licensing](../../../concepts/gitgalaxy-licensing.md)
- `test_routing_forgery_hammer(mock_validate, monkeypatch, capsys)` — [`L167`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_licensing.py#L167) — Proves forged keys trigger the maximum 10-second penalty. — documented in [gitgalaxy-licensing](../../../concepts/gitgalaxy-licensing.md)
- `test_routing_valid_enterprise_tier(mock_validate, monkeypatch, capsys)` — [`L152`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_licensing.py#L152) — Proves a valid enterprise key executes silently with NO sleep penalty. — documented in [gitgalaxy-licensing](../../../concepts/gitgalaxy-licensing.md)
- `test_validate_key_cryptographic_authenticity(mock_pow)` — [`L93`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_licensing.py#L93) — Proves the engine authenticates exact hash matches and correctly evaluates dates. — documented in [gitgalaxy-licensing](../../../concepts/gitgalaxy-licensing.md)
- `test_validate_key_missing_or_malformed()` — [`L76`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_licensing.py#L76) — Proves empty, malformed, or tampered keys are flagged accurately. — documented in [gitgalaxy-licensing](../../../concepts/gitgalaxy-licensing.md)

