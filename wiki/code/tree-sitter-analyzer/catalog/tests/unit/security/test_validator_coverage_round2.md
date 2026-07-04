---
title: 'Module: tests/unit/security/test_validator_coverage_round2.py'
type: catalog
provenance: extracted
module: tests/unit/security/test_validator_coverage_round2.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.security.test_validator_coverage_round2`/TestValidatorCoverageRound2#
symbols:
  TestValidatorCoverageRound2.test_symlink_original_path_rejected: test_symlink_original_path_rejected().
  TestValidatorCoverageRound2.test_junction_original_path_rejected: test_junction_original_path_rejected().
  TestValidatorCoverageRound2.test_symlink_check_oserror_fallback: test_symlink_check_oserror_fallback().
  TestValidatorCoverageRound2.test_full_path_symlink_rejected: test_full_path_symlink_rejected().
  TestValidatorCoverageRound2.test_junction_in_path_hierarchy_rejected: test_junction_in_path_hierarchy_rejected().
  TestValidatorCoverageRound2.test_junction_hierarchy_oserror_fallback: test_junction_hierarchy_oserror_fallback().
  TestValidatorCoverageRound2.test_no_base_path_junction_hierarchy_rejected: test_no_base_path_junction_hierarchy_rejected().
  TestValidatorCoverageRound2.test_no_base_path_junction_oserror_fallback: test_no_base_path_junction_oserror_fallback().
  TestValidatorCoverageRound2.test_path_traversal_regex_error: test_path_traversal_regex_error().
  TestValidatorCoverageRound2.test_validate_absolute_path_test_env_not_allowed: test_validate_absolute_path_test_env_not_allowed().
  TestValidatorCoverageRound2.test_validate_file_path_absolute_denied: test_validate_file_path_absolute_denied().
  TestValidatorCoverageRound2.test_windows_drive_letter_pass_through: test_windows_drive_letter_pass_through().
  TestValidatorCoverageRound2.test_is_junction_non_windows: test_is_junction_non_windows().
  TestValidatorCoverageRound2.test_has_ctypes_false_on_import_error: test_has_ctypes_false_on_import_error().
  TestValidatorCoverageRound2: ''
---
# Module: [`tests/unit/security/test_validator_coverage_round2.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator_coverage_round2.py)

## Classes
### `TestValidatorCoverageRound2`
- def: [`tests/unit/security/test_validator_coverage_round2.py:13`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator_coverage_round2.py#L13)
- doc: Additional coverage for remaining uncovered branches.
- signature: `class TestValidatorCoverageRound2:`
- members:
  - `test_full_path_symlink_rejected(self, mock_log)` — [`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator_coverage_round2.py#L65) — Lines 165-166: symlink in full path (base_path + file_path).
  - `test_has_ctypes_false_on_import_error(self)` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator_coverage_round2.py#L18) — Test that HAS_CTYPES is False when ctypes import fails.
  - `test_is_junction_non_windows(self)` — [`L202`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator_coverage_round2.py#L202) — Non-Windows systems always return False.
  - `test_junction_hierarchy_oserror_fallback(self)` — [`L91`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator_coverage_round2.py#L91) — Line 187: OSError during junction hierarchy check.
  - `test_junction_in_path_hierarchy_rejected(self, mock_log_warning)` — [`L77`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator_coverage_round2.py#L77) — Lines 183-184: junction in path hierarchy returns False.
  - `test_junction_original_path_rejected(self, mock_log)` — [`L40`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator_coverage_round2.py#L40) — Lines 146-149: junction in original path returns False.
  - `test_no_base_path_junction_hierarchy_rejected(self)` — [`L105`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator_coverage_round2.py#L105) — Lines 195-197: junction in hierarchy when no base_path.
  - `test_no_base_path_junction_oserror_fallback(self)` — [`L131`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator_coverage_round2.py#L131) — Line 199: OSError during junction check without base_path.
  - `test_path_traversal_regex_error(self, mock_re)` — [`L158`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator_coverage_round2.py#L158) — Lines 387-389: regex error during traversal check.
  - `test_symlink_check_oserror_fallback(self)` — [`L52`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator_coverage_round2.py#L52) — Lines 151-154: OSError during symlink check is caught.
  - `test_symlink_original_path_rejected(self, mock_log)` — [`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator_coverage_round2.py#L31) — Line 140: symlink in original path returns False.
  - `test_validate_absolute_path_test_env_not_allowed(self)` — [`L168`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator_coverage_round2.py#L168) — Line 549: test env check returns non-empty error.
  - `test_validate_file_path_absolute_denied(self)` — [`L181`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator_coverage_round2.py#L181) — Line 126: absolute path validation fails within validate_file_path.
  - `test_windows_drive_letter_pass_through(self)` — [`L193`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator_coverage_round2.py#L193) — Normal paths pass through windows drive letter check.
- uses (calls/refs, reference-scoped): [`SecurityValidator`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator), [`validate_file_path`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator.validate_file_path), [`_validate_absolute_path`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator._validate_absolute_path), [`HAS_CTYPES`](../../../tree_sitter_analyzer/security/validator.md#HAS_CTYPES), [`_is_junction_or_reparse_point`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator._is_junction_or_reparse_point), [`_validate_path_traversal`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator._validate_path_traversal), [`_validate_windows_drive_letter`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator._validate_windows_drive_letter)

