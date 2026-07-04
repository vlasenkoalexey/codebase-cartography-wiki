---
title: 'Module: src/codegraphcontext/tools/languages/dart.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/tools/languages/dart.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.tools.languages.dart`/
symbols:
  DartTreeSitterParser.parse: DartTreeSitterParser#parse().
  DartTreeSitterParser._get_node_text: DartTreeSitterParser#_get_node_text().
  DartTreeSitterParser._find_functions: DartTreeSitterParser#_find_functions().
  DartTreeSitterParser._find_calls: DartTreeSitterParser#_find_calls().
  DartTreeSitterParser._find_types: DartTreeSitterParser#_find_types().
  DartTreeSitterParser._find_variables: DartTreeSitterParser#_find_variables().
  DartTreeSitterParser._find_imports: DartTreeSitterParser#_find_imports().
  pre_scan_dart: pre_scan_dart().
  DartTreeSitterParser._get_parent_context: DartTreeSitterParser#_get_parent_context().
  DartTreeSitterParser.traverse: DartTreeSitterParser#traverse().
  DartTreeSitterParser._receiver_name_for_call_selector: DartTreeSitterParser#_receiver_name_for_call_selector().
  DartTreeSitterParser._calculate_complexity: DartTreeSitterParser#_calculate_complexity().
  DartTreeSitterParser._initializer_type_name: DartTreeSitterParser#_initializer_type_name().
  DartTreeSitterParser.collect_bases: DartTreeSitterParser#collect_bases().
  DartTreeSitterParser.find_id: DartTreeSitterParser#find_id().
  DartTreeSitterParser.language_name: DartTreeSitterParser#language_name.
  DartTreeSitterParser._name_node_for_call_selector: DartTreeSitterParser#_name_node_for_call_selector().
  DartTreeSitterParser._last_identifier_in: DartTreeSitterParser#_last_identifier_in().
  DART_QUERIES: DART_QUERIES.
  DartTreeSitterParser.language: DartTreeSitterParser#language.
  DartTreeSitterParser.find_uri: DartTreeSitterParser#find_uri().
  DartTreeSitterParser._extract_param_name: DartTreeSitterParser#_extract_param_name().
  DartTreeSitterParser: DartTreeSitterParser#
  DartTreeSitterParser.index_source: DartTreeSitterParser#index_source.
  SIGNATURE_TYPES: SIGNATURE_TYPES.
  _CALL_PUNCTUATION: _CALL_PUNCTUATION.
  pre_scan_dart.register: pre_scan_dart().register().
  CONTAINER_TYPES: CONTAINER_TYPES.
  DartTreeSitterParser.parser: DartTreeSitterParser#parser.
  DartTreeSitterParser._has_call_selector_sibling: DartTreeSitterParser#_has_call_selector_sibling().
  DartTreeSitterParser._parse_library_parts: DartTreeSitterParser#_parse_library_parts().
  DartTreeSitterParser.__init__: DartTreeSitterParser#__init__().
  DartTreeSitterParser.generic_parser_wrapper: DartTreeSitterParser#generic_parser_wrapper.
---
# Module: [`src/codegraphcontext/tools/languages/dart.py`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/dart.py)

## Classes
### `DartTreeSitterParser`
- def: [`src/codegraphcontext/tools/languages/dart.py:84`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/dart.py#L84)
- doc: A Dart-specific parser using tree-sitter, encapsulating language-specific logic.
- signature: `class DartTreeSitterParser:`
- members:
  - `_has_call_selector_sibling(self, name_node)` — [`L207`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/dart.py#L207) — Return True if an identifier is a receiver beside a call selector.
  - `_last_identifier_in(self, node)` — [`L143`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/dart.py#L143) — Return the deepest-last identifier under node.
  - `_name_node_for_call_selector(self, call_node)` — [`L183`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/dart.py#L183) — Find the receiver/member name paired with a captured argument selector.
  - `_receiver_name_for_call_selector(self, call_node: Any)` — [`L155`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/dart.py#L155) — Return the receiver identifier for `receiver.method()` calls.
  - `collect_bases(n)` — [`L352`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/dart.py#L352)
  - `find_id(n)` — [`L464`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/dart.py#L464)
  - `find_uri(n)` — [`L480`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/dart.py#L480)
  - `parse(self, path: Path, is_dependency: bool = False, index_source: bool = False)` — [`L254`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/dart.py#L254) — Parses a Dart file and returns its structure in a standardized dictionary format.
  - `traverse(n, depth=0)` — [`L231`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/dart.py#L231)
  - `generic_parser_wrapper` — [`L88`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/dart.py#L88)
  - `index_source` — [`L92`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/dart.py#L92)
  - `language` — [`L90`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/dart.py#L90)
  - `language_name` — [`L89`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/dart.py#L89)
  - `parser` — [`L91`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/dart.py#L91)
- protocol/private: `__init__`[`L87`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/dart.py#L87), `_calculate_complexity`[`L221`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/dart.py#L221), `_extract_param_name`[`L461`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/dart.py#L461), `_find_calls`[`L513`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/dart.py#L513), `_find_functions`[`L376`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/dart.py#L376), `_find_imports`[`L473`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/dart.py#L473), `_find_types`[`L327`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/dart.py#L327), `_find_variables`[`L600`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/dart.py#L600), `_get_node_text`[`L94`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/dart.py#L94), `_get_parent_context`[`L98`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/dart.py#L98), `_initializer_type_name`[`L567`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/dart.py#L567), `_parse_library_parts`[`L308`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/dart.py#L308)
- uses (calls/refs, reference-scoped): [`warning_logger`](../../utils/debug_log.md#warning_logger), [`execute_query`](../../utils/tree_sitter_manager.md#execute_query), [`error_logger`](../../utils/debug_log.md#error_logger), [`MAX_AST_DEPTH`](../indexing/constants.md#MAX_AST_DEPTH), [`DART_QUERIES`](dart.md#DART_QUERIES), [`SIGNATURE_TYPES`](dart.md#SIGNATURE_TYPES), [`_CALL_PUNCTUATION`](dart.md#_CALL_PUNCTUATION), [`CONTAINER_TYPES`](dart.md#CONTAINER_TYPES)
- used by: [`language_specific_parser`](../tree_sitter_parser.md#TreeSitterParser.language_specific_parser), [`pre_scan_dart`](dart.md#pre_scan_dart)

## Functions
- `pre_scan_dart(files: List[Path], parser_wrapper)` — [`L645`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/dart.py#L645) — Scans Dart files to create a map of class/function names to their file paths.
- `register(name: str, file_path: str)` — [`L650`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/dart.py#L650)

## Module values
- `CONTAINER_TYPES` — [`L76`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/dart.py#L76)
- `DART_QUERIES` — [`L9`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/dart.py#L9)
- `SIGNATURE_TYPES` — [`L67`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/dart.py#L67)
- `_CALL_PUNCTUATION` — [`L81`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/dart.py#L81)

