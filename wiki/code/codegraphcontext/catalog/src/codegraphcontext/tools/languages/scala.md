---
title: 'Module: src/codegraphcontext/tools/languages/scala.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/tools/languages/scala.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.tools.languages.scala`/
symbols:
  ScalaTreeSitterParser.index_source: ScalaTreeSitterParser#index_source.
  ScalaTreeSitterParser._get_node_text: ScalaTreeSitterParser#_get_node_text().
  ScalaTreeSitterParser._parse_functions: ScalaTreeSitterParser#_parse_functions().
  ScalaTreeSitterParser._parse_classes: ScalaTreeSitterParser#_parse_classes().
  ScalaTreeSitterParser._parse_calls: ScalaTreeSitterParser#_parse_calls().
  ScalaTreeSitterParser._parse_variables: ScalaTreeSitterParser#_parse_variables().
  ScalaTreeSitterParser._parse_imports: ScalaTreeSitterParser#_parse_imports().
  ScalaTreeSitterParser.language_name: ScalaTreeSitterParser#language_name.
  ScalaTreeSitterParser.collect_types: ScalaTreeSitterParser#collect_types().
  ScalaTreeSitterParser._get_parent_context: ScalaTreeSitterParser#_get_parent_context().
  pre_scan_scala: pre_scan_scala().
  SCALA_QUERIES: SCALA_QUERIES.
  ScalaTreeSitterParser: ScalaTreeSitterParser#
  ScalaTreeSitterParser.language: ScalaTreeSitterParser#language.
  ScalaTreeSitterParser.parser: ScalaTreeSitterParser#parser.
  ScalaTreeSitterParser._extract_parameter_names: ScalaTreeSitterParser#_extract_parameter_names().
  ScalaTreeSitterParser.__init__: ScalaTreeSitterParser#__init__().
  ScalaTreeSitterParser.generic_parser_wrapper: ScalaTreeSitterParser#generic_parser_wrapper.
  ScalaTreeSitterParser.parse: ScalaTreeSitterParser#parse().
---
# Module: [`src/codegraphcontext/tools/languages/scala.py`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/scala.py)

## Classes
### `ScalaTreeSitterParser`
- def: [`src/codegraphcontext/tools/languages/scala.py:42`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/scala.py#L42)
- signature: `class ScalaTreeSitterParser:`
- members:
  - `collect_types(node)` — [`L250`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/scala.py#L250)
  - `parse(self, path: Path, is_dependency: bool = False, index_source: bool = False)` — [`L49`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/scala.py#L49)
  - `generic_parser_wrapper` — [`L44`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/scala.py#L44)
  - `index_source` — [`L51`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/scala.py#L51)
  - `language` — [`L46`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/scala.py#L46)
  - `language_name` — [`L45`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/scala.py#L45)
  - `parser` — [`L47`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/scala.py#L47)
- protocol/private: `__init__`[`L43`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/scala.py#L43), `_extract_parameter_names`[`L470`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/scala.py#L470), `_get_node_text`[`L162`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/scala.py#L162), `_get_parent_context`[`L142`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/scala.py#L142), `_parse_calls`[`L385`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/scala.py#L385), `_parse_classes`[`L218`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/scala.py#L218), `_parse_functions`[`L166`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/scala.py#L166), `_parse_imports`[`L353`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/scala.py#L353), `_parse_variables`[`L290`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/scala.py#L290)
- uses (calls/refs, reference-scoped): [`warning_logger`](../../utils/debug_log.md#warning_logger), [`execute_query`](../../utils/tree_sitter_manager.md#execute_query), [`error_logger`](../../utils/debug_log.md#error_logger), [`SCALA_QUERIES`](scala.md#SCALA_QUERIES)
- used by: [`language_specific_parser`](../tree_sitter_parser.md#TreeSitterParser.language_specific_parser)

## Functions
- `pre_scan_scala(files: list[Path], parser_wrapper)` — [`L497`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/scala.py#L497)

## Module values
- `SCALA_QUERIES` — [`L8`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/scala.py#L8)

