---
title: 'Module: tree_sitter_analyzer/mcp/tools/utils/parse_validity.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/utils/parse_validity.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.utils.parse_validity`/
symbols:
  is_file_parse_broken: is_file_parse_broken().
  _file_byte_diagnostics: _file_byte_diagnostics().
  _is_null_byte_false_positive: _is_null_byte_false_positive().
  file_input_diagnostics: file_input_diagnostics().
  _decode_replacement_used: _decode_replacement_used().
  _KNOWN_SOURCE_EXTENSIONS._KNOWN_SOURCE_EXTENSIONS: _KNOWN_SOURCE_EXTENSIONS._KNOWN_SOURCE_EXTENSIONS.
  is_parse_broken: is_parse_broken().
  syntax_error_envelope: syntax_error_envelope().
  _is_utf8_decodable: _is_utf8_decodable().
  __all__: __all__.
---
# Module: [`tree_sitter_analyzer/mcp/tools/utils/parse_validity.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/parse_validity.py)

## Functions
- `_decode_replacement_used(raw_bytes: bytes, detected_encoding: str)` — [`L227`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/parse_validity.py#L227)
- `_file_byte_diagnostics(file_path: str)` — [`L184`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/parse_validity.py#L184)
- `_is_null_byte_false_positive(file_path: str, language: str)` — [`L240`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/parse_validity.py#L240) — Return ``True`` when ``file_path``'s ``has_error`` is caused only
- `_is_utf8_decodable(raw_bytes: bytes)` — [`L219`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/parse_validity.py#L219)
- `file_input_diagnostics(file_path: str, language: str | None = None)` — [`L164`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/parse_validity.py#L164) — Return parse/encoding signals for symbol-returning tools.
- `is_file_parse_broken(file_path: str, language: str | None = None)` — [`L107`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/parse_validity.py#L107) — Convenience wrapper that parses ``file_path`` and checks the tree.
- `is_parse_broken(tree: Any)` — [`L81`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/parse_validity.py#L81) — Return ``True`` when tree-sitter detected syntax errors.
- `syntax_error_envelope(file_path: str, *, tool: str, output_format: str = "toon")` — [`L283`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/parse_validity.py#L283) — Build the canonical short-circuit envelope for a syntax error.

## Module values
- `_KNOWN_SOURCE_EXTENSIONS` — [`L37`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/parse_validity.py#L37)
- `__all__` — [`L328`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/parse_validity.py#L328)

