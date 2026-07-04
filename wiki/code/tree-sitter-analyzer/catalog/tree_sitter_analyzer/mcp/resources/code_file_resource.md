---
title: 'Module: tree_sitter_analyzer/mcp/resources/code_file_resource.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/resources/code_file_resource.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.resources.code_file_resource`/
symbols:
  CodeFileResource: CodeFileResource#
  CodeFileResource.read_resource: CodeFileResource#read_resource().
  CodeFileResource.matches_uri: CodeFileResource#matches_uri().
  logger: logger.
  CodeFileResource.get_resource_info: CodeFileResource#get_resource_info().
  CodeFileResource._read_file_content: CodeFileResource#_read_file_content().
  CodeFileResource._extract_file_path: CodeFileResource#_extract_file_path().
  CodeFileResource._uri_pattern: CodeFileResource#_uri_pattern.
  CodeFileResource.__repr__: CodeFileResource#__repr__().
  CodeFileResource._validate_file_path: CodeFileResource#_validate_file_path().
  CodeFileResource.get_supported_schemes: CodeFileResource#get_supported_schemes().
  CodeFileResource.get_supported_resource_types: CodeFileResource#get_supported_resource_types().
  CodeFileResource.__init__: CodeFileResource#__init__().
  CodeFileResource.__str__: CodeFileResource#__str__().
---
# Module: [`tree_sitter_analyzer/mcp/resources/code_file_resource.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/resources/code_file_resource.py)

## Classes
### `CodeFileResource`
- def: [`tree_sitter_analyzer/mcp/resources/code_file_resource.py:19`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/resources/code_file_resource.py#L19)
- doc: MCP resource for accessing code file content
- signature: `class CodeFileResource:`
- members:
  - `__init__(self)` — [`L34`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/resources/code_file_resource.py#L34) — Initialize the code file resource
  - `__repr__(self)` — [`L210`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/resources/code_file_resource.py#L210) — Detailed string representation of the resource
  - `__str__(self)` — [`L206`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/resources/code_file_resource.py#L206) — String representation of the resource
  - `_extract_file_path(self, uri: str)` — [`L66`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/resources/code_file_resource.py#L66) — Extract file path from URI
  - `_read_file_content(self, file_path: str)` — [`L87`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/resources/code_file_resource.py#L87) — Read file content with proper encoding detection
  - `_validate_file_path(self, file_path: str)` — [`L124`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/resources/code_file_resource.py#L124) — Validate file path for security and correctness
  - `get_resource_info(self)` — [`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/resources/code_file_resource.py#L38) — Get resource information for MCP registration
  - `get_supported_resource_types(self)` — [`L197`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/resources/code_file_resource.py#L197) — Get list of supported resource types
  - `get_supported_schemes(self)` — [`L188`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/resources/code_file_resource.py#L188) — Get list of supported URI schemes
  - `matches_uri(self, uri: str)` — [`L52`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/resources/code_file_resource.py#L52) — Check if the URI matches this resource pattern
  - `read_resource(self, uri: str)` — [`L148`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/resources/code_file_resource.py#L148) — Read resource content from URI
- protocol/private: `_uri_pattern`[`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/resources/code_file_resource.py#L36)
- uses (calls/refs, reference-scoped): [`read_file_safe`](../../encoding_utils.md#read_file_safe), [`logger`](code_file_resource.md#logger)
- used by: [`code_file_resource`](../server.md#TreeSitterAnalyzerMCPServer.code_file_resource), [`_read_resource`](../server.md#TreeSitterAnalyzerMCPServer._read_resource)  (49 test-only)

## Module values
- `logger` — [`L16`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/resources/code_file_resource.py#L16)

