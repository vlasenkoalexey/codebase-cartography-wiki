---
title: 'Module: tests/unit/security/test_security_boundary_properties.py'
type: catalog
provenance: extracted
module: tests/unit/security/test_security_boundary_properties.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.security.test_security_boundary_properties`/
symbols:
  COMMON_HEALTH_CHECKS: COMMON_HEALTH_CHECKS.
  safe_name: safe_name.
  TestSecurityBoundaryEnforcementProperties.test_property_4_boundary_manager_rejects_external_paths: TestSecurityBoundaryEnforcementProperties#test_property_4_boundary_manager_rejects_external_paths().
  TestSecurityBoundaryEdgeCases.test_property_4_get_relative_path_returns_none_for_external: TestSecurityBoundaryEdgeCases#test_property_4_get_relative_path_returns_none_for_external().
  TestSecurityValidatorIntegrationProperties.test_property_4_is_safe_path_consistent_with_validate: TestSecurityValidatorIntegrationProperties#test_property_4_is_safe_path_consistent_with_validate().
  TestSecurityValidatorIntegrationProperties.test_property_4_validate_path_alias_consistent: TestSecurityValidatorIntegrationProperties#test_property_4_validate_path_alias_consistent().
  TestProjectBoundaryManagerInitializationProperties.test_property_4_valid_directory_initializes_successfully: TestProjectBoundaryManagerInitializationProperties#test_property_4_valid_directory_initializes_successfully().
  relative_path_within_project: relative_path_within_project().
  TestSecurityBoundaryEnforcementProperties.test_property_4_path_traversal_rejected: TestSecurityBoundaryEnforcementProperties#test_property_4_path_traversal_rejected().
  TestSecurityBoundaryEnforcementProperties.test_property_4_null_byte_injection_rejected: TestSecurityBoundaryEnforcementProperties#test_property_4_null_byte_injection_rejected().
  TestSecurityBoundaryEnforcementProperties.test_property_4_valid_relative_paths_accepted: TestSecurityBoundaryEnforcementProperties#test_property_4_valid_relative_paths_accepted().
  TestSecurityBoundaryEnforcementProperties.test_property_4_boundary_manager_accepts_internal_paths: TestSecurityBoundaryEnforcementProperties#test_property_4_boundary_manager_accepts_internal_paths().
  TestSecurityBoundaryEnforcementProperties.test_property_4_boundary_manager_rejects_traversal: TestSecurityBoundaryEnforcementProperties#test_property_4_boundary_manager_rejects_traversal().
  TestSecurityBoundaryEnforcementProperties.test_property_4_validate_and_resolve_returns_resolved_path: TestSecurityBoundaryEnforcementProperties#test_property_4_validate_and_resolve_returns_resolved_path().
  TestSecurityBoundaryEnforcementProperties.test_property_4_validate_and_resolve_rejects_traversal: TestSecurityBoundaryEnforcementProperties#test_property_4_validate_and_resolve_rejects_traversal().
  TestSecurityBoundaryEdgeCases.test_property_4_boundary_manager_empty_path_rejected: TestSecurityBoundaryEdgeCases#test_property_4_boundary_manager_empty_path_rejected().
  TestSecurityBoundaryEdgeCases.test_property_4_get_relative_path_consistency: TestSecurityBoundaryEdgeCases#test_property_4_get_relative_path_consistency().
  TestProjectBoundaryManagerInitializationProperties.test_property_4_file_as_root_raises_security_error: TestProjectBoundaryManagerInitializationProperties#test_property_4_file_as_root_raises_security_error().
  TestSecurityBoundaryEnforcementProperties.test_property_4_absolute_paths_outside_boundary_rejected: TestSecurityBoundaryEnforcementProperties#test_property_4_absolute_paths_outside_boundary_rejected().
  TestSecurityBoundaryEdgeCases.test_property_4_empty_paths_rejected: TestSecurityBoundaryEdgeCases#test_property_4_empty_paths_rejected().
  TestSecurityValidatorIntegrationProperties.test_property_4_valid_glob_patterns_accepted: TestSecurityValidatorIntegrationProperties#test_property_4_valid_glob_patterns_accepted().
  TestSecurityValidatorIntegrationProperties.test_property_4_dangerous_glob_patterns_rejected: TestSecurityValidatorIntegrationProperties#test_property_4_dangerous_glob_patterns_rejected().
  path_traversal_attempt: path_traversal_attempt().
  absolute_path_outside_project: absolute_path_outside_project().
  relative_path_component: relative_path_component.
  TestProjectBoundaryManagerInitializationProperties.test_property_4_empty_root_raises_security_error: TestProjectBoundaryManagerInitializationProperties#test_property_4_empty_root_raises_security_error().
  TestProjectBoundaryManagerInitializationProperties.test_property_4_nonexistent_root_raises_security_error: TestProjectBoundaryManagerInitializationProperties#test_property_4_nonexistent_root_raises_security_error().
  null_byte_injection: null_byte_injection().
  EXTERNAL_PATH_MAX_EXAMPLES: EXTERNAL_PATH_MAX_EXAMPLES.
  boundary_manager: boundary_manager().
  security_validator: security_validator().
  file_extension: file_extension.
  WINDOWS_RESERVED_NAMES: WINDOWS_RESERVED_NAMES.
  temp_project_dir: temp_project_dir().
  TestSecurityBoundaryEnforcementProperties: TestSecurityBoundaryEnforcementProperties#
  TestSecurityBoundaryEdgeCases: TestSecurityBoundaryEdgeCases#
  TestSecurityValidatorIntegrationProperties: TestSecurityValidatorIntegrationProperties#
  TestProjectBoundaryManagerInitializationProperties: TestProjectBoundaryManagerInitializationProperties#
---
# Module: [`tests/unit/security/test_security_boundary_properties.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_security_boundary_properties.py)

## Classes
### `TestProjectBoundaryManagerInitializationProperties`
- def: [`tests/unit/security/test_security_boundary_properties.py:670`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_security_boundary_properties.py#L670)
- doc: Property-based tests for ProjectBoundaryManager initialization.
- signature: `class TestProjectBoundaryManagerInitializationProperties:`
- members:
  - `test_property_4_empty_root_raises_security_error(self)` — [`L678`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_security_boundary_properties.py#L678) — **Feature: test-coverage-improvement, Property 4: Security Boundary Enforcement**
  - `test_property_4_file_as_root_raises_security_error(self, temp_project_dir, name)` — [`L708`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_security_boundary_properties.py#L708) — **Feature: test-coverage-improvement, Property 4: Security Boundary Enforcement**
  - `test_property_4_nonexistent_root_raises_security_error(self)` — [`L691`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_security_boundary_properties.py#L691) — **Feature: test-coverage-improvement, Property 4: Security Boundary Enforcement**
  - `test_property_4_valid_directory_initializes_successfully(self, temp_project_dir, name)` — [`L729`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_security_boundary_properties.py#L729) — **Feature: test-coverage-improvement, Property 4: Security Boundary Enforcement**
- uses (calls/refs, reference-scoped): [`ProjectBoundaryManager`](../../../tree_sitter_analyzer/security/boundary_manager.md#ProjectBoundaryManager), [`SecurityError`](../../../tree_sitter_analyzer/_exceptions_security.md#SecurityError), [`allowed_directories`](../../../tree_sitter_analyzer/security/boundary_manager.md#ProjectBoundaryManager.allowed_directories), [`project_root`](../../../tree_sitter_analyzer/security/boundary_manager.md#ProjectBoundaryManager.project_root)  (2 test-only)

### `TestSecurityBoundaryEdgeCases`
- def: [`tests/unit/security/test_security_boundary_properties.py:453`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_security_boundary_properties.py#L453)
- doc: Property-based tests for edge cases in security boundary enforcement.
- signature: `class TestSecurityBoundaryEdgeCases:`
- members:
  - `test_property_4_boundary_manager_empty_path_rejected(self, temp_project_dir, name)` — [`L486`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_security_boundary_properties.py#L486) — **Feature: test-coverage-improvement, Property 4: Security Boundary Enforcement**
  - `test_property_4_empty_paths_rejected(self, temp_project_dir, empty_or_whitespace)` — [`L463`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_security_boundary_properties.py#L463) — **Feature: test-coverage-improvement, Property 4: Security Boundary Enforcement**
  - `test_property_4_get_relative_path_consistency(self, temp_project_dir, rel_path)` — [`L505`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_security_boundary_properties.py#L505) — **Feature: test-coverage-improvement, Property 4: Security Boundary Enforcement**
  - `test_property_4_get_relative_path_returns_none_for_external(self, temp_project_dir, abs_path)` — [`L535`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_security_boundary_properties.py#L535) — **Feature: test-coverage-improvement, Property 4: Security Boundary Enforcement**
- uses (calls/refs, reference-scoped): [`SecurityValidator`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator), [`ProjectBoundaryManager`](../../../tree_sitter_analyzer/security/boundary_manager.md#ProjectBoundaryManager), [`validate_file_path`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator.validate_file_path), [`is_within_project`](../../../tree_sitter_analyzer/security/boundary_manager.md#ProjectBoundaryManager.is_within_project), [`get_relative_path`](../../../tree_sitter_analyzer/security/boundary_manager.md#ProjectBoundaryManager.get_relative_path)  (5 test-only)

### `TestSecurityBoundaryEnforcementProperties`
- def: [`tests/unit/security/test_security_boundary_properties.py:209`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_security_boundary_properties.py#L209)
- doc: Property-based tests for security boundary enforcement.
- signature: `class TestSecurityBoundaryEnforcementProperties:`
- members:
  - `test_property_4_absolute_paths_outside_boundary_rejected(self, temp_project_dir, security_validator, abs_path)` — [`L291`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_security_boundary_properties.py#L291) — **Feature: test-coverage-improvement, Property 4: Security Boundary Enforcement**
  - `test_property_4_boundary_manager_accepts_internal_paths(self, temp_project_dir, rel_path)` — [`L316`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_security_boundary_properties.py#L316) — **Feature: test-coverage-improvement, Property 4: Security Boundary Enforcement**
  - `test_property_4_boundary_manager_rejects_external_paths(self, temp_project_dir, abs_path)` — [`L342`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_security_boundary_properties.py#L342) — **Feature: test-coverage-improvement, Property 4: Security Boundary Enforcement**
  - `test_property_4_boundary_manager_rejects_traversal(self, temp_project_dir, traversal_path)` — [`L365`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_security_boundary_properties.py#L365) — **Feature: test-coverage-improvement, Property 4: Security Boundary Enforcement**
  - `test_property_4_null_byte_injection_rejected(self, temp_project_dir, null_path)` — [`L246`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_security_boundary_properties.py#L246) — **Feature: test-coverage-improvement, Property 4: Security Boundary Enforcement**
  - `test_property_4_path_traversal_rejected(self, temp_project_dir, traversal_path)` — [`L219`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_security_boundary_properties.py#L219) — **Feature: test-coverage-improvement, Property 4: Security Boundary Enforcement**
  - `test_property_4_valid_relative_paths_accepted(self, temp_project_dir, rel_path)` — [`L268`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_security_boundary_properties.py#L268) — **Feature: test-coverage-improvement, Property 4: Security Boundary Enforcement**
  - `test_property_4_validate_and_resolve_rejects_traversal(self, temp_project_dir, traversal_path)` — [`L423`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_security_boundary_properties.py#L423) — **Feature: test-coverage-improvement, Property 4: Security Boundary Enforcement**
  - `test_property_4_validate_and_resolve_returns_resolved_path(self, temp_project_dir, rel_path)` — [`L398`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_security_boundary_properties.py#L398) — **Feature: test-coverage-improvement, Property 4: Security Boundary Enforcement**
- uses (calls/refs, reference-scoped): [`SecurityValidator`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator), [`ProjectBoundaryManager`](../../../tree_sitter_analyzer/security/boundary_manager.md#ProjectBoundaryManager), [`validate_file_path`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator.validate_file_path), [`is_within_project`](../../../tree_sitter_analyzer/security/boundary_manager.md#ProjectBoundaryManager.is_within_project), [`validate_and_resolve_path`](../../../tree_sitter_analyzer/security/boundary_manager.md#ProjectBoundaryManager.validate_and_resolve_path)  (6 test-only)

### `TestSecurityValidatorIntegrationProperties`
- def: [`tests/unit/security/test_security_boundary_properties.py:558`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_security_boundary_properties.py#L558)
- doc: Property-based tests for SecurityValidator integration with boundary enforcement.
- signature: `class TestSecurityValidatorIntegrationProperties:`
- members:
  - `test_property_4_dangerous_glob_patterns_rejected(self, temp_project_dir, dangerous_glob)` — [`L649`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_security_boundary_properties.py#L649) — **Feature: test-coverage-improvement, Property 4: Security Boundary Enforcement**
  - `test_property_4_is_safe_path_consistent_with_validate(self, temp_project_dir, rel_path)` — [`L568`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_security_boundary_properties.py#L568) — **Feature: test-coverage-improvement, Property 4: Security Boundary Enforcement**
  - `test_property_4_valid_glob_patterns_accepted(self, temp_project_dir, glob_pattern)` — [`L621`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_security_boundary_properties.py#L621) — **Feature: test-coverage-improvement, Property 4: Security Boundary Enforcement**
  - `test_property_4_validate_path_alias_consistent(self, temp_project_dir, rel_path)` — [`L590`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_security_boundary_properties.py#L590) — **Feature: test-coverage-improvement, Property 4: Security Boundary Enforcement**
- uses (calls/refs, reference-scoped): [`SecurityValidator`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator), [`validate_file_path`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator.validate_file_path), [`validate_glob_pattern`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator.validate_glob_pattern), [`is_safe_path`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator.is_safe_path), [`validate_path`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator.validate_path)  (2 test-only)

## Functions
- `absolute_path_outside_project(draw)` — [`L141`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_security_boundary_properties.py#L141) — Generate absolute paths that are outside any project boundary.
- `boundary_manager(temp_project_dir)` — [`L193`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_security_boundary_properties.py#L193) — Create a ProjectBoundaryManager for testing.
- `null_byte_injection(draw)` — [`L161`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_security_boundary_properties.py#L161) — Generate paths with null byte injection attempts.
- `path_traversal_attempt(draw)` — [`L114`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_security_boundary_properties.py#L114) — Generate paths that attempt directory traversal.
- `relative_path_within_project(draw)` — [`L103`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_security_boundary_properties.py#L103) — Generate a relative path that should be within project boundaries.
- `security_validator(temp_project_dir)` — [`L199`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_security_boundary_properties.py#L199) — Create a SecurityValidator for testing.
- `temp_project_dir()` — [`L174`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_security_boundary_properties.py#L174) — Create a temporary project directory for testing.

## Module values
- `COMMON_HEALTH_CHECKS` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_security_boundary_properties.py#L24)
- `EXTERNAL_PATH_MAX_EXAMPLES` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_security_boundary_properties.py#L25)
- `WINDOWS_RESERVED_NAMES` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_security_boundary_properties.py#L33)
- `file_extension` — [`L70`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_security_boundary_properties.py#L70)
- `relative_path_component` — [`L95`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_security_boundary_properties.py#L95)
- `safe_name` — [`L59`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_security_boundary_properties.py#L59)

