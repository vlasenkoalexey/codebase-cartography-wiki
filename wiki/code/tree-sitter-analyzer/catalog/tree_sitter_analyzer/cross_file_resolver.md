---
title: 'Module: tree_sitter_analyzer/cross_file_resolver.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/cross_file_resolver.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.cross_file_resolver`/
symbols:
  CrossFileResolver.build: CrossFileResolver#build().
  CrossFileResolver.resolve_call_edges: CrossFileResolver#resolve_call_edges().
  CrossFileResolver._build_function_index: CrossFileResolver#_build_function_index().
  ResolvedEdge.to_dict: ResolvedEdge#to_dict().
  CrossFileResolver._module_to_file: CrossFileResolver#_module_to_file.
  CrossFileResolver.find_caller_function: CrossFileResolver#find_caller_function().
  CrossFileResolver._parse_python_import: CrossFileResolver#_parse_python_import().
  CrossFileResolver._parse_js_import: CrossFileResolver#_parse_js_import().
  CrossFileResolver: CrossFileResolver#
  CrossFileResolver._parse_java_import: CrossFileResolver#_parse_java_import().
  CrossFileResolver._build_name_resolution_map: CrossFileResolver#_build_name_resolution_map().
  ImportEntry.to_dict: ImportEntry#to_dict().
  ImportEntry: ImportEntry#
  CrossFileResolver.resolve_callee: CrossFileResolver#resolve_callee().
  FunctionDef.line: FunctionDef#line.
  CrossFileResolver._build_import_index: CrossFileResolver#_build_import_index().
  CrossFileResolver._parse_import: CrossFileResolver#_parse_import().
  ImportEntry.module_path: ImportEntry#module_path.
  FunctionDef.key: FunctionDef#key().
  ImportEntry.imported_names: ImportEntry#imported_names.
  ImportEntry.is_relative: ImportEntry#is_relative.
  CrossFileResolver._functions_by_name: CrossFileResolver#_functions_by_name.
  ImportEntry.source_file: ImportEntry#source_file.
  ImportEntry.language: ImportEntry#language.
  CrossFileResolver._imports_by_file: CrossFileResolver#_imports_by_file.
  FunctionDef: FunctionDef#
  FunctionDef.name: FunctionDef#name.
  ResolvedEdge.callee_resolved_file: ResolvedEdge#callee_resolved_file.
  CrossFileResolver._build_module_map: CrossFileResolver#_build_module_map().
  CrossFileResolver._functions_by_file: CrossFileResolver#_functions_by_file.
  CrossFileResolver._callee_resolver: CrossFileResolver#_callee_resolver.
  FunctionDef.end_line: FunctionDef#end_line.
  ResolvedEdge: ResolvedEdge#
  ResolvedEdge.caller_line: ResolvedEdge#caller_line.
  ResolvedEdge.caller_name: ResolvedEdge#caller_name.
  ResolvedEdge.caller_file: ResolvedEdge#caller_file.
  ResolvedEdge.confidence: ResolvedEdge#confidence.
  CrossFileResolver._cache: CrossFileResolver#_cache.
  CrossFileResolver._register_module_path: CrossFileResolver#_register_module_path().
  CrossFileResolver._resolve_module_to_file: CrossFileResolver#_resolve_module_to_file().
  FunctionDef.file: FunctionDef#file.
  ResolvedEdge.callee_name: ResolvedEdge#callee_name.
  ResolvedEdge.callee_file: ResolvedEdge#callee_file.
  ResolvedEdge.callee_line: ResolvedEdge#callee_line.
  FunctionDef.language: FunctionDef#language.
  CrossFileResolver._name_to_source: CrossFileResolver#_name_to_source.
  CrossFileResolver._built: CrossFileResolver#_built.
  _PY_FROM_IMPORT_RE: _PY_FROM_IMPORT_RE.
  _PY_IMPORT_RE: _PY_IMPORT_RE.
  _JS_IMPORT_RE: _JS_IMPORT_RE.
  _JAVA_IMPORT_RE: _JAVA_IMPORT_RE.
  _alias_name: _alias_name().
  FunctionDef.parent_class: FunctionDef#parent_class.
  logger: logger.
  _GO_IMPORT_RE: _GO_IMPORT_RE.
  CrossFileResolver.__init__: CrossFileResolver#__init__().
---
# Module: [`tree_sitter_analyzer/cross_file_resolver.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cross_file_resolver.py)

## Classes
### `CrossFileResolver`
- def: [`tree_sitter_analyzer/cross_file_resolver.py:103`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cross_file_resolver.py#L103)
- doc: Resolve cross-file symbol references using indexed AST cache data.
- signature: `class CrossFileResolver:`
- members:
  - `build(self)` — [`L122`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cross_file_resolver.py#L122)
  - `find_caller_function(self, call_line: int, source_file: str)` — [`L154`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cross_file_resolver.py#L154) — Find the enclosing function for a call at the given line.
  - `resolve_call_edges(self)` — [`L182`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cross_file_resolver.py#L182) — Re-resolve all call edges with improved cross-file resolution.
  - `resolve_callee(self, callee_name: str, source_file: str)` — [`L136`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cross_file_resolver.py#L136) — Resolve a callee name to likely definition files.
- protocol/private: `__init__`[`L112`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cross_file_resolver.py#L112), `_build_function_index`[`L268`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cross_file_resolver.py#L268), `_build_import_index`[`L291`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cross_file_resolver.py#L291), `_build_module_map`[`L227`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cross_file_resolver.py#L227), `_build_name_resolution_map`[`L401`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cross_file_resolver.py#L401), `_built`[`L120`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cross_file_resolver.py#L120), `_cache`[`L113`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cross_file_resolver.py#L113), `_callee_resolver`[`L119`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cross_file_resolver.py#L119), `_functions_by_file`[`L116`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cross_file_resolver.py#L116), `_functions_by_name`[`L115`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cross_file_resolver.py#L115), `_imports_by_file`[`L117`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cross_file_resolver.py#L117), `_module_to_file`[`L114`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cross_file_resolver.py#L114), `_name_to_source`[`L118`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cross_file_resolver.py#L118), `_parse_import`[`L308`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cross_file_resolver.py#L308), `_parse_java_import`[`L383`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cross_file_resolver.py#L383), `_parse_js_import`[`L351`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cross_file_resolver.py#L351), `_parse_python_import`[`L322`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cross_file_resolver.py#L322), `_register_module_path`[`L235`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cross_file_resolver.py#L235), `_resolve_module_to_file`[`L418`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cross_file_resolver.py#L418)
- uses (calls/refs, reference-scoped): [`CalleeResolver`](callee_resolution.md#CalleeResolver), [`ImportEntry`](cross_file_resolver.md#ImportEntry), [`resolve_files`](callee_resolution.md#CalleeResolver.resolve_files), [`line`](cross_file_resolver.md#FunctionDef.line), [`module_path`](cross_file_resolver.md#ImportEntry.module_path), [`imported_names`](cross_file_resolver.md#ImportEntry.imported_names), [`is_relative`](cross_file_resolver.md#ImportEntry.is_relative), [`language`](cross_file_resolver.md#ImportEntry.language), [`source_file`](cross_file_resolver.md#ImportEntry.source_file), [`FunctionDef`](cross_file_resolver.md#FunctionDef), [`callee_resolved_file`](cross_file_resolver.md#ResolvedEdge.callee_resolved_file), [`name`](cross_file_resolver.md#FunctionDef.name), [`ResolvedEdge`](cross_file_resolver.md#ResolvedEdge), [`caller_line`](cross_file_resolver.md#ResolvedEdge.caller_line), [`end_line`](cross_file_resolver.md#FunctionDef.end_line), [`caller_file`](cross_file_resolver.md#ResolvedEdge.caller_file), [`caller_name`](cross_file_resolver.md#ResolvedEdge.caller_name), [`confidence`](cross_file_resolver.md#ResolvedEdge.confidence), [`callee_file`](cross_file_resolver.md#ResolvedEdge.callee_file), [`callee_line`](cross_file_resolver.md#ResolvedEdge.callee_line), [`callee_name`](cross_file_resolver.md#ResolvedEdge.callee_name), [`file`](cross_file_resolver.md#FunctionDef.file), [`language`](cross_file_resolver.md#FunctionDef.language), [`_JAVA_IMPORT_RE`](cross_file_resolver.md#_JAVA_IMPORT_RE), [`_JS_IMPORT_RE`](cross_file_resolver.md#_JS_IMPORT_RE), [`_PY_FROM_IMPORT_RE`](cross_file_resolver.md#_PY_FROM_IMPORT_RE), [`_PY_IMPORT_RE`](cross_file_resolver.md#_PY_IMPORT_RE), [`_alias_name`](cross_file_resolver.md#_alias_name), [`parent_class`](cross_file_resolver.md#FunctionDef.parent_class)
- used by: [`backfill_cross_file_edges`](_ast_cache_query.md#backfill_cross_file_edges), [`get_cross_file_resolver`](ast_cache.md#ASTCache.get_cross_file_resolver)  (15 test-only)

### `FunctionDef`
- def: [`tree_sitter_analyzer/cross_file_resolver.py:64`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cross_file_resolver.py#L64)
- signature: `class FunctionDef:`
- members:
  - `key(self)` — [`L73`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cross_file_resolver.py#L73)
  - `end_line` — [`L68`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cross_file_resolver.py#L68)
  - `file` — [`L66`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cross_file_resolver.py#L66)
  - `language` — [`L69`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cross_file_resolver.py#L69)
  - `line` — [`L67`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cross_file_resolver.py#L67)
  - `name` — [`L65`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cross_file_resolver.py#L65)
  - `parent_class` — [`L70`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cross_file_resolver.py#L70)
- used by: [`_build_function_index`](cross_file_resolver.md#CrossFileResolver._build_function_index), [`find_caller_function`](cross_file_resolver.md#CrossFileResolver.find_caller_function), [`_functions_by_name`](cross_file_resolver.md#CrossFileResolver._functions_by_name), [`_functions_by_file`](cross_file_resolver.md#CrossFileResolver._functions_by_file)  (1 test-only)

### `ImportEntry`
- def: [`tree_sitter_analyzer/cross_file_resolver.py:46`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cross_file_resolver.py#L46)
- signature: `class ImportEntry:`
- members:
  - `to_dict(self)` — [`L53`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cross_file_resolver.py#L53)
  - `imported_names` — [`L49`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cross_file_resolver.py#L49)
  - `is_relative` — [`L50`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cross_file_resolver.py#L50)
  - `language` — [`L51`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cross_file_resolver.py#L51)
  - `module_path` — [`L48`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cross_file_resolver.py#L48)
  - `source_file` — [`L47`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cross_file_resolver.py#L47)
- used by: [`_parse_js_import`](cross_file_resolver.md#CrossFileResolver._parse_js_import), [`_parse_python_import`](cross_file_resolver.md#CrossFileResolver._parse_python_import), [`_parse_java_import`](cross_file_resolver.md#CrossFileResolver._parse_java_import), [`_build_name_resolution_map`](cross_file_resolver.md#CrossFileResolver._build_name_resolution_map), [`_build_import_index`](cross_file_resolver.md#CrossFileResolver._build_import_index), [`_parse_import`](cross_file_resolver.md#CrossFileResolver._parse_import), [`_imports_by_file`](cross_file_resolver.md#CrossFileResolver._imports_by_file)  (2 test-only)

### `ResolvedEdge`
- def: [`tree_sitter_analyzer/cross_file_resolver.py:78`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cross_file_resolver.py#L78)
- signature: `class ResolvedEdge:`
- members:
  - `to_dict(self)` — [`L88`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cross_file_resolver.py#L88)
  - `callee_file` — [`L83`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cross_file_resolver.py#L83)
  - `callee_line` — [`L84`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cross_file_resolver.py#L84)
  - `callee_name` — [`L82`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cross_file_resolver.py#L82)
  - `callee_resolved_file` — [`L85`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cross_file_resolver.py#L85)
  - `caller_file` — [`L80`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cross_file_resolver.py#L80)
  - `caller_line` — [`L81`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cross_file_resolver.py#L81)
  - `caller_name` — [`L79`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cross_file_resolver.py#L79)
  - `confidence` — [`L86`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cross_file_resolver.py#L86)
- used by: [`resolve_call_edges`](cross_file_resolver.md#CrossFileResolver.resolve_call_edges), [`backfill_cross_file_edges`](_ast_cache_query.md#backfill_cross_file_edges)  (3 test-only)

## Functions
- `_alias_name(s: str)` — [`L40`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cross_file_resolver.py#L40) — Extract the local alias from 'name as alias', or return the stripped name.

## Module values
- `_GO_IMPORT_RE` — [`L37`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cross_file_resolver.py#L37)
- `_JAVA_IMPORT_RE` — [`L36`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cross_file_resolver.py#L36)
- `_JS_IMPORT_RE` — [`L32`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cross_file_resolver.py#L32)
- `_PY_FROM_IMPORT_RE` — [`L30`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cross_file_resolver.py#L30)
- `_PY_IMPORT_RE` — [`L31`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cross_file_resolver.py#L31)
- `logger` — [`L28`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cross_file_resolver.py#L28)

