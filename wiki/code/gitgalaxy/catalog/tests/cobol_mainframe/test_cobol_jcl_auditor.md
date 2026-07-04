---
title: 'Module: tests/cobol_mainframe/test_cobol_jcl_auditor.py'
type: catalog
provenance: extracted
module: tests/cobol_mainframe/test_cobol_jcl_auditor.py
status: fresh
symbol_base: scip-python python gitgalaxy 0.0.0 `tests.cobol_mainframe.test_cobol_jcl_auditor`/test_
symbols:
  test_parse_jcl_intent: parse_jcl_intent().
  test_audit_zero_trust_jcls: audit_zero_trust_jcls().
  test_auditor_cli_json_output: auditor_cli_json_output().
---
# Module: [`tests/cobol_mainframe/test_cobol_jcl_auditor.py`](../../../../../../raw/code/gitgalaxy/tests/cobol_mainframe/test_cobol_jcl_auditor.py)

## Functions
- `test_audit_zero_trust_jcls(tmp_path)` — [`L56`](../../../../../../raw/code/gitgalaxy/tests/cobol_mainframe/test_cobol_jcl_auditor.py#L56) — Proves that the core audit loop correctly maps forged JCLs to their legacy
- `test_auditor_cli_json_output(tmp_path, capsys)` — [`L99`](../../../../../../raw/code/gitgalaxy/tests/cobol_mainframe/test_cobol_jcl_auditor.py#L99) — Proves the CLI wrapper correctly handles the --json flag, outputting pure
- `test_parse_jcl_intent(tmp_path)` — [`L12`](../../../../../../raw/code/gitgalaxy/tests/cobol_mainframe/test_cobol_jcl_auditor.py#L12) — Proves that the JCL parser correctly counts LOC while ignoring comments,

