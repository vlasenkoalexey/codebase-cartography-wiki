---
title: 'Module: src/codegraphcontext/tools/languages/perl.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/tools/languages/perl.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.tools.languages.perl`/
symbols:
  PerlTreeSitterParser.parse: PerlTreeSitterParser#parse().
  PerlTreeSitterParser._find_functions: PerlTreeSitterParser#_find_functions().
  PerlTreeSitterParser._find_calls: PerlTreeSitterParser#_find_calls().
  PerlTreeSitterParser._find_variables: PerlTreeSitterParser#_find_variables().
  PerlTreeSitterParser._find_classes: PerlTreeSitterParser#_find_classes().
  PerlTreeSitterParser._find_imports: PerlTreeSitterParser#_find_imports().
  PerlTreeSitterParser._calculate_complexity: PerlTreeSitterParser#_calculate_complexity().
  PerlTreeSitterParser._get_node_text: PerlTreeSitterParser#_get_node_text().
  PerlTreeSitterParser.traverse: PerlTreeSitterParser#traverse().
  pre_scan_perl: pre_scan_perl().
  PERL_QUERIES: PERL_QUERIES.
  PerlTreeSitterParser.language_name: PerlTreeSitterParser#language_name.
  PerlTreeSitterParser.language: PerlTreeSitterParser#language.
  PerlTreeSitterParser._get_parent_context: PerlTreeSitterParser#_get_parent_context().
  PerlTreeSitterParser: PerlTreeSitterParser#
  PerlTreeSitterParser.index_source: PerlTreeSitterParser#index_source.
  PerlTreeSitterParser.parser: PerlTreeSitterParser#parser.
  PerlTreeSitterParser.__init__: PerlTreeSitterParser#__init__().
  PerlTreeSitterParser.generic_parser_wrapper: PerlTreeSitterParser#generic_parser_wrapper.
---
# Module: [`src/codegraphcontext/tools/languages/perl.py`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/perl.py)

## Classes
### `PerlTreeSitterParser`
- def: [`src/codegraphcontext/tools/languages/perl.py:47`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/perl.py#L47)
- doc: A Perl-specific parser using tree-sitter, encapsulating language-specific logic.
- signature: `class PerlTreeSitterParser:`
- members:
  - `parse(self, path: Path, is_dependency: bool = False, index_source: bool = False)` — [`L106`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/perl.py#L106) — Parses a Perl file and returns its structure in a standardized dictionary format.
  - `traverse(n, depth=0)` — [`L80`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/perl.py#L80)
  - `generic_parser_wrapper` — [`L51`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/perl.py#L51)
  - `index_source` — [`L55`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/perl.py#L55)
  - `language` — [`L53`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/perl.py#L53)
  - `language_name` — [`L52`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/perl.py#L52)
  - `parser` — [`L54`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/perl.py#L54)
- protocol/private: `__init__`[`L50`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/perl.py#L50), `_calculate_complexity`[`L70`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/perl.py#L70), `_find_calls`[`L262`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/perl.py#L262), `_find_classes`[`L194`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/perl.py#L194), `_find_functions`[`L136`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/perl.py#L136), `_find_imports`[`L235`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/perl.py#L235), `_find_variables`[`L284`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/perl.py#L284), `_get_node_text`[`L57`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/perl.py#L57), `_get_parent_context`[`L61`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/perl.py#L61)
- uses (calls/refs, reference-scoped): [`warning_logger`](../../utils/debug_log.md#warning_logger), [`execute_query`](../../utils/tree_sitter_manager.md#execute_query), [`error_logger`](../../utils/debug_log.md#error_logger), [`MAX_AST_DEPTH`](../indexing/constants.md#MAX_AST_DEPTH), [`PERL_QUERIES`](perl.md#PERL_QUERIES)
- used by: [`language_specific_parser`](../tree_sitter_parser.md#TreeSitterParser.language_specific_parser)

## Functions
- `pre_scan_perl(files: List[Path], parser_wrapper)` — [`L303`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/perl.py#L303) — Scans Perl files to create a map of package/subroutine names to their file paths.

## Module values
- `PERL_QUERIES` — [`L9`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/perl.py#L9)

