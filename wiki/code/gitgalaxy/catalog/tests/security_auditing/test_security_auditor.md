---
title: 'Module: tests/security_auditing/test_security_auditor.py'
type: catalog
provenance: extracted
module: tests/security_auditing/test_security_auditor.py
status: fresh
symbol_base: scip-python python gitgalaxy 0.0.0 `tests.security_auditing.test_security_auditor`/
symbols:
  test_audit_repository_threshold_gating: test_audit_repository_threshold_gating().
  test_construct_feature_matrix: test_construct_feature_matrix().
  test_audit_repository_ml_inference: test_audit_repository_ml_inference().
  test_audit_repository_fatal_desync: test_audit_repository_fatal_desync().
  test_construct_feature_matrix_exclusion_list: test_construct_feature_matrix_exclusion_list().
  MOCK_SCHEMAS: MOCK_SCHEMAS.
  test_dependency_graph_pure_python: test_dependency_graph_pure_python().
  test_dependency_graph_networkx: test_dependency_graph_networkx().
  test_construct_feature_matrix_exception_fallback: test_construct_feature_matrix_exception_fallback().
  test_audit_repository_no_model: test_audit_repository_no_model().
  test_audit_repository_empty_state: test_audit_repository_empty_state().
  mock_artifacts: mock_artifacts().
---
# Module: [`tests/security_auditing/test_security_auditor.py`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_security_auditor.py)

## Functions
- `mock_artifacts()` — [`L13`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_security_auditor.py#L13) — Provides a baseline payload with a circular dependency to test the graph resolver.
- `test_audit_repository_empty_state()` — [`L226`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_security_auditor.py#L226) — Proves the auditor safely exits without crashing if the repository has 0 artifacts.
- `test_audit_repository_fatal_desync(mock_xgb_class, mock_artifacts)` — [`L150`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_security_auditor.py#L150) — Proves the engine aborts cleanly if XGBoost returns the wrong number of rows.
- `test_audit_repository_ml_inference(mock_xgb_class, mock_artifacts)` — [`L104`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_security_auditor.py#L104) — Proves the orchestrator successfully formats data, predicts Multiclass threats,
- `test_audit_repository_no_model(mock_artifacts)` — [`L167`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_security_auditor.py#L167) — Proves the engine gracefully skips ML if the model file is missing.
- `test_audit_repository_threshold_gating(mock_xgb_class, mock_artifacts)` — [`L181`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_security_auditor.py#L181) — Proves that a threat prediction below the strict AI_THREAT_THRESHOLD is safely ignored.
- `test_construct_feature_matrix(mock_artifacts)` — [`L69`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_security_auditor.py#L69) — Proves the matrix builder accurately maps artifact metrics to a Pandas DataFrame.
- `test_construct_feature_matrix_exception_fallback()` — [`L86`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_security_auditor.py#L86) — Proves a corrupted artifact payload generates a safe, empty fallback row.
- `test_construct_feature_matrix_exclusion_list(mock_artifacts)` — [`L206`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_security_auditor.py#L206) — Ensures noisy signals (like indentation factions) are stripped before ML evaluation.
- `test_dependency_graph_networkx(mock_artifacts)` — [`L55`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_security_auditor.py#L55) — Proves the C-optimized NetworkX resolver handles the exact same circular loop.
- `test_dependency_graph_pure_python(mock_artifacts)` — [`L41`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_security_auditor.py#L41) — Proves the pure-Python O(1) Deque resolver survives circular dependencies.

## Module values
- `MOCK_SCHEMAS` — [`L6`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_security_auditor.py#L6)

