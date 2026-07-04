---
title: 'Module: gitgalaxy/tools/cobol_to_cobol/cobol_jcl_auditor.py'
type: catalog
provenance: extracted
module: gitgalaxy/tools/cobol_to_cobol/cobol_jcl_auditor.py
status: fresh
symbol_base: scip-python python gitgalaxy 0.0.0 `gitgalaxy.tools.cobol_to_cobol.cobol_jcl_auditor`/
symbols:
  parse_jcl_intent: parse_jcl_intent().
  main: main().
  audit_zero_trust_jcls: audit_zero_trust_jcls().
  SYSTEM_DDS: SYSTEM_DDS.
  SYSTEM_PGMS: SYSTEM_PGMS.
---
# Module: [`gitgalaxy/tools/cobol_to_cobol/cobol_jcl_auditor.py`](../../../../../../../raw/code/gitgalaxy/gitgalaxy/tools/cobol_to_cobol/cobol_jcl_auditor.py)

## Functions
- `audit_zero_trust_jcls(generated_dir: Path, original_dir: Path)` — [`L75`](../../../../../../../raw/code/gitgalaxy/gitgalaxy/tools/cobol_to_cobol/cobol_jcl_auditor.py#L75) — Core logic to calculate architectural bloat and privilege reduction metrics. — documented in [gitgalaxy-cobol_refractor_controller](../../../../concepts/gitgalaxy-cobol_refractor_controller.md)
- `main()` — [`L140`](../../../../../../../raw/code/gitgalaxy/gitgalaxy/tools/cobol_to_cobol/cobol_jcl_auditor.py#L140)
- `parse_jcl_intent(filepath: Path)` — [`L45`](../../../../../../../raw/code/gitgalaxy/gitgalaxy/tools/cobol_to_cobol/cobol_jcl_auditor.py#L45) — Parses a JCL file to extract its raw execution and dataset allocation intent.

## Module values
- `SYSTEM_DDS` — [`L23`](../../../../../../../raw/code/gitgalaxy/gitgalaxy/tools/cobol_to_cobol/cobol_jcl_auditor.py#L23)
- `SYSTEM_PGMS` — [`L33`](../../../../../../../raw/code/gitgalaxy/gitgalaxy/tools/cobol_to_cobol/cobol_jcl_auditor.py#L33)

