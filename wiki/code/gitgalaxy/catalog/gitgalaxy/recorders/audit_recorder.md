---
title: 'Module: gitgalaxy/recorders/audit_recorder.py'
type: catalog
provenance: extracted
module: gitgalaxy/recorders/audit_recorder.py
status: fresh
symbol_base: scip-python python gitgalaxy 0.0.0 `gitgalaxy.recorders.audit_recorder`/
symbols:
  AuditRecorder.generate_report: AuditRecorder#generate_report().
  AuditRecorder.format_label: AuditRecorder#format_label().
  parser: parser.
  AuditRecorder.RISK_SCHEMA: AuditRecorder#RISK_SCHEMA.
  AuditRecorder: AuditRecorder#
  AuditRecorder.HIT_SCHEMA: AuditRecorder#HIT_SCHEMA.
  AuditRecorder._label_cache: AuditRecorder#_label_cache.
  args: args.
  AuditRecorder.logger: AuditRecorder#logger.
  AuditRecorder._friendly_map: AuditRecorder#_friendly_map.
  AuditRecorder.__init__: AuditRecorder#__init__().
  AuditRecorder.descale: AuditRecorder#descale().
  decode_galaxy: decode_galaxy().
---
# Module: [`gitgalaxy/recorders/audit_recorder.py`](../../../../../../raw/code/gitgalaxy/gitgalaxy/recorders/audit_recorder.py)

## Classes
### `AuditRecorder`
- def: [`gitgalaxy/recorders/audit_recorder.py:25`](../../../../../../raw/code/gitgalaxy/gitgalaxy/recorders/audit_recorder.py#L25)
- doc: Forensic Audit Recorder.
- signature: `class AuditRecorder:`
- members:
  - `descale(self, key: str, value: Any, default_scalar: float = 1)` — [`L63`](../../../../../../raw/code/gitgalaxy/gitgalaxy/recorders/audit_recorder.py#L63) — Dynamically scales integers back to floats using a fixed-string check.
  - `format_label(self, key: str)` — [`L49`](../../../../../../raw/code/gitgalaxy/gitgalaxy/recorders/audit_recorder.py#L49) — Translates raw dictionary keys into descriptive human-readable labels.
  - `generate_report(self, parsed_files, unparsable_files, summary, forensic_report, session_meta, output_path)` — [`L77`](../../../../../../raw/code/gitgalaxy/gitgalaxy/recorders/audit_recorder.py#L77) — Transforms raw pipeline state into a verbose forensic compliance manifest. — documented in [gitgalaxy-galaxyscope](../../../concepts/gitgalaxy-galaxyscope.md)
  - `HIT_SCHEMA` — [`L43`](../../../../../../raw/code/gitgalaxy/gitgalaxy/recorders/audit_recorder.py#L43)
  - `RISK_SCHEMA` — [`L41`](../../../../../../raw/code/gitgalaxy/gitgalaxy/recorders/audit_recorder.py#L41)
  - `logger` — [`L37`](../../../../../../raw/code/gitgalaxy/gitgalaxy/recorders/audit_recorder.py#L37)
- protocol/private: `__init__`[`L34`](../../../../../../raw/code/gitgalaxy/gitgalaxy/recorders/audit_recorder.py#L34), `_friendly_map`[`L47`](../../../../../../raw/code/gitgalaxy/gitgalaxy/recorders/audit_recorder.py#L47), `_label_cache`[`L46`](../../../../../../raw/code/gitgalaxy/gitgalaxy/recorders/audit_recorder.py#L46)
- used by: [`execute_pipeline`](../galaxyscope.md#Orchestrator.execute_pipeline), [`audit_recorder`](../galaxyscope.md#Orchestrator.audit_recorder)  (1 test-only)

## Functions
- `decode_galaxy(input_path, output_path=None)` — [`L570`](../../../../../../raw/code/gitgalaxy/gitgalaxy/recorders/audit_recorder.py#L570) — Standalone decoding logic preserved for CLI compatibility.

## Module values
- `args` — [`L579`](../../../../../../raw/code/gitgalaxy/gitgalaxy/recorders/audit_recorder.py#L579)
- `parser` — [`L576`](../../../../../../raw/code/gitgalaxy/gitgalaxy/recorders/audit_recorder.py#L576)

