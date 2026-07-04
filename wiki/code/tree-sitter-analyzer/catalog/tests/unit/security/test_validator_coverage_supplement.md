---
title: 'Module: tests/unit/security/test_validator_coverage_supplement.py'
type: catalog
provenance: extracted
module: tests/unit/security/test_validator_coverage_supplement.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.security.test_validator_coverage_supplement`/TestValidatorUncovered#
symbols:
  TestValidatorUncovered.test_boundary_manager_init_failure_fallback: test_boundary_manager_init_failure_fallback().
  TestValidatorUncovered.test_validate_project_boundary_outside_rejected: test_validate_project_boundary_outside_rejected().
  TestValidatorUncovered.test_validate_project_boundary_no_boundary_manager: test_validate_project_boundary_no_boundary_manager().
  TestValidatorUncovered.test_validate_file_path_windows_drive_letter_rejected: test_validate_file_path_windows_drive_letter_rejected().
  TestValidatorUncovered.test_validate_absolute_path_test_env_temp_pattern_match: test_validate_absolute_path_test_env_temp_pattern_match().
  TestValidatorUncovered.test_validate_absolute_path_test_env_multiple_temp_dirs: test_validate_absolute_path_test_env_multiple_temp_dirs().
  TestValidatorUncovered.test_validate_absolute_path_test_env_tmp_pattern: test_validate_absolute_path_test_env_tmp_pattern().
  TestValidatorUncovered.test_validate_file_path_none_input: test_validate_file_path_none_input().
  TestValidatorUncovered.test_validate_file_path_null_byte: test_validate_file_path_null_byte().
  TestValidatorUncovered.test_validate_absolute_path_test_env_exception_fallback: test_validate_absolute_path_test_env_exception_fallback().
  TestValidatorUncovered.test_validate_path_traversal_double_dot_slash: test_validate_path_traversal_double_dot_slash().
  TestValidatorUncovered.test_validate_path_traversal_dotdot_backslash: test_validate_path_traversal_dotdot_backslash().
  TestValidatorUncovered.test_validate_path_traversal_dotdot_start: test_validate_path_traversal_dotdot_start().
  TestValidatorUncovered.test_validate_project_boundary_no_base_path: test_validate_project_boundary_no_base_path().
  TestValidatorUncovered.test_validate_absolute_path_basic_denial: test_validate_absolute_path_basic_denial().
  TestValidatorUncovered: ''
---
# Module: [`tests/unit/security/test_validator_coverage_supplement.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator_coverage_supplement.py)

## Classes
### `TestValidatorUncovered`
- def: [`tests/unit/security/test_validator_coverage_supplement.py:15`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator_coverage_supplement.py#L15)
- doc: Targets uncovered validator branches.
- signature: `class TestValidatorUncovered:`
- members:
  - `test_boundary_manager_init_failure_fallback(self)` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator_coverage_supplement.py#L18) — Lines 19-20: ProjectBoundaryManager init failure fallback.
  - `test_validate_absolute_path_basic_denial(self)` — [`L133`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator_coverage_supplement.py#L133) — Lines 550-558: fallback absolute path denial.
  - `test_validate_absolute_path_test_env_exception_fallback(self)` — [`L79`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator_coverage_supplement.py#L79) — Line 416: exception in test env check falls through to deny.
  - `test_validate_absolute_path_test_env_multiple_temp_dirs(self)` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator_coverage_supplement.py#L45) — Lines 165-177: test env with /var/tmp fallback.
  - `test_validate_absolute_path_test_env_temp_pattern_match(self)` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator_coverage_supplement.py#L36) — Lines 165-199: test environment file pattern matching.
  - `test_validate_absolute_path_test_env_tmp_pattern(self)` — [`L56`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator_coverage_supplement.py#L56) — Lines 185-199: file name starts with tmp/temp/tmp_test.
  - `test_validate_file_path_none_input(self)` — [`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator_coverage_supplement.py#L65) — Line 126: None file path.
  - `test_validate_file_path_null_byte(self)` — [`L72`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator_coverage_supplement.py#L72) — Line 129-132: null byte injection.
  - `test_validate_file_path_windows_drive_letter_rejected(self)` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator_coverage_supplement.py#L26) — Line 146-154: Windows drive letter check on non-Windows.
  - `test_validate_path_traversal_dotdot_backslash(self)` — [`L97`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator_coverage_supplement.py#L97)
  - `test_validate_path_traversal_dotdot_start(self)` — [`L102`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator_coverage_supplement.py#L102)
  - `test_validate_path_traversal_double_dot_slash(self)` — [`L90`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator_coverage_supplement.py#L90) — Lines 370-398: path traversal patterns.
  - `test_validate_project_boundary_no_base_path(self)` — [`L127`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator_coverage_supplement.py#L127) — Line 519: returns True when base_path is None.
  - `test_validate_project_boundary_no_boundary_manager(self)` — [`L120`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator_coverage_supplement.py#L120) — Line 519: returns True when no boundary manager.
  - `test_validate_project_boundary_outside_rejected(self)` — [`L107`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator_coverage_supplement.py#L107) — Lines 536-539: project boundary rejection.
- uses (calls/refs, reference-scoped): [`SecurityValidator`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator), [`ProjectBoundaryManager`](../../../tree_sitter_analyzer/security/boundary_manager.md#ProjectBoundaryManager), [`validate_file_path`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator.validate_file_path), [`boundary_manager`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator.boundary_manager), [`_validate_absolute_path`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator._validate_absolute_path), [`_validate_project_boundary`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator._validate_project_boundary), [`_validate_path_traversal`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator._validate_path_traversal), [`_validate_windows_drive_letter`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator._validate_windows_drive_letter)

