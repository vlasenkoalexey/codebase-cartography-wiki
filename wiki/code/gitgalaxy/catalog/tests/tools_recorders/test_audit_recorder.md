---
title: 'Module: tests/tools_recorders/test_audit_recorder.py'
type: catalog
provenance: extracted
module: tests/tools_recorders/test_audit_recorder.py
status: fresh
symbol_base: scip-python python gitgalaxy 0.0.0 `tests.tools_recorders.test_audit_recorder`/
symbols:
  recorder: recorder().
  test_audit_recorder_format_label_and_descale: test_audit_recorder_format_label_and_descale().
  test_audit_recorder_generate_ml_threat_report: test_audit_recorder_generate_ml_threat_report().
  test_audit_recorder_rule_based_threat_routing: test_audit_recorder_rule_based_threat_routing().
  test_audit_recorder_formatting_edge_cases: test_audit_recorder_formatting_edge_cases().
  test_audit_recorder_empty_state: test_audit_recorder_empty_state().
---
# Module: [`tests/tools_recorders/test_audit_recorder.py`](../../../../../../raw/code/gitgalaxy/tests/tools_recorders/test_audit_recorder.py)

## Functions
- `recorder()` — [`L8`](../../../../../../raw/code/gitgalaxy/tests/tools_recorders/test_audit_recorder.py#L8) — Initializes the AuditRecorder for forensic JSON generation testing.
- `test_audit_recorder_empty_state(recorder, tmp_path)` — [`L181`](../../../../../../raw/code/gitgalaxy/tests/tools_recorders/test_audit_recorder.py#L181) — Proves the JSON generator survives a completely empty repository.
- `test_audit_recorder_format_label_and_descale(recorder)` — [`L27`](../../../../../../raw/code/gitgalaxy/tests/tools_recorders/test_audit_recorder.py#L27) — Proves the recorder correctly strips internal suffixes and scales metrics.
- `test_audit_recorder_formatting_edge_cases(recorder, tmp_path)` — [`L134`](../../../../../../raw/code/gitgalaxy/tests/tools_recorders/test_audit_recorder.py#L134) — Proves the recorder dynamically pads missing Markdown risk vectors to prevent
- `test_audit_recorder_generate_ml_threat_report(recorder, tmp_path)` — [`L38`](../../../../../../raw/code/gitgalaxy/tests/tools_recorders/test_audit_recorder.py#L38) — Proves the recorder prioritizes ML threats, processes Parser Bypasses,
- `test_audit_recorder_rule_based_threat_routing(recorder, tmp_path)` — [`L103`](../../../../../../raw/code/gitgalaxy/tests/tools_recorders/test_audit_recorder.py#L103) — Proves that if XGBoost clears a file, but the rule-based engine flags a

