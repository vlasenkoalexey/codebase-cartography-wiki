---
title: 'Module: tests/unit/security/test_integration.py'
type: catalog
provenance: extracted
module: tests/unit/security/test_integration.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.security.test_integration`/TestSecurityIntegration#
symbols:
  TestSecurityIntegration.project_root: project_root.
  TestSecurityIntegration.test_boundary_manager_integration: test_boundary_manager_integration().
  TestSecurityIntegration.test_multi_directory_boundary_control: test_multi_directory_boundary_control().
  TestSecurityIntegration.test_symlink_safety_comprehensive: test_symlink_safety_comprehensive().
  TestSecurityIntegration.test_file: test_file.
  TestSecurityIntegration.test_complete_security_workflow: test_complete_security_workflow().
  TestSecurityIntegration.test_security_exceptions_integration: test_security_exceptions_integration().
  TestSecurityIntegration.test_audit_logging_integration: test_audit_logging_integration().
  TestSecurityIntegration.src_dir: src_dir.
  TestSecurityIntegration.test_regex_checker_integration: test_regex_checker_integration().
  TestSecurityIntegration.test_comprehensive_path_validation: test_comprehensive_path_validation().
  TestSecurityIntegration.temp_dir: temp_dir.
  TestSecurityIntegration.test_regex_performance_and_safety: test_regex_performance_and_safety().
  TestSecurityIntegration.teardown_method: teardown_method().
  TestSecurityIntegration: ''
  TestSecurityIntegration.setup_method: setup_method().
---
# Module: [`tests/unit/security/test_integration.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_integration.py)

## Classes
### `TestSecurityIntegration`
- def: [`tests/unit/security/test_integration.py:19`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_integration.py#L19)
- doc: Integration test suite for security module.
- signature: `class TestSecurityIntegration:`
- members:
  - `setup_method(self)` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_integration.py#L22) — Set up test fixtures.
  - `teardown_method(self)` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_integration.py#L36) — Clean up test fixtures.
  - `test_audit_logging_integration(self)` — [`L225`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_integration.py#L225) — Test audit logging functionality.
  - `test_boundary_manager_integration(self)` — [`L71`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_integration.py#L71) — Test boundary manager integration with validator.
  - `test_complete_security_workflow(self)` — [`L43`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_integration.py#L43) — Test complete security validation workflow.
  - `test_comprehensive_path_validation(self)` — [`L157`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_integration.py#L157) — Test comprehensive path validation with all security layers.
  - `test_multi_directory_boundary_control(self)` — [`L130`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_integration.py#L130) — Test boundary control with multiple allowed directories.
  - `test_regex_checker_integration(self)` — [`L90`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_integration.py#L90) — Test regex checker integration with validator.
  - `test_regex_performance_and_safety(self)` — [`L200`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_integration.py#L200) — Test regex performance monitoring and safety checks.
  - `test_security_exceptions_integration(self)` — [`L112`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_integration.py#L112) — Test security exceptions are properly raised.
  - `test_symlink_safety_comprehensive(self)` — [`L239`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_integration.py#L239) — Test comprehensive symlink safety checks.
  - `project_root` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_integration.py#L25)
  - `src_dir` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_integration.py#L29)
  - `temp_dir` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_integration.py#L24)
  - `test_file` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_integration.py#L32)
- uses (calls/refs, reference-scoped): [`SecurityValidator`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator), [`ProjectBoundaryManager`](../../../tree_sitter_analyzer/security/boundary_manager.md#ProjectBoundaryManager), [`SecurityError`](../../../tree_sitter_analyzer/_exceptions_security.md#SecurityError), [`RegexSafetyChecker`](../../../tree_sitter_analyzer/security/regex_checker.md#RegexSafetyChecker), [`validate_file_path`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator.validate_file_path), [`validate_pattern`](../../../tree_sitter_analyzer/security/regex_checker.md#RegexSafetyChecker.validate_pattern), [`is_within_project`](../../../tree_sitter_analyzer/security/boundary_manager.md#ProjectBoundaryManager.is_within_project), [`sanitize_input`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator.sanitize_input), [`add_allowed_directory`](../../../tree_sitter_analyzer/security/boundary_manager.md#ProjectBoundaryManager.add_allowed_directory), [`is_symlink_safe`](../../../tree_sitter_analyzer/security/boundary_manager.md#ProjectBoundaryManager.is_symlink_safe), [`create_safe_pattern`](../../../tree_sitter_analyzer/security/regex_checker.md#RegexSafetyChecker.create_safe_pattern), [`audit_access`](../../../tree_sitter_analyzer/security/boundary_manager.md#ProjectBoundaryManager.audit_access), [`validate_regex_pattern`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator.validate_regex_pattern)

