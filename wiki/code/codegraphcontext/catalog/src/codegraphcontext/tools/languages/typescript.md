---
title: 'Module: src/codegraphcontext/tools/languages/typescript.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/tools/languages/typescript.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.tools.languages.typescript`/
symbols:
  TypescriptTreeSitterParser._get_node_text: TypescriptTreeSitterParser#_get_node_text().
  TypescriptTreeSitterParser._find_functions: TypescriptTreeSitterParser#_find_functions().
  TypescriptTreeSitterParser.parse: TypescriptTreeSitterParser#parse().
  TypescriptTreeSitterParser._find_classes: TypescriptTreeSitterParser#_find_classes().
  TypescriptTreeSitterParser._find_calls: TypescriptTreeSitterParser#_find_calls().
  TypescriptTreeSitterParser._find_variables: TypescriptTreeSitterParser#_find_variables().
  TypescriptTreeSitterParser._find_interfaces: TypescriptTreeSitterParser#_find_interfaces().
  TypescriptTreeSitterParser._find_type_aliases: TypescriptTreeSitterParser#_find_type_aliases().
  TypescriptTreeSitterParser._find_imports: TypescriptTreeSitterParser#_find_imports().
  TypescriptTreeSitterParser._find_dynamic_imports: TypescriptTreeSitterParser#_find_dynamic_imports().
  TypescriptTreeSitterParser.language_name: TypescriptTreeSitterParser#language_name.
  TypescriptTreeSitterParser.language: TypescriptTreeSitterParser#language.
  pre_scan_typescript: pre_scan_typescript().
  TypescriptTreeSitterParser._get_parent_context: TypescriptTreeSitterParser#_get_parent_context().
  TypescriptTreeSitterParser._calculate_complexity: TypescriptTreeSitterParser#_calculate_complexity().
  TS_QUERIES: TS_QUERIES.
  TypescriptTreeSitterParser.traverse: TypescriptTreeSitterParser#traverse().
  TypescriptTreeSitterParser._collect_preceding_decorators: TypescriptTreeSitterParser#_collect_preceding_decorators().
  TypescriptTreeSitterParser: TypescriptTreeSitterParser#
  TypescriptTreeSitterParser._bucket_for: TypescriptTreeSitterParser#_bucket_for().
  TypescriptTreeSitterParser.index_source: TypescriptTreeSitterParser#index_source.
  TypescriptTreeSitterParser._extract_parameters: TypescriptTreeSitterParser#_extract_parameters().
  TypescriptTreeSitterParser.parser: TypescriptTreeSitterParser#parser.
  TypescriptTreeSitterParser._fn_for_params: TypescriptTreeSitterParser#_fn_for_params().
  TypescriptTreeSitterParser.__init__: TypescriptTreeSitterParser#__init__().
  TypescriptTreeSitterParser._get_docstring: TypescriptTreeSitterParser#_get_docstring().
  TypescriptTreeSitterParser._same_node: TypescriptTreeSitterParser#_same_node().
  TypescriptTreeSitterParser._fn_for_name: TypescriptTreeSitterParser#_fn_for_name().
  TypescriptTreeSitterParser._key: TypescriptTreeSitterParser#_key().
  is_typescript_file: is_typescript_file().
  TypescriptTreeSitterParser.generic_parser_wrapper: TypescriptTreeSitterParser#generic_parser_wrapper.
---
# Module: [`src/codegraphcontext/tools/languages/typescript.py`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/typescript.py)

## Classes
### `TypescriptTreeSitterParser`
- def: [`src/codegraphcontext/tools/languages/typescript.py:96`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/typescript.py#L96)
- doc: A TypeScript-specific parser using tree-sitter, encapsulating language-specific logic.
- signature: `class TypescriptTreeSitterParser:`
- members:
  - `_collect_preceding_decorators(self, node)` — [`L162`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/typescript.py#L162) — Collect decorator siblings immediately before a class or method node. — documented in [codegraphcontext-tools-languages-typescript](../../../../../concepts/codegraphcontext-tools-languages-typescript.md)
  - `parse(self, path: Path, is_dependency: bool = False, index_source: bool = False)` — [`L179`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/typescript.py#L179) — documented in [codegraphcontext-tools-languages-typescript](../../../../../concepts/codegraphcontext-tools-languages-typescript.md)
  - `traverse(n, depth=0)` — [`L135`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/typescript.py#L135) — documented in [codegraphcontext-tools-languages-typescript](../../../../../concepts/codegraphcontext-tools-languages-typescript.md)
  - `generic_parser_wrapper` — [`L100`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/typescript.py#L100)
  - `index_source` — [`L180`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/typescript.py#L180) — documented in [codegraphcontext-tools-languages-typescript](../../../../../concepts/codegraphcontext-tools-languages-typescript.md)
  - `language` — [`L102`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/typescript.py#L102) — documented in [codegraphcontext-tools-languages-typescript](../../../../../concepts/codegraphcontext-tools-languages-typescript.md)
  - `language_name` — [`L101`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/typescript.py#L101) — documented in [codegraphcontext-tools-languages-typescript](../../../../../concepts/codegraphcontext-tools-languages-typescript.md)
  - `parser` — [`L103`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/typescript.py#L103) — documented in [codegraphcontext-tools-languages-typescript](../../../../../concepts/codegraphcontext-tools-languages-typescript.md)
- protocol/private: `__init__`[`L99`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/typescript.py#L99), `_bucket_for`[`L232`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/typescript.py#L232), `_calculate_complexity`[`L126`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/typescript.py#L126), `_extract_parameters`[`L293`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/typescript.py#L293), `_find_calls`[`L479`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/typescript.py#L479), `_find_classes`[`L324`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/typescript.py#L324), `_find_dynamic_imports`[`L449`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/typescript.py#L449), `_find_functions`[`L208`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/typescript.py#L208), `_find_imports`[`L400`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/typescript.py#L400), `_find_interfaces`[`L362`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/typescript.py#L362), `_find_type_aliases`[`L381`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/typescript.py#L381), `_find_variables`[`L520`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/typescript.py#L520), `_fn_for_name`[`L211`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/typescript.py#L211), `_fn_for_params`[`L222`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/typescript.py#L222), `_get_docstring`[`L152`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/typescript.py#L152), `_get_node_text`[`L105`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/typescript.py#L105), `_get_parent_context`[`L108`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/typescript.py#L108), `_key`[`L229`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/typescript.py#L229), `_same_node`[`L155`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/typescript.py#L155)
- uses (calls/refs, reference-scoped): [`warning_logger`](../../utils/debug_log.md#warning_logger), [`execute_query`](../../utils/tree_sitter_manager.md#execute_query), [`MAX_AST_DEPTH`](../indexing/constants.md#MAX_AST_DEPTH), [`TS_QUERIES`](typescript.md#TS_QUERIES), [`TypescriptJSXTreeSitterParser`](typescriptjsx.md#TypescriptJSXTreeSitterParser), [`parse`](typescriptjsx.md#TypescriptJSXTreeSitterParser.parse)
- used by: [`language_specific_parser`](../tree_sitter_parser.md#TreeSitterParser.language_specific_parser), [`index_source`](typescriptjsx.md#TypescriptJSXTreeSitterParser.index_source), [`_find_react_components`](typescriptjsx.md#TypescriptJSXTreeSitterParser._find_react_components), [`TypescriptJSXTreeSitterParser`](typescriptjsx.md#TypescriptJSXTreeSitterParser), [`__init__`](typescriptjsx.md#TypescriptJSXTreeSitterParser.__init__)

## Functions
- `is_typescript_file(path: Path)` — [`L93`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/typescript.py#L93)
- `pre_scan_typescript(files: list[Path], parser_wrapper)` — [`L568`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/typescript.py#L568) — Scans TypeScript files to create a map of class/function names to their file paths.

## Module values
- `TS_QUERIES` — [`L7`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/typescript.py#L7) — documented in [codegraphcontext-tools-languages-typescript](../../../../../concepts/codegraphcontext-tools-languages-typescript.md)

