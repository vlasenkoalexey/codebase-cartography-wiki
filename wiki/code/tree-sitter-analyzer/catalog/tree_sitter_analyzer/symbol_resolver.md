---
title: 'Module: tree_sitter_analyzer/symbol_resolver.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/symbol_resolver.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.symbol_resolver`/
symbols:
  ResolveResult.definitions: ResolveResult#definitions.
  SymbolResolver._find_import_references: SymbolResolver#_find_import_references().
  SymbolResolver._find_defs_in_file: SymbolResolver#_find_defs_in_file().
  DefinitionLocation: DefinitionLocation#
  SymbolResolver._find_references: SymbolResolver#_find_references().
  DefinitionLocation.to_dict: DefinitionLocation#to_dict().
  SymbolResolver: SymbolResolver#
  _definition_location: _definition_location().
  SymbolResolver.resolve: SymbolResolver#resolve().
  ReferenceLocation.to_dict: ReferenceLocation#to_dict().
  SymbolResolver.find_references: SymbolResolver#find_references().
  _collect_import_refs_from_list: _collect_import_refs_from_list().
  SymbolResolver._resolve_from_imports: SymbolResolver#_resolve_from_imports().
  ResolveResult.to_dict: ResolveResult#to_dict().
  DefinitionLocation.name: DefinitionLocation#name.
  SymbolResolver._resolve_qualified: SymbolResolver#_resolve_qualified().
  SymbolResolver._is_child_of: SymbolResolver#_is_child_of().
  DefinitionLocation.kind: DefinitionLocation#kind.
  SymbolResolver._lookup_by_module: SymbolResolver#_lookup_by_module().
  DefinitionLocation.file: DefinitionLocation#file.
  SymbolResolver._find_definitions: SymbolResolver#_find_definitions().
  SymbolResolver._resolve_simple: SymbolResolver#_resolve_simple().
  ResolveResult.references: ResolveResult#references.
  ReferenceLocation: ReferenceLocation#
  DefinitionLocation.line: DefinitionLocation#line.
  DefinitionLocation.end_line: DefinitionLocation#end_line.
  DefinitionLocation.language: DefinitionLocation#language.
  DefinitionLocation.confidence: DefinitionLocation#confidence.
  ReferenceLocation.file: ReferenceLocation#file.
  ReferenceLocation.line: ReferenceLocation#line.
  ResolveResult: ResolveResult#
  ReferenceLocation.name: ReferenceLocation#name.
  ReferenceLocation.kind: ReferenceLocation#kind.
  ReferenceLocation.language: ReferenceLocation#language.
  _apply_confidence: _apply_confidence().
  SymbolResolver._cache: SymbolResolver#_cache.
  SymbolResolver._import_map: SymbolResolver#_import_map.
  ReferenceLocation.end_line: ReferenceLocation#end_line.
  ReferenceLocation.reference_type: ReferenceLocation#reference_type.
  ResolveResult.symbol: ResolveResult#symbol.
  DefinitionLocation.context: DefinitionLocation#context.
  SymbolResolver._module_to_file: SymbolResolver#_module_to_file.
  SymbolResolver._definition_backend: SymbolResolver#_definition_backend.
  ResolveResult.resolved_via: ResolveResult#resolved_via.
  _DEFINITION_KINDS: _DEFINITION_KINDS.
  _parse_qualified_name: _parse_qualified_name().
  _build_import_map: _build_import_map().
  _build_module_to_file_map: _build_module_to_file_map().
  logger: logger.
  _REFERENCE_KINDS: _REFERENCE_KINDS.
  SymbolResolver.__init__: SymbolResolver#__init__().
---
# Module: [`tree_sitter_analyzer/symbol_resolver.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/symbol_resolver.py)

## Classes
### `DefinitionLocation`
- def: [`tree_sitter_analyzer/symbol_resolver.py:38`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/symbol_resolver.py#L38)
- signature: `class DefinitionLocation:`
- members:
  - `to_dict(self)` — [`L48`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/symbol_resolver.py#L48)
  - `confidence` — [`L45`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/symbol_resolver.py#L45)
  - `context` — [`L46`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/symbol_resolver.py#L46)
  - `end_line` — [`L43`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/symbol_resolver.py#L43)
  - `file` — [`L39`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/symbol_resolver.py#L39)
  - `kind` — [`L41`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/symbol_resolver.py#L41)
  - `language` — [`L44`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/symbol_resolver.py#L44)
  - `line` — [`L42`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/symbol_resolver.py#L42)
  - `name` — [`L40`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/symbol_resolver.py#L40)
- used by: [`execute`](mcp/tools/symbol_resolve_tool.md#CodeGraphSymbolResolveTool.execute), [`definitions`](symbol_resolver.md#ResolveResult.definitions), [`_find_defs_in_file`](symbol_resolver.md#SymbolResolver._find_defs_in_file), [`_definition_location`](symbol_resolver.md#_definition_location), [`_resolve_definition`](mcp/tools/codegraph_navigate_tool.md#CodeGraphNavigateTool._resolve_definition), [`_resolve_from_imports`](symbol_resolver.md#SymbolResolver._resolve_from_imports), [`to_dict`](symbol_resolver.md#ResolveResult.to_dict), [`_is_child_of`](symbol_resolver.md#SymbolResolver._is_child_of), [`_resolve_qualified`](symbol_resolver.md#SymbolResolver._resolve_qualified), [`_lookup_by_module`](symbol_resolver.md#SymbolResolver._lookup_by_module), [`_find_definitions`](symbol_resolver.md#SymbolResolver._find_definitions), [`_resolve_simple`](symbol_resolver.md#SymbolResolver._resolve_simple), [`_apply_confidence`](symbol_resolver.md#_apply_confidence)  (15 test-only)

### `ReferenceLocation`
- def: [`tree_sitter_analyzer/symbol_resolver.py:64`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/symbol_resolver.py#L64)
- signature: `class ReferenceLocation:`
- members:
  - `to_dict(self)` — [`L73`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/symbol_resolver.py#L73)
  - `end_line` — [`L69`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/symbol_resolver.py#L69)
  - `file` — [`L65`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/symbol_resolver.py#L65)
  - `kind` — [`L67`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/symbol_resolver.py#L67)
  - `language` — [`L70`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/symbol_resolver.py#L70)
  - `line` — [`L68`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/symbol_resolver.py#L68)
  - `name` — [`L66`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/symbol_resolver.py#L66)
  - `reference_type` — [`L71`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/symbol_resolver.py#L71)
- used by: [`execute`](mcp/tools/symbol_resolve_tool.md#CodeGraphSymbolResolveTool.execute), [`_find_import_references`](symbol_resolver.md#SymbolResolver._find_import_references), [`_find_references`](symbol_resolver.md#SymbolResolver._find_references), [`_collect_import_refs_from_list`](symbol_resolver.md#_collect_import_refs_from_list), [`_find_references`](mcp/tools/codegraph_navigate_tool.md#CodeGraphNavigateTool._find_references), [`to_dict`](symbol_resolver.md#ResolveResult.to_dict), [`references`](symbol_resolver.md#ResolveResult.references)  (2 test-only)

### `ResolveResult`
- def: [`tree_sitter_analyzer/symbol_resolver.py:86`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/symbol_resolver.py#L86)
- signature: `class ResolveResult:`
- members:
  - `to_dict(self)` — [`L92`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/symbol_resolver.py#L92)
  - `definitions` — [`L88`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/symbol_resolver.py#L88)
  - `references` — [`L89`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/symbol_resolver.py#L89)
  - `resolved_via` — [`L90`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/symbol_resolver.py#L90)
  - `symbol` — [`L87`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/symbol_resolver.py#L87)
- uses (calls/refs, reference-scoped): [`DefinitionLocation`](symbol_resolver.md#DefinitionLocation), [`to_dict`](symbol_resolver.md#DefinitionLocation.to_dict), [`to_dict`](symbol_resolver.md#ReferenceLocation.to_dict), [`ReferenceLocation`](symbol_resolver.md#ReferenceLocation)
- used by: [`execute`](mcp/tools/symbol_resolve_tool.md#CodeGraphSymbolResolveTool.execute), [`resolve`](symbol_resolver.md#SymbolResolver.resolve), [`find_references`](symbol_resolver.md#SymbolResolver.find_references), [`_find_references`](mcp/tools/codegraph_navigate_tool.md#CodeGraphNavigateTool._find_references), [`_resolve_definition`](mcp/tools/codegraph_navigate_tool.md#CodeGraphNavigateTool._resolve_definition)  (10 test-only)

### `SymbolResolver`
- def: [`tree_sitter_analyzer/symbol_resolver.py:204`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/symbol_resolver.py#L204)
- doc: Resolve symbol definitions and find references using the AST cache.
- signature: `class SymbolResolver:`
- members:
  - `_lookup_by_module(self, module: str, name: str)` — [`L299`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/symbol_resolver.py#L299) — Resolve *module* to a file and return definitions of *name* with confidence 0.8.
  - `find_references(self, symbol: str)` — [`L224`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/symbol_resolver.py#L224)
  - `resolve(self, symbol: str)` — [`L218`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/symbol_resolver.py#L218)
- protocol/private: `__init__`[`L212`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/symbol_resolver.py#L212), `_cache`[`L213`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/symbol_resolver.py#L213), `_definition_backend`[`L214`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/symbol_resolver.py#L214), `_find_definitions`[`L231`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/symbol_resolver.py#L231), `_find_defs_in_file`[`L345`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/symbol_resolver.py#L345), `_find_import_references`[`L432`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/symbol_resolver.py#L432), `_find_references`[`L391`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/symbol_resolver.py#L391), `_import_map`[`L215`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/symbol_resolver.py#L215), `_is_child_of`[`L269`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/symbol_resolver.py#L269), `_module_to_file`[`L216`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/symbol_resolver.py#L216), `_resolve_from_imports`[`L312`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/symbol_resolver.py#L312), `_resolve_qualified`[`L249`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/symbol_resolver.py#L249), `_resolve_simple`[`L243`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/symbol_resolver.py#L243)
- uses (calls/refs, reference-scoped): [`definitions`](symbol_resolver.md#ResolveResult.definitions), [`CodeGraphQueryBackend`](codegraph_query_backend.md#CodeGraphQueryBackend), [`DefinitionLocation`](symbol_resolver.md#DefinitionLocation), [`_definition_location`](symbol_resolver.md#_definition_location), [`_collect_import_refs_from_list`](symbol_resolver.md#_collect_import_refs_from_list), [`name`](symbol_resolver.md#DefinitionLocation.name), [`resolve_definitions`](codegraph_query_backend.md#CodeGraphQueryBackend.resolve_definitions), [`kind`](symbol_resolver.md#DefinitionLocation.kind), [`file`](symbol_resolver.md#DefinitionLocation.file), [`references`](symbol_resolver.md#ResolveResult.references), [`ReferenceLocation`](symbol_resolver.md#ReferenceLocation), [`line`](symbol_resolver.md#DefinitionLocation.line), [`ResolveResult`](symbol_resolver.md#ResolveResult), [`confidence`](symbol_resolver.md#DefinitionLocation.confidence), [`end_line`](symbol_resolver.md#DefinitionLocation.end_line), [`file`](symbol_resolver.md#ReferenceLocation.file), [`language`](symbol_resolver.md#DefinitionLocation.language), [`line`](symbol_resolver.md#ReferenceLocation.line), [`_apply_confidence`](symbol_resolver.md#_apply_confidence), [`kind`](symbol_resolver.md#ReferenceLocation.kind), [`language`](symbol_resolver.md#ReferenceLocation.language), [`name`](symbol_resolver.md#ReferenceLocation.name), [`end_line`](symbol_resolver.md#ReferenceLocation.end_line), [`reference_type`](symbol_resolver.md#ReferenceLocation.reference_type), [`symbol`](symbol_resolver.md#ResolveResult.symbol), [`_DEFINITION_KINDS`](symbol_resolver.md#_DEFINITION_KINDS), [`_build_import_map`](symbol_resolver.md#_build_import_map), [`_parse_qualified_name`](symbol_resolver.md#_parse_qualified_name), [`_build_module_to_file_map`](symbol_resolver.md#_build_module_to_file_map)
- used by: [`execute`](mcp/tools/codegraph_explore_tool.md#CodeGraphExploreTool.execute), [`rename_symbol`](rename_symbol.md#rename_symbol), [`execute`](mcp/tools/symbol_resolve_tool.md#CodeGraphSymbolResolveTool.execute), [`_find_references`](mcp/tools/codegraph_navigate_tool.md#CodeGraphNavigateTool._find_references), [`_resolve_definition`](mcp/tools/codegraph_navigate_tool.md#CodeGraphNavigateTool._resolve_definition)  (12 test-only)

## Functions
- `_apply_confidence(defs: list[DefinitionLocation], confidence: float = 0.8)` — [`L152`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/symbol_resolver.py#L152) — Set confidence on every DefinitionLocation in *defs* and return *defs*.
- `_build_import_map(cache: Any)` — [`L108`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/symbol_resolver.py#L108) — Import entries may be `str` (module path) or `dict` (qualified import).
- `_build_module_to_file_map(cache: Any)` — [`L125`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/symbol_resolver.py#L125)
- `_collect_import_refs_from_list(imported_names: list, name: str, file_path: str, imp_line: int, refs: list[ReferenceLocation])` — [`L165`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/symbol_resolver.py#L165) — Append import ReferenceLocations to *refs* for each matching name in *imported_names*.
- `_definition_location(item: dict[str, Any])` — [`L191`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/symbol_resolver.py#L191)
- `_parse_qualified_name(symbol: str)` — [`L103`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/symbol_resolver.py#L103)

## Module values
- `_DEFINITION_KINDS` — [`L30`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/symbol_resolver.py#L30)
- `_REFERENCE_KINDS` — [`L34`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/symbol_resolver.py#L34)
- `logger` — [`L27`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/symbol_resolver.py#L27)

