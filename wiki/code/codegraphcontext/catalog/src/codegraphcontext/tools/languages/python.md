---
title: 'Module: src/codegraphcontext/tools/languages/python.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/tools/languages/python.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.tools.languages.python`/
symbols:
  PythonTreeSitterParser._get_node_text: PythonTreeSitterParser#_get_node_text().
  PythonTreeSitterParser.index_source: PythonTreeSitterParser#index_source.
  PythonTreeSitterParser._find_functions: PythonTreeSitterParser#_find_functions().
  PythonTreeSitterParser._find_classes: PythonTreeSitterParser#_find_classes().
  PythonTreeSitterParser._find_lambda_assignments: PythonTreeSitterParser#_find_lambda_assignments().
  PythonTreeSitterParser._find_imports: PythonTreeSitterParser#_find_imports().
  PythonTreeSitterParser._find_dict_method_references: PythonTreeSitterParser#_find_dict_method_references().
  PythonTreeSitterParser._find_variables: PythonTreeSitterParser#_find_variables().
  PythonTreeSitterParser._get_parent_context: PythonTreeSitterParser#_get_parent_context().
  PythonTreeSitterParser._record_call: PythonTreeSitterParser#_record_call().
  PythonTreeSitterParser.language_name: PythonTreeSitterParser#language_name.
  PythonTreeSitterParser._calculate_complexity: PythonTreeSitterParser#_calculate_complexity().
  PythonTreeSitterParser._attach_module_context: PythonTreeSitterParser#_attach_module_context().
  PythonTreeSitterParser._walk_call_tree: PythonTreeSitterParser#_walk_call_tree().
  PythonTreeSitterParser.traverse: PythonTreeSitterParser#traverse().
  PY_QUERIES: PY_QUERIES.
  PythonTreeSitterParser.language: PythonTreeSitterParser#language.
  PythonTreeSitterParser._find_calls: PythonTreeSitterParser#_find_calls().
  pre_scan_python: pre_scan_python().
  PythonTreeSitterParser._get_docstring: PythonTreeSitterParser#_get_docstring().
  PythonTreeSitterParser._extract_call_name: PythonTreeSitterParser#_extract_call_name().
  PythonTreeSitterParser._call_args: PythonTreeSitterParser#_call_args().
  PythonTreeSitterParser: PythonTreeSitterParser#
  PythonTreeSitterParser.parser: PythonTreeSitterParser#parser.
  PythonTreeSitterParser.parse: PythonTreeSitterParser#parse().
  PythonTreeSitterParser.__init__: PythonTreeSitterParser#__init__().
  PythonTreeSitterParser.generic_parser_wrapper: PythonTreeSitterParser#generic_parser_wrapper.
---
# Module: [`src/codegraphcontext/tools/languages/python.py`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/python.py)

## Classes
### `PythonTreeSitterParser`
- def: [`src/codegraphcontext/tools/languages/python.py:66`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/python.py#L66)
- doc: A Python-specific parser using tree-sitter, encapsulating language-specific logic.
- signature: `class PythonTreeSitterParser:`
- members:
  - `_attach_module_context(self, functions, function_calls, root_node, index_source: bool = False)` — [`L182`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/python.py#L182) — Represent module-level executable code as Python's <module> frame.
  - `_find_dict_method_references(self, root_node)` — [`L514`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/python.py#L514) — Detects indirect function calls through dictionary mappings.
  - `parse(self, path: Path, is_dependency: bool = False, is_notebook: bool = False, index_source: bool = False)` — [`L127`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/python.py#L127) — Parses a file and returns its structure in a standardized dictionary format.
  - `traverse(n, depth=0)` — [`L99`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/python.py#L99)
  - `generic_parser_wrapper` — [`L70`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/python.py#L70)
  - `index_source` — [`L132`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/python.py#L132)
  - `language` — [`L72`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/python.py#L72)
  - `language_name` — [`L71`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/python.py#L71)
  - `parser` — [`L73`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/python.py#L73)
- protocol/private: `__init__`[`L69`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/python.py#L69), `_calculate_complexity`[`L89`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/python.py#L89), `_call_args`[`L452`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/python.py#L452), `_extract_call_name`[`L443`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/python.py#L443), `_find_calls`[`L504`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/python.py#L504), `_find_classes`[`L327`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/python.py#L327), `_find_functions`[`L253`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/python.py#L253), `_find_imports`[`L375`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/python.py#L375), `_find_lambda_assignments`[`L215`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/python.py#L215), `_find_variables`[`L595`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/python.py#L595), `_get_docstring`[`L117`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/python.py#L117), `_get_node_text`[`L75`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/python.py#L75), `_get_parent_context`[`L80`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/python.py#L80), `_record_call`[`L462`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/python.py#L462), `_walk_call_tree`[`L490`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/python.py#L490)
- uses (calls/refs, reference-scoped): [`info_logger`](../../utils/debug_log.md#info_logger), [`warning_logger`](../../utils/debug_log.md#warning_logger), [`execute_query`](../../utils/tree_sitter_manager.md#execute_query), [`error_logger`](../../utils/debug_log.md#error_logger), [`MAX_AST_DEPTH`](../indexing/constants.md#MAX_AST_DEPTH), [`PY_QUERIES`](python.md#PY_QUERIES)
- used by: [`language_specific_parser`](../tree_sitter_parser.md#TreeSitterParser.language_specific_parser), [`parse`](../tree_sitter_parser.md#TreeSitterParser.parse)

## Functions
- `pre_scan_python(files: list[Path], parser_wrapper)` — [`L632`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/python.py#L632) — Scans Python files to create a map of class/function names to their file paths.

## Module values
- `PY_QUERIES` — [`L22`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/python.py#L22)

