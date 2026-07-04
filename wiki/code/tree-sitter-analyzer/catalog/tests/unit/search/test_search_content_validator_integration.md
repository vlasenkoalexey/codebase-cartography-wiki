---
title: 'Module: tests/unit/search/test_search_content_validator_integration.py'
type: catalog
provenance: extracted
module: tests/unit/search/test_search_content_validator_integration.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.search.test_search_content_validator_integration`/TestSearchContentToolIntegration#
symbols:
  TestSearchContentToolIntegration.test_search_content_validates_mutual_exclusion: test_search_content_validates_mutual_exclusion().
  TestSearchContentToolIntegration.test_search_content_no_format_parameter: test_search_content_no_format_parameter().
  TestSearchContentToolIntegration.test_error_message_multilingual: test_error_message_multilingual().
  TestSearchContentToolIntegration: ''
---
# Module: [`tests/unit/search/test_search_content_validator_integration.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/search/test_search_content_validator_integration.py)

## Classes
### `TestSearchContentToolIntegration`
- def: [`tests/unit/search/test_search_content_validator_integration.py:11`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/search/test_search_content_validator_integration.py#L11)
- doc: Test OutputFormatValidator integration with SearchContentTool.
- signature: `class TestSearchContentToolIntegration:`
- members:
  - `test_error_message_multilingual(self, tmp_path)` — [`L63`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/search/test_search_content_validator_integration.py#L63) — Test that error messages are multilingual.
  - `test_search_content_no_format_parameter(self, tmp_path)` — [`L52`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/search/test_search_content_validator_integration.py#L52) — Test that no format parameter is valid (normal mode).
  - `test_search_content_validates_mutual_exclusion(self, tmp_path)` — [`L14`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/search/test_search_content_validator_integration.py#L14) — Test that search_content_tool validates mutual exclusion.
- uses (calls/refs, reference-scoped): [`SearchContentTool`](../../../tree_sitter_analyzer/mcp/tools/search_content_tool.md#SearchContentTool), [`validate_arguments`](../../../tree_sitter_analyzer/mcp/tools/search_content_tool.md#SearchContentTool.validate_arguments)

