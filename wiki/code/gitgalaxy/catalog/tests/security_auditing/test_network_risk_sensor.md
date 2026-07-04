---
title: 'Module: tests/security_auditing/test_network_risk_sensor.py'
type: catalog
provenance: extracted
module: tests/security_auditing/test_network_risk_sensor.py
status: fresh
symbol_base: scip-python python gitgalaxy 0.0.0 `tests.security_auditing.test_network_risk_sensor`/
symbols:
  sensor: sensor().
  parsed_files_universe: parsed_files_universe().
  test_network_isolated_island: test_network_isolated_island().
  test_network_cyclic_loop_resilience: test_network_cyclic_loop_resilience().
  test_network_ecosystem_roles: test_network_ecosystem_roles().
  test_network_algorithmic_bottleneck: test_network_algorithmic_bottleneck().
  MOCK_PARSED_FILES: MOCK_PARSED_FILES.
  test_network_fallback_mode: test_network_fallback_mode().
---
# Module: [`tests/security_auditing/test_network_risk_sensor.py`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_network_risk_sensor.py)

## Functions
- `parsed_files_universe()` — [`L63`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_network_risk_sensor.py#L63) — Returns a fresh copy of the mock universe for each test.
- `sensor()` — [`L57`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_network_risk_sensor.py#L57) — Initializes the Network Risk Sensor.
- `test_network_algorithmic_bottleneck(sensor, parsed_files_universe)` — [`L144`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_network_risk_sensor.py#L144) — Proves that a file requires BOTH high network gravity (PageRank > 1.0)
- `test_network_cyclic_loop_resilience(sensor, parsed_files_universe)` — [`L93`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_network_risk_sensor.py#L93) — Proves that A -> B -> A loops do not crash the PageRank / Graph traversal.
- `test_network_ecosystem_roles(sensor, parsed_files_universe)` — [`L113`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_network_risk_sensor.py#L113) — Proves the engine accurately classifies Producers, Consumers, and Transceivers.
- `test_network_fallback_mode(sensor, parsed_files_universe)` — [`L173`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_network_risk_sensor.py#L173) — Proves the fallback mode safely maps roles without NetworkX installed.
- `test_network_isolated_island(sensor, parsed_files_universe)` — [`L72`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_network_risk_sensor.py#L72) — Proves that a node with 0 edges does not trigger divide-by-zero math.

## Module values
- `MOCK_PARSED_FILES` — [`L14`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_network_risk_sensor.py#L14)

