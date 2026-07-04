---
title: 'Module: tests/unit/mcp/test_resources/test_base_resource_contract.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_resources/test_base_resource_contract.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_resources.test_base_resource_contract`/
symbols:
  _RESOURCE_CASES._RESOURCE_CASES: _RESOURCE_CASES._RESOURCE_CASES.
  resource_and_valid_uris: resource_and_valid_uris().
  _resource_id: _resource_id().
  TestBaseResourceContract: TestBaseResourceContract#
  TestBaseResourceContract.test_initialization: TestBaseResourceContract#test_initialization().
  TestBaseResourceContract.test_uri_pattern_validation: TestBaseResourceContract#test_uri_pattern_validation().
  TestBaseResourceContract.test_get_resource_info: TestBaseResourceContract#test_get_resource_info().
  TestBaseResourceContract.test_resource_info_structure: TestBaseResourceContract#test_resource_info_structure().
  TestBaseResourceContract.test_matches_valid_uri: TestBaseResourceContract#test_matches_valid_uri().
  TestBaseResourceContract.test_malformed_uri_handling: TestBaseResourceContract#test_malformed_uri_handling().
  TestBaseResourceContract.test_rejects_invalid_scheme: TestBaseResourceContract#test_rejects_invalid_scheme().
---
# Module: [`tests/unit/mcp/test_resources/test_base_resource_contract.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_base_resource_contract.py)

## Classes
### `TestBaseResourceContract`
- def: [`tests/unit/mcp/test_resources/test_base_resource_contract.py:72`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_base_resource_contract.py#L72)
- doc: Invariants shared by every concrete resource class.
- signature: `class TestBaseResourceContract:`
- members:
  - `test_get_resource_info(self, resource_and_valid_uris)` — [`L84`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_base_resource_contract.py#L84)
  - `test_initialization(self, resource_and_valid_uris)` — [`L75`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_base_resource_contract.py#L75)
  - `test_malformed_uri_handling(self, resource_and_valid_uris)` — [`L105`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_base_resource_contract.py#L105) — URIs without a path segment after the authority must be rejected.
  - `test_matches_valid_uri(self, resource_and_valid_uris)` — [`L98`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_base_resource_contract.py#L98)
  - `test_rejects_invalid_scheme(self, resource_and_valid_uris)` — [`L118`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_base_resource_contract.py#L118)
  - `test_resource_info_structure(self, resource_and_valid_uris)` — [`L89`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_base_resource_contract.py#L89)
  - `test_uri_pattern_validation(self, resource_and_valid_uris)` — [`L80`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_base_resource_contract.py#L80)

## Functions
- `_resource_id(param: tuple)` — [`L56`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_base_resource_contract.py#L56)
- `resource_and_valid_uris(request)` — [`L62`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_base_resource_contract.py#L62)

## Module values
- `_RESOURCE_CASES` — [`L35`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_base_resource_contract.py#L35)

