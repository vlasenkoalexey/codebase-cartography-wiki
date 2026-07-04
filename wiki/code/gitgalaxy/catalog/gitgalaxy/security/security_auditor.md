---
title: 'Module: gitgalaxy/security/security_auditor.py'
type: catalog
provenance: extracted
module: gitgalaxy/security/security_auditor.py
status: fresh
symbol_base: scip-python python gitgalaxy 0.0.0 `gitgalaxy.security.security_auditor`/
symbols:
  SecurityAuditor.audit_repository: SecurityAuditor#audit_repository().
  SecurityAuditor.logger: SecurityAuditor#logger.
  SecurityAuditor.feature_names: SecurityAuditor#feature_names.
  SecurityAuditor: SecurityAuditor#
  ML_AVAILABLE: ML_AVAILABLE.
  SecurityAuditor._resolve_dependency_graph: SecurityAuditor#_resolve_dependency_graph().
  HAS_NETWORKX: HAS_NETWORKX.
  SecurityAuditor.ai_threshold: SecurityAuditor#ai_threshold.
  SecurityAuditor.model: SecurityAuditor#model.
  SecurityAuditor._construct_feature_matrix: SecurityAuditor#_construct_feature_matrix().
  SecurityAuditor.SIGNAL_SCHEMA: SecurityAuditor#SIGNAL_SCHEMA.
  SecurityAuditor.get_nth_degree: SecurityAuditor#get_nth_degree().
  SecurityAuditor.CLASS_NAMES: SecurityAuditor#CLASS_NAMES.
  SecurityAuditor.__init__: SecurityAuditor#__init__().
---
# Module: [`gitgalaxy/security/security_auditor.py`](../../../../../../raw/code/gitgalaxy/gitgalaxy/security/security_auditor.py)

## Classes
### `SecurityAuditor`
- def: [`gitgalaxy/security/security_auditor.py:28`](../../../../../../raw/code/gitgalaxy/gitgalaxy/security/security_auditor.py#L28) — documented in [gitgalaxy-galaxyscope](../../../concepts/gitgalaxy-galaxyscope.md)
- doc: Machine Learning Threat Inference Engine.
- signature: `class SecurityAuditor:`
- members:
  - `_construct_feature_matrix(self, artifacts)` — [`L290`](../../../../../../raw/code/gitgalaxy/gitgalaxy/security/security_auditor.py#L290) — Reconstructs the Pandas DataFrame exactly as train_threat_model.py did. — documented in [gitgalaxy-security-security_auditor](../../../concepts/gitgalaxy-security-security_auditor.md)
  - `_resolve_dependency_graph(self, artifacts)` — [`L186`](../../../../../../raw/code/gitgalaxy/gitgalaxy/security/security_auditor.py#L186) — Resolves transitive fragility and Downstream Exposure using C-optimized traversals (NetworkX) — documented in [gitgalaxy-security-security_auditor](../../../concepts/gitgalaxy-security-security_auditor.md)
  - `audit_repository(self, artifacts, is_shadow_patch=False)` — [`L94`](../../../../../../raw/code/gitgalaxy/gitgalaxy/security/security_auditor.py#L94) — Orchestrates the resolution of transitive dependency graphs and — documented in [gitgalaxy-galaxyscope](../../../concepts/gitgalaxy-galaxyscope.md)
  - `get_nth_degree(start, graph, max_nodes=500)` — [`L258`](../../../../../../raw/code/gitgalaxy/gitgalaxy/security/security_auditor.py#L258) — BFS using collections.deque for O(1) popping. — documented in [gitgalaxy-security-security_auditor](../../../concepts/gitgalaxy-security-security_auditor.md)
  - `CLASS_NAMES` — [`L39`](../../../../../../raw/code/gitgalaxy/gitgalaxy/security/security_auditor.py#L39) — documented in [gitgalaxy-security-security_auditor](../../../concepts/gitgalaxy-security-security_auditor.md)
  - `SIGNAL_SCHEMA` — [`L52`](../../../../../../raw/code/gitgalaxy/gitgalaxy/security/security_auditor.py#L52) — documented in [gitgalaxy-security-security_auditor](../../../concepts/gitgalaxy-security-security_auditor.md)
  - `ai_threshold` — [`L55`](../../../../../../raw/code/gitgalaxy/gitgalaxy/security/security_auditor.py#L55) — documented in [gitgalaxy-security-security_auditor](../../../concepts/gitgalaxy-security-security_auditor.md)
  - `feature_names` — [`L63`](../../../../../../raw/code/gitgalaxy/gitgalaxy/security/security_auditor.py#L63) — documented in [gitgalaxy-galaxyscope](../../../concepts/gitgalaxy-galaxyscope.md)
  - `logger` — [`L49`](../../../../../../raw/code/gitgalaxy/gitgalaxy/security/security_auditor.py#L49)
  - `model` — [`L62`](../../../../../../raw/code/gitgalaxy/gitgalaxy/security/security_auditor.py#L62) — documented in [gitgalaxy-security-security_auditor](../../../concepts/gitgalaxy-security-security_auditor.md)
- protocol/private: `__init__`[`L48`](../../../../../../raw/code/gitgalaxy/gitgalaxy/security/security_auditor.py#L48)
- uses (calls/refs, reference-scoped): [`ML_AVAILABLE`](security_auditor.md#ML_AVAILABLE), [`RECORDING_SCHEMAS`](../standards/analysis_lens.md#RECORDING_SCHEMAS), [`HAS_NETWORKX`](security_auditor.md#HAS_NETWORKX), [`AI_THREAT_THRESHOLD`](../standards/analysis_lens.md#AI_THREAT_THRESHOLD)
- used by: [`execute_pipeline`](../galaxyscope.md#Orchestrator.execute_pipeline), [`execute_incremental_scan`](../galaxyscope.md#Orchestrator.execute_incremental_scan), [`model_auditor`](../galaxyscope.md#Orchestrator.model_auditor)  (12 test-only)

## Module values
- `HAS_NETWORKX` — [`L21`](../../../../../../raw/code/gitgalaxy/gitgalaxy/security/security_auditor.py#L21) — documented in [gitgalaxy-security-security_auditor](../../../concepts/gitgalaxy-security-security_auditor.md)
- `ML_AVAILABLE` — [`L14`](../../../../../../raw/code/gitgalaxy/gitgalaxy/security/security_auditor.py#L14) — documented in [gitgalaxy-galaxyscope](../../../concepts/gitgalaxy-galaxyscope.md)

