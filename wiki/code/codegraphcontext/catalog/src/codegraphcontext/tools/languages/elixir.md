---
title: 'Module: src/codegraphcontext/tools/languages/elixir.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/tools/languages/elixir.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.tools.languages.elixir`/
symbols:
  ElixirTreeSitterParser._get_node_text: ElixirTreeSitterParser#_get_node_text().
  ElixirTreeSitterParser._find_functions_recursive: ElixirTreeSitterParser#_find_functions_recursive().
  ElixirTreeSitterParser.parse: ElixirTreeSitterParser#parse().
  ElixirTreeSitterParser._find_calls_recursive: ElixirTreeSitterParser#_find_calls_recursive().
  ElixirTreeSitterParser._find_modules_recursive: ElixirTreeSitterParser#_find_modules_recursive().
  ElixirTreeSitterParser._find_imports_recursive: ElixirTreeSitterParser#_find_imports_recursive().
  ElixirTreeSitterParser._get_parent_context: ElixirTreeSitterParser#_get_parent_context().
  ElixirTreeSitterParser.traverse: ElixirTreeSitterParser#traverse().
  _pre_scan_recursive: _pre_scan_recursive().
  ELIXIR_KEYWORDS: ELIXIR_KEYWORDS.
  ElixirTreeSitterParser._enclosing_module_name: ElixirTreeSitterParser#_enclosing_module_name().
  ElixirTreeSitterParser._calculate_complexity: ElixirTreeSitterParser#_calculate_complexity().
  pre_scan_elixir: pre_scan_elixir().
  ElixirTreeSitterParser.language_name: ElixirTreeSitterParser#language_name.
  MODULE_KEYWORDS: MODULE_KEYWORDS.
  FUNCTION_KEYWORDS: FUNCTION_KEYWORDS.
  ElixirTreeSitterParser._get_docstring: ElixirTreeSitterParser#_get_docstring().
  ElixirTreeSitterParser._find_modules: ElixirTreeSitterParser#_find_modules().
  ElixirTreeSitterParser._find_functions: ElixirTreeSitterParser#_find_functions().
  ElixirTreeSitterParser._find_imports: ElixirTreeSitterParser#_find_imports().
  ElixirTreeSitterParser._find_calls: ElixirTreeSitterParser#_find_calls().
  ElixirTreeSitterParser.index_source: ElixirTreeSitterParser#index_source.
  IMPORT_KEYWORDS: IMPORT_KEYWORDS.
  ElixirTreeSitterParser: ElixirTreeSitterParser#
  ElixirTreeSitterParser.parser: ElixirTreeSitterParser#parser.
  ELIXIR_QUERIES: ELIXIR_QUERIES.
  ElixirTreeSitterParser.__init__: ElixirTreeSitterParser#__init__().
  ElixirTreeSitterParser.generic_parser_wrapper: ElixirTreeSitterParser#generic_parser_wrapper.
  ElixirTreeSitterParser.language: ElixirTreeSitterParser#language.
---
# Module: [`src/codegraphcontext/tools/languages/elixir.py`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elixir.py)

## Classes
### `ElixirTreeSitterParser`
- def: [`src/codegraphcontext/tools/languages/elixir.py:78`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elixir.py#L78)
- doc: An Elixir-specific parser using tree-sitter.
- signature: `class ElixirTreeSitterParser:`
- members:
  - `_calculate_complexity(self, node: Any)` — [`L163`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elixir.py#L163) — Calculate cyclomatic complexity for Elixir constructs.
  - `_enclosing_module_name(self, node: Any)` — [`L122`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elixir.py#L122) — Find the enclosing module name.
  - `_find_calls(self, root_node: Any)` — [`L400`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elixir.py#L400) — Find all function calls (excluding def/defmodule/etc keywords).
  - `_find_calls_recursive(self, node: Any, calls: list)` — [`L406`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elixir.py#L406) — Recursively find function calls.
  - `_find_functions(self, root_node: Any)` — [`L301`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elixir.py#L301) — Find all def, defp, defmacro, etc. definitions.
  - `_find_functions_recursive(self, node: Any, functions: list)` — [`L307`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elixir.py#L307) — Recursively find function definitions.
  - `_find_imports(self, root_node: Any)` — [`L363`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elixir.py#L363) — Find all use, import, alias, require statements.
  - `_find_imports_recursive(self, node: Any, imports: list)` — [`L369`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elixir.py#L369) — Recursively find import-like statements.
  - `_find_modules(self, root_node: Any)` — [`L237`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elixir.py#L237) — Find all defmodule, defprotocol, defimpl definitions.
  - `_find_modules_recursive(self, node: Any, modules: list)` — [`L243`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elixir.py#L243) — Recursively find module definitions.
  - `_get_docstring(self, node: Any)` — [`L195`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elixir.py#L195) — Extract @doc or @moduledoc attribute as docstring.
  - `_get_parent_context(self, node: Any)` — [`L91`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elixir.py#L91) — Find parent module or function context.
  - `parse(self, path: Path, is_dependency: bool = False, index_source: bool = False)` — [`L210`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elixir.py#L210) — Parses an Elixir file and returns its structure.
  - `traverse(n, depth=0)` — [`L173`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elixir.py#L173)
  - `generic_parser_wrapper` — [`L82`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elixir.py#L82)
  - `index_source` — [`L86`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elixir.py#L86)
  - `language` — [`L84`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elixir.py#L84)
  - `language_name` — [`L83`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elixir.py#L83)
  - `parser` — [`L85`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elixir.py#L85)
- protocol/private: `__init__`[`L81`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elixir.py#L81), `_get_node_text`[`L88`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elixir.py#L88)
- uses (calls/refs, reference-scoped): [`warning_logger`](../../utils/debug_log.md#warning_logger), [`MAX_AST_DEPTH`](../indexing/constants.md#MAX_AST_DEPTH), [`ELIXIR_KEYWORDS`](elixir.md#ELIXIR_KEYWORDS), [`MODULE_KEYWORDS`](elixir.md#MODULE_KEYWORDS), [`FUNCTION_KEYWORDS`](elixir.md#FUNCTION_KEYWORDS), [`IMPORT_KEYWORDS`](elixir.md#IMPORT_KEYWORDS)
- used by: [`language_specific_parser`](../tree_sitter_parser.md#TreeSitterParser.language_specific_parser)

## Functions
- `_pre_scan_recursive(node, path: Path, imports_map: dict)` — [`L488`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elixir.py#L488) — Recursively scan for module and function names.
- `pre_scan_elixir(files: list[Path], parser_wrapper)` — [`L472`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elixir.py#L472) — Scans Elixir files to create a map of module/function names to their file paths.

## Module values
- `ELIXIR_KEYWORDS` — [`L72`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elixir.py#L72)
- `ELIXIR_QUERIES` — [`L9`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elixir.py#L9)
- `FUNCTION_KEYWORDS` — [`L66`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elixir.py#L66)
- `IMPORT_KEYWORDS` — [`L69`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elixir.py#L69)
- `MODULE_KEYWORDS` — [`L63`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/elixir.py#L63)

