---
title: 'Module: tree_sitter_analyzer/_exceptions_security.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/_exceptions_security.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer._exceptions_security`/
symbols:
  SecurityError: SecurityError#
  FileRestrictionError: FileRestrictionError#
  PathTraversalError: PathTraversalError#
  RegexSecurityError: RegexSecurityError#
  SecurityError.security_type: SecurityError#security_type.
  SecurityError.__init__: SecurityError#__init__().
  SecurityError.file_path: SecurityError#file_path.
  FileRestrictionError.current_mode: FileRestrictionError#current_mode.
  FileRestrictionError.allowed_patterns: FileRestrictionError#allowed_patterns.
  PathTraversalError.attempted_path: PathTraversalError#attempted_path.
  RegexSecurityError.pattern: RegexSecurityError#pattern.
  RegexSecurityError.dangerous_construct: RegexSecurityError#dangerous_construct.
  PathTraversalError.__init__: PathTraversalError#__init__().
  RegexSecurityError.__init__: RegexSecurityError#__init__().
  FileRestrictionError.__init__: FileRestrictionError#__init__().
---
# Module: [`tree_sitter_analyzer/_exceptions_security.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_security.py)

## Classes
### `FileRestrictionError`  ·  implements/extends SecurityError
- def: [`tree_sitter_analyzer/_exceptions_security.py:72`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_security.py#L72) — documented in [tree_sitter_analyzer-security-validator](../../concepts/tree_sitter_analyzer-security-validator.md)
- doc: Raised when file access is restricted by mode or security policy.
- signature: `class FileRestrictionError(SecurityError):`
- members:
  - `allowed_patterns` — [`L97`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_security.py#L97)
  - `current_mode` — [`L96`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_security.py#L96)
- protocol/private: `__init__`[`L75`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_security.py#L75)
- uses (calls/refs, reference-scoped): [`SecurityError`](_exceptions_security.md#SecurityError), [`__init__`](_exceptions_security.md#SecurityError.__init__)
- used by: [`SecurityError`](_exceptions_security.md#SecurityError), [`_attach_exception_details`](_exceptions_mcp_response.md#_attach_exception_details)  (7 test-only)

### `PathTraversalError`  ·  implements/extends SecurityError
- def: [`tree_sitter_analyzer/_exceptions_security.py:30`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_security.py#L30)
- doc: Raised when path traversal attack is detected.
- signature: `class PathTraversalError(SecurityError):`
- members:
  - `attempted_path` — [`L46`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_security.py#L46)
- protocol/private: `__init__`[`L33`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_security.py#L33)
- uses (calls/refs, reference-scoped): [`SecurityError`](_exceptions_security.md#SecurityError), [`__init__`](_exceptions_security.md#SecurityError.__init__)
- used by: [`SecurityError`](_exceptions_security.md#SecurityError)  (7 test-only)

### `RegexSecurityError`  ·  implements/extends SecurityError
- def: [`tree_sitter_analyzer/_exceptions_security.py:49`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_security.py#L49)
- doc: Raised when unsafe regex pattern is detected.
- signature: `class RegexSecurityError(SecurityError):`
- members:
  - `dangerous_construct` — [`L69`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_security.py#L69)
  - `pattern` — [`L68`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_security.py#L68)
- protocol/private: `__init__`[`L52`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_security.py#L52)
- uses (calls/refs, reference-scoped): [`SecurityError`](_exceptions_security.md#SecurityError), [`__init__`](_exceptions_security.md#SecurityError.__init__)
- used by: [`SecurityError`](_exceptions_security.md#SecurityError)  (6 test-only)

### `SecurityError`  ·  implements/extends TreeSitterAnalyzerError
- def: [`tree_sitter_analyzer/_exceptions_security.py:9`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_security.py#L9) — documented in [tree_sitter_analyzer-security-validator](../../concepts/tree_sitter_analyzer-security-validator.md)
- doc: Raised when security validation fails.
- signature: `class SecurityError(TreeSitterAnalyzerError):`
- members:
  - `file_path` — [`L27`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_security.py#L27)
  - `security_type` — [`L26`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_security.py#L26)
- protocol/private: `__init__`[`L12`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_security.py#L12)
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerError`](_exceptions_core.md#TreeSitterAnalyzerError), [`FileRestrictionError`](_exceptions_security.md#FileRestrictionError), [`PathTraversalError`](_exceptions_security.md#PathTraversalError), [`RegexSecurityError`](_exceptions_security.md#RegexSecurityError), [`__init__`](_exceptions_core.md#TreeSitterAnalyzerError.__init__)
- used by: [`TreeSitterAnalyzerError`](_exceptions_core.md#TreeSitterAnalyzerError), [`sanitize_input`](security/validator.md#SecurityValidator.sanitize_input), [`add_allowed_directory`](security/boundary_manager.md#ProjectBoundaryManager.add_allowed_directory), [`allowed_directories`](security/boundary_manager.md#ProjectBoundaryManager.allowed_directories), [`HAS_CTYPES`](security/validator.md#HAS_CTYPES), [`FileRestrictionError`](_exceptions_security.md#FileRestrictionError), [`PathTraversalError`](_exceptions_security.md#PathTraversalError), [`RegexSecurityError`](_exceptions_security.md#RegexSecurityError), [`__init__`](_exceptions_security.md#FileRestrictionError.__init__), [`__init__`](_exceptions_security.md#PathTraversalError.__init__), [`__init__`](_exceptions_security.md#RegexSecurityError.__init__), [`__init__`](security/boundary_manager.md#ProjectBoundaryManager.__init__)  (55 test-only)

