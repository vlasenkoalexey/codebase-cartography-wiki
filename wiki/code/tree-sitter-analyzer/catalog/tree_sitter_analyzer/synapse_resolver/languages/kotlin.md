---
title: 'Module: tree_sitter_analyzer/synapse_resolver/languages/kotlin.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/synapse_resolver/languages/kotlin.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.synapse_resolver.languages.kotlin`/
symbols:
  resolve_kotlin_callee: resolve_kotlin_callee().
  build_kotlin_resolver_context: build_kotlin_resolver_context().
  _project_owns: _project_owns().
  _lookup_bare_in_file: _lookup_bare_in_file().
  _lookup_unique_method_in_file: _lookup_unique_method_in_file().
  KotlinResolverContext: KotlinResolverContext#
  KotlinResolverContext.member_owner_class_count: KotlinResolverContext#member_owner_class_count().
  _KOTLIN_LANG: _KOTLIN_LANG.
  KotlinResolverContext.file_symbols: KotlinResolverContext#file_symbols.
  KotlinResolverContext.class_methods_thunk: KotlinResolverContext#class_methods_thunk.
  KotlinResolverContext._class_methods: KotlinResolverContext#_class_methods.
  KotlinResolverContext.global_name_table: KotlinResolverContext#global_name_table.
  KotlinResolverContext.file_languages: KotlinResolverContext#file_languages.
  _split_receiver: _split_receiver().
  _SELF_RECEIVERS._SELF_RECEIVERS: _SELF_RECEIVERS._SELF_RECEIVERS.
  _LOCAL_KINDS._LOCAL_KINDS: _LOCAL_KINDS._LOCAL_KINDS.
  __all__: __all__.
---
# Module: [`tree_sitter_analyzer/synapse_resolver/languages/kotlin.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/kotlin.py)

## Classes
### `KotlinResolverContext`
- def: [`tree_sitter_analyzer/synapse_resolver/languages/kotlin.py:70`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/kotlin.py#L70)
- doc: Per-index Kotlin resolution maps (built once per pass).
- signature: `class KotlinResolverContext:`
- members:
  - `member_owner_class_count(self, file_path: str, method_name: str)` — [`L95`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/kotlin.py#L95) — Return how many classes in ``file_path`` define ``method_name``.
  - `class_methods_thunk` — [`L92`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/kotlin.py#L92)
  - `file_languages` — [`L87`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/kotlin.py#L87)
  - `file_symbols` — [`L80`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/kotlin.py#L80)
  - `global_name_table` — [`L84`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/kotlin.py#L84)
- protocol/private: `_class_methods`[`L93`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/kotlin.py#L93)
- used by: [`resolve_kotlin_callee`](kotlin.md#resolve_kotlin_callee), [`build_kotlin_resolver_context`](kotlin.md#build_kotlin_resolver_context), [`_project_owns`](kotlin.md#_project_owns), [`_lookup_bare_in_file`](kotlin.md#_lookup_bare_in_file), [`_lookup_unique_method_in_file`](kotlin.md#_lookup_unique_method_in_file)

## Functions
- `_lookup_bare_in_file(ctx: KotlinResolverContext, file_path: str, simple: str)` — [`L154`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/kotlin.py#L154) — Return the symbol id of a same-file top-level ``function``/``class`` (or a
- `_lookup_unique_method_in_file(ctx: KotlinResolverContext, file_path: str, simple: str)` — [`L171`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/kotlin.py#L171) — Return the symbol id of a same-file ``method`` named ``simple``, but ONLY
- `_project_owns(ctx: KotlinResolverContext, simple: str, caller_file: str)` — [`L195`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/kotlin.py#L195) — True when a COMPATIBLE-LANGUAGE (Kotlin) project symbol named ``simple``
- `_split_receiver(callee_full: str, callee_name: str)` — [`L139`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/kotlin.py#L139) — Return ``(receiver, simple_name)`` from a Kotlin call's full name.
- `build_kotlin_resolver_context(*, imports_by_file: dict[str, Any], file_languages: dict[str, str], file_symbols: dict[str, Any], global_name_table: dict[str, Any], file_class_methods: Callable[[], dict[str, Any]], **_ignored: Any)` — [`L112`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/kotlin.py#L112) — Build the Kotlin context, or ``None`` when no Kotlin file is indexed.
- `resolve_kotlin_callee(callee_name: str, callee_full: str, caller_file: str, ctx: KotlinResolverContext)` — [`L213`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/kotlin.py#L213) — Resolve one Kotlin call edge.

## Module values
- `_KOTLIN_LANG` — [`L57`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/kotlin.py#L57)
- `_LOCAL_KINDS` — [`L66`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/kotlin.py#L66)
- `_SELF_RECEIVERS` — [`L62`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/kotlin.py#L62)
- `__all__` — [`L269`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/kotlin.py#L269)

