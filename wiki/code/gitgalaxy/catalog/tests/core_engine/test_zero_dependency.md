---
title: 'Module: tests/core_engine/test_zero_dependency.py'
type: catalog
provenance: extracted
module: tests/core_engine/test_zero_dependency.py
status: fresh
symbol_base: scip-python python gitgalaxy 0.0.0 `tests.core_engine.test_zero_dependency`/TestZeroDependencyMode#
symbols:
  TestZeroDependencyMode.test_fallback_does_not_crash_signal_processor: test_fallback_does_not_crash_signal_processor().
  TestZeroDependencyMode.test_fallback_does_not_crash_security_auditor: test_fallback_does_not_crash_security_auditor().
  TestZeroDependencyMode: ''
---
# Module: [`tests/core_engine/test_zero_dependency.py`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_zero_dependency.py)

## Classes
### `TestZeroDependencyMode`  ·  implements/extends TestCase
- def: [`tests/core_engine/test_zero_dependency.py:8`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_zero_dependency.py#L8)
- signature: `class TestZeroDependencyMode(unittest.TestCase):`
- members:
  - `test_fallback_does_not_crash_security_auditor(self)` — [`L51`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_zero_dependency.py#L51) — Simulates a user running GalaxyScope without 'xgboost' or 'pandas' installed.
  - `test_fallback_does_not_crash_signal_processor(self)` — [`L10`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_zero_dependency.py#L10) — Simulates a user running GalaxyScope without 'networkx' installed. — documented in [gitgalaxy-metrics-signal_processor](../../../concepts/gitgalaxy-metrics-signal_processor.md)
- uses (calls/refs, reference-scoped): [`audit_repository`](../../gitgalaxy/security/security_auditor.md#SecurityAuditor.audit_repository), [`SignalProcessor`](../../gitgalaxy/metrics/signal_processor.md#SignalProcessor), [`summarize_galaxy_metrics`](../../gitgalaxy/metrics/signal_processor.md#SignalProcessor.summarize_galaxy_metrics), [`generate_forensic_report`](../../gitgalaxy/metrics/signal_processor.md#SignalProcessor.generate_forensic_report), [`SecurityAuditor`](../../gitgalaxy/security/security_auditor.md#SecurityAuditor), [`build_dependency_graph`](../../gitgalaxy/core/network_risk_sensor.md#NetworkRiskSensor.build_dependency_graph), [`NetworkRiskSensor`](../../gitgalaxy/core/network_risk_sensor.md#NetworkRiskSensor)

