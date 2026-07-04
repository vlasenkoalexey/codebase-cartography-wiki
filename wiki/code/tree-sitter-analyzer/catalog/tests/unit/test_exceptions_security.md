---
title: 'Module: tests/unit/test_exceptions_security.py'
type: catalog
provenance: extracted
module: tests/unit/test_exceptions_security.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_exceptions_security`/Test
symbols:
  TestFileRestrictionError.test_with_mode_and_patterns: FileRestrictionError#test_with_mode_and_patterns().
  TestPathTraversalError.test_with_attempted_path: PathTraversalError#test_with_attempted_path().
  TestRegexSecurityError.test_with_pattern_and_construct: RegexSecurityError#test_with_pattern_and_construct().
  TestSecurityError.test_basic_construction: SecurityError#test_basic_construction().
  TestSecurityError.test_with_security_type: SecurityError#test_with_security_type().
  TestSecurityError.test_with_file_path: SecurityError#test_with_file_path().
  TestPathTraversalError.test_inherits_from_security_error: PathTraversalError#test_inherits_from_security_error().
  TestRegexSecurityError.test_without_optional_fields: RegexSecurityError#test_without_optional_fields().
  TestFileRestrictionError.test_without_optional_fields: FileRestrictionError#test_without_optional_fields().
  TestSecurityError.test_path_object_converted_to_string: SecurityError#test_path_object_converted_to_string().
  TestSecurityError.test_inherits_from_base: SecurityError#test_inherits_from_base().
  TestSecurityError.test_to_dict_includes_context: SecurityError#test_to_dict_includes_context().
  TestPathTraversalError.test_without_attempted_path: PathTraversalError#test_without_attempted_path().
  TestPathTraversalError.test_inherits_security_type: PathTraversalError#test_inherits_security_type().
  TestRegexSecurityError.test_security_type_is_regex: RegexSecurityError#test_security_type_is_regex().
  TestFileRestrictionError.test_security_type_is_file_restriction: FileRestrictionError#test_security_type_is_file_restriction().
  TestSecurityError: SecurityError#
  TestPathTraversalError: PathTraversalError#
  TestRegexSecurityError: RegexSecurityError#
  TestFileRestrictionError: FileRestrictionError#
---
# Module: [`tests/unit/test_exceptions_security.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_security.py)

## Classes
### `TestFileRestrictionError`
- def: [`tests/unit/test_exceptions_security.py:96`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_security.py#L96)
- doc: Tests for FileRestrictionError.
- signature: `class TestFileRestrictionError:`
- members:
  - `test_security_type_is_file_restriction(self)` — [`L111`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_security.py#L111)
  - `test_with_mode_and_patterns(self)` — [`L99`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_security.py#L99)
  - `test_without_optional_fields(self)` — [`L115`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_security.py#L115)
- uses (calls/refs, reference-scoped): [`context`](../../tree_sitter_analyzer/_exceptions_core.md#TreeSitterAnalyzerError.context), [`FileRestrictionError`](../../tree_sitter_analyzer/_exceptions_security.md#FileRestrictionError), [`security_type`](../../tree_sitter_analyzer/_exceptions_security.md#SecurityError.security_type), [`allowed_patterns`](../../tree_sitter_analyzer/_exceptions_security.md#FileRestrictionError.allowed_patterns), [`current_mode`](../../tree_sitter_analyzer/_exceptions_security.md#FileRestrictionError.current_mode), [`file_path`](../../tree_sitter_analyzer/_exceptions_security.md#SecurityError.file_path)

### `TestPathTraversalError`
- def: [`tests/unit/test_exceptions_security.py:47`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_security.py#L47)
- doc: Tests for PathTraversalError.
- signature: `class TestPathTraversalError:`
- members:
  - `test_inherits_from_security_error(self)` — [`L66`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_security.py#L66)
  - `test_inherits_security_type(self)` — [`L62`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_security.py#L62)
  - `test_with_attempted_path(self)` — [`L50`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_security.py#L50)
  - `test_without_attempted_path(self)` — [`L58`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_security.py#L58)
- uses (calls/refs, reference-scoped): [`context`](../../tree_sitter_analyzer/_exceptions_core.md#TreeSitterAnalyzerError.context), [`SecurityError`](../../tree_sitter_analyzer/_exceptions_security.md#SecurityError), [`TreeSitterAnalyzerError`](../../tree_sitter_analyzer/_exceptions_core.md#TreeSitterAnalyzerError), [`PathTraversalError`](../../tree_sitter_analyzer/_exceptions_security.md#PathTraversalError), [`security_type`](../../tree_sitter_analyzer/_exceptions_security.md#SecurityError.security_type), [`attempted_path`](../../tree_sitter_analyzer/_exceptions_security.md#PathTraversalError.attempted_path)

### `TestRegexSecurityError`
- def: [`tests/unit/test_exceptions_security.py:72`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_security.py#L72)
- doc: Tests for RegexSecurityError.
- signature: `class TestRegexSecurityError:`
- members:
  - `test_security_type_is_regex(self)` — [`L91`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_security.py#L91)
  - `test_with_pattern_and_construct(self)` — [`L75`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_security.py#L75)
  - `test_without_optional_fields(self)` — [`L86`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_security.py#L86)
- uses (calls/refs, reference-scoped): [`context`](../../tree_sitter_analyzer/_exceptions_core.md#TreeSitterAnalyzerError.context), [`RegexSecurityError`](../../tree_sitter_analyzer/_exceptions_security.md#RegexSecurityError), [`security_type`](../../tree_sitter_analyzer/_exceptions_security.md#SecurityError.security_type), [`dangerous_construct`](../../tree_sitter_analyzer/_exceptions_security.md#RegexSecurityError.dangerous_construct), [`pattern`](../../tree_sitter_analyzer/_exceptions_security.md#RegexSecurityError.pattern)

### `TestSecurityError`
- def: [`tests/unit/test_exceptions_security.py:12`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_security.py#L12)
- doc: Tests for SecurityError base class.
- signature: `class TestSecurityError:`
- members:
  - `test_basic_construction(self)` — [`L15`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_security.py#L15)
  - `test_inherits_from_base(self)` — [`L37`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_security.py#L37)
  - `test_path_object_converted_to_string(self)` — [`L31`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_security.py#L31)
  - `test_to_dict_includes_context(self)` — [`L41`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_security.py#L41)
  - `test_with_file_path(self)` — [`L26`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_security.py#L26)
  - `test_with_security_type(self)` — [`L21`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_exceptions_security.py#L21)
- uses (calls/refs, reference-scoped): [`context`](../../tree_sitter_analyzer/_exceptions_core.md#TreeSitterAnalyzerError.context), [`SecurityError`](../../tree_sitter_analyzer/_exceptions_security.md#SecurityError), [`TreeSitterAnalyzerError`](../../tree_sitter_analyzer/_exceptions_core.md#TreeSitterAnalyzerError), [`to_dict`](../../tree_sitter_analyzer/_exceptions_core.md#TreeSitterAnalyzerError.to_dict), [`security_type`](../../tree_sitter_analyzer/_exceptions_security.md#SecurityError.security_type), [`file_path`](../../tree_sitter_analyzer/_exceptions_security.md#SecurityError.file_path)

