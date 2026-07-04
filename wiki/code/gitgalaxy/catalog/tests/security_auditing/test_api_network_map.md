---
title: 'Module: tests/security_auditing/test_api_network_map.py'
type: catalog
provenance: extracted
module: tests/security_auditing/test_api_network_map.py
status: fresh
symbol_base: scip-python python gitgalaxy 0.0.0 `tests.security_auditing.test_api_network_map`/test_
symbols:
  test_framework_regex_extraction: framework_regex_extraction().
  test_endpoint_variable_extraction: endpoint_variable_extraction().
  test_swagger_parser_yaml_and_corruption: swagger_parser_yaml_and_corruption().
  test_swagger_parser_edge_cases: swagger_parser_edge_cases().
  test_auto_discover_files: auto_discover_files().
  test_auto_discover_directories: auto_discover_directories().
  test_physical_mapper_exception_handling: physical_mapper_exception_handling().
  test_cli_missing_target: cli_missing_target().
  test_cli_no_swagger_found: cli_no_swagger_found().
  test_cli_ambiguous_swaggers: cli_ambiguous_swaggers().
  test_cli_ambiguous_merge_all: cli_ambiguous_merge_all().
  test_cli_explicit_swagger_flag: cli_explicit_swagger_flag().
  test_cli_presentation_dashboard_findings: cli_presentation_dashboard_findings().
  test_cli_presentation_dashboard_perfect: cli_presentation_dashboard_perfect().
  test_programmatic_edge_cases: programmatic_edge_cases().
  test_programmatic_success: programmatic_success().
---
# Module: [`tests/security_auditing/test_api_network_map.py`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_api_network_map.py)

## Functions
- `test_auto_discover_directories(tmp_path)` — [`L171`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_api_network_map.py#L171) — Verifies that the auto-discovery engine recursively searches all directories.
- `test_auto_discover_files(tmp_path)` — [`L147`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_api_network_map.py#L147) — Verifies the engine finds exact filenames OR deep-greps for OpenAPI signatures.
- `test_cli_ambiguous_merge_all(tmp_path, capsys)` — [`L270`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_api_network_map.py#L270) — Verifies the --merge-all flag unifies multiple schemas into one verified state.
- `test_cli_ambiguous_swaggers(tmp_path, capsys)` — [`L246`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_api_network_map.py#L246) — Verifies the CLI halts and requires intervention if multiple primary schemas exist.
- `test_cli_explicit_swagger_flag(tmp_path, capsys)` — [`L300`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_api_network_map.py#L300) — Verifies the --swagger flag bypasses discovery, handling both valid and invalid paths.
- `test_cli_missing_target(capsys)` — [`L219`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_api_network_map.py#L219) — Verifies the CLI aborts gracefully if the target directory doesn't exist.
- `test_cli_no_swagger_found(tmp_path, capsys)` — [`L231`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_api_network_map.py#L231) — Verifies the CLI aborts gracefully if auto-discovery finds zero schemas.
- `test_cli_presentation_dashboard_findings(tmp_path, capsys)` — [`L327`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_api_network_map.py#L327) — Verifies the CLI successfully prints the full Shadow/Ghost API dashboard.
- `test_cli_presentation_dashboard_perfect(tmp_path, capsys)` — [`L357`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_api_network_map.py#L357) — Verifies the CLI correctly displays a clean bill of health when schemas and code match.
- `test_endpoint_variable_extraction(tmp_path)` — [`L57`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_api_network_map.py#L57) — Verifies that different framework syntaxes for path variables are extracted as-is.
- `test_framework_regex_extraction(tmp_path)` — [`L18`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_api_network_map.py#L18) — Verifies the physical mapper correctly extracts endpoints from all supported backends.
- `test_physical_mapper_exception_handling(tmp_path)` — [`L203`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_api_network_map.py#L203) — Verifies the physical mapper skips unreadable or corrupted files without crashing.
- `test_programmatic_edge_cases(tmp_path)` — [`L378`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_api_network_map.py#L378) — Verifies the programmatic entry point safely returns structured error states.
- `test_programmatic_success(tmp_path)` — [`L400`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_api_network_map.py#L400) — Verifies the programmatic entry point successfully maps a standard repo.
- `test_swagger_parser_edge_cases(tmp_path)` — [`L111`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_api_network_map.py#L111) — Verifies the parser survives schemas without paths and grabs all path keys.
- `test_swagger_parser_yaml_and_corruption(tmp_path, capsys)` — [`L86`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_api_network_map.py#L86) — Verifies the parser handles YAML specs and correctly exits on file corruption.

