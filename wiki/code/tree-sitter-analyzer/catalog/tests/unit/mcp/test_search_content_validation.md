---
title: 'Module: tests/unit/mcp/test_search_content_validation.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_search_content_validation.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_search_content_validation`/
symbols:
  tool: tool().
  sample_project_structure: sample_project_structure().
  TestValidateRoots: TestValidateRoots#
  TestValidateRoots.test_validate_roots_success: TestValidateRoots#test_validate_roots_success().
  TestValidateRoots.test_validate_roots_invalid_directory: TestValidateRoots#test_validate_roots_invalid_directory().
  TestValidateFiles: TestValidateFiles#
  TestValidateFiles.test_validate_files_success: TestValidateFiles#test_validate_files_success().
  TestValidateFiles.test_validate_files_empty_string: TestValidateFiles#test_validate_files_empty_string().
  TestValidateFiles.test_validate_files_not_found: TestValidateFiles#test_validate_files_not_found().
  TestValidateArguments: TestValidateArguments#
  TestValidateArguments.test_validate_valid_arguments_with_roots: TestValidateArguments#test_validate_valid_arguments_with_roots().
  TestValidateArguments.test_validate_valid_arguments_with_files: TestValidateArguments#test_validate_valid_arguments_with_files().
  TestValidateArguments.test_validate_missing_query: TestValidateArguments#test_validate_missing_query().
  TestValidateArguments.test_validate_empty_query: TestValidateArguments#test_validate_empty_query().
  TestValidateArguments.test_validate_whitespace_query: TestValidateArguments#test_validate_whitespace_query().
  TestValidateArguments.test_validate_missing_both_roots_and_files: TestValidateArguments#test_validate_missing_both_roots_and_files().
  TestValidateArguments.test_validate_invalid_case_type: TestValidateArguments#test_validate_invalid_case_type().
  TestValidateArguments.test_validate_invalid_encoding_type: TestValidateArguments#test_validate_invalid_encoding_type().
  TestValidateArguments.test_validate_invalid_max_filesize_type: TestValidateArguments#test_validate_invalid_max_filesize_type().
  TestValidateArguments.test_validate_invalid_fixed_strings_type: TestValidateArguments#test_validate_invalid_fixed_strings_type().
  TestValidateArguments.test_validate_invalid_word_type: TestValidateArguments#test_validate_invalid_word_type().
  TestValidateArguments.test_validate_invalid_multiline_type: TestValidateArguments#test_validate_invalid_multiline_type().
  TestValidateArguments.test_validate_invalid_include_globs_type: TestValidateArguments#test_validate_invalid_include_globs_type().
---
# Module: [`tests/unit/mcp/test_search_content_validation.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_validation.py)

## Classes
### `TestValidateArguments`
- def: [`tests/unit/mcp/test_search_content_validation.py:63`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_validation.py#L63)
- doc: Tests for validate_arguments method.
- signature: `class TestValidateArguments:`
- members:
  - `test_validate_empty_query(self, tool)` — [`L85`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_validation.py#L85)
  - `test_validate_invalid_case_type(self, tool)` — [`L100`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_validation.py#L100)
  - `test_validate_invalid_encoding_type(self, tool)` — [`L105`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_validation.py#L105)
  - `test_validate_invalid_fixed_strings_type(self, tool)` — [`L123`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_validation.py#L123)
  - `test_validate_invalid_include_globs_type(self, tool)` — [`L146`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_validation.py#L146)
  - `test_validate_invalid_max_filesize_type(self, tool)` — [`L114`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_validation.py#L114)
  - `test_validate_invalid_multiline_type(self, tool)` — [`L137`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_validation.py#L137)
  - `test_validate_invalid_word_type(self, tool)` — [`L132`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_validation.py#L132)
  - `test_validate_missing_both_roots_and_files(self, tool)` — [`L95`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_validation.py#L95)
  - `test_validate_missing_query(self, tool)` — [`L80`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_validation.py#L80)
  - `test_validate_valid_arguments_with_files(self, tool, sample_project_structure)` — [`L73`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_validation.py#L73)
  - `test_validate_valid_arguments_with_roots(self, tool, sample_project_structure)` — [`L66`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_validation.py#L66)
  - `test_validate_whitespace_query(self, tool)` — [`L90`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_validation.py#L90)

### `TestValidateFiles`
- def: [`tests/unit/mcp/test_search_content_validation.py:44`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_validation.py#L44)
- doc: Tests for _validate_files method.
- signature: `class TestValidateFiles:`
- members:
  - `test_validate_files_empty_string(self, tool)` — [`L52`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_validation.py#L52)
  - `test_validate_files_not_found(self, tool)` — [`L57`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_validation.py#L57)
  - `test_validate_files_success(self, tool, sample_project_structure)` — [`L47`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_validation.py#L47)

### `TestValidateRoots`
- def: [`tests/unit/mcp/test_search_content_validation.py:29`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_validation.py#L29)
- doc: Tests for _validate_roots method.
- signature: `class TestValidateRoots:`
- members:
  - `test_validate_roots_invalid_directory(self, tool)` — [`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_validation.py#L38)
  - `test_validate_roots_success(self, tool, sample_project_structure)` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_validation.py#L32)

## Functions
- `sample_project_structure(tmp_path: Path)` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_validation.py#L19)
- `tool()` — [`L14`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_validation.py#L14)

