---
title: 'Module: tests/unit/security/test_security_edge_cases.py'
type: catalog
provenance: extracted
module: tests/unit/security/test_security_edge_cases.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.security.test_security_edge_cases`/TestSecurityValidator
symbols:
  TestSecurityValidatorPathTraversal.test_double_dot_traversal_rejected: PathTraversal#test_double_dot_traversal_rejected().
  TestSecurityValidatorPathTraversal.test_null_byte_injection_rejected: PathTraversal#test_null_byte_injection_rejected().
  TestSecurityValidatorPathTraversal.test_mixed_path_separators_rejected: PathTraversal#test_mixed_path_separators_rejected().
  TestSecurityValidatorPathTraversal.test_valid_relative_path_accepted: PathTraversal#test_valid_relative_path_accepted().
  TestSecurityValidatorSanitization.test_sanitize_removes_null_bytes: Sanitization#test_sanitize_removes_null_bytes().
  TestSecurityValidatorSanitization.test_sanitize_normalizes_path: Sanitization#test_sanitize_normalizes_path().
  TestSecurityValidatorSanitization.test_sanitize_empty_path: Sanitization#test_sanitize_empty_path().
  TestSecurityValidatorEdgeCases.test_very_long_path: EdgeCases#test_very_long_path().
  TestSecurityValidatorEdgeCases.test_unicode_path: EdgeCases#test_unicode_path().
  TestSecurityValidatorEdgeCases.test_symlink_path_validation: EdgeCases#test_symlink_path_validation().
  TestSecurityValidatorNonWindows.test_junction_check_returns_false_on_posix: NonWindows#test_junction_check_returns_false_on_posix().
  TestSecurityValidatorPathTraversal: PathTraversal#
  TestSecurityValidatorSanitization: Sanitization#
  TestSecurityValidatorEdgeCases: EdgeCases#
  TestSecurityValidatorNonWindows: NonWindows#
---
# Module: [`tests/unit/security/test_security_edge_cases.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_security_edge_cases.py)

## Classes
### `TestSecurityValidatorEdgeCases`
- def: [`tests/unit/security/test_security_edge_cases.py:52`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_security_edge_cases.py#L52)
- signature: `class TestSecurityValidatorEdgeCases:`
- members:
  - `test_symlink_path_validation(self)` — [`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_security_edge_cases.py#L65)
  - `test_unicode_path(self)` — [`L60`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_security_edge_cases.py#L60)
  - `test_very_long_path(self)` — [`L53`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_security_edge_cases.py#L53)
- uses (calls/refs, reference-scoped): [`SecurityValidator`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator), [`validate_file_path`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator.validate_file_path)

### `TestSecurityValidatorNonWindows`
- def: [`tests/unit/security/test_security_edge_cases.py:71`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_security_edge_cases.py#L71)
- doc: Junction detection is Windows-only; on POSIX it should return False.
- signature: `class TestSecurityValidatorNonWindows:`
- members:
  - `test_junction_check_returns_false_on_posix(self)` — [`L74`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_security_edge_cases.py#L74)
- uses (calls/refs, reference-scoped): [`SecurityValidator`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator), [`_is_junction_or_reparse_point`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator._is_junction_or_reparse_point)

### `TestSecurityValidatorPathTraversal`
- def: [`tests/unit/security/test_security_edge_cases.py:9`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_security_edge_cases.py#L9)
- signature: `class TestSecurityValidatorPathTraversal:`
- members:
  - `test_double_dot_traversal_rejected(self)` — [`L10`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_security_edge_cases.py#L10)
  - `test_mixed_path_separators_rejected(self)` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_security_edge_cases.py#L22)
  - `test_null_byte_injection_rejected(self)` — [`L16`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_security_edge_cases.py#L16)
  - `test_valid_relative_path_accepted(self)` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_security_edge_cases.py#L28)
- uses (calls/refs, reference-scoped): [`SecurityValidator`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator), [`validate_file_path`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator.validate_file_path)

### `TestSecurityValidatorSanitization`
- def: [`tests/unit/security/test_security_edge_cases.py:35`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_security_edge_cases.py#L35)
- signature: `class TestSecurityValidatorSanitization:`
- members:
  - `test_sanitize_empty_path(self)` — [`L46`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_security_edge_cases.py#L46)
  - `test_sanitize_normalizes_path(self)` — [`L41`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_security_edge_cases.py#L41)
  - `test_sanitize_removes_null_bytes(self)` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_security_edge_cases.py#L36)
- uses (calls/refs, reference-scoped): [`SecurityValidator`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator), [`sanitize_input`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator.sanitize_input)

