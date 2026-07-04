---
title: 'Module: src/codegraphcontext/tools/languages/php.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/tools/languages/php.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.tools.languages.php`/
symbols:
  PhpTreeSitterParser.index_source: PhpTreeSitterParser#index_source.
  PhpTreeSitterParser._get_node_text: PhpTreeSitterParser#_get_node_text().
  PhpTreeSitterParser._parse_functions: PhpTreeSitterParser#_parse_functions().
  PhpTreeSitterParser._parse_types: PhpTreeSitterParser#_parse_types().
  PhpTreeSitterParser._parse_calls: PhpTreeSitterParser#_parse_calls().
  PhpTreeSitterParser.language_name: PhpTreeSitterParser#language_name.
  PhpTreeSitterParser._parse_variables: PhpTreeSitterParser#_parse_variables().
  PhpTreeSitterParser._parse_imports: PhpTreeSitterParser#_parse_imports().
  PhpTreeSitterParser._get_parent_context: PhpTreeSitterParser#_get_parent_context().
  PhpTreeSitterParser._get_enclosing_class_name: PhpTreeSitterParser#_get_enclosing_class_name().
  PhpTreeSitterParser: PhpTreeSitterParser#
  PHP_QUERIES: PHP_QUERIES.
  PhpTreeSitterParser.language: PhpTreeSitterParser#language.
  PhpTreeSitterParser.parser: PhpTreeSitterParser#parser.
  PhpTreeSitterParser._parse_trait_method_map: PhpTreeSitterParser#_parse_trait_method_map().
  pre_scan_php: pre_scan_php().
  PhpTreeSitterParser.__init__: PhpTreeSitterParser#__init__().
  PhpTreeSitterParser.generic_parser_wrapper: PhpTreeSitterParser#generic_parser_wrapper.
  PhpTreeSitterParser.parse: PhpTreeSitterParser#parse().
---
# Module: [`src/codegraphcontext/tools/languages/php.py`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/php.py)

## Classes
### `PhpTreeSitterParser`
- def: [`src/codegraphcontext/tools/languages/php.py:63`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/php.py#L63)
- signature: `class PhpTreeSitterParser:`
- members:
  - `_parse_trait_method_map(self, class_source: str)` — [`L171`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/php.py#L171) — Map callable names to (trait, method) from PHP use-trait conflict blocks.
  - `parse(self, path: Path, is_dependency: bool = False, index_source: bool = False)` — [`L70`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/php.py#L70)
  - `generic_parser_wrapper` — [`L65`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/php.py#L65)
  - `index_source` — [`L72`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/php.py#L72)
  - `language` — [`L67`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/php.py#L67)
  - `language_name` — [`L66`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/php.py#L66)
  - `parser` — [`L68`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/php.py#L68)
- protocol/private: `__init__`[`L64`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/php.py#L64), `_get_enclosing_class_name`[`L158`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/php.py#L158), `_get_node_text`[`L167`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/php.py#L167), `_get_parent_context`[`L145`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/php.py#L145), `_parse_calls`[`L433`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/php.py#L433), `_parse_functions`[`L201`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/php.py#L201), `_parse_imports`[`L391`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/php.py#L391), `_parse_types`[`L266`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/php.py#L266), `_parse_variables`[`L343`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/php.py#L343)
- uses (calls/refs, reference-scoped): [`warning_logger`](../../utils/debug_log.md#warning_logger), [`execute_query`](../../utils/tree_sitter_manager.md#execute_query), [`error_logger`](../../utils/debug_log.md#error_logger), [`PHP_QUERIES`](php.md#PHP_QUERIES)
- used by: [`language_specific_parser`](../tree_sitter_parser.md#TreeSitterParser.language_specific_parser)

## Functions
- `pre_scan_php(files: list[Path], parser_wrapper)` — [`L561`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/php.py#L561)

## Module values
- `PHP_QUERIES` — [`L9`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/php.py#L9)

