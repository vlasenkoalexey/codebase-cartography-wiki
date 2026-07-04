---
title: 'Module: tests/security_auditing/test_terabyte_log_scanner.py'
type: catalog
provenance: extracted
module: tests/security_auditing/test_terabyte_log_scanner.py
status: fresh
symbol_base: scip-python python gitgalaxy 0.0.0 `tests.security_auditing.test_terabyte_log_scanner`/test_
symbols:
  test_scanner_json_ingestion_and_extraction: scanner_json_ingestion_and_extraction().
  test_scanner_invalid_json_schema: scanner_invalid_json_schema().
  test_scanner_manual_keyword_override: scanner_manual_keyword_override().
  test_missing_target_argument: missing_target_argument().
  test_invalid_target_path: invalid_target_path().
  test_missing_state_file: missing_state_file().
  test_empty_known_programs: empty_known_programs().
  test_custom_output_directory: custom_output_directory().
---
# Module: [`tests/security_auditing/test_terabyte_log_scanner.py`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_terabyte_log_scanner.py)

## Functions
- `test_custom_output_directory(tmp_path)` — [`L238`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_terabyte_log_scanner.py#L238) — Verifies that the --out argument redirects the generated files successfully.
- `test_empty_known_programs(tmp_path, capsys)` — [`L205`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_terabyte_log_scanner.py#L205) — Ensures the tool exits cleanly (code 0) if the known_programs array is empty.
- `test_invalid_target_path(tmp_path, capsys)` — [`L159`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_terabyte_log_scanner.py#L159) — Ensures the tool exits cleanly when provided a non-existent file.
- `test_missing_state_file(tmp_path, capsys)` — [`L176`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_terabyte_log_scanner.py#L176) — Ensures the tool exits cleanly when the specified --input_state file is missing.
- `test_missing_target_argument(capsys)` — [`L144`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_terabyte_log_scanner.py#L144) — Ensures the CLI gracefully exits when no target is provided.
- `test_scanner_invalid_json_schema(tmp_path)` — [`L80`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_terabyte_log_scanner.py#L80) — Proves that if a malformed or incorrect JSON schema is provided, the
- `test_scanner_json_ingestion_and_extraction(tmp_path)` — [`L13`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_terabyte_log_scanner.py#L13) — Validates that the scanner correctly parses the IR state JSON, extracts the targets,
- `test_scanner_manual_keyword_override(tmp_path)` — [`L113`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_terabyte_log_scanner.py#L113) — Proves that the scanner can bypass the JSON input state and process

