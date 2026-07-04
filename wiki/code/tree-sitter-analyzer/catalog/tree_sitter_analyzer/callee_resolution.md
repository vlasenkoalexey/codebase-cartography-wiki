---
title: 'Module: tree_sitter_analyzer/callee_resolution.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/callee_resolution.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.callee_resolution`/
symbols:
  CalleeResolver._resolve: CalleeResolver#_resolve().
  CalleeResolver: CalleeResolver#
  CalleeResolver.resolve_items: CalleeResolver#resolve_items().
  _append_resolution: _append_resolution().
  CalleeResolver.resolve_first_item: CalleeResolver#resolve_first_item().
  CalleeResolver.resolve_first_file: CalleeResolver#resolve_first_file().
  CalleeResolver.resolve_files: CalleeResolver#resolve_files().
  CalleeResolver._source_language: CalleeResolver#_source_language().
  _append_file_resolution: _append_file_resolution().
  CalleeResolution: CalleeResolution#
  _item_key: _item_key().
  CalleeResolver._import_target: CalleeResolver#_import_target().
  CalleeResolver._functions_by_file: CalleeResolver#_functions_by_file.
  _item_name: _item_name().
  CalleeResolution.confidence: CalleeResolution#confidence.
  _item_file: _item_file().
  CalleeResolution.file: CalleeResolution#file.
  CalleeResolution.item: CalleeResolution#item.
  _split_qualifier: _split_qualifier().
  _item_language: _item_language().
  CalleeResolver._functions_by_name: CalleeResolver#_functions_by_name.
  CalleeResolver._name_to_source: CalleeResolver#_name_to_source.
  CalleeResolver.__init__: CalleeResolver#__init__().
---
# Module: [`tree_sitter_analyzer/callee_resolution.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/callee_resolution.py)

## Classes
### `CalleeResolution`
- def: [`tree_sitter_analyzer/callee_resolution.py:13`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/callee_resolution.py#L13)
- signature: `class CalleeResolution:`
- members:
  - `confidence` — [`L15`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/callee_resolution.py#L15)
  - `file` — [`L14`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/callee_resolution.py#L14)
  - `item` — [`L16`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/callee_resolution.py#L16)
- used by: [`_resolve`](callee_resolution.md#CalleeResolver._resolve), [`resolve_items`](callee_resolution.md#CalleeResolver.resolve_items), [`_append_resolution`](callee_resolution.md#_append_resolution), [`resolve_files`](callee_resolution.md#CalleeResolver.resolve_files), [`_append_file_resolution`](callee_resolution.md#_append_file_resolution)

### `CalleeResolver`
- def: [`tree_sitter_analyzer/callee_resolution.py:19`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/callee_resolution.py#L19) — documented in [tree_sitter_analyzer-call_graph](../../concepts/tree_sitter_analyzer-call_graph.md)
- doc: Resolve call targets using local, import, then global project matches.
- signature: `class CalleeResolver:`
- members:
  - `_source_language(self, source_file: str)` — [`L208`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/callee_resolution.py#L208) — Best-effort language of ``source_file``.
  - `resolve_files(self, callee_name: str, source_file: str, *, include_unmatched_import: bool = False, include_local: bool = True, include_import: bool = True, include_global: bool = True)` — [`L84`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/callee_resolution.py#L84)
  - `resolve_first_file(self, callee_name: str, source_file: str, *, include_unmatched_import: bool = False, include_local: bool = True, include_import: bool = True, include_global: bool = True)` — [`L107`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/callee_resolution.py#L107)
  - `resolve_first_item(self, callee_name: str, source_file: str, *, include_local: bool = True, include_import: bool = True, include_global: bool = True)` — [`L55`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/callee_resolution.py#L55)
  - `resolve_items(self, callee_name: str, source_file: str, *, include_local: bool = True, include_import: bool = True, include_global: bool = True)` — [`L33`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/callee_resolution.py#L33)
- protocol/private: `__init__`[`L22`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/callee_resolution.py#L22), `_functions_by_file`[`L30`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/callee_resolution.py#L30), `_functions_by_name`[`L29`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/callee_resolution.py#L29), `_import_target`[`L222`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/callee_resolution.py#L222), `_name_to_source`[`L31`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/callee_resolution.py#L31), `_resolve`[`L134`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/callee_resolution.py#L134)
- uses (calls/refs, reference-scoped): [`languages_compatible`](_language_family.md#languages_compatible), [`_append_resolution`](callee_resolution.md#_append_resolution), [`language_from_path`](_language_family.md#language_from_path), [`_append_file_resolution`](callee_resolution.md#_append_file_resolution), [`CalleeResolution`](callee_resolution.md#CalleeResolution), [`_item_name`](callee_resolution.md#_item_name), [`_item_file`](callee_resolution.md#_item_file), [`confidence`](callee_resolution.md#CalleeResolution.confidence), [`_item_language`](callee_resolution.md#_item_language), [`_split_qualifier`](callee_resolution.md#_split_qualifier), [`file`](callee_resolution.md#CalleeResolution.file), [`item`](callee_resolution.md#CalleeResolution.item)  (1 test-only)
- used by: [`build`](call_graph.md#CallGraph.build), [`build`](cross_file_resolver.md#CrossFileResolver.build), [`_build_from_cache`](call_graph.md#CachedCallGraph._build_from_cache), [`_try_stdlib_method`](synapse_resolver/__init__.md#_try_stdlib_method), [`_try_import`](synapse_resolver/__init__.md#_try_import), [`_try_builtin_method`](synapse_resolver/__init__.md#_try_builtin_method), [`_try_external_method`](synapse_resolver/__init__.md#_try_external_method), [`callee_resolver`](synapse_resolver/_context.md#ResolverContext.callee_resolver), [`_resolve_callee`](call_graph.md#CallGraph._resolve_callee), [`_try_local`](synapse_resolver/__init__.md#_try_local), [`_try_single_global`](synapse_resolver/__init__.md#_try_single_global), [`resolve_callee`](cross_file_resolver.md#CrossFileResolver.resolve_callee), [`_callee_resolver`](call_graph.md#CallGraph._callee_resolver), [`__init__`](synapse_resolver/_context.md#ResolverContext.__init__), [`_callee_resolver`](cross_file_resolver.md#CrossFileResolver._callee_resolver), [`_build_callee_resolver`](synapse_resolver/_context.md#_build_callee_resolver)  (11 test-only)

## Functions
- `_append_file_resolution(results: list[CalleeResolution], seen: set[str], file_path: str, confidence: float)` — [`L281`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/callee_resolution.py#L281)
- `_append_resolution(results: list[CalleeResolution], seen: set[str], item: Any, confidence: float, *, keep_items: bool)` — [`L259`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/callee_resolution.py#L259)
- `_item_file(item: Any)` — [`L247`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/callee_resolution.py#L247)
- `_item_key(item: Any)` — [`L293`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/callee_resolution.py#L293)
- `_item_language(item: Any)` — [`L253`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/callee_resolution.py#L253)
- `_item_name(item: Any)` — [`L241`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/callee_resolution.py#L241)
- `_split_qualifier(callee_name: str)` — [`L234`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/callee_resolution.py#L234)

