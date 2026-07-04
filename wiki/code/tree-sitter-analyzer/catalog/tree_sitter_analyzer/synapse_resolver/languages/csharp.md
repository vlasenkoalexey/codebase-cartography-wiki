---
title: 'Module: tree_sitter_analyzer/synapse_resolver/languages/csharp.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/synapse_resolver/languages/csharp.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.synapse_resolver.languages.csharp`/
symbols:
  resolve_csharp_callee: resolve_csharp_callee().
  build_csharp_context: build_csharp_context().
  _project_owns: _project_owns().
  CSharpResolverContext: CSharpResolverContext#
  _lookup_in_file: _lookup_in_file().
  CSharpResolverContext.member_owner_class_count: CSharpResolverContext#member_owner_class_count().
  CSharpResolverContext.file_languages: CSharpResolverContext#file_languages.
  CSharpResolverContext.global_name_table: CSharpResolverContext#global_name_table.
  CSharpResolverContext.class_methods_thunk: CSharpResolverContext#class_methods_thunk.
  CSharpResolverContext._class_methods: CSharpResolverContext#_class_methods.
  _CSHARP_LANG._CSHARP_LANG: _CSHARP_LANG._CSHARP_LANG.
  CSharpResolverContext.file_symbols: CSharpResolverContext#file_symbols.
  _split_qualifier: _split_qualifier().
  _SELF_RECEIVERS._SELF_RECEIVERS: _SELF_RECEIVERS._SELF_RECEIVERS.
  _LOCAL_KINDS._LOCAL_KINDS: _LOCAL_KINDS._LOCAL_KINDS.
  _MEMBER_KINDS._MEMBER_KINDS: _MEMBER_KINDS._MEMBER_KINDS.
  __all__: __all__.
---
# Module: [`tree_sitter_analyzer/synapse_resolver/languages/csharp.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/csharp.py)

## Classes
### `CSharpResolverContext`
- def: [`tree_sitter_analyzer/synapse_resolver/languages/csharp.py:78`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/csharp.py#L78)
- doc: Per-index C# resolution maps (built once per pass).
- signature: `class CSharpResolverContext:`
- members:
  - `member_owner_class_count(self, file_path: str, method_name: str)` — [`L104`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/csharp.py#L104) — Return how many classes in ``file_path`` define ``method_name``.
  - `class_methods_thunk` — [`L100`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/csharp.py#L100)
  - `file_languages` — [`L93`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/csharp.py#L93)
  - `file_symbols` — [`L88`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/csharp.py#L88)
  - `global_name_table` — [`L90`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/csharp.py#L90)
- protocol/private: `_class_methods`[`L102`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/csharp.py#L102)
- used by: [`resolve_csharp_callee`](csharp.md#resolve_csharp_callee), [`build_csharp_context`](csharp.md#build_csharp_context), [`_project_owns`](csharp.md#_project_owns), [`_lookup_in_file`](csharp.md#_lookup_in_file)  (3 test-only)

## Functions
- `_lookup_in_file(ctx: CSharpResolverContext, file_path: str, simple: str, kinds: frozenset[str])` — [`L166`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/csharp.py#L166) — Resolve ``simple`` to a same-file symbol of an allowed ``kind``.
- `_project_owns(ctx: CSharpResolverContext, simple: str)` — [`L197`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/csharp.py#L197) — True when a COMPATIBLE-LANGUAGE project symbol of name ``simple`` exists.
- `_split_qualifier(callee_full: str, callee_name: str)` — [`L149`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/csharp.py#L149) — Return ``(qualifier, simple_name)`` from a C# call's full name.
- `build_csharp_context(*, imports_by_file: dict[str, Any], file_languages: dict[str, str], file_symbols: dict[str, Any], global_name_table: dict[str, Any], file_class_methods: Callable[[], dict[str, Any]], **_ignored: Any)` — [`L121`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/csharp.py#L121) — Build the C# context, or ``None`` when no C# file is indexed.
- `resolve_csharp_callee(callee_name: str, callee_full: str, caller_file: str, ctx: CSharpResolverContext)` — [`L213`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/csharp.py#L213) — Resolve one C# call edge.

## Module values
- `_CSHARP_LANG` — [`L60`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/csharp.py#L60)
- `_LOCAL_KINDS` — [`L70`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/csharp.py#L70)
- `_MEMBER_KINDS` — [`L74`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/csharp.py#L74)
- `_SELF_RECEIVERS` — [`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/csharp.py#L65)
- `__all__` — [`L290`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/csharp.py#L290)

