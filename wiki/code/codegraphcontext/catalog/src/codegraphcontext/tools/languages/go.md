---
title: 'Module: src/codegraphcontext/tools/languages/go.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/tools/languages/go.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.tools.languages.go`/
symbols:
  GoTreeSitterParser._find_functions: GoTreeSitterParser#_find_functions().
  GoTreeSitterParser._get_node_text: GoTreeSitterParser#_get_node_text().
  GoTreeSitterParser._find_interfaces: GoTreeSitterParser#_find_interfaces().
  GoTreeSitterParser.parse: GoTreeSitterParser#parse().
  GoTreeSitterParser._find_structs: GoTreeSitterParser#_find_structs().
  GoTreeSitterParser._find_calls: GoTreeSitterParser#_find_calls().
  GoTreeSitterParser._find_imports: GoTreeSitterParser#_find_imports().
  GoTreeSitterParser._find_variables: GoTreeSitterParser#_find_variables().
  GoTreeSitterParser.traverse: GoTreeSitterParser#traverse().
  GoTreeSitterParser._calculate_complexity: GoTreeSitterParser#_calculate_complexity().
  GoTreeSitterParser.language_name: GoTreeSitterParser#language_name.
  GO_QUERIES: GO_QUERIES.
  GoTreeSitterParser.language: GoTreeSitterParser#language.
  pre_scan_go: pre_scan_go().
  GoTreeSitterParser._get_docstring: GoTreeSitterParser#_get_docstring().
  GoTreeSitterParser._get_parent_context: GoTreeSitterParser#_get_parent_context().
  GoTreeSitterParser.index_source: GoTreeSitterParser#index_source.
  GoTreeSitterParser._extract_parameters: GoTreeSitterParser#_extract_parameters().
  GoTreeSitterParser._extract_receiver: GoTreeSitterParser#_extract_receiver().
  GoTreeSitterParser._extract_interface_methods: GoTreeSitterParser#_extract_interface_methods().
  GoTreeSitterParser: GoTreeSitterParser#
  GoTreeSitterParser._find_type_declaration_for_name: GoTreeSitterParser#_find_type_declaration_for_name().
  GoTreeSitterParser.parser: GoTreeSitterParser#parser.
  GoTreeSitterParser._find_function_node_for_name: GoTreeSitterParser#_find_function_node_for_name().
  GoTreeSitterParser._find_function_node_for_params: GoTreeSitterParser#_find_function_node_for_params().
  GoTreeSitterParser.__init__: GoTreeSitterParser#__init__().
  GoTreeSitterParser.generic_parser_wrapper: GoTreeSitterParser#generic_parser_wrapper.
---
# Module: [`src/codegraphcontext/tools/languages/go.py`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/go.py)

## Classes
### `GoTreeSitterParser`
- def: [`src/codegraphcontext/tools/languages/go.py:75`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/go.py#L75)
- doc: A Go-specific parser using tree-sitter, encapsulating language-specific logic.
- signature: `class GoTreeSitterParser:`
- members:
  - `_get_docstring(self, func_node)` — [`L166`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/go.py#L166) — Extract Go doc comment preceding the function.
  - `parse(self, path: Path, is_dependency: bool = False, index_source: bool = False)` — [`L177`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/go.py#L177) — Parses a file and returns its structure in a standardized dictionary format.
  - `traverse(n, depth=0)` — [`L137`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/go.py#L137)
  - `generic_parser_wrapper` — [`L79`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/go.py#L79)
  - `index_source` — [`L83`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/go.py#L83)
  - `language` — [`L81`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/go.py#L81)
  - `language_name` — [`L80`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/go.py#L80)
  - `parser` — [`L82`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/go.py#L82)
- protocol/private: `__init__`[`L78`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/go.py#L78), `_calculate_complexity`[`L103`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/go.py#L103), `_extract_interface_methods`[`L431`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/go.py#L431), `_extract_parameters`[`L319`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/go.py#L319), `_extract_receiver`[`L337`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/go.py#L337), `_find_calls`[`L530`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/go.py#L530), `_find_function_node_for_name`[`L303`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/go.py#L303), `_find_function_node_for_params`[`L311`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/go.py#L311), `_find_functions`[`L211`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/go.py#L211), `_find_imports`[`L502`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/go.py#L502), `_find_interfaces`[`L447`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/go.py#L447), `_find_structs`[`L346`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/go.py#L346), `_find_type_declaration_for_name`[`L494`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/go.py#L494), `_find_variables`[`L576`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/go.py#L576), `_get_node_text`[`L85`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/go.py#L85), `_get_parent_context`[`L88`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/go.py#L88)
- uses (calls/refs, reference-scoped): [`warning_logger`](../../utils/debug_log.md#warning_logger), [`execute_query`](../../utils/tree_sitter_manager.md#execute_query), [`MAX_AST_DEPTH`](../indexing/constants.md#MAX_AST_DEPTH), [`GO_QUERIES`](go.md#GO_QUERIES)
- used by: [`language_specific_parser`](../tree_sitter_parser.md#TreeSitterParser.language_specific_parser)

## Functions
- `pre_scan_go(files: list[Path], parser_wrapper)` — [`L598`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/go.py#L598) — Scans Go files to create a map of function/struct names to their file paths.

## Module values
- `GO_QUERIES` — [`L8`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/go.py#L8)

