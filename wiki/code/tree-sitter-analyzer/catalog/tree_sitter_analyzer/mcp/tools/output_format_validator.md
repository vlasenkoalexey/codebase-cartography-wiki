---
title: 'Module: tree_sitter_analyzer/mcp/tools/output_format_validator.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/output_format_validator.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.output_format_validator`/
symbols:
  OutputFormatValidator: OutputFormatValidator#
  OutputFormatValidator.validate_output_format_exclusion: OutputFormatValidator#validate_output_format_exclusion().
  OutputFormatValidator.get_active_format: OutputFormatValidator#get_active_format().
  get_default_validator: get_default_validator().
  OutputFormatValidator._get_error_message: OutputFormatValidator#_get_error_message().
  _default_validator._default_validator: _default_validator._default_validator.
  OutputFormatValidator.OUTPUT_FORMAT_PARAMS: OutputFormatValidator#OUTPUT_FORMAT_PARAMS.
  OutputFormatValidator._detect_language: OutputFormatValidator#_detect_language().
  OutputFormatValidator.FORMAT_EFFICIENCY_GUIDE: OutputFormatValidator#FORMAT_EFFICIENCY_GUIDE.
---
# Module: [`tree_sitter_analyzer/mcp/tools/output_format_validator.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/output_format_validator.py)

## Classes
### `OutputFormatValidator`
- def: [`tree_sitter_analyzer/mcp/tools/output_format_validator.py:12`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/output_format_validator.py#L12)
- doc: Validator for output format parameters mutual exclusion.
- signature: `class OutputFormatValidator:`
- members:
  - `_detect_language(self)` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/output_format_validator.py#L33) — Always use English for MCP tool error messages sent to Claude.
  - `_get_error_message(self, specified_formats: list[str])` — [`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/output_format_validator.py#L37) — Generate localized error message with usage examples.
  - `get_active_format(self, arguments: dict[str, Any])` — [`L107`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/output_format_validator.py#L107) — Get the active output format from arguments.
  - `validate_output_format_exclusion(self, arguments: dict[str, Any])` — [`L87`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/output_format_validator.py#L87) — Validate that only one output format parameter is specified.
  - `FORMAT_EFFICIENCY_GUIDE` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/output_format_validator.py#L25)
  - `OUTPUT_FORMAT_PARAMS` — [`L16`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/output_format_validator.py#L16)
- used by: [`validate_search_arguments`](search_content_validation.md#validate_search_arguments), [`get_default_validator`](output_format_validator.md#get_default_validator), [`_default_validator`](output_format_validator.md#_default_validator._default_validator)  (33 test-only)

## Functions
- `get_default_validator()` — [`L127`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/output_format_validator.py#L127) — Get the default output format validator instance.

## Module values
- `_default_validator` — [`L124`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/output_format_validator.py#L124)

