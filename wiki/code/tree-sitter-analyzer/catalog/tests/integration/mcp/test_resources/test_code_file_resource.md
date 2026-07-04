---
title: 'Module: tests/integration/mcp/test_resources/test_code_file_resource.py'
type: catalog
provenance: extracted
module: tests/integration/mcp/test_resources/test_code_file_resource.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.mcp.test_resources.test_code_file_resource`/TestCodeFileResource
symbols:
  TestCodeFileResourceFunctionality.resource: Functionality#resource.
  TestCodeFileResourceFunctionality.test_read_existing_file: Functionality#test_read_existing_file().
  TestCodeFileResourceSchema.resource: Schema#resource.
  TestCodeFileResourceSchema.test_resource_info_structure: Schema#test_resource_info_structure().
  TestCodeFileResourceSchema.test_uri_pattern_validation: Schema#test_uri_pattern_validation().
  TestCodeFileResourceSchema.test_extract_file_path: Schema#test_extract_file_path().
  TestCodeFileResourceFunctionality.test_read_nonexistent_file: Functionality#test_read_nonexistent_file().
  TestCodeFileResourceFunctionality.test_read_invalid_uri: Functionality#test_read_invalid_uri().
  TestCodeFileResourceFunctionality.test_read_file_with_encoding: Functionality#test_read_file_with_encoding().
  TestCodeFileResourceFunctionality.test_read_large_file: Functionality#test_read_large_file().
  TestCodeFileResourceIntegration.test_integration_with_file_handler: Integration#test_integration_with_file_handler().
  TestCodeFileResourceErrorHandling.test_permission_denied_error: ErrorHandling#test_permission_denied_error().
  TestCodeFileResourceErrorHandling.test_invalid_file_path_characters: ErrorHandling#test_invalid_file_path_characters().
  TestCodeFileResourceErrorHandling.test_malformed_uri_handling: ErrorHandling#test_malformed_uri_handling().
  TestCodeFileResourcePerformance.test_multiple_file_access: Performance#test_multiple_file_access().
  TestCodeFileResourceErrorHandling.resource: ErrorHandling#resource.
  TestCodeFileResourceIntegration.resource: Integration#resource.
  TestCodeFileResourceIntegration.test_integration_with_encoding_utils: Integration#test_integration_with_encoding_utils().
  TestCodeFileResourceErrorHandling.setup_method: ErrorHandling#setup_method().
  TestCodeFileResourcePerformance.setup_method: Performance#setup_method().
  TestCodeFileResourceFunctionality.sample_java_code: Functionality#sample_java_code.
  TestCodeFileResourcePerformance.resource: Performance#resource.
  TestCodeFileResourceSchema: Schema#
  TestCodeFileResourceSchema.setup_method: Schema#setup_method().
  TestCodeFileResourceFunctionality: Functionality#
  TestCodeFileResourceFunctionality.setup_method: Functionality#setup_method().
  TestCodeFileResourceIntegration: Integration#
  TestCodeFileResourceIntegration.setup_method: Integration#setup_method().
  TestCodeFileResourceErrorHandling: ErrorHandling#
  TestCodeFileResourcePerformance: Performance#
---
# Module: [`tests/integration/mcp/test_resources/test_code_file_resource.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_code_file_resource.py)

## Classes
### `TestCodeFileResourceErrorHandling`
- def: [`tests/integration/mcp/test_resources/test_code_file_resource.py:242`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_code_file_resource.py#L242)
- doc: Test error handling in code file resource
- signature: `class TestCodeFileResourceErrorHandling:`
- members:
  - `setup_method(self)` — [`L245`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_code_file_resource.py#L245) — Set up test fixtures
  - `test_invalid_file_path_characters(self)` — [`L264`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_code_file_resource.py#L264) — Test handling of invalid file path characters
  - `test_malformed_uri_handling(self)` — [`L275`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_code_file_resource.py#L275) — Test handling of malformed URIs
  - `test_permission_denied_error(self, mocker)` — [`L250`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_code_file_resource.py#L250) — Test handling of permission denied errors
  - `resource` — [`L247`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_code_file_resource.py#L247)
- uses (calls/refs, reference-scoped): [`CodeFileResource`](../../../../tree_sitter_analyzer/mcp/resources/code_file_resource.md#CodeFileResource), [`read_resource`](../../../../tree_sitter_analyzer/mcp/resources/code_file_resource.md#CodeFileResource.read_resource), [`matches_uri`](../../../../tree_sitter_analyzer/mcp/resources/code_file_resource.md#CodeFileResource.matches_uri)

### `TestCodeFileResourceFunctionality`
- def: [`tests/integration/mcp/test_resources/test_code_file_resource.py:78`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_code_file_resource.py#L78)
- doc: Test code file resource core functionality
- signature: `class TestCodeFileResourceFunctionality:`
- members:
  - `setup_method(self)` — [`L81`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_code_file_resource.py#L81) — Set up test fixtures
  - `test_read_existing_file(self)` — [`L105`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_code_file_resource.py#L105) — Test reading an existing file
  - `test_read_file_with_encoding(self)` — [`L141`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_code_file_resource.py#L141) — Test reading file with different encodings
  - `test_read_invalid_uri(self)` — [`L133`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_code_file_resource.py#L133) — Test error handling for invalid URI
  - `test_read_large_file(self)` — [`L174`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_code_file_resource.py#L174) — Test reading larger files
  - `test_read_nonexistent_file(self)` — [`L125`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_code_file_resource.py#L125) — Test error handling for nonexistent file
  - `resource` — [`L83`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_code_file_resource.py#L83)
  - `sample_java_code` — [`L84`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_code_file_resource.py#L84)
- uses (calls/refs, reference-scoped): [`CodeFileResource`](../../../../tree_sitter_analyzer/mcp/resources/code_file_resource.md#CodeFileResource), [`read_resource`](../../../../tree_sitter_analyzer/mcp/resources/code_file_resource.md#CodeFileResource.read_resource)

### `TestCodeFileResourceIntegration`
- def: [`tests/integration/mcp/test_resources/test_code_file_resource.py:216`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_code_file_resource.py#L216)
- doc: Test integration with existing file handler components
- signature: `class TestCodeFileResourceIntegration:`
- members:
  - `setup_method(self)` — [`L219`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_code_file_resource.py#L219) — Set up test fixtures
  - `test_integration_with_encoding_utils(self)` — [`L234`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_code_file_resource.py#L234) — Test integration with encoding utilities
  - `test_integration_with_file_handler(self)` — [`L223`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_code_file_resource.py#L223) — Test integration with existing file_handler module
  - `resource` — [`L221`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_code_file_resource.py#L221)
- uses (calls/refs, reference-scoped): [`EncodingManager`](../../../../tree_sitter_analyzer/encoding_utils.md#EncodingManager), [`read_file_safe`](../../../../tree_sitter_analyzer/encoding_utils.md#read_file_safe), [`CodeFileResource`](../../../../tree_sitter_analyzer/mcp/resources/code_file_resource.md#CodeFileResource)

### `TestCodeFileResourcePerformance`
- def: [`tests/integration/mcp/test_resources/test_code_file_resource.py:289`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_code_file_resource.py#L289)
- doc: Test performance characteristics of code file resource
- signature: `class TestCodeFileResourcePerformance:`
- members:
  - `setup_method(self)` — [`L292`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_code_file_resource.py#L292) — Set up test fixtures
  - `test_multiple_file_access(self)` — [`L297`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_code_file_resource.py#L297) — Test accessing multiple files efficiently
  - `resource` — [`L294`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_code_file_resource.py#L294)
- uses (calls/refs, reference-scoped): [`CodeFileResource`](../../../../tree_sitter_analyzer/mcp/resources/code_file_resource.md#CodeFileResource), [`read_resource`](../../../../tree_sitter_analyzer/mcp/resources/code_file_resource.md#CodeFileResource.read_resource)

### `TestCodeFileResourceSchema`
- def: [`tests/integration/mcp/test_resources/test_code_file_resource.py:18`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_code_file_resource.py#L18)
- doc: Test code file resource schema and validation
- signature: `class TestCodeFileResourceSchema:`
- members:
  - `setup_method(self)` — [`L21`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_code_file_resource.py#L21) — Set up test fixtures
  - `test_extract_file_path(self)` — [`L65`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_code_file_resource.py#L65) — Test file path extraction from URI
  - `test_resource_info_structure(self)` — [`L25`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_code_file_resource.py#L25) — Test that resource info has required structure
  - `test_uri_pattern_validation(self)` — [`L40`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_code_file_resource.py#L40) — Test URI pattern validation
  - `resource` — [`L23`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_code_file_resource.py#L23)
- uses (calls/refs, reference-scoped): [`CodeFileResource`](../../../../tree_sitter_analyzer/mcp/resources/code_file_resource.md#CodeFileResource), [`matches_uri`](../../../../tree_sitter_analyzer/mcp/resources/code_file_resource.md#CodeFileResource.matches_uri), [`get_resource_info`](../../../../tree_sitter_analyzer/mcp/resources/code_file_resource.md#CodeFileResource.get_resource_info), [`_extract_file_path`](../../../../tree_sitter_analyzer/mcp/resources/code_file_resource.md#CodeFileResource._extract_file_path)

