---
title: 'Module: src/codegraphcontext/tools/languages/cpp.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/tools/languages/cpp.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.tools.languages.cpp`/
symbols:
  CppTreeSitterParser.index_source: CppTreeSitterParser#index_source.
  CppTreeSitterParser._get_node_text: CppTreeSitterParser#_get_node_text().
  CppTreeSitterParser._find_lambda_assignments: CppTreeSitterParser#_find_lambda_assignments().
  CppTreeSitterParser._find_functions: CppTreeSitterParser#_find_functions().
  CppTreeSitterParser._find_classes: CppTreeSitterParser#_find_classes().
  CppTreeSitterParser._find_variables: CppTreeSitterParser#_find_variables().
  CppTreeSitterParser._find_calls: CppTreeSitterParser#_find_calls().
  CppTreeSitterParser._find_enums: CppTreeSitterParser#_find_enums().
  CppTreeSitterParser._find_structs: CppTreeSitterParser#_find_structs().
  CppTreeSitterParser._find_unions: CppTreeSitterParser#_find_unions().
  CppTreeSitterParser._find_macros: CppTreeSitterParser#_find_macros().
  CppTreeSitterParser._find_imports: CppTreeSitterParser#_find_imports().
  CPP_QUERIES: CPP_QUERIES.
  CppTreeSitterParser.language: CppTreeSitterParser#language.
  pre_scan_cpp: pre_scan_cpp().
  CppTreeSitterParser._get_parent_context: CppTreeSitterParser#_get_parent_context().
  CppTreeSitterParser.language_name: CppTreeSitterParser#language_name.
  CppTreeSitterParser._extract_function_params: CppTreeSitterParser#_extract_function_params().
  CppTreeSitterParser._extract_base_classes: CppTreeSitterParser#_extract_base_classes().
  CppTreeSitterParser: CppTreeSitterParser#
  CppTreeSitterParser.parser: CppTreeSitterParser#parser.
  CppTreeSitterParser.__init__: CppTreeSitterParser#__init__().
  CppTreeSitterParser.generic_parser_wrapper: CppTreeSitterParser#generic_parser_wrapper.
  CppTreeSitterParser.parse: CppTreeSitterParser#parse().
  CppTreeSitterParser._get_full_name: CppTreeSitterParser#_get_full_name().
---
# Module: [`src/codegraphcontext/tools/languages/cpp.py`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/cpp.py)

## Classes
### `CppTreeSitterParser`
- def: [`src/codegraphcontext/tools/languages/cpp.py:129`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/cpp.py#L129)
- doc: A C++-specific parser using tree-sitter.
- signature: `class CppTreeSitterParser:`
- members:
  - `_extract_base_classes(self, class_node)` — [`L279`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/cpp.py#L279) — Extract base class names from a class_specifier node.
  - `_get_full_name(self, node)` — [`L611`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/cpp.py#L611) — Builds a fully qualified name for a function or call node.
  - `parse(self, path: Path, is_dependency: bool = False, index_source: bool = False, **kwargs)` — [`L141`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/cpp.py#L141) — Parses a C++ file and returns its structure.
  - `generic_parser_wrapper` — [`L133`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/cpp.py#L133)
  - `index_source` — [`L143`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/cpp.py#L143)
  - `language` — [`L135`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/cpp.py#L135)
  - `language_name` — [`L134`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/cpp.py#L134)
  - `parser` — [`L136`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/cpp.py#L136)
- protocol/private: `__init__`[`L132`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/cpp.py#L132), `_extract_function_params`[`L220`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/cpp.py#L220), `_find_calls`[`L550`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/cpp.py#L550), `_find_classes`[`L258`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/cpp.py#L258), `_find_enums`[`L329`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/cpp.py#L329), `_find_functions`[`L177`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/cpp.py#L177), `_find_imports`[`L313`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/cpp.py#L313), `_find_lambda_assignments`[`L433`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/cpp.py#L433), `_find_macros`[`L414`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/cpp.py#L414), `_find_structs`[`L356`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/cpp.py#L356), `_find_unions`[`L387`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/cpp.py#L387), `_find_variables`[`L479`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/cpp.py#L479), `_get_node_text`[`L138`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/cpp.py#L138), `_get_parent_context`[`L516`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/cpp.py#L516)
- uses (calls/refs, reference-scoped): [`execute_query`](../../utils/tree_sitter_manager.md#execute_query), [`CPP_QUERIES`](cpp.md#CPP_QUERIES)
- used by: [`language_specific_parser`](../tree_sitter_parser.md#TreeSitterParser.language_specific_parser)

## Functions
- `pre_scan_cpp(files: list[Path], parser_wrapper)` — [`L640`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/cpp.py#L640) — Quickly scans C++ files to build a map of top-level class, struct, and function names

## Module values
- `CPP_QUERIES` — [`L8`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/cpp.py#L8)

