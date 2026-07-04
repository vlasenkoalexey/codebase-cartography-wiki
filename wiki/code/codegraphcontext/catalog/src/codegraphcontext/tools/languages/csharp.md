---
title: 'Module: src/codegraphcontext/tools/languages/csharp.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/tools/languages/csharp.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.tools.languages.csharp`/
symbols:
  CSharpTreeSitterParser.index_source: CSharpTreeSitterParser#index_source.
  CSharpTreeSitterParser._get_node_text: CSharpTreeSitterParser#_get_node_text().
  CSharpTreeSitterParser._parse_functions: CSharpTreeSitterParser#_parse_functions().
  CSharpTreeSitterParser._parse_type_declarations: CSharpTreeSitterParser#_parse_type_declarations().
  CSharpTreeSitterParser._parse_properties: CSharpTreeSitterParser#_parse_properties().
  CSharpTreeSitterParser._parse_calls: CSharpTreeSitterParser#_parse_calls().
  CSharpTreeSitterParser._parse_imports: CSharpTreeSitterParser#_parse_imports().
  CSharpTreeSitterParser.language_name: CSharpTreeSitterParser#language_name.
  CSharpTreeSitterParser._find_containing_type: CSharpTreeSitterParser#_find_containing_type().
  CSharpTreeSitterParser._get_parent_context: CSharpTreeSitterParser#_get_parent_context().
  CSharpTreeSitterParser._extract_parameters: CSharpTreeSitterParser#_extract_parameters().
  pre_scan_csharp: pre_scan_csharp().
  CSharpTreeSitterParser: CSharpTreeSitterParser#
  CSHARP_QUERIES: CSHARP_QUERIES.
  CSharpTreeSitterParser.language: CSharpTreeSitterParser#language.
  CSharpTreeSitterParser.parser: CSharpTreeSitterParser#parser.
  CSharpTreeSitterParser.__init__: CSharpTreeSitterParser#__init__().
  CSharpTreeSitterParser.generic_parser_wrapper: CSharpTreeSitterParser#generic_parser_wrapper.
  CSharpTreeSitterParser.parse: CSharpTreeSitterParser#parse().
---
# Module: [`src/codegraphcontext/tools/languages/csharp.py`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/csharp.py)

## Classes
### `CSharpTreeSitterParser`
- def: [`src/codegraphcontext/tools/languages/csharp.py:82`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/csharp.py#L82)
- signature: `class CSharpTreeSitterParser:`
- members:
  - `_find_containing_type(self, node, source_code)` — [`L452`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/csharp.py#L452) — Find the containing class, struct, interface, or record for a given node.
  - `_get_parent_context(self, node: Any, types: Tuple[str, ...] = ('class_declaration', 'struct_declaration', 'function_declaration', 'method_declaration'))` — [`L362`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/csharp.py#L362) — Find parent context for C# constructs.
  - `_parse_properties(self, captures: list, source_code: str, path: Path, root_node)` — [`L464`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/csharp.py#L464) — Parse C# properties.
  - `_parse_type_declarations(self, captures: list, source_code: str, path: Path, type_label: str)` — [`L251`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/csharp.py#L251) — Parse class, interface, struct, enum, or record declarations with inheritance info.
  - `parse(self, path: Path, is_dependency: bool = False, index_source: bool = False)` — [`L89`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/csharp.py#L89)
  - `generic_parser_wrapper` — [`L84`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/csharp.py#L84)
  - `index_source` — [`L91`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/csharp.py#L91) — documented in [codegraphcontext-utils-tree_sitter_manager](../../../../../concepts/codegraphcontext-utils-tree_sitter_manager.md)
  - `language` — [`L86`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/csharp.py#L86)
  - `language_name` — [`L85`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/csharp.py#L85)
  - `parser` — [`L87`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/csharp.py#L87)
- protocol/private: `__init__`[`L83`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/csharp.py#L83), `_extract_parameters`[`L432`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/csharp.py#L432), `_get_node_text`[`L377`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/csharp.py#L377), `_parse_calls`[`L381`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/csharp.py#L381), `_parse_functions`[`L186`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/csharp.py#L186), `_parse_imports`[`L327`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/csharp.py#L327)
- uses (calls/refs, reference-scoped): [`warning_logger`](../../utils/debug_log.md#warning_logger), [`execute_query`](../../utils/tree_sitter_manager.md#execute_query), [`error_logger`](../../utils/debug_log.md#error_logger), [`CSHARP_QUERIES`](csharp.md#CSHARP_QUERIES)
- used by: [`language_specific_parser`](../tree_sitter_parser.md#TreeSitterParser.language_specific_parser)

## Functions
- `pre_scan_csharp(files: list[Path], parser_wrapper)` — [`L521`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/csharp.py#L521) — Pre-scan C# files to build a name-to-files mapping.

## Module values
- `CSHARP_QUERIES` — [`L8`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/csharp.py#L8)

