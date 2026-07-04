---
title: 'Module: tree_sitter_analyzer/synapse_resolver/languages/cpp.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/synapse_resolver/languages/cpp.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.synapse_resolver.languages.cpp`/
symbols:
  resolve_cpp_callee: resolve_cpp_callee().
  build_cpp_context: build_cpp_context().
  _project_owns: _project_owns().
  CppResolverContext: CppResolverContext#
  _lookup_in_file: _lookup_in_file().
  __all__: __all__.
  CppResolverContext.member_owner_class_count: CppResolverContext#member_owner_class_count().
  CppResolverContext.file_languages: CppResolverContext#file_languages.
  CppResolverContext.global_name_table: CppResolverContext#global_name_table.
  CppResolverContext.class_methods_thunk: CppResolverContext#class_methods_thunk.
  CppResolverContext._class_methods: CppResolverContext#_class_methods.
  CppResolverContext.file_symbols: CppResolverContext#file_symbols.
  _split_qualifier: _split_qualifier().
  _CPP_LANGS._CPP_LANGS: _CPP_LANGS._CPP_LANGS.
  _SELF_RECEIVERS._SELF_RECEIVERS: _SELF_RECEIVERS._SELF_RECEIVERS.
  _LOCAL_KINDS._LOCAL_KINDS: _LOCAL_KINDS._LOCAL_KINDS.
  _MEMBER_KINDS._MEMBER_KINDS: _MEMBER_KINDS._MEMBER_KINDS.
---
# Module: [`tree_sitter_analyzer/synapse_resolver/languages/cpp.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/cpp.py)

## Classes
### `CppResolverContext`
- def: [`tree_sitter_analyzer/synapse_resolver/languages/cpp.py:75`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/cpp.py#L75)
- doc: Per-index C++ resolution maps (built once per pass).
- signature: `class CppResolverContext:`
- members:
  - `member_owner_class_count(self, file_path: str, method_name: str)` — [`L101`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/cpp.py#L101) — Return how many classes in ``file_path`` define ``method_name``.
  - `class_methods_thunk` — [`L97`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/cpp.py#L97)
  - `file_languages` — [`L89`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/cpp.py#L89)
  - `file_symbols` — [`L84`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/cpp.py#L84)
  - `global_name_table` — [`L86`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/cpp.py#L86)
- protocol/private: `_class_methods`[`L99`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/cpp.py#L99)
- used by: [`resolve_cpp_callee`](cpp.md#resolve_cpp_callee), [`build_cpp_context`](cpp.md#build_cpp_context), [`_project_owns`](cpp.md#_project_owns), [`_lookup_in_file`](cpp.md#_lookup_in_file)  (4 test-only)

## Functions
- `_lookup_in_file(ctx: CppResolverContext, file_path: str, simple: str, kinds: frozenset[str])` — [`L184`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/cpp.py#L184) — Resolve ``simple`` to a same-file symbol of an allowed ``kind``.
- `_project_owns(ctx: CppResolverContext, simple: str)` — [`L217`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/cpp.py#L217) — True when a COMPATIBLE-LANGUAGE project symbol of name ``simple`` exists.
- `_split_qualifier(callee_full: str, callee_name: str)` — [`L147`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/cpp.py#L147) — Return ``(qualifier, simple_name)`` from a C++ call's full name.
- `build_cpp_context(*, imports_by_file: dict[str, Any], file_languages: dict[str, str], file_symbols: dict[str, Any], global_name_table: dict[str, Any], file_class_methods: Callable[[], dict[str, Any]], **_ignored: Any)` — [`L119`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/cpp.py#L119) — Build the C++ context, or ``None`` when no C++ file is indexed.
- `resolve_cpp_callee(callee_name: str, callee_full: str, caller_file: str, ctx: CppResolverContext)` — [`L233`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/cpp.py#L233) — Resolve one C++ call edge.

## Module values
- `_CPP_LANGS` — [`L66`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/cpp.py#L66)
- `_LOCAL_KINDS` — [`L176`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/cpp.py#L176)
- `_MEMBER_KINDS` — [`L181`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/cpp.py#L181)
- `_SELF_RECEIVERS` — [`L71`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/cpp.py#L71)
- `__all__` — [`L295`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/cpp.py#L295)

