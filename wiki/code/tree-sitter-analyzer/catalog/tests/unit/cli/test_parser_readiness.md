---
title: 'Module: tests/unit/cli/test_parser_readiness.py'
type: catalog
provenance: extracted
module: tests/unit/cli/test_parser_readiness.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.cli.test_parser_readiness`/
symbols:
  _is_error_envelope: _is_error_envelope().
  TestInvalidLanguageNamesRejected.test_path_traversal_rejected: TestInvalidLanguageNamesRejected#test_path_traversal_rejected().
  TestInvalidLanguageNamesRejected.test_shell_injection_semicolon_rejected: TestInvalidLanguageNamesRejected#test_shell_injection_semicolon_rejected().
  TestInvalidLanguageNamesRejected.test_shell_injection_pipe_rejected: TestInvalidLanguageNamesRejected#test_shell_injection_pipe_rejected().
  TestInvalidLanguageNamesRejected.test_uppercase_language_rejected: TestInvalidLanguageNamesRejected#test_uppercase_language_rejected().
  TestInvalidLanguageNamesRejected.test_empty_language_rejected: TestInvalidLanguageNamesRejected#test_empty_language_rejected().
  TestInvalidLanguageNamesRejected.test_space_in_language_rejected: TestInvalidLanguageNamesRejected#test_space_in_language_rejected().
  TestVerificationCommandsSanitized.test_verification_commands_safe_for_python: TestVerificationCommandsSanitized#test_verification_commands_safe_for_python().
  TestVerificationCommandsSanitized.test_verification_commands_safe_for_swift: TestVerificationCommandsSanitized#test_verification_commands_safe_for_swift().
  TestInvalidLanguageNamesRejected.test_garbage_language_name_returns_validation_error: TestInvalidLanguageNamesRejected#test_garbage_language_name_returns_validation_error().
  TestValidLanguageStillWorks.test_python_language_succeeds: TestValidLanguageStillWorks#test_python_language_succeeds().
  TestValidLanguageStillWorks.test_javascript_language_succeeds: TestValidLanguageStillWorks#test_javascript_language_succeeds().
  TestLangNameRegex.test_valid_names_match: TestLangNameRegex#test_valid_names_match().
  TestLangNameRegex.test_invalid_names_do_not_match: TestLangNameRegex#test_invalid_names_do_not_match().
  TestParserPackageWarnings.test_warnings_field_exists_on_response: TestParserPackageWarnings#test_warnings_field_exists_on_response().
  TestParserPackageWarnings.test_real_project_has_dogfood_warnings: TestParserPackageWarnings#test_real_project_has_dogfood_warnings().
  TestParserPackageWarnings.test_warning_entry_shape: TestParserPackageWarnings#test_warning_entry_shape().
  TestParserReadinessReportedCount.test_reported_count_matches_non_empty_readiness_list: TestParserReadinessReportedCount#test_reported_count_matches_non_empty_readiness_list().
  TestParserReadinessReportedCount.test_no_gap_report_uses_implemented_language_count: TestParserReadinessReportedCount#test_no_gap_report_uses_implemented_language_count().
  TestParserReadinessMatrixTruth.test_plugin_entrypoint_without_parser_package_is_reported: TestParserReadinessMatrixTruth#test_plugin_entrypoint_without_parser_package_is_reported().
  _SHELL_SPECIAL: _SHELL_SPECIAL.
  TestInvalidLanguageNamesRejected: TestInvalidLanguageNamesRejected#
  TestValidLanguageStillWorks: TestValidLanguageStillWorks#
  TestVerificationCommandsSanitized: TestVerificationCommandsSanitized#
  TestLangNameRegex: TestLangNameRegex#
  TestParserPackageWarnings: TestParserPackageWarnings#
  TestParserReadinessReportedCount: TestParserReadinessReportedCount#
  TestParserReadinessMatrixTruth: TestParserReadinessMatrixTruth#
---
# Module: [`tests/unit/cli/test_parser_readiness.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness.py)

## Classes
### `TestInvalidLanguageNamesRejected`
- def: [`tests/unit/cli/test_parser_readiness.py:42`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness.py#L42)
- doc: G5: garbage / path-traversal / injection language names are rejected.
- signature: `class TestInvalidLanguageNamesRejected:`
- members:
  - `test_empty_language_rejected(self, tmp_path)` — [`L96`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness.py#L96) — Empty / whitespace-only language must be rejected.
  - `test_garbage_language_name_returns_validation_error(self, tmp_path)` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness.py#L45) — 'fakelang' is not a real language; must return success=False.
  - `test_path_traversal_rejected(self, tmp_path)` — [`L63`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness.py#L63) — '../etc/passwd' must be rejected by the regex gate.
  - `test_shell_injection_pipe_rejected(self, tmp_path)` — [`L82`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness.py#L82) — 'fake|malicious' must be rejected by the regex gate.
  - `test_shell_injection_semicolon_rejected(self, tmp_path)` — [`L73`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness.py#L73) — 'fake; rm -rf /tmp/x' must be rejected by the regex gate.
  - `test_space_in_language_rejected(self, tmp_path)` — [`L103`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness.py#L103) — Language names containing spaces are rejected.
  - `test_uppercase_language_rejected(self, tmp_path)` — [`L89`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness.py#L89) — Uppercase characters are rejected — regex requires [a-z] start.
- uses (calls/refs, reference-scoped): [`build_parser_readiness_advice`](../../../tree_sitter_analyzer/cli/parser_readiness.md#build_parser_readiness_advice)  (1 test-only)

### `TestLangNameRegex`
- def: [`tests/unit/cli/test_parser_readiness.py:178`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness.py#L178)
- doc: Direct unit tests for the _LANG_NAME_RE constant.
- signature: `class TestLangNameRegex:`
- members:
  - `test_invalid_names_do_not_match(self, name)` — [`L222`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness.py#L222)
  - `test_valid_names_match(self, name)` — [`L200`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness.py#L200)
- uses (calls/refs, reference-scoped): [`_LANG_NAME_RE`](../../../tree_sitter_analyzer/cli/parser_readiness.md#_LANG_NAME_RE)

### `TestParserPackageWarnings`
- def: [`tests/unit/cli/test_parser_readiness.py:233`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness.py#L233)
- doc: r37o: parser_readiness must flag duplicate parser declarations.
- signature: `class TestParserPackageWarnings:`
- members:
  - `test_real_project_has_dogfood_warnings(self)` — [`L263`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness.py#L263) — On our own pyproject.toml: must surface known redundancies.
  - `test_warning_entry_shape(self)` — [`L281`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness.py#L281) — Each warning entry must have the documented field set.
  - `test_warnings_field_exists_on_response(self, tmp_path)` — [`L252`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness.py#L252) — Even a project with NO duplicates must expose the empty list.
- uses (calls/refs, reference-scoped): [`build_parser_readiness_advice`](../../../tree_sitter_analyzer/cli/parser_readiness.md#build_parser_readiness_advice)

### `TestParserReadinessMatrixTruth`
- def: [`tests/unit/cli/test_parser_readiness.py:335`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness.py#L335)
- doc: The roadmap must report every broken side of the support matrix.
- signature: `class TestParserReadinessMatrixTruth:`
- members:
  - `test_plugin_entrypoint_without_parser_package_is_reported(self, tmp_path)` — [`L338`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness.py#L338)
- uses (calls/refs, reference-scoped): [`build_parser_readiness_advice`](../../../tree_sitter_analyzer/cli/parser_readiness.md#build_parser_readiness_advice)

### `TestParserReadinessReportedCount`
- def: [`tests/unit/cli/test_parser_readiness.py:307`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness.py#L307)
- doc: Dogfood contract: reported counts must describe the emitted records.
- signature: `class TestParserReadinessReportedCount:`
- members:
  - `test_no_gap_report_uses_implemented_language_count(self)` — [`L323`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness.py#L323)
  - `test_reported_count_matches_non_empty_readiness_list(self)` — [`L310`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness.py#L310)
- uses (calls/refs, reference-scoped): [`_ensure_no_gap_consistency`](../../../tree_sitter_analyzer/cli/parser_readiness.md#_ensure_no_gap_consistency)

### `TestValidLanguageStillWorks`
- def: [`tests/unit/cli/test_parser_readiness.py:116`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness.py#L116)
- doc: A valid language name must produce a successful (non-error) response.
- signature: `class TestValidLanguageStillWorks:`
- members:
  - `test_javascript_language_succeeds(self, tmp_path)` — [`L128`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness.py#L128) — 'javascript' is a valid language token; must not produce a validation error.
  - `test_python_language_succeeds(self, tmp_path)` — [`L119`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness.py#L119) — 'python' is a valid language token; the call must not return an error.
- uses (calls/refs, reference-scoped): [`build_parser_readiness_advice`](../../../tree_sitter_analyzer/cli/parser_readiness.md#build_parser_readiness_advice)

### `TestVerificationCommandsSanitized`
- def: [`tests/unit/cli/test_parser_readiness.py:141`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness.py#L141)
- doc: G10: verification_commands for valid languages contain no shell specials.
- signature: `class TestVerificationCommandsSanitized:`
- members:
  - `test_verification_commands_safe_for_python(self, tmp_path)` — [`L144`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness.py#L144) — verification_commands for 'python' must not contain shell metacharacters.
  - `test_verification_commands_safe_for_swift(self, tmp_path)` — [`L158`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness.py#L158) — verification_commands for 'swift' must not contain shell metacharacters.
- uses (calls/refs, reference-scoped): [`build_parser_readiness_advice`](../../../tree_sitter_analyzer/cli/parser_readiness.md#build_parser_readiness_advice)  (1 test-only)

## Functions
- `_is_error_envelope(result: dict)` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness.py#L27) — Return True when result is a canonical validation error envelope.

## Module values
- `_SHELL_SPECIAL` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness.py#L24)

