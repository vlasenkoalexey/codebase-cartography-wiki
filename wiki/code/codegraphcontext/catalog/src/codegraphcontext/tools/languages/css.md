---
title: 'Module: src/codegraphcontext/tools/languages/css.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/tools/languages/css.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.tools.languages.css`/
symbols:
  CSSTreeSitterParser.parse: CSSTreeSitterParser#parse().
  CSSTreeSitterParser._get_node_text: CSSTreeSitterParser#_get_node_text().
  CSSTreeSitterParser: CSSTreeSitterParser#
  CSSTreeSitterParser.language: CSSTreeSitterParser#language.
  CSSTreeSitterParser.parser: CSSTreeSitterParser#parser.
  CSSTreeSitterParser.language_name: CSSTreeSitterParser#language_name.
  pre_scan_css: pre_scan_css().
  CSSTreeSitterParser.__init__: CSSTreeSitterParser#__init__().
  CSSTreeSitterParser.generic_parser_wrapper: CSSTreeSitterParser#generic_parser_wrapper.
---
# Module: [`src/codegraphcontext/tools/languages/css.py`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/css.py)

## Classes
### `CSSTreeSitterParser`
- def: [`src/codegraphcontext/tools/languages/css.py:6`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/css.py#L6)
- doc: A parser for CSS files using tree-sitter.
- signature: `class CSSTreeSitterParser:`
- members:
  - `parse(self, path: Path, is_dependency: bool = False, index_source: bool = False)` — [`L18`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/css.py#L18) — Parses a CSS file and returns its structure.
  - `generic_parser_wrapper` — [`L10`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/css.py#L10)
  - `language` — [`L11`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/css.py#L11)
  - `language_name` — [`L13`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/css.py#L13)
  - `parser` — [`L12`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/css.py#L12)
- protocol/private: `__init__`[`L9`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/css.py#L9), `_get_node_text`[`L15`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/css.py#L15)
- uses (calls/refs, reference-scoped): [`execute_query`](../../utils/tree_sitter_manager.md#execute_query)
- used by: [`language_specific_parser`](../tree_sitter_parser.md#TreeSitterParser.language_specific_parser)

## Functions
- `pre_scan_css(files: list[Path], parser_wrapper)` — [`L92`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/css.py#L92)

