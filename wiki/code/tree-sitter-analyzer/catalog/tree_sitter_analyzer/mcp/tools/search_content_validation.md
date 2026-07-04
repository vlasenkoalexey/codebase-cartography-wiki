---
title: 'Module: tree_sitter_analyzer/mcp/tools/search_content_validation.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/search_content_validation.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.search_content_validation`/
symbols:
  validate_search_arguments: validate_search_arguments().
  _validate_option_types: _validate_option_types().
  _validate_options: _validate_options().
  PathListValidator: PathListValidator.
  _STRING_OPTIONS: _STRING_OPTIONS.
  _BOOLEAN_OPTIONS: _BOOLEAN_OPTIONS.
  _INTEGER_OPTIONS: _INTEGER_OPTIONS.
  _STRING_LIST_OPTIONS: _STRING_LIST_OPTIONS.
  _validate_query_and_inputs: _validate_query_and_inputs().
---
# Module: [`tree_sitter_analyzer/mcp/tools/search_content_validation.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_validation.py)

## Functions
- `_validate_option_types(arguments: dict[str, Any])` — [`L72`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_validation.py#L72) — Validate optional ripgrep argument types.
- `_validate_options(arguments: dict[str, Any], keys: list[str], expected_type: type, type_phrase: str)` — [`L86`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_validation.py#L86) — Validate homogeneous optional argument types.
- `_validate_query_and_inputs(arguments: dict[str, Any])` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_validation.py#L48) — Require a non-empty query and at least one search target.
- `validate_search_arguments(arguments: dict[str, Any], validate_roots: PathListValidator, validate_files: PathListValidator)` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_validation.py#L28) — Validate query, roots/files, and search option types.

## Module values
- `PathListValidator` — [`L10`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_validation.py#L10)
- `_BOOLEAN_OPTIONS` — [`L13`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_validation.py#L13)
- `_INTEGER_OPTIONS` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_validation.py#L24)
- `_STRING_LIST_OPTIONS` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_validation.py#L25)
- `_STRING_OPTIONS` — [`L12`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_validation.py#L12)

