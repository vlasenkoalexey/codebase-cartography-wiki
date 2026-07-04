---
title: 'Module: tests/unit/mcp/test_resources/test_code_file_resource.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_resources/test_code_file_resource.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_resources.test_code_file_resource`/Test
symbols:
  TestGetSupportedSchemes.test_get_supported_schemes: GetSupportedSchemes#test_get_supported_schemes().
  TestGetSupportedResourceTypes.test_get_supported_resource_types: GetSupportedResourceTypes#test_get_supported_resource_types().
  TestMatchesUri.resource: MatchesUri#resource().
  TestMatchesUri.test_matches_uri_with_anyurl_type: MatchesUri#test_matches_uri_with_anyurl_type().
  TestExtractFilePath.resource: ExtractFilePath#resource().
  TestValidateFilePath.resource: ValidateFilePath#resource().
  TestReadFileContent.resource: ReadFileContent#resource().
  TestReadResource.resource: ReadResource#resource().
  TestStringRepresentations.test_str_representation: StringRepresentations#test_str_representation().
  TestStringRepresentations.test_repr_representation: StringRepresentations#test_repr_representation().
  TestIntegration.resource: Integration#resource().
  TestMatchesUri.test_matches_uri_with_anyurl_type.MockAnyUrl: MatchesUri#test_matches_uri_with_anyurl_type().MockAnyUrl#
  TestMatchesUri: MatchesUri#
  TestMatchesUri.test_matches_uri_with_anyurl_type.MockAnyUrl.__str__: MatchesUri#test_matches_uri_with_anyurl_type().MockAnyUrl#__str__().
  TestExtractFilePath: ExtractFilePath#
  TestExtractFilePath.test_extract_valid_path: ExtractFilePath#test_extract_valid_path().
  TestExtractFilePath.test_extract_path_with_subdirectories: ExtractFilePath#test_extract_path_with_subdirectories().
  TestExtractFilePath.test_extract_path_with_special_chars: ExtractFilePath#test_extract_path_with_special_chars().
  TestExtractFilePath.test_extract_invalid_uri_raises_error: ExtractFilePath#test_extract_invalid_uri_raises_error().
  TestValidateFilePath: ValidateFilePath#
  TestValidateFilePath.test_validate_valid_path: ValidateFilePath#test_validate_valid_path().
  TestValidateFilePath.test_validate_empty_path_raises_error: ValidateFilePath#test_validate_empty_path_raises_error().
  TestValidateFilePath.test_validate_null_bytes_raises_error: ValidateFilePath#test_validate_null_bytes_raises_error().
  TestValidateFilePath.test_validate_path_traversal_raises_error: ValidateFilePath#test_validate_path_traversal_raises_error().
  TestReadFileContent: ReadFileContent#
  TestReadFileContent.test_read_existing_file: ReadFileContent#test_read_existing_file().
  TestReadFileContent.test_read_file_with_encoding: ReadFileContent#test_read_file_with_encoding().
  TestReadFileContent.test_read_nonexistent_file_raises_error: ReadFileContent#test_read_nonexistent_file_raises_error().
  TestReadFileContent.test_read_file_permission_error: ReadFileContent#test_read_file_permission_error().
  TestReadFileContent.test_read_file_os_error: ReadFileContent#test_read_file_os_error().
  TestReadFileContent.test_read_file_unexpected_error: ReadFileContent#test_read_file_unexpected_error().
  TestReadResource: ReadResource#
  TestReadResource.test_read_resource_success: ReadResource#test_read_resource_success().
  TestReadResource.test_read_resource_invalid_uri: ReadResource#test_read_resource_invalid_uri().
  TestReadResource.test_read_resource_nonexistent_file: ReadResource#test_read_resource_nonexistent_file().
  TestReadResource.test_read_resource_with_path_traversal: ReadResource#test_read_resource_with_path_traversal().
  TestReadResource.test_read_resource_empty_path: ReadResource#test_read_resource_empty_path().
  TestReadResource.test_read_resource_with_null_bytes: ReadResource#test_read_resource_with_null_bytes().
  TestGetSupportedSchemes: GetSupportedSchemes#
  TestGetSupportedResourceTypes: GetSupportedResourceTypes#
  TestStringRepresentations: StringRepresentations#
  TestIntegration: Integration#
  TestIntegration.test_full_workflow: Integration#test_full_workflow().
  TestIntegration.test_multiple_files: Integration#test_multiple_files().
---
# Module: [`tests/unit/mcp/test_resources/test_code_file_resource.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_code_file_resource.py)

## Classes
### `MockAnyUrl`
- def: [`tests/unit/mcp/test_resources/test_code_file_resource.py:34`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_code_file_resource.py#L34)
- signature: `class MockAnyUrl:`
- protocol/private: `__str__`[`L35`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_code_file_resource.py#L35)
- used by: (1 test-only callers)

### `TestExtractFilePath`
- def: [`tests/unit/mcp/test_resources/test_code_file_resource.py:41`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_code_file_resource.py#L41)
- doc: Test _extract_file_path method
- signature: `class TestExtractFilePath:`
- members:
  - `resource(self)` — [`L45`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_code_file_resource.py#L45) — Create resource instance
  - `test_extract_invalid_uri_raises_error(self, resource)` — [`L67`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_code_file_resource.py#L67) — Test that invalid URI raises ValueError
  - `test_extract_path_with_special_chars(self, resource)` — [`L61`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_code_file_resource.py#L61) — Test extracting path with special characters
  - `test_extract_path_with_subdirectories(self, resource)` — [`L55`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_code_file_resource.py#L55) — Test extracting path with multiple subdirectories
  - `test_extract_valid_path(self, resource)` — [`L49`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_code_file_resource.py#L49) — Test extracting valid file path
- uses (calls/refs, reference-scoped): [`CodeFileResource`](../../../../tree_sitter_analyzer/mcp/resources/code_file_resource.md#CodeFileResource)

### `TestGetSupportedResourceTypes`
- def: [`tests/unit/mcp/test_resources/test_code_file_resource.py:263`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_code_file_resource.py#L263)
- doc: Test get_supported_resource_types method
- signature: `class TestGetSupportedResourceTypes:`
- members:
  - `test_get_supported_resource_types(self)` — [`L266`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_code_file_resource.py#L266) — Test getting supported resource types
- uses (calls/refs, reference-scoped): [`CodeFileResource`](../../../../tree_sitter_analyzer/mcp/resources/code_file_resource.md#CodeFileResource), [`get_supported_resource_types`](../../../../tree_sitter_analyzer/mcp/resources/code_file_resource.md#CodeFileResource.get_supported_resource_types)

### `TestGetSupportedSchemes`
- def: [`tests/unit/mcp/test_resources/test_code_file_resource.py:251`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_code_file_resource.py#L251)
- doc: Test get_supported_schemes method
- signature: `class TestGetSupportedSchemes:`
- members:
  - `test_get_supported_schemes(self)` — [`L254`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_code_file_resource.py#L254) — Test getting supported URI schemes
- uses (calls/refs, reference-scoped): [`CodeFileResource`](../../../../tree_sitter_analyzer/mcp/resources/code_file_resource.md#CodeFileResource), [`get_supported_schemes`](../../../../tree_sitter_analyzer/mcp/resources/code_file_resource.md#CodeFileResource.get_supported_schemes)

### `TestIntegration`
- def: [`tests/unit/mcp/test_resources/test_code_file_resource.py:296`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_code_file_resource.py#L296)
- doc: Integration tests for CodeFileResource
- signature: `class TestIntegration:`
- members:
  - `resource(self)` — [`L300`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_code_file_resource.py#L300) — Create resource instance
  - `test_full_workflow(self, resource)` — [`L305`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_code_file_resource.py#L305) — Test complete workflow from URI to content
  - `test_multiple_files(self, resource)` — [`L341`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_code_file_resource.py#L341) — Test reading multiple files
- uses (calls/refs, reference-scoped): [`CodeFileResource`](../../../../tree_sitter_analyzer/mcp/resources/code_file_resource.md#CodeFileResource)

### `TestMatchesUri`
- def: [`tests/unit/mcp/test_resources/test_code_file_resource.py:17`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_code_file_resource.py#L17)
- doc: Test matches_uri method — resource-specific edge cases.
- signature: `class TestMatchesUri:`
- members:
  - `resource(self)` — [`L26`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_code_file_resource.py#L26) — Create resource instance
  - `test_matches_uri_with_anyurl_type(self, resource)` — [`L30`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_code_file_resource.py#L30) — Test matching URI with AnyUrl type (string conversion)
- uses (calls/refs, reference-scoped): [`CodeFileResource`](../../../../tree_sitter_analyzer/mcp/resources/code_file_resource.md#CodeFileResource)  (1 test-only)

### `TestReadFileContent`
- def: [`tests/unit/mcp/test_resources/test_code_file_resource.py:113`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_code_file_resource.py#L113)
- doc: Test _read_file_content method
- signature: `class TestReadFileContent:`
- members:
  - `resource(self)` — [`L117`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_code_file_resource.py#L117) — Create resource instance
  - `test_read_existing_file(self, resource)` — [`L122`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_code_file_resource.py#L122) — Test reading an existing file
  - `test_read_file_os_error(self, mock_read, mock_path, resource)` — [`L171`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_code_file_resource.py#L171) — Test reading file with OS error
  - `test_read_file_permission_error(self, mock_read, mock_path, resource)` — [`L159`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_code_file_resource.py#L159) — Test reading file with permission error
  - `test_read_file_unexpected_error(self, mock_read, mock_path, resource)` — [`L183`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_code_file_resource.py#L183) — Test reading file with unexpected error
  - `test_read_file_with_encoding(self, resource)` — [`L135`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_code_file_resource.py#L135) — Test reading file with UTF-8 encoding
  - `test_read_nonexistent_file_raises_error(self, resource)` — [`L151`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_code_file_resource.py#L151) — Test reading non-existent file raises FileNotFoundError
- uses (calls/refs, reference-scoped): [`CodeFileResource`](../../../../tree_sitter_analyzer/mcp/resources/code_file_resource.md#CodeFileResource)

### `TestReadResource`
- def: [`tests/unit/mcp/test_resources/test_code_file_resource.py:193`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_code_file_resource.py#L193)
- doc: Test read_resource method
- signature: `class TestReadResource:`
- members:
  - `resource(self)` — [`L197`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_code_file_resource.py#L197) — Create resource instance
  - `test_read_resource_empty_path(self, resource)` — [`L236`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_code_file_resource.py#L236) — Test reading resource with empty path
  - `test_read_resource_invalid_uri(self, resource)` — [`L216`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_code_file_resource.py#L216) — Test reading resource with invalid URI
  - `test_read_resource_nonexistent_file(self, resource)` — [`L222`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_code_file_resource.py#L222) — Test reading resource for non-existent file
  - `test_read_resource_success(self, resource)` — [`L202`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_code_file_resource.py#L202) — Test reading resource successfully
  - `test_read_resource_with_null_bytes(self, resource)` — [`L244`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_code_file_resource.py#L244) — Test reading resource with null bytes in path
  - `test_read_resource_with_path_traversal(self, resource)` — [`L229`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_code_file_resource.py#L229) — Test reading resource with path traversal is blocked
- uses (calls/refs, reference-scoped): [`CodeFileResource`](../../../../tree_sitter_analyzer/mcp/resources/code_file_resource.md#CodeFileResource)

### `TestStringRepresentations`
- def: [`tests/unit/mcp/test_resources/test_code_file_resource.py:275`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_code_file_resource.py#L275)
- doc: Test __str__ and __repr__ methods
- signature: `class TestStringRepresentations:`
- members:
  - `test_repr_representation(self)` — [`L286`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_code_file_resource.py#L286) — Test detailed string representation
  - `test_str_representation(self)` — [`L278`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_code_file_resource.py#L278) — Test string representation
- uses (calls/refs, reference-scoped): [`CodeFileResource`](../../../../tree_sitter_analyzer/mcp/resources/code_file_resource.md#CodeFileResource)

### `TestValidateFilePath`
- def: [`tests/unit/mcp/test_resources/test_code_file_resource.py:76`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_code_file_resource.py#L76)
- doc: Test _validate_file_path method
- signature: `class TestValidateFilePath:`
- members:
  - `resource(self)` — [`L80`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_code_file_resource.py#L80) — Create resource instance
  - `test_validate_empty_path_raises_error(self, resource)` — [`L91`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_code_file_resource.py#L91) — Test that empty path raises ValueError
  - `test_validate_null_bytes_raises_error(self, resource)` — [`L96`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_code_file_resource.py#L96) — Test that null bytes in path raise ValueError
  - `test_validate_path_traversal_raises_error(self, resource)` — [`L101`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_code_file_resource.py#L101) — Test that path traversal raises ValueError
  - `test_validate_valid_path(self, resource)` — [`L84`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_code_file_resource.py#L84) — Test validating a valid file path
- uses (calls/refs, reference-scoped): [`CodeFileResource`](../../../../tree_sitter_analyzer/mcp/resources/code_file_resource.md#CodeFileResource)

