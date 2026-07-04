---
title: 'Module: src/codegraphcontext/tools/languages/elisp.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/tools/languages/elisp.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.tools.languages.elisp`/
symbols:
  ElispTreeSitterParser._find_functions: ElispTreeSitterParser#_find_functions().
  ElispTreeSitterParser.parse: ElispTreeSitterParser#parse().
  ElispTreeSitterParser._find_imports: ElispTreeSitterParser#_find_imports().
  pre_scan_elisp: pre_scan_elisp().
  ElispTreeSitterParser._append_variable: ElispTreeSitterParser#_append_variable().
  ElispTreeSitterParser._named_children: ElispTreeSitterParser#_named_children().
  CALL_EXCLUDED_FORMS: CALL_EXCLUDED_FORMS.
  ElispTreeSitterParser._is_call_node: ElispTreeSitterParser#_is_call_node().
  ElispTreeSitterParser._find_calls: ElispTreeSitterParser#_find_calls().
  ElispTreeSitterParser._form_head: ElispTreeSitterParser#_form_head().
  ElispTreeSitterParser._function_identity: ElispTreeSitterParser#_function_identity().
  ElispTreeSitterParser.traverse: ElispTreeSitterParser#traverse().
  ElispTreeSitterParser._find_variables: ElispTreeSitterParser#_find_variables().
  ElispTreeSitterParser._get_node_text: ElispTreeSitterParser#_get_node_text().
  ElispTreeSitterParser._append_call: ElispTreeSitterParser#_append_call().
  ElispTreeSitterParser._function_docstring: ElispTreeSitterParser#_function_docstring().
  ElispTreeSitterParser._is_parameter_list: ElispTreeSitterParser#_is_parameter_list().
  ElispTreeSitterParser._is_binding_list: ElispTreeSitterParser#_is_binding_list().
  ElispTreeSitterParser._calculate_complexity: ElispTreeSitterParser#_calculate_complexity().
  ElispTreeSitterParser._quoted_symbol_argument: ElispTreeSitterParser#_quoted_symbol_argument().
  ElispTreeSitterParser._iter_nodes: ElispTreeSitterParser#_iter_nodes().
  ElispTreeSitterParser._string_value: ElispTreeSitterParser#_string_value().
  ElispTreeSitterParser._is_cl_defun: ElispTreeSitterParser#_is_cl_defun().
  ElispTreeSitterParser._parameter_node: ElispTreeSitterParser#_parameter_node().
  ElispTreeSitterParser._extract_parameters: ElispTreeSitterParser#_extract_parameters().
  ElispTreeSitterParser._first_symbol_in_quote: ElispTreeSitterParser#_first_symbol_in_quote().
  ElispTreeSitterParser._extract_call_args: ElispTreeSitterParser#_extract_call_args().
  ElispTreeSitterParser._variable_docstring: ElispTreeSitterParser#_variable_docstring().
  ElispTreeSitterParser._form_arguments: ElispTreeSitterParser#_form_arguments().
  ElispTreeSitterParser.language_name: ElispTreeSitterParser#language_name.
  ElispTreeSitterParser.add_symbol: ElispTreeSitterParser#add_symbol().
  ElispTreeSitterParser._enclosing_function: ElispTreeSitterParser#_enclosing_function().
  ElispTreeSitterParser._has_parameter_list_ancestor: ElispTreeSitterParser#_has_parameter_list_ancestor().
  ElispTreeSitterParser: ElispTreeSitterParser#
  ElispTreeSitterParser.index_source: ElispTreeSitterParser#index_source.
  VARIABLE_FORMS: VARIABLE_FORMS.
  IMPORT_FORMS: IMPORT_FORMS.
  BINDING_FORMS: BINDING_FORMS.
  FUNCTION_FORMS: FUNCTION_FORMS.
  SPECIAL_FORMS: SPECIAL_FORMS.
  CONTROL_FORMS: CONTROL_FORMS.
  ElispTreeSitterParser.parser: ElispTreeSitterParser#parser.
  ElispTreeSitterParser._has_quote_ancestor: ElispTreeSitterParser#_has_quote_ancestor().
  ELISP_QUERIES: ELISP_QUERIES.
  ElispTreeSitterParser.__init__: ElispTreeSitterParser#__init__().
  ElispTreeSitterParser.generic_parser_wrapper: ElispTreeSitterParser#generic_parser_wrapper.
  ElispTreeSitterParser.language: ElispTreeSitterParser#language.
---
# Module: [`src/codegraphcontext/tools/languages/elisp.py`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elisp.py)

## Classes
### `ElispTreeSitterParser`
- def: [`src/codegraphcontext/tools/languages/elisp.py:115`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elisp.py#L115) — documented in [codegraphcontext-tools-languages-elisp](../../../../../concepts/codegraphcontext-tools-languages-elisp.md)
- doc: An Emacs Lisp-specific parser using tree-sitter.
- signature: `class ElispTreeSitterParser:`
- members:
  - `add_symbol(symbol_node: Any)` — [`L200`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elisp.py#L200)
  - `parse(self, path: Path, is_dependency: bool = False, index_source: bool = False)` — [`L372`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elisp.py#L372) — Parse an Emacs Lisp file and return CGC's normalized structure. — documented in [codegraphcontext-tools-languages-elisp](../../../../../concepts/codegraphcontext-tools-languages-elisp.md)
  - `traverse(current: Any, depth: int = 0)` — [`L352`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elisp.py#L352) — documented in [codegraphcontext-tools-languages-elisp](../../../../../concepts/codegraphcontext-tools-languages-elisp.md)
  - `generic_parser_wrapper` — [`L119`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elisp.py#L119)
  - `index_source` — [`L123`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elisp.py#L123) — documented in [codegraphcontext-tools-languages-elisp](../../../../../concepts/codegraphcontext-tools-languages-elisp.md)
  - `language` — [`L121`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elisp.py#L121)
  - `language_name` — [`L120`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elisp.py#L120) — documented in [codegraphcontext-tools-languages-elisp](../../../../../concepts/codegraphcontext-tools-languages-elisp.md)
  - `parser` — [`L122`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elisp.py#L122)
- protocol/private: `__init__`[`L118`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elisp.py#L118), `_append_call`[`L631`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elisp.py#L631), `_append_variable`[`L497`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elisp.py#L497), `_calculate_complexity`[`L347`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elisp.py#L347), `_enclosing_function`[`L258`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elisp.py#L258), `_extract_call_args`[`L341`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elisp.py#L341), `_extract_parameters`[`L193`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elisp.py#L193), `_find_calls`[`L600`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elisp.py#L600), `_find_functions`[`L398`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elisp.py#L398), `_find_imports`[`L545`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elisp.py#L545), `_find_variables`[`L443`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elisp.py#L443), `_first_symbol_in_quote`[`L244`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elisp.py#L244), `_form_arguments`[`L139`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elisp.py#L139), `_form_head`[`L145`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elisp.py#L145), `_function_docstring`[`L230`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elisp.py#L230), `_function_identity`[`L163`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elisp.py#L163), `_get_node_text`[`L125`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elisp.py#L125), `_has_parameter_list_ancestor`[`L285`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elisp.py#L285), `_has_quote_ancestor`[`L314`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elisp.py#L314), `_is_binding_list`[`L293`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elisp.py#L293), `_is_call_node`[`L322`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elisp.py#L322), `_is_cl_defun`[`L160`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elisp.py#L160), `_is_parameter_list`[`L267`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elisp.py#L267), `_iter_nodes`[`L130`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elisp.py#L130), `_named_children`[`L136`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elisp.py#L136), `_parameter_node`[`L182`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elisp.py#L182), `_quoted_symbol_argument`[`L252`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elisp.py#L252), `_string_value`[`L218`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elisp.py#L218), `_variable_docstring`[`L533`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elisp.py#L533)
- uses (calls/refs, reference-scoped): [`warning_logger`](../../utils/debug_log.md#warning_logger), [`error_logger`](../../utils/debug_log.md#error_logger), [`MAX_AST_DEPTH`](../indexing/constants.md#MAX_AST_DEPTH), [`CALL_EXCLUDED_FORMS`](elisp.md#CALL_EXCLUDED_FORMS), [`BINDING_FORMS`](elisp.md#BINDING_FORMS), [`IMPORT_FORMS`](elisp.md#IMPORT_FORMS), [`CONTROL_FORMS`](elisp.md#CONTROL_FORMS)
- used by: [`language_specific_parser`](../tree_sitter_parser.md#TreeSitterParser.language_specific_parser), [`pre_scan_elisp`](elisp.md#pre_scan_elisp)

## Functions
- `pre_scan_elisp(files: list[Path], parser_wrapper)` — [`L663`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elisp.py#L663) — Scan Emacs Lisp files to map functions, macros, variables, and provided features to file paths. — documented in [codegraphcontext-tools-languages-elisp](../../../../../concepts/codegraphcontext-tools-languages-elisp.md)

## Module values
- `BINDING_FORMS` — [`L95`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elisp.py#L95) — documented in [codegraphcontext-tools-languages-elisp](../../../../../concepts/codegraphcontext-tools-languages-elisp.md)
- `CALL_EXCLUDED_FORMS` — [`L96`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elisp.py#L96) — documented in [codegraphcontext-tools-languages-elisp](../../../../../concepts/codegraphcontext-tools-languages-elisp.md)
- `CONTROL_FORMS` — [`L99`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elisp.py#L99) — documented in [codegraphcontext-tools-languages-elisp](../../../../../concepts/codegraphcontext-tools-languages-elisp.md)
- `ELISP_QUERIES` — [`L9`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elisp.py#L9)
- `FUNCTION_FORMS` — [`L64`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elisp.py#L64) — documented in [codegraphcontext-tools-languages-elisp](../../../../../concepts/codegraphcontext-tools-languages-elisp.md)
- `IMPORT_FORMS` — [`L66`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elisp.py#L66) — documented in [codegraphcontext-tools-languages-elisp](../../../../../concepts/codegraphcontext-tools-languages-elisp.md)
- `SPECIAL_FORMS` — [`L67`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elisp.py#L67) — documented in [codegraphcontext-tools-languages-elisp](../../../../../concepts/codegraphcontext-tools-languages-elisp.md)
- `VARIABLE_FORMS` — [`L65`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elisp.py#L65) — documented in [codegraphcontext-tools-languages-elisp](../../../../../concepts/codegraphcontext-tools-languages-elisp.md)

