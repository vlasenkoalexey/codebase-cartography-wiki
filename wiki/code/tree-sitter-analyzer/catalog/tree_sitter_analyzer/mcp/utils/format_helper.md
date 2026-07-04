---
title: 'Module: tree_sitter_analyzer/mcp/utils/format_helper.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/utils/format_helper.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.utils.format_helper`/
symbols:
  apply_toon_format_to_response: apply_toon_format_to_response().
  format_for_file_output: format_for_file_output().
  format_as_toon: format_as_toon().
  format_output: format_output().
  get_formatter: get_formatter().
  TOON_CONTROL_SURFACE.TOON_CONTROL_SURFACE: TOON_CONTROL_SURFACE.TOON_CONTROL_SURFACE.
  attach_toon_content_to_response: attach_toon_content_to_response().
  format_as_json: format_as_json().
  apply_output_format: apply_output_format().
  JsonFormatter: JsonFormatter#
  reduce_to_control_surface: reduce_to_control_surface().
  _get_formatter_for_toon: _get_formatter_for_toon().
  logger: logger.
  _copy_metadata_fields: _copy_metadata_fields().
  JsonFormatter.format: JsonFormatter#format().
  TOON_DICT_PASSTHROUGH.TOON_DICT_PASSTHROUGH: TOON_DICT_PASSTHROUGH.TOON_DICT_PASSTHROUGH.
  TOON_LARGE_STRING_FIELDS.TOON_LARGE_STRING_FIELDS: TOON_LARGE_STRING_FIELDS.TOON_LARGE_STRING_FIELDS.
---
# Module: [`tree_sitter_analyzer/mcp/utils/format_helper.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/format_helper.py)

## Classes
### `JsonFormatter`
- def: [`tree_sitter_analyzer/mcp/utils/format_helper.py:147`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/format_helper.py#L147)
- members:
  - `format(self, data: Any)` — [`L150`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/format_helper.py#L150) — Format data as JSON string.
- used by: [`get_formatter`](format_helper.md#get_formatter), [`_get_formatter_for_toon`](format_helper.md#_get_formatter_for_toon)  (8 test-only)

## Functions
- `_copy_metadata_fields(result: dict[str, Any], toon_response: dict[str, Any])` — [`L245`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/format_helper.py#L245) — Copy non-bulk metadata fields from result into toon_response.
- `_get_formatter_for_toon()` — [`L121`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/format_helper.py#L121) — Return ToonFormatter or JsonFormatter fallback on import failure.
- `apply_output_format(result: dict[str, Any], output_format: str = "json", return_formatted_string: bool = False)` — [`L155`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/format_helper.py#L155) — Apply output format to a result dictionary.
- `apply_toon_format_to_response(result: dict[str, Any], output_format: str = "json", *, compact_only: bool = False)` — [`L284`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/format_helper.py#L284) — Apply TOON format to MCP tool response if requested. — documented in [tree_sitter_analyzer-mcp-tools-base_tool](../../../../concepts/tree_sitter_analyzer-mcp-tools-base_tool.md)
- `attach_toon_content_to_response(result: dict[str, Any])` — [`L362`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/format_helper.py#L362) — Attach TOON formatted content to a response *without removing* any existing fields.
- `format_as_json(data: dict[str, Any])` — [`L85`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/format_helper.py#L85) — Format data as JSON string.
- `format_as_toon(data: dict[str, Any])` — [`L98`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/format_helper.py#L98) — Format data as TOON string.
- `format_for_file_output(data: dict[str, Any], output_format: str = "json")` — [`L183`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/format_helper.py#L183) — Format data for file output and return content with appropriate extension.
- `format_output(data: dict[str, Any], output_format: str = "json")` — [`L68`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/format_helper.py#L68) — Format data according to the specified output format.
- `get_formatter(output_format: str = "json")` — [`L132`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/format_helper.py#L132) — Get a formatter instance for the specified format.
- `reduce_to_control_surface(result: dict[str, Any])` — [`L53`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/format_helper.py#L53) — Drop TOON-response metadata already encoded inside ``toon_content``.

## Module values
- `TOON_CONTROL_SURFACE` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/format_helper.py#L26)
- `TOON_DICT_PASSTHROUGH` — [`L220`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/format_helper.py#L220)
- `TOON_LARGE_STRING_FIELDS` — [`L235`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/format_helper.py#L235)
- `logger` — [`L14`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/format_helper.py#L14)

