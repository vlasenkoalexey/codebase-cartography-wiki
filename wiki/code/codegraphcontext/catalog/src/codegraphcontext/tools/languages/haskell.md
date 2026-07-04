---
title: 'Module: src/codegraphcontext/tools/languages/haskell.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/tools/languages/haskell.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.tools.languages.haskell`/
symbols:
  HaskellTreeSitterParser.parse: HaskellTreeSitterParser#parse().
  HaskellTreeSitterParser._get_node_text: HaskellTreeSitterParser#_get_node_text().
  HaskellTreeSitterParser._parse_functions: HaskellTreeSitterParser#_parse_functions().
  HaskellTreeSitterParser._parse_variables: HaskellTreeSitterParser#_parse_variables().
  HaskellTreeSitterParser.language_name: HaskellTreeSitterParser#language_name.
  HaskellTreeSitterParser.walk: HaskellTreeSitterParser#walk().
  HaskellTreeSitterParser._parse_classes: HaskellTreeSitterParser#_parse_classes().
  HaskellTreeSitterParser._parse_calls: HaskellTreeSitterParser#_parse_calls().
  HaskellTreeSitterParser._get_parent_context: HaskellTreeSitterParser#_get_parent_context().
  HaskellTreeSitterParser._parse_instances: HaskellTreeSitterParser#_parse_instances().
  HaskellTreeSitterParser._parse_imports: HaskellTreeSitterParser#_parse_imports().
  HaskellTreeSitterParser._empty_result: HaskellTreeSitterParser#_empty_result().
  HaskellTreeSitterParser.index_source: HaskellTreeSitterParser#index_source.
  HaskellTreeSitterParser._get_enclosing_function_context: HaskellTreeSitterParser#_get_enclosing_function_context().
  HaskellTreeSitterParser._pattern_arg_names: HaskellTreeSitterParser#_pattern_arg_names().
  HaskellTreeSitterParser._apply_callee_name: HaskellTreeSitterParser#_apply_callee_name().
  HaskellTreeSitterParser._variables_in_type_ast: HaskellTreeSitterParser#_variables_in_type_ast().
  HASKELL_QUERIES: HASKELL_QUERIES.
  HaskellTreeSitterParser: HaskellTreeSitterParser#
  HaskellTreeSitterParser.language: HaskellTreeSitterParser#language.
  HaskellTreeSitterParser.parser: HaskellTreeSitterParser#parser.
  pre_scan_haskell: pre_scan_haskell().
  HaskellTreeSitterParser.__init__: HaskellTreeSitterParser#__init__().
  HaskellTreeSitterParser.generic_parser_wrapper: HaskellTreeSitterParser#generic_parser_wrapper.
---
# Module: [`src/codegraphcontext/tools/languages/haskell.py`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/haskell.py)

## Classes
### `HaskellTreeSitterParser`
- def: [`src/codegraphcontext/tools/languages/haskell.py:44`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/haskell.py#L44)
- doc: Parse Haskell sources using tree-sitter-haskell.
- signature: `class HaskellTreeSitterParser:`
- members:
  - `_get_enclosing_function_context(self, node: Any)` — [`L93`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/haskell.py#L93) — Return the nearest enclosing function (skip local do-notation bind nodes).
  - `_variables_in_type_ast(self, type_root: Any)` — [`L403`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/haskell.py#L403) — Collect `variable` nodes that appear in a type (tree-sitter-haskell type parameters).
  - `parse(self, path: Path, is_dependency: bool = False, index_source: bool = False)` — [`L138`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/haskell.py#L138) — documented in [codegraphcontext-utils-debug_log](../../../../../concepts/codegraphcontext-utils-debug_log.md)
  - `walk(n: Any)` — [`L128`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/haskell.py#L128)
  - `generic_parser_wrapper` — [`L48`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/haskell.py#L48)
  - `index_source` — [`L52`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/haskell.py#L52)
  - `language` — [`L50`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/haskell.py#L50)
  - `language_name` — [`L49`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/haskell.py#L49)
  - `parser` — [`L51`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/haskell.py#L51)
- protocol/private: `__init__`[`L47`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/haskell.py#L47), `_apply_callee_name`[`L204`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/haskell.py#L204), `_empty_result`[`L191`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/haskell.py#L191), `_get_node_text`[`L54`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/haskell.py#L54), `_get_parent_context`[`L59`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/haskell.py#L59), `_parse_calls`[`L442`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/haskell.py#L442), `_parse_classes`[`L309`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/haskell.py#L309), `_parse_functions`[`L242`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/haskell.py#L242), `_parse_imports`[`L417`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/haskell.py#L417), `_parse_instances`[`L212`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/haskell.py#L212), `_parse_variables`[`L347`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/haskell.py#L347), `_pattern_arg_names`[`L123`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/haskell.py#L123)
- uses (calls/refs, reference-scoped): [`warning_logger`](../../utils/debug_log.md#warning_logger), [`execute_query`](../../utils/tree_sitter_manager.md#execute_query), [`error_logger`](../../utils/debug_log.md#error_logger), [`HASKELL_QUERIES`](haskell.md#HASKELL_QUERIES)
- used by: [`language_specific_parser`](../tree_sitter_parser.md#TreeSitterParser.language_specific_parser)

## Functions
- `pre_scan_haskell(files: list[Path], parser_wrapper)` — [`L479`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/haskell.py#L479) — Map declared names to file paths using lightweight regex (no full parse).

## Module values
- `HASKELL_QUERIES` — [`L14`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/haskell.py#L14)

