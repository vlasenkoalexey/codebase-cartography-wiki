---
title: 'Module: tree_sitter_analyzer/synapse_resolver/languages/javascript.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/synapse_resolver/languages/javascript.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.synapse_resolver.languages.javascript`/
symbols:
  resolve_javascript_callee: resolve_javascript_callee().
  JavaScriptResolverContext: JavaScriptResolverContext#
  _dialect: _dialect.
  build_javascript_context: build_javascript_context().
  _lookup_in_file: _lookup_in_file().
  _js_project_owns: _js_project_owns().
  _js_shadowed_globals_from_conn: _js_shadowed_globals_from_conn().
  _owner_kind: _owner_kind().
  JavaScriptResolverContext.__init__: JavaScriptResolverContext#__init__().
  _JS_DIALECTS._JS_DIALECTS: _JS_DIALECTS._JS_DIALECTS.
  _BARE_CALLABLE_KINDS._BARE_CALLABLE_KINDS: _BARE_CALLABLE_KINDS._BARE_CALLABLE_KINDS.
  _split_receiver: _split_receiver().
  JavaScriptResolverContext.__slots__: JavaScriptResolverContext#__slots__.
---
# Module: [`tree_sitter_analyzer/synapse_resolver/languages/javascript.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/javascript.py)

## Classes
### `JavaScriptResolverContext`
- def: [`tree_sitter_analyzer/synapse_resolver/languages/javascript.py:54`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/javascript.py#L54)
- doc: Per-index JavaScript resolution maps (built once per pass).
- signature: `class JavaScriptResolverContext:`
- protocol/private: `__init__`[`L69`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/javascript.py#L69), `__slots__`[`L61`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/javascript.py#L61)
- used by: [`resolve_javascript_callee`](javascript.md#resolve_javascript_callee), [`build_javascript_context`](javascript.md#build_javascript_context), [`_js_project_owns`](javascript.md#_js_project_owns), [`_lookup_in_file`](javascript.md#_lookup_in_file), [`_owner_kind`](javascript.md#_owner_kind)

## Functions
- `_js_project_owns(ctx: JavaScriptResolverContext, simple: str)` — [`L205`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/javascript.py#L205) — True when a JS-FAMILY project symbol is named ``simple``.
- `_js_shadowed_globals_from_conn(conn: Any, file_languages: dict[str, str])` — [`L90`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/javascript.py#L90) — JS-family ``variable``-kind symbol names, for the builtin-shadow gate.
- `_lookup_in_file(ctx: JavaScriptResolverContext, file_path: str, simple: str)` — [`L163`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/javascript.py#L163) — Symbol id of a same-file BARE-CALLABLE named ``simple`` in ``file_path``.
- `_owner_kind(ctx: JavaScriptResolverContext, owner_file: str, sym_id: int)` — [`L192`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/javascript.py#L192) — Kind (``function``/``method``/``class``) of ``sym_id`` in ``owner_file``.
- `_split_receiver(full_name: str, bare_name: str)` — [`L154`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/javascript.py#L154) — Return ``(receiver, simple_name)`` from a JS call's full name.
- `build_javascript_context(*, imports_by_file: dict[str, Any], file_languages: dict[str, str], file_symbols: dict[str, Any], global_name_table: dict[str, Any], file_class_methods: Any, conn: Any = None, js_shadowed_globals: Any = None, **_ignored: Any)` — [`L119`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/javascript.py#L119) — Build the JS context, or ``None`` when no ``.js``/``.jsx`` file is indexed.
- `resolve_javascript_callee(bare_name: str, full_name: str, caller_file: str, lang_ctx: JavaScriptResolverContext)` — [`L226`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/javascript.py#L226) — Resolve one JavaScript call edge.

## Module values
- `_BARE_CALLABLE_KINDS` — [`L189`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/javascript.py#L189)
- `_JS_DIALECTS` — [`L51`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/javascript.py#L51)
- `_dialect` — [`L310`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/javascript.py#L310)

