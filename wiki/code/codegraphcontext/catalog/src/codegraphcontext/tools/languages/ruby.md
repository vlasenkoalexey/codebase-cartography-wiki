---
title: 'Module: src/codegraphcontext/tools/languages/ruby.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/tools/languages/ruby.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.tools.languages.ruby`/
symbols:
  RubyTreeSitterParser.index_source: RubyTreeSitterParser#index_source.
  RubyTreeSitterParser._find_functions: RubyTreeSitterParser#_find_functions().
  RubyTreeSitterParser._find_classes: RubyTreeSitterParser#_find_classes().
  RubyTreeSitterParser._get_node_text: RubyTreeSitterParser#_get_node_text().
  RubyTreeSitterParser._find_modules: RubyTreeSitterParser#_find_modules().
  RubyTreeSitterParser._find_module_inclusions: RubyTreeSitterParser#_find_module_inclusions().
  RubyTreeSitterParser._find_calls: RubyTreeSitterParser#_find_calls().
  RubyTreeSitterParser._find_imports: RubyTreeSitterParser#_find_imports().
  RubyTreeSitterParser._find_variables: RubyTreeSitterParser#_find_variables().
  RubyTreeSitterParser.language_name: RubyTreeSitterParser#language_name.
  RubyTreeSitterParser.language: RubyTreeSitterParser#language.
  RubyTreeSitterParser._get_parent_context: RubyTreeSitterParser#_get_parent_context().
  RubyTreeSitterParser._calculate_complexity: RubyTreeSitterParser#_calculate_complexity().
  RUBY_QUERIES: RUBY_QUERIES.
  RubyTreeSitterParser.traverse: RubyTreeSitterParser#traverse().
  pre_scan_ruby: pre_scan_ruby().
  RubyTreeSitterParser._get_docstring: RubyTreeSitterParser#_get_docstring().
  RubyTreeSitterParser._enclosing_class_name: RubyTreeSitterParser#_enclosing_class_name().
  RubyTreeSitterParser._parse_method_parameters: RubyTreeSitterParser#_parse_method_parameters().
  RubyTreeSitterParser: RubyTreeSitterParser#
  RubyTreeSitterParser.parser: RubyTreeSitterParser#parser.
  RubyTreeSitterParser.__init__: RubyTreeSitterParser#__init__().
  RubyTreeSitterParser.generic_parser_wrapper: RubyTreeSitterParser#generic_parser_wrapper.
  RubyTreeSitterParser.parse: RubyTreeSitterParser#parse().
---
# Module: [`src/codegraphcontext/tools/languages/ruby.py`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/ruby.py)

## Classes
### `RubyTreeSitterParser`
- def: [`src/codegraphcontext/tools/languages/ruby.py:60`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/ruby.py#L60)
- doc: A Ruby-specific parser using tree-sitter.
- signature: `class RubyTreeSitterParser:`
- members:
  - `_calculate_complexity(self, node: Any)` — [`L143`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/ruby.py#L143) — Calculate cyclomatic complexity for Ruby constructs.
  - `_find_calls(self, root_node: Any)` — [`L414`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/ruby.py#L414) — Find all function and method calls.
  - `_find_classes(self, root_node: Any)` — [`L292`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/ruby.py#L292) — Find all class and module definitions. — documented in [codegraphcontext-utils-tree_sitter_manager](../../../../../concepts/codegraphcontext-utils-tree_sitter_manager.md)
  - `_find_functions(self, root_node: Any)` — [`L236`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/ruby.py#L236) — Find all function/method definitions.
  - `_find_imports(self, root_node: Any)` — [`L357`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/ruby.py#L357) — Find all require/load statements.
  - `_find_variables(self, root_node: Any)` — [`L480`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/ruby.py#L480) — Find all variable assignments.
  - `_get_docstring(self, node: Any)` — [`L171`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/ruby.py#L171) — Extract comments as docstrings for Ruby constructs.
  - `_get_parent_context(self, node: Any, types: Tuple[str, ...] = ('class', 'module', 'method'))` — [`L132`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/ruby.py#L132) — Find parent context for Ruby constructs.
  - `_parse_method_parameters(self, method_node: Any)` — [`L183`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/ruby.py#L183) — Parse method parameters from a method node.
  - `parse(self, path: Path, is_dependency: bool = False, index_source: bool = False)` — [`L193`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/ruby.py#L193) — Parses a Ruby file and returns its structure.
  - `traverse(n, depth=0)` — [`L153`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/ruby.py#L153)
  - `generic_parser_wrapper` — [`L64`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/ruby.py#L64)
  - `index_source` — [`L195`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/ruby.py#L195)
  - `language` — [`L66`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/ruby.py#L66)
  - `language_name` — [`L65`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/ruby.py#L65)
  - `parser` — [`L67`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/ruby.py#L67)
- protocol/private: `__init__`[`L63`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/ruby.py#L63), `_enclosing_class_name`[`L72`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/ruby.py#L72), `_find_module_inclusions`[`L103`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/ruby.py#L103), `_find_modules`[`L76`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/ruby.py#L76), `_get_node_text`[`L69`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/ruby.py#L69)
- uses (calls/refs, reference-scoped): [`warning_logger`](../../utils/debug_log.md#warning_logger), [`execute_query`](../../utils/tree_sitter_manager.md#execute_query), [`MAX_AST_DEPTH`](../indexing/constants.md#MAX_AST_DEPTH), [`RUBY_QUERIES`](ruby.md#RUBY_QUERIES)
- used by: [`language_specific_parser`](../tree_sitter_parser.md#TreeSitterParser.language_specific_parser)

## Functions
- `pre_scan_ruby(files: list[Path], parser_wrapper)` — [`L538`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/ruby.py#L538) — Scans Ruby files to create a map of class/method names to their file paths.

## Module values
- `RUBY_QUERIES` — [`L7`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/ruby.py#L7)

