---
title: 'Module: tree_sitter_analyzer/formatters/toon_decoder.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/formatters/toon_decoder.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.formatters.toon_decoder`/
symbols:
  decode_toon: decode_toon().
  _unescape: _unescape().
  ToonDecodeError: ToonDecodeError#
  _NUMBER_PATTERN: _NUMBER_PATTERN.
  _UNESCAPE_MAP._UNESCAPE_MAP: _UNESCAPE_MAP._UNESCAPE_MAP.
  __all__: __all__.
---
# Module: [`tree_sitter_analyzer/formatters/toon_decoder.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_decoder.py)

## Classes
### `ToonDecodeError`  ·  implements/extends Exception
- def: [`tree_sitter_analyzer/formatters/toon_decoder.py:34`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_decoder.py#L34)
- doc: Raised when a TOON token cannot be decoded.
- signature: `class ToonDecodeError(Exception):`
- used by: [`decode_toon`](toon_decoder.md#decode_toon)

## Functions
- `_unescape(s: str)` — [`L52`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_decoder.py#L52) — Resolve backslash escape sequences inside a quoted TOON string.
- `decode_toon(token: str)` — [`L73`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_decoder.py#L73) — Decode a single TOON scalar token to the corresponding Python value.

## Module values
- `_NUMBER_PATTERN` — [`L40`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_decoder.py#L40)
- `_UNESCAPE_MAP` — [`L43`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_decoder.py#L43)
- `__all__` — [`L31`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_decoder.py#L31)

