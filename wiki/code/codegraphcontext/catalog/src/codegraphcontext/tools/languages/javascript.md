---
title: 'Module: src/codegraphcontext/tools/languages/javascript.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/tools/languages/javascript.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.tools.languages.javascript`/
symbols:
  JavascriptTreeSitterParser._find_functions: JavascriptTreeSitterParser#_find_functions().
  JavascriptTreeSitterParser._get_node_text: JavascriptTreeSitterParser#_get_node_text().
  JavascriptTreeSitterParser.index_source: JavascriptTreeSitterParser#index_source.
  JavascriptTreeSitterParser._find_classes: JavascriptTreeSitterParser#_find_classes().
  JavascriptTreeSitterParser._find_calls: JavascriptTreeSitterParser#_find_calls().
  JavascriptTreeSitterParser._find_variables: JavascriptTreeSitterParser#_find_variables().
  JavascriptTreeSitterParser._find_imports: JavascriptTreeSitterParser#_find_imports().
  JavascriptTreeSitterParser._find_react_components: JavascriptTreeSitterParser#_find_react_components().
  JavascriptTreeSitterParser.language_name: JavascriptTreeSitterParser#language_name.
  _classify_method_kind: _classify_method_kind().
  JavascriptTreeSitterParser._calculate_complexity: JavascriptTreeSitterParser#_calculate_complexity().
  JavascriptTreeSitterParser.language: JavascriptTreeSitterParser#language.
  JavascriptTreeSitterParser.traverse: JavascriptTreeSitterParser#traverse().
  JavascriptTreeSitterParser._get_parent_context: JavascriptTreeSitterParser#_get_parent_context().
  JavascriptTreeSitterParser._bucket_for: JavascriptTreeSitterParser#_bucket_for().
  JS_QUERIES: JS_QUERIES.
  pre_scan_javascript: pre_scan_javascript().
  JavascriptTreeSitterParser._extract_parameters: JavascriptTreeSitterParser#_extract_parameters().
  JavascriptTreeSitterParser._get_jsdoc_comment: JavascriptTreeSitterParser#_get_jsdoc_comment().
  JavascriptTreeSitterParser: JavascriptTreeSitterParser#
  JavascriptTreeSitterParser._fn_for_params: JavascriptTreeSitterParser#_fn_for_params().
  _GETTER_RE: _GETTER_RE.
  _SETTER_RE: _SETTER_RE.
  _STATIC_RE: _STATIC_RE.
  _first_line_before_body: _first_line_before_body().
  JavascriptTreeSitterParser.parser: JavascriptTreeSitterParser#parser.
  JavascriptTreeSitterParser._get_docstring: JavascriptTreeSitterParser#_get_docstring().
  JavascriptTreeSitterParser._fn_for_name: JavascriptTreeSitterParser#_fn_for_name().
  JavascriptTreeSitterParser._key: JavascriptTreeSitterParser#_key().
  JavascriptTreeSitterParser.__init__: JavascriptTreeSitterParser#__init__().
  JavascriptTreeSitterParser.generic_parser_wrapper: JavascriptTreeSitterParser#generic_parser_wrapper.
  JavascriptTreeSitterParser.parse: JavascriptTreeSitterParser#parse().
  JavascriptTreeSitterParser._find_function_node_for_name: JavascriptTreeSitterParser#_find_function_node_for_name().
  JavascriptTreeSitterParser._find_function_node_for_params: JavascriptTreeSitterParser#_find_function_node_for_params().
---
# Module: [`src/codegraphcontext/tools/languages/javascript.py`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/javascript.py)

## Classes
### `JavascriptTreeSitterParser`
- def: [`src/codegraphcontext/tools/languages/javascript.py:119`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/javascript.py#L119)
- doc: A JavaScript-specific parser using tree-sitter, encapsulating language-specific logic.
- signature: `class JavascriptTreeSitterParser:`
- members:
  - `_extract_parameters(self, params_node)` — [`L346`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/javascript.py#L346) — Extract parameter names from formal_parameters node.
  - `_find_function_node_for_name(self, name_node)` — [`L320`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/javascript.py#L320) — Find the function node that contains this name node.
  - `_find_function_node_for_params(self, params_node)` — [`L335`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/javascript.py#L335) — Find the function node that contains this parameters node.
  - `_find_react_components(self, root_node)` — [`L570`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/javascript.py#L570) — Find React components in JavaScript/JSX files.
  - `_get_jsdoc_comment(self, func_node)` — [`L366`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/javascript.py#L366) — Extract JSDoc comment preceding the function.
  - `parse(self, path: Path, is_dependency: bool = False, index_source: bool = False)` — [`L184`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/javascript.py#L184) — Parses a file and returns its structure in a standardized dictionary format.
  - `traverse(n, depth=0)` — [`L161`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/javascript.py#L161)
  - `generic_parser_wrapper` — [`L123`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/javascript.py#L123)
  - `index_source` — [`L186`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/javascript.py#L186)
  - `language` — [`L125`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/javascript.py#L125)
  - `language_name` — [`L124`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/javascript.py#L124)
  - `parser` — [`L126`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/javascript.py#L126)
- protocol/private: `__init__`[`L122`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/javascript.py#L122), `_bucket_for`[`L242`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/javascript.py#L242), `_calculate_complexity`[`L150`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/javascript.py#L150), `_find_calls`[`L481`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/javascript.py#L481), `_find_classes`[`L379`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/javascript.py#L379), `_find_functions`[`L212`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/javascript.py#L212), `_find_imports`[`L418`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/javascript.py#L418), `_find_variables`[`L520`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/javascript.py#L520), `_fn_for_name`[`L217`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/javascript.py#L217), `_fn_for_params`[`L229`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/javascript.py#L229), `_get_docstring`[`L179`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/javascript.py#L179), `_get_node_text`[`L128`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/javascript.py#L128), `_get_parent_context`[`L131`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/javascript.py#L131), `_key`[`L237`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/javascript.py#L237)
- uses (calls/refs, reference-scoped): [`warning_logger`](../../utils/debug_log.md#warning_logger), [`execute_query`](../../utils/tree_sitter_manager.md#execute_query), [`MAX_AST_DEPTH`](../indexing/constants.md#MAX_AST_DEPTH), [`_classify_method_kind`](javascript.md#_classify_method_kind), [`JS_QUERIES`](javascript.md#JS_QUERIES), [`_first_line_before_body`](javascript.md#_first_line_before_body)
- used by: [`language_specific_parser`](../tree_sitter_parser.md#TreeSitterParser.language_specific_parser)

## Functions
- `_classify_method_kind(header: str)` — [`L25`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/javascript.py#L25) — Return 'getter' | 'setter' | 'static' | None.
- `_first_line_before_body(text: str)` — [`L14`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/javascript.py#L14) — Best-effort header extraction: take text before the first '{'
- `pre_scan_javascript(files: list[Path], parser_wrapper)` — [`L603`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/javascript.py#L603) — Scans JavaScript files to create a map of class/function names to their file paths.

## Module values
- `JS_QUERIES` — [`L39`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/javascript.py#L39)
- `_GETTER_RE` — [`L9`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/javascript.py#L9)
- `_SETTER_RE` — [`L10`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/javascript.py#L10)
- `_STATIC_RE` — [`L11`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/javascript.py#L11)

