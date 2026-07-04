---
title: 'Module: src/codegraphcontext/tools/languages/c.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/tools/languages/c.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.tools.languages.c`/
symbols:
  CTreeSitterParser.index_source: CTreeSitterParser#index_source.
  CTreeSitterParser._get_node_text: CTreeSitterParser#_get_node_text().
  CTreeSitterParser._find_functions: CTreeSitterParser#_find_functions().
  CTreeSitterParser._find_structs_unions_enums: CTreeSitterParser#_find_structs_unions_enums().
  CTreeSitterParser._find_macros: CTreeSitterParser#_find_macros().
  CTreeSitterParser._find_imports: CTreeSitterParser#_find_imports().
  CTreeSitterParser._find_calls: CTreeSitterParser#_find_calls().
  CTreeSitterParser._find_variables: CTreeSitterParser#_find_variables().
  CTreeSitterParser._find_enum_members: CTreeSitterParser#_find_enum_members().
  CTreeSitterParser.language_name: CTreeSitterParser#language_name.
  CTreeSitterParser._get_parent_context: CTreeSitterParser#_get_parent_context().
  CTreeSitterParser.language: CTreeSitterParser#language.
  C_QUERIES: C_QUERIES.
  CTreeSitterParser._calculate_complexity: CTreeSitterParser#_calculate_complexity().
  CTreeSitterParser._get_docstring: CTreeSitterParser#_get_docstring().
  CTreeSitterParser.traverse: CTreeSitterParser#traverse().
  pre_scan_c: pre_scan_c().
  CTreeSitterParser._parse_function_args: CTreeSitterParser#_parse_function_args().
  CTreeSitterParser._synthesize_define_handler_functions: CTreeSitterParser#_synthesize_define_handler_functions().
  CTreeSitterParser._find_xmacro_enum_members: CTreeSitterParser#_find_xmacro_enum_members().
  CTreeSitterParser: CTreeSitterParser#
  CTreeSitterParser.parser: CTreeSitterParser#parser.
  CTreeSitterParser.__init__: CTreeSitterParser#__init__().
  CTreeSitterParser.generic_parser_wrapper: CTreeSitterParser#generic_parser_wrapper.
  CTreeSitterParser.parse: CTreeSitterParser#parse().
---
# Module: [`src/codegraphcontext/tools/languages/c.py`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/c.py)

## Classes
### `CTreeSitterParser`
- def: [`src/codegraphcontext/tools/languages/c.py:131`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/c.py#L131)
- doc: A C-specific parser using tree-sitter.
- signature: `class CTreeSitterParser:`
- members:
  - `_calculate_complexity(self, node: Any)` — [`L200`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/c.py#L200) — Calculate cyclomatic complexity for C functions.
  - `_find_calls(self, root_node: Any)` — [`L620`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/c.py#L620) — Enhanced function call detection. — documented in [codegraphcontext-utils-tree_sitter_manager](../../../../../concepts/codegraphcontext-utils-tree_sitter_manager.md)
  - `_find_macros(self, root_node: Any)` — [`L712`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/c.py#L712) — Enhanced preprocessor macro detection.
  - `_find_structs_unions_enums(self, root_node: Any)` — [`L358`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/c.py#L358) — Find structs, unions, and enums (treated as classes in C).
  - `_find_variables(self, root_node: Any)` — [`L656`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/c.py#L656) — Enhanced variable declaration detection.
  - `_get_docstring(self, node: Any)` — [`L229`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/c.py#L229) — Extract comments as documentation.
  - `_get_parent_context(self, node: Any, types: tuple = ('function_definition', 'struct_specifier', 'union_specifier', 'enum_specifier'))` — [`L174`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/c.py#L174) — Get parent context for nested constructs.
  - `_parse_function_args(self, params_node: Any)` — [`L238`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/c.py#L238) — Enhanced helper to parse function arguments from a (parameter_list) node.
  - `_synthesize_define_handler_functions(self, source_code: str, path: Path)` — [`L277`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/c.py#L277) — Synthesize functions emitted by DEFINE_HANDLER(name) macro invocations.
  - `parse(self, path: Path, is_dependency: bool = False, index_source: bool = False)` — [`L143`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/c.py#L143) — Parses a C file and returns its structure.
  - `traverse(n, depth=0)` — [`L211`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/c.py#L211)
  - `generic_parser_wrapper` — [`L135`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/c.py#L135)
  - `index_source` — [`L145`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/c.py#L145)
  - `language` — [`L137`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/c.py#L137)
  - `language_name` — [`L136`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/c.py#L136)
  - `parser` — [`L138`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/c.py#L138)
- protocol/private: `__init__`[`L134`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/c.py#L134), `_find_enum_members`[`L488`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/c.py#L488), `_find_functions`[`L310`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/c.py#L310), `_find_imports`[`L599`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/c.py#L599), `_find_xmacro_enum_members`[`L542`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/c.py#L542), `_get_node_text`[`L140`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/c.py#L140)
- uses (calls/refs, reference-scoped): [`warning_logger`](../../utils/debug_log.md#warning_logger), [`execute_query`](../../utils/tree_sitter_manager.md#execute_query), [`MAX_AST_DEPTH`](../indexing/constants.md#MAX_AST_DEPTH), [`C_QUERIES`](c.md#C_QUERIES)
- used by: [`language_specific_parser`](../tree_sitter_parser.md#TreeSitterParser.language_specific_parser)

## Functions
- `pre_scan_c(files: list[Path], parser_wrapper)` — [`L756`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/c.py#L756) — Scans C files to create a map of function/struct/union/enum names to their file paths.

## Module values
- `C_QUERIES` — [`L8`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/c.py#L8)

