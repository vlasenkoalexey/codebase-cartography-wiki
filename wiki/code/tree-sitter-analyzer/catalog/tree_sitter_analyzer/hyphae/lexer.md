---
title: 'Module: tree_sitter_analyzer/hyphae/lexer.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/hyphae/lexer.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.hyphae.lexer`/
symbols:
  tokenize: tokenize().
  Token: Token#
  Token.value: Token#value.
  _read_while: _read_while().
  _IDENT_CHARS: _IDENT_CHARS.
  _NAME_CHARS: _NAME_CHARS.
  _SINGLE: _SINGLE.
---
# Module: [`tree_sitter_analyzer/hyphae/lexer.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/lexer.py)

## Classes
### `Token`
- def: [`tree_sitter_analyzer/hyphae/lexer.py:35`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/lexer.py#L35)
- doc: A lexical token. `value` carries the identifier for HASH/DOT/COLON/IDENT
- signature: `class Token:`
- members:
  - `value` — [`L40`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/lexer.py#L40)
- used by: [`_parse_simple`](parser.md#_Parser._parse_simple), [`_parse_attribute`](parser.md#_Parser._parse_attribute), [`_parse_pseudo`](parser.md#_Parser._parse_pseudo), [`tokenize`](lexer.md#tokenize), [`_advance`](parser.md#_Parser._advance), [`_peek`](parser.md#_Parser._peek), [`_expect`](parser.md#_Parser._expect), [`_parse_pseudo_arg`](parser.md#_Parser._parse_pseudo_arg), [`_read_value_text`](parser.md#_Parser._read_value_text), [`__init__`](parser.md#_Parser.__init__)  (3 test-only)

## Functions
- `_read_while(text: str, start: int, allowed: frozenset[str])` — [`L43`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/lexer.py#L43)
- `tokenize(text: str)` — [`L51`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/lexer.py#L51) — Tokenize a Hyphae selector string.

## Module values
- `_IDENT_CHARS` — [`L19`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/lexer.py#L19)
- `_NAME_CHARS` — [`L16`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/lexer.py#L16)
- `_SINGLE` — [`L21`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/lexer.py#L21)

