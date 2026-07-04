---
title: 'Module: src/codegraphcontext/tools/languages/lua.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/tools/languages/lua.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.tools.languages.lua`/
symbols:
  LuaTreeSitterParser._find_functions: LuaTreeSitterParser#_find_functions().
  LuaTreeSitterParser.parse: LuaTreeSitterParser#parse().
  LuaTreeSitterParser._find_calls: LuaTreeSitterParser#_find_calls().
  LuaTreeSitterParser._find_variables: LuaTreeSitterParser#_find_variables().
  LuaTreeSitterParser._get_node_text: LuaTreeSitterParser#_get_node_text().
  LuaTreeSitterParser._find_imports: LuaTreeSitterParser#_find_imports().
  LuaTreeSitterParser._function_identity: LuaTreeSitterParser#_function_identity().
  LuaTreeSitterParser.traverse: LuaTreeSitterParser#traverse().
  pre_scan_lua: pre_scan_lua().
  LuaTreeSitterParser._iter_nodes: LuaTreeSitterParser#_iter_nodes().
  LuaTreeSitterParser._assigned_name_node: LuaTreeSitterParser#_assigned_name_node().
  LuaTreeSitterParser._calculate_complexity: LuaTreeSitterParser#_calculate_complexity().
  LuaTreeSitterParser._require_alias: LuaTreeSitterParser#_require_alias().
  LuaTreeSitterParser._first_string_argument: LuaTreeSitterParser#_first_string_argument().
  LuaTreeSitterParser._get_parent_context: LuaTreeSitterParser#_get_parent_context().
  LuaTreeSitterParser.language_name: LuaTreeSitterParser#language_name.
  LuaTreeSitterParser._table_context_for_field: LuaTreeSitterParser#_table_context_for_field().
  LuaTreeSitterParser._extract_parameters: LuaTreeSitterParser#_extract_parameters().
  LuaTreeSitterParser._get_docstring: LuaTreeSitterParser#_get_docstring().
  LuaTreeSitterParser._extract_call_args: LuaTreeSitterParser#_extract_call_args().
  LuaTreeSitterParser: LuaTreeSitterParser#
  LuaTreeSitterParser._assignment_name_nodes: LuaTreeSitterParser#_assignment_name_nodes().
  LuaTreeSitterParser.index_source: LuaTreeSitterParser#index_source.
  LuaTreeSitterParser._split_qualified_name: LuaTreeSitterParser#_split_qualified_name().
  LuaTreeSitterParser._assignment_for_expression_list: LuaTreeSitterParser#_assignment_for_expression_list().
  LUA_CONTROL_NODES: LUA_CONTROL_NODES.
  LuaTreeSitterParser.parser: LuaTreeSitterParser#parser.
  LuaTreeSitterParser._first_named_child: LuaTreeSitterParser#_first_named_child().
  LuaTreeSitterParser._assignment_value_nodes: LuaTreeSitterParser#_assignment_value_nodes().
  _resolve_lua_module_path: _resolve_lua_module_path().
  LuaTreeSitterParser.__init__: LuaTreeSitterParser#__init__().
  LuaTreeSitterParser.generic_parser_wrapper: LuaTreeSitterParser#generic_parser_wrapper.
  LuaTreeSitterParser.language: LuaTreeSitterParser#language.
---
# Module: [`src/codegraphcontext/tools/languages/lua.py`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/lua.py)

## Classes
### `LuaTreeSitterParser`
- def: [`src/codegraphcontext/tools/languages/lua.py:17`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/lua.py#L17)
- doc: A Lua-specific parser using tree-sitter.
- signature: `class LuaTreeSitterParser:`
- members:
  - `parse(self, path: Path, is_dependency: bool = False, index_source: bool = False)` — [`L198`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/lua.py#L198)
  - `traverse(current, depth=0)` — [`L156`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/lua.py#L156)
  - `generic_parser_wrapper` — [`L21`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/lua.py#L21)
  - `index_source` — [`L25`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/lua.py#L25)
  - `language` — [`L23`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/lua.py#L23)
  - `language_name` — [`L22`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/lua.py#L22)
  - `parser` — [`L24`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/lua.py#L24)
- protocol/private: `__init__`[`L20`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/lua.py#L20), `_assigned_name_node`[`L75`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/lua.py#L75), `_assignment_for_expression_list`[`L49`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/lua.py#L49), `_assignment_name_nodes`[`L59`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/lua.py#L59), `_assignment_value_nodes`[`L67`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/lua.py#L67), `_calculate_complexity`[`L151`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/lua.py#L151), `_extract_call_args`[`L398`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/lua.py#L398), `_extract_parameters`[`L133`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/lua.py#L133), `_find_calls`[`L293`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/lua.py#L293), `_find_functions`[`L217`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/lua.py#L217), `_find_imports`[`L259`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/lua.py#L259), `_find_variables`[`L328`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/lua.py#L328), `_first_named_child`[`L43`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/lua.py#L43), `_first_string_argument`[`L375`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/lua.py#L375), `_function_identity`[`L114`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/lua.py#L114), `_get_docstring`[`L179`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/lua.py#L179), `_get_node_text`[`L27`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/lua.py#L27), `_get_parent_context`[`L189`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/lua.py#L189), `_iter_nodes`[`L30`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/lua.py#L30), `_require_alias`[`L387`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/lua.py#L387), `_split_qualified_name`[`L36`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/lua.py#L36), `_table_context_for_field`[`L103`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/lua.py#L103)
- uses (calls/refs, reference-scoped): [`warning_logger`](../../utils/debug_log.md#warning_logger), [`MAX_AST_DEPTH`](../indexing/constants.md#MAX_AST_DEPTH), [`LUA_CONTROL_NODES`](lua.md#LUA_CONTROL_NODES)
- used by: [`language_specific_parser`](../tree_sitter_parser.md#TreeSitterParser.language_specific_parser), [`pre_scan_lua`](lua.md#pre_scan_lua)

## Functions
- `_resolve_lua_module_path(requiring_file: Path, module_name: str)` — [`L410`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/lua.py#L410) — Resolve require('name') to a .lua file next to the requiring file.
- `pre_scan_lua(files: list[Path], parser_wrapper)` — [`L425`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/lua.py#L425) — Map Lua function names and require() aliases to defining file paths.

## Module values
- `LUA_CONTROL_NODES` — [`L9`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/lua.py#L9)

