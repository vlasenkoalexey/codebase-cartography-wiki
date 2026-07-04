---
title: 'Module: src/codegraphcontext/tools/languages/swift.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/tools/languages/swift.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.tools.languages.swift`/
symbols:
  SwiftTreeSitterParser.index_source: SwiftTreeSitterParser#index_source.
  SwiftTreeSitterParser._get_node_text: SwiftTreeSitterParser#_get_node_text().
  SwiftTreeSitterParser._parse_functions: SwiftTreeSitterParser#_parse_functions().
  SwiftTreeSitterParser._parse_classes: SwiftTreeSitterParser#_parse_classes().
  SwiftTreeSitterParser._parse_variables: SwiftTreeSitterParser#_parse_variables().
  SwiftTreeSitterParser._calculate_complexity: SwiftTreeSitterParser#_calculate_complexity().
  SwiftTreeSitterParser._parse_calls: SwiftTreeSitterParser#_parse_calls().
  SwiftTreeSitterParser.language_name: SwiftTreeSitterParser#language_name.
  SwiftTreeSitterParser.traverse: SwiftTreeSitterParser#traverse().
  SwiftTreeSitterParser.find_id: SwiftTreeSitterParser#find_id().
  SwiftTreeSitterParser._parse_imports: SwiftTreeSitterParser#_parse_imports().
  SwiftTreeSitterParser._get_parent_context: SwiftTreeSitterParser#_get_parent_context().
  SwiftTreeSitterParser._extract_parameter_name: SwiftTreeSitterParser#_extract_parameter_name().
  SWIFT_QUERIES: SWIFT_QUERIES.
  SwiftTreeSitterParser: SwiftTreeSitterParser#
  SwiftTreeSitterParser.language: SwiftTreeSitterParser#language.
  SwiftTreeSitterParser.parser: SwiftTreeSitterParser#parser.
  pre_scan_swift: pre_scan_swift().
  SwiftTreeSitterParser.__init__: SwiftTreeSitterParser#__init__().
  SwiftTreeSitterParser.generic_parser_wrapper: SwiftTreeSitterParser#generic_parser_wrapper.
  SwiftTreeSitterParser.parse: SwiftTreeSitterParser#parse().
---
# Module: [`src/codegraphcontext/tools/languages/swift.py`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/swift.py)

## Classes
### `SwiftTreeSitterParser`
- def: [`src/codegraphcontext/tools/languages/swift.py:38`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/swift.py#L38)
- signature: `class SwiftTreeSitterParser:`
- members:
  - `_calculate_complexity(self, node: Any)` — [`L198`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/swift.py#L198) — Cyclomatic complexity for a Swift function/init body.
  - `_extract_parameter_name(self, param_node: Any)` — [`L575`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/swift.py#L575) — Extract parameter name from a parameter node.
  - `find_id(n)` — [`L420`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/swift.py#L420)
  - `parse(self, path: Path, is_dependency: bool = False, index_source: bool = False)` — [`L45`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/swift.py#L45)
  - `traverse(n: Any, depth: int = 0)` — [`L219`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/swift.py#L219)
  - `generic_parser_wrapper` — [`L40`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/swift.py#L40)
  - `index_source` — [`L47`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/swift.py#L47)
  - `language` — [`L42`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/swift.py#L42)
  - `language_name` — [`L41`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/swift.py#L41)
  - `parser` — [`L43`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/swift.py#L43)
- protocol/private: `__init__`[`L39`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/swift.py#L39), `_get_node_text`[`L194`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/swift.py#L194), `_get_parent_context`[`L130`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/swift.py#L130), `_parse_calls`[`L500`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/swift.py#L500), `_parse_classes`[`L309`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/swift.py#L309), `_parse_functions`[`L242`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/swift.py#L242), `_parse_imports`[`L473`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/swift.py#L473), `_parse_variables`[`L406`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/swift.py#L406)
- uses (calls/refs, reference-scoped): [`warning_logger`](../../utils/debug_log.md#warning_logger), [`execute_query`](../../utils/tree_sitter_manager.md#execute_query), [`error_logger`](../../utils/debug_log.md#error_logger), [`MAX_AST_DEPTH`](../indexing/constants.md#MAX_AST_DEPTH), [`SWIFT_QUERIES`](swift.md#SWIFT_QUERIES)
- used by: [`language_specific_parser`](../tree_sitter_parser.md#TreeSitterParser.language_specific_parser)

## Functions
- `pre_scan_swift(files: list[Path], parser_wrapper)` — [`L584`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/swift.py#L584) — Pre-scan Swift files to build a map of class/struct/enum/protocol names to file paths.

## Module values
- `SWIFT_QUERIES` — [`L8`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/swift.py#L8)

