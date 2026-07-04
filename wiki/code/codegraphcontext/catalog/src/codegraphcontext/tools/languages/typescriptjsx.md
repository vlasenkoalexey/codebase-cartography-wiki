---
title: 'Module: src/codegraphcontext/tools/languages/typescriptjsx.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/tools/languages/typescriptjsx.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.tools.languages.typescriptjsx`/
symbols:
  TypescriptJSXTreeSitterParser.index_source: TypescriptJSXTreeSitterParser#index_source.
  TypescriptJSXTreeSitterParser._find_react_components: TypescriptJSXTreeSitterParser#_find_react_components().
  pre_scan_typescript: pre_scan_typescript().
  TypescriptJSXTreeSitterParser: TypescriptJSXTreeSitterParser#
  TypescriptJSXTreeSitterParser.__init__: TypescriptJSXTreeSitterParser#__init__().
  TypescriptJSXTreeSitterParser.language_name: TypescriptJSXTreeSitterParser#language_name.
  TypescriptJSXTreeSitterParser.jsx_enabled: TypescriptJSXTreeSitterParser#jsx_enabled.
  TypescriptJSXTreeSitterParser.parse: TypescriptJSXTreeSitterParser#parse().
---
# Module: [`src/codegraphcontext/tools/languages/typescriptjsx.py`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/typescriptjsx.py)

## Classes
### `TypescriptJSXTreeSitterParser`  ·  implements/extends TypescriptTreeSitterParser
- def: [`src/codegraphcontext/tools/languages/typescriptjsx.py:70`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/typescriptjsx.py#L70)
- doc: A parser for TypeScript JSX (.tsx) files.
- signature: `class TypescriptJSXTreeSitterParser(TypescriptTreeSitterParser):`
- members:
  - `_find_react_components(self, root_node)` — [`L115`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/typescriptjsx.py#L115) — Find React components in .tsx files (function and class components).
  - `parse(self, path: Path, is_dependency: bool = False, index_source: bool = False)` — [`L78`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/typescriptjsx.py#L78) — Parse a .tsx file, reusing TypeScript logic and ensuring JSX nodes are handled. — documented in [codegraphcontext-tools-languages-typescript](../../../../../concepts/codegraphcontext-tools-languages-typescript.md)
  - `index_source` — [`L83`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/typescriptjsx.py#L83)
  - `jsx_enabled` — [`L77`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/typescriptjsx.py#L77)
  - `language_name` — [`L76`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/typescriptjsx.py#L76)
- protocol/private: `__init__`[`L74`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/typescriptjsx.py#L74)
- uses (calls/refs, reference-scoped): [`execute_query`](../../utils/tree_sitter_manager.md#execute_query), [`_find_functions`](typescript.md#TypescriptTreeSitterParser._find_functions), [`_find_classes`](typescript.md#TypescriptTreeSitterParser._find_classes), [`_find_calls`](typescript.md#TypescriptTreeSitterParser._find_calls), [`_find_variables`](typescript.md#TypescriptTreeSitterParser._find_variables), [`_find_imports`](typescript.md#TypescriptTreeSitterParser._find_imports), [`_find_interfaces`](typescript.md#TypescriptTreeSitterParser._find_interfaces), [`_find_type_aliases`](typescript.md#TypescriptTreeSitterParser._find_type_aliases), [`language`](typescript.md#TypescriptTreeSitterParser.language), [`TypescriptTreeSitterParser`](typescript.md#TypescriptTreeSitterParser), [`parser`](typescript.md#TypescriptTreeSitterParser.parser), [`__init__`](typescript.md#TypescriptTreeSitterParser.__init__)
- used by: [`language_specific_parser`](../tree_sitter_parser.md#TreeSitterParser.language_specific_parser), [`parse`](typescript.md#TypescriptTreeSitterParser.parse), [`TypescriptTreeSitterParser`](typescript.md#TypescriptTreeSitterParser)

## Functions
- `pre_scan_typescript(files: list[Path], parser_wrapper)` — [`L4`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/typescriptjsx.py#L4) — Scans TypeScript JSX (.tsx) files to create a map of class/function names to their file paths.

