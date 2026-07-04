---
title: 'Module: tree_sitter_analyzer/synapse_resolver/__init__.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/synapse_resolver/__init__.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.synapse_resolver`/
symbols:
  resolve_callee: resolve_callee().
  ResolvedCallee.resolution: ResolvedCallee#resolution.
  ResolvedCallee: ResolvedCallee#
  _resolve_callee_python: _resolve_callee_python().
  _try_stdlib_method: _try_stdlib_method().
  _try_import: _try_import().
  _try_external_method: _try_external_method().
  _try_builtin_method: _try_builtin_method().
  ResolvedCallee.resolved_file: ResolvedCallee#resolved_file.
  _try_local: _try_local().
  _try_stdlib: _try_stdlib().
  _try_single_global: _try_single_global().
  ResolvedCallee.callee_symbol_id: ResolvedCallee#callee_symbol_id.
  _try_unique_method: _try_unique_method().
  _is_cross_language: _is_cross_language().
  _lookup_symbol_id: _lookup_symbol_id().
  _table_language: _table_language().
  _try_self_method: _try_self_method().
  _try_builtin: _try_builtin().
  _try_class_method: _try_class_method().
  _item_file: _item_file().
  _item_symbol_id: _item_symbol_id().
  _split_qualifier: _split_qualifier().
  __all__: __all__.
---
# Module: [`tree_sitter_analyzer/synapse_resolver/__init__.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/__init__.py)

## Classes
### `ResolvedCallee`
- def: [`tree_sitter_analyzer/synapse_resolver/__init__.py:46`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/__init__.py#L46)
- doc: One resolution per call edge — written into the unified `edges` table.
- signature: `class ResolvedCallee:`
- members:
  - `callee_symbol_id` — [`L49`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/__init__.py#L49)
  - `resolution` — [`L50`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/__init__.py#L50)
  - `resolved_file` — [`L51`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/__init__.py#L51)
- used by: [`resolve_callee`](__init__.md#resolve_callee), [`_resolve_callee_python`](__init__.md#_resolve_callee_python), [`_try_stdlib_method`](__init__.md#_try_stdlib_method), [`_try_import`](__init__.md#_try_import), [`_try_builtin_method`](__init__.md#_try_builtin_method), [`_try_external_method`](__init__.md#_try_external_method), [`_try_local`](__init__.md#_try_local), [`_try_single_global`](__init__.md#_try_single_global), [`_try_stdlib`](__init__.md#_try_stdlib), [`resolve_call_edges_for_file`](../_ast_cache_synapse.md#resolve_call_edges_for_file), [`run_synapse_backfill`](../_ast_cache_synapse.md#run_synapse_backfill), [`_is_cross_language`](__init__.md#_is_cross_language), [`_try_unique_method`](__init__.md#_try_unique_method), [`_try_builtin`](__init__.md#_try_builtin), [`_try_class_method`](__init__.md#_try_class_method), [`_try_self_method`](__init__.md#_try_self_method)  (31 test-only)

## Functions
- `_is_cross_language(out: ResolvedCallee, caller_lang: str, ctx: ResolverContext)` — [`L573`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/__init__.py#L573) — True when a project bind crosses a language boundary.
- `_item_file(item: object)` — [`L78`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/__init__.py#L78)
- `_item_symbol_id(item: object)` — [`L70`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/__init__.py#L70)
- `_lookup_symbol_id(file: str, name: str, ctx: ResolverContext)` — [`L62`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/__init__.py#L62) — Find a project symbol id for ``name`` in ``file``.
- `_resolve_callee_python(callee_name: str, caller_file: str, ctx: ResolverContext, callee_full: str | None = None, caller_name: str = "")` — [`L514`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/__init__.py#L514) — Resolve a single callee per the priority cascade above.
- `_split_qualifier(name: str)` — [`L54`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/__init__.py#L54) — Split ``"a.b.c"`` into ``("a.b", "c")``. Returns ``("", name)`` if no dot.
- `_table_language(ctx: ResolverContext, caller_file: str)` — [`L216`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/__init__.py#L216) — Language key for the RFC-0004/5/7 method tables (stdlib/external/builtin).
- `_try_builtin(base: str, qualifier: str, ctx: ResolverContext)` — [`L206`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/__init__.py#L206)
- `_try_builtin_method(base: str, qualifier: str, caller_file: str, ctx: ResolverContext)` — [`L319`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/__init__.py#L319) — RFC-0007 FINAL tier: classify a qualified Python builtin name as ``builtin``.
- `_try_class_method(base: str, qualifier: str, ctx: ResolverContext)` — [`L392`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/__init__.py#L392) — RFC-0002: receiver-type-aware method resolution.
- `_try_external_method(base: str, qualifier: str, caller_file: str, ctx: ResolverContext)` — [`L277`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/__init__.py#L277) — RFC-0005 FINAL tier: classify a bare third-party library method name as
- `_try_import(base: str, qualifier: str, caller_file: str, ctx: ResolverContext)` — [`L132`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/__init__.py#L132) — Two cases:
- `_try_local(base: str, caller_file: str, ctx: ResolverContext)` — [`L112`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/__init__.py#L112)
- `_try_self_method(base: str, qualifier: str, caller_file: str, caller_name: str, ctx: ResolverContext)` — [`L84`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/__init__.py#L84)
- `_try_single_global(base: str, qualifier: str, ctx: ResolverContext)` — [`L369`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/__init__.py#L369)
- `_try_stdlib(base: str, qualifier: str, caller_file: str, ctx: ResolverContext)` — [`L181`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/__init__.py#L181) — Two strategies:
- `_try_stdlib_method(base: str, qualifier: str, caller_file: str, ctx: ResolverContext)` — [`L234`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/__init__.py#L234) — RFC-0004 FINAL tier: classify a bare stdlib/builtin method name as
- `_try_unique_method(base: str, qualifier: str, caller_file: str, ctx: ResolverContext)` — [`L426`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/__init__.py#L426) — RFC-0002 Phase 1: receiver method call where the method name is unique.
- `resolve_callee(callee_name: str, caller_file: str, ctx: ResolverContext, callee_full: str | None = None, caller_name: str = "")` — [`L476`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/__init__.py#L476) — Resolve a single callee, dispatching by the caller file's language.

## Module values
- `__all__` — [`L592`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/__init__.py#L592)

