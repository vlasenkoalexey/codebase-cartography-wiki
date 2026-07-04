---
title: 'Module: src/codegraphcontext/tools/languages/html.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/tools/languages/html.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.tools.languages.html`/
symbols:
  HTMLTreeSitterParser.parse: HTMLTreeSitterParser#parse().
  HTMLTreeSitterParser._get_node_text: HTMLTreeSitterParser#_get_node_text().
  HTMLTreeSitterParser.language_name: HTMLTreeSitterParser#language_name.
  HTMLTreeSitterParser: HTMLTreeSitterParser#
  HTMLTreeSitterParser.language: HTMLTreeSitterParser#language.
  HTMLTreeSitterParser.parser: HTMLTreeSitterParser#parser.
  pre_scan_html: pre_scan_html().
  HTML_QUERIES: HTML_QUERIES.
  HTMLTreeSitterParser.__init__: HTMLTreeSitterParser#__init__().
  HTMLTreeSitterParser.generic_parser_wrapper: HTMLTreeSitterParser#generic_parser_wrapper.
---
# Module: [`src/codegraphcontext/tools/languages/html.py`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/html.py)

## Classes
### `HTMLTreeSitterParser`
- def: [`src/codegraphcontext/tools/languages/html.py:28`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/html.py#L28)
- doc: A parser for HTML files using tree-sitter.
- signature: `class HTMLTreeSitterParser:`
- members:
  - `parse(self, path: Path, is_dependency: bool = False, index_source: bool = False)` — [`L40`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/html.py#L40) — Parses an HTML file and returns its structure.
  - `generic_parser_wrapper` — [`L32`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/html.py#L32)
  - `language` — [`L33`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/html.py#L33)
  - `language_name` — [`L35`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/html.py#L35)
  - `parser` — [`L34`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/html.py#L34)
- protocol/private: `__init__`[`L31`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/html.py#L31), `_get_node_text`[`L37`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/html.py#L37)
- uses (calls/refs, reference-scoped): [`execute_query`](../../utils/tree_sitter_manager.md#execute_query)
- used by: [`language_specific_parser`](../tree_sitter_parser.md#TreeSitterParser.language_specific_parser)

## Functions
- `pre_scan_html(files: list[Path], parser_wrapper)` — [`L138`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/html.py#L138)

## Module values
- `HTML_QUERIES` — [`L6`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/html.py#L6)

