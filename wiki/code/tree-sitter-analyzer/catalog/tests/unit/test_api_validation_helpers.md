---
title: 'Module: tests/unit/test_api_validation_helpers.py'
type: catalog
provenance: extracted
module: tests/unit/test_api_validation_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_api_validation_helpers`/Test
symbols:
  TestMarkValidationReadable.test_readable_file: MarkValidationReadable#test_readable_file().
  TestMarkValidationReadable.test_nonexistent_file: MarkValidationReadable#test_nonexistent_file().
  TestMarkValidationReadable.test_permission_denied: MarkValidationReadable#test_permission_denied().
  TestMarkValidationReadable.test_unreadable_file_preserves_existing_errors: MarkValidationReadable#test_unreadable_file_preserves_existing_errors().
  TestValidationResultTemplate.test_default_shape: ValidationResultTemplate#test_default_shape().
  TestValidationResultTemplate.test_nonexistent_file: ValidationResultTemplate#test_nonexistent_file().
  TestApplyLanguageValidation.test_supported_language: ApplyLanguageValidation#test_supported_language().
  TestApplyLanguageValidation.test_unsupported_language: ApplyLanguageValidation#test_unsupported_language().
  TestApplyLanguageValidation.test_empty_language: ApplyLanguageValidation#test_empty_language().
  TestApplyLanguageValidation.test_none_language: ApplyLanguageValidation#test_none_language().
  TestApplyLanguageValidation.test_mutation_is_in_place: ApplyLanguageValidation#test_mutation_is_in_place().
  TestValidationResultTemplate: ValidationResultTemplate#
  TestMarkValidationReadable: MarkValidationReadable#
  TestApplyLanguageValidation: ApplyLanguageValidation#
---
# Module: [`tests/unit/test_api_validation_helpers.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_validation_helpers.py)

## Classes
### `TestApplyLanguageValidation`
- def: [`tests/unit/test_api_validation_helpers.py:74`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_validation_helpers.py#L74)
- doc: Tests for apply_language_validation.
- signature: `class TestApplyLanguageValidation:`
- members:
  - `test_empty_language(self)` — [`L90`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_validation_helpers.py#L90)
  - `test_mutation_is_in_place(self)` — [`L100`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_validation_helpers.py#L100)
  - `test_none_language(self)` — [`L95`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_validation_helpers.py#L95)
  - `test_supported_language(self)` — [`L77`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_validation_helpers.py#L77)
  - `test_unsupported_language(self)` — [`L84`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_validation_helpers.py#L84)
- uses (calls/refs, reference-scoped): [`apply_language_validation`](../../tree_sitter_analyzer/_api_validation_helpers.md#apply_language_validation)

### `TestMarkValidationReadable`
- def: [`tests/unit/test_api_validation_helpers.py:33`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_validation_helpers.py#L33)
- doc: Tests for mark_validation_readable.
- signature: `class TestMarkValidationReadable:`
- members:
  - `test_nonexistent_file(self, tmp_path)` — [`L44`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_validation_helpers.py#L44)
  - `test_permission_denied(self, tmp_path)` — [`L50`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_validation_helpers.py#L50)
  - `test_readable_file(self, tmp_path)` — [`L36`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_validation_helpers.py#L36)
  - `test_unreadable_file_preserves_existing_errors(self, tmp_path)` — [`L61`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_validation_helpers.py#L61)
- uses (calls/refs, reference-scoped): [`mark_validation_readable`](../../tree_sitter_analyzer/_api_validation_helpers.md#mark_validation_readable), [`validation_result_template`](../../tree_sitter_analyzer/_api_validation_helpers.md#validation_result_template)

### `TestValidationResultTemplate`
- def: [`tests/unit/test_api_validation_helpers.py:12`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_validation_helpers.py#L12)
- doc: Tests for validation_result_template.
- signature: `class TestValidationResultTemplate:`
- members:
  - `test_default_shape(self, tmp_path)` — [`L15`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_validation_helpers.py#L15)
  - `test_nonexistent_file(self, tmp_path)` — [`L27`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_api_validation_helpers.py#L27)
- uses (calls/refs, reference-scoped): [`validation_result_template`](../../tree_sitter_analyzer/_api_validation_helpers.md#validation_result_template)

