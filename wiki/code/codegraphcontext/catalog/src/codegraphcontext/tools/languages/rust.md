---
title: 'Module: src/codegraphcontext/tools/languages/rust.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/tools/languages/rust.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.tools.languages.rust`/
symbols:
  RustTreeSitterParser._find_functions: RustTreeSitterParser#_find_functions().
  RustTreeSitterParser._get_node_text: RustTreeSitterParser#_get_node_text().
  RustTreeSitterParser.index_source: RustTreeSitterParser#index_source.
  RustTreeSitterParser._find_calls: RustTreeSitterParser#_find_calls().
  RustTreeSitterParser._find_types: RustTreeSitterParser#_find_types().
  RustTreeSitterParser._find_imports: RustTreeSitterParser#_find_imports().
  RustTreeSitterParser.language: RustTreeSitterParser#language.
  pre_scan_rust: pre_scan_rust().
  RustTreeSitterParser._parse_function_args: RustTreeSitterParser#_parse_function_args().
  RustTreeSitterParser._module_path_for_node: RustTreeSitterParser#_module_path_for_node().
  RustTreeSitterParser.collect_extern_functions: RustTreeSitterParser#collect_extern_functions().
  RustTreeSitterParser.language_name: RustTreeSitterParser#language_name.
  RustTreeSitterParser._get_parent_context: RustTreeSitterParser#_get_parent_context().
  RUST_QUERIES: RUST_QUERIES.
  RustTreeSitterParser: RustTreeSitterParser#
  RustTreeSitterParser.parser: RustTreeSitterParser#parser.
  RustTreeSitterParser.__init__: RustTreeSitterParser#__init__().
  RustTreeSitterParser.generic_parser_wrapper: RustTreeSitterParser#generic_parser_wrapper.
  RustTreeSitterParser.parse: RustTreeSitterParser#parse().
---
# Module: [`src/codegraphcontext/tools/languages/rust.py`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/rust.py)

## Classes
### `RustTreeSitterParser`
- def: [`src/codegraphcontext/tools/languages/rust.py:36`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/rust.py#L36)
- doc: A Rust-specific parser using tree-sitter.
- signature: `class RustTreeSitterParser:`
- members:
  - `_find_calls(self, root_node: Any)` — [`L321`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/rust.py#L321) — Finds all function and method calls.
  - `_parse_function_args(self, params_node: Any)` — [`L98`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/rust.py#L98) — Helper to parse function arguments from a (parameters) node.
  - `collect_extern_functions(item_node: Any)` — [`L173`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/rust.py#L173)
  - `parse(self, path: Path, is_dependency: bool = False, index_source: bool = False)` — [`L48`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/rust.py#L48) — Parses a Rust file and returns its structure.
  - `generic_parser_wrapper` — [`L40`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/rust.py#L40)
  - `index_source` — [`L50`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/rust.py#L50)
  - `language` — [`L42`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/rust.py#L42)
  - `language_name` — [`L41`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/rust.py#L41)
  - `parser` — [`L43`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/rust.py#L43)
- protocol/private: `__init__`[`L39`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/rust.py#L39), `_find_functions`[`L128`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/rust.py#L128), `_find_imports`[`L291`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/rust.py#L291), `_find_types`[`L216`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/rust.py#L216), `_get_node_text`[`L45`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/rust.py#L45), `_get_parent_context`[`L75`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/rust.py#L75), `_module_path_for_node`[`L117`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/rust.py#L117)
- uses (calls/refs, reference-scoped): [`execute_query`](../../utils/tree_sitter_manager.md#execute_query), [`RUST_QUERIES`](rust.md#RUST_QUERIES)
- used by: [`language_specific_parser`](../tree_sitter_parser.md#TreeSitterParser.language_specific_parser)

## Functions
- `pre_scan_rust(files: list[Path], parser_wrapper)` — [`L356`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/rust.py#L356) — Scans Rust files to create a map of function/struct/enum/trait names to their file paths.

## Module values
- `RUST_QUERIES` — [`L8`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/rust.py#L8)

