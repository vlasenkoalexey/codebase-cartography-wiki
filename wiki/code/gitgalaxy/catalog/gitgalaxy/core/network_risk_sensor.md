---
title: 'Module: gitgalaxy/core/network_risk_sensor.py'
type: catalog
provenance: extracted
module: gitgalaxy/core/network_risk_sensor.py
status: fresh
symbol_base: scip-python python gitgalaxy 0.0.0 `gitgalaxy.core.network_risk_sensor`/
symbols:
  HAS_NETWORKX: HAS_NETWORKX.
  NetworkRiskSensor.build_dependency_graph: NetworkRiskSensor#build_dependency_graph().
  NetworkRiskSensor.logger: NetworkRiskSensor#logger.
  NetworkRiskSensor: NetworkRiskSensor#
  NetworkRiskSensor.RISK_SCHEMA: NetworkRiskSensor#RISK_SCHEMA.
  NetworkRiskSensor._fallback_build_graph: NetworkRiskSensor#_fallback_build_graph().
  NetworkRiskSensor.extract_test_coverage_mapping: NetworkRiskSensor#extract_test_coverage_mapping().
  NetworkRiskSensor.__init__: NetworkRiskSensor#__init__().
---
# Module: [`gitgalaxy/core/network_risk_sensor.py`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/network_risk_sensor.py)

## Classes
### `NetworkRiskSensor`
- def: [`gitgalaxy/core/network_risk_sensor.py:21`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/network_risk_sensor.py#L21)
- doc: The GitGalaxy Network Risk Sensor (Graph Topology & Blast Radius).
- signature: `class NetworkRiskSensor:`
- members:
  - `build_dependency_graph(self, parsed_files: List[Dict[str, Any]])` — [`L102`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/network_risk_sensor.py#L102) — Builds the directed graph and calculates multi-dimensional risk vectors. — documented in [gitgalaxy-galaxyscope](../../../concepts/gitgalaxy-galaxyscope.md)
  - `extract_test_coverage_mapping(self, files: List[Dict[str, Any]])` — [`L34`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/network_risk_sensor.py#L34) — Maps function calls from test files to their imported production targets.
  - `RISK_SCHEMA` — [`L32`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/network_risk_sensor.py#L32) — documented in [gitgalaxy-standards-analysis_lens](../../../concepts/gitgalaxy-standards-analysis_lens.md)
  - `logger` — [`L31`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/network_risk_sensor.py#L31)
- protocol/private: `__init__`[`L30`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/network_risk_sensor.py#L30), `_fallback_build_graph`[`L328`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/network_risk_sensor.py#L328)
- uses (calls/refs, reference-scoped): [`HAS_NETWORKX`](network_risk_sensor.md#HAS_NETWORKX), [`RECORDING_SCHEMAS`](../standards/analysis_lens.md#RECORDING_SCHEMAS)
- used by: [`execute_pipeline`](../galaxyscope.md#Orchestrator.execute_pipeline), [`execute_incremental_scan`](../galaxyscope.md#Orchestrator.execute_incremental_scan), [`used_tokens`](../galaxyscope.md#Orchestrator.used_tokens), [`network_sensor`](../galaxyscope.md#Orchestrator.network_sensor)  (2 test-only)

## Module values
- `HAS_NETWORKX` — [`L11`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/network_risk_sensor.py#L11) — documented in [gitgalaxy-galaxyscope](../../../concepts/gitgalaxy-galaxyscope.md)

