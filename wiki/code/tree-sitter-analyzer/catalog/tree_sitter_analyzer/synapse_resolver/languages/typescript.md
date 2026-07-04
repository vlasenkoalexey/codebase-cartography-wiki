---
title: 'Module: tree_sitter_analyzer/synapse_resolver/languages/typescript.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/synapse_resolver/languages/typescript.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.synapse_resolver.languages.typescript`/
symbols:
  resolve_typescript_callee: resolve_typescript_callee().
  build_typescript_resolver_context: build_typescript_resolver_context().
  _project_owns: _project_owns().
  _import_binding_names: _import_binding_names().
  TypeScriptResolverContext: TypeScriptResolverContext#
  _lookup_in_file: _lookup_in_file().
  _unique_class_method: _unique_class_method().
  _build_shadow_locals: _build_shadow_locals().
  _TYPESCRIPT_LANG: _TYPESCRIPT_LANG.
  TypeScriptResolverContext.file_symbols: TypeScriptResolverContext#file_symbols.
  TypeScriptResolverContext.file_class_methods: TypeScriptResolverContext#file_class_methods.
  TypeScriptResolverContext.global_name_table: TypeScriptResolverContext#global_name_table.
  TypeScriptResolverContext.file_languages: TypeScriptResolverContext#file_languages.
  TypeScriptResolverContext.shadow_locals: TypeScriptResolverContext#shadow_locals.
  _SELF_RECEIVERS: _SELF_RECEIVERS.
  _IMPORT_DEFAULT_RE: _IMPORT_DEFAULT_RE.
  _IMPORT_NAMESPACE_RE: _IMPORT_NAMESPACE_RE.
  _IMPORT_NAMED_BLOCK_RE: _IMPORT_NAMED_BLOCK_RE.
  _IMPORT_NAMED_ITEM_RE: _IMPORT_NAMED_ITEM_RE.
  _split_receiver: _split_receiver().
  __all__: __all__.
---
# Module: [`tree_sitter_analyzer/synapse_resolver/languages/typescript.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/typescript.py)

## Classes
### `TypeScriptResolverContext`
- def: [`tree_sitter_analyzer/synapse_resolver/languages/typescript.py:44`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/typescript.py#L44)
- doc: Per-index TypeScript resolution maps (built once per pass).
- signature: `class TypeScriptResolverContext:`
- members:
  - `file_class_methods` — [`L54`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/typescript.py#L54)
  - `file_languages` — [`L60`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/typescript.py#L60)
  - `file_symbols` — [`L52`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/typescript.py#L52)
  - `global_name_table` — [`L58`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/typescript.py#L58)
  - `shadow_locals` — [`L66`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/typescript.py#L66)
- used by: [`resolve_typescript_callee`](typescript.md#resolve_typescript_callee), [`build_typescript_resolver_context`](typescript.md#build_typescript_resolver_context), [`_project_owns`](typescript.md#_project_owns), [`_lookup_in_file`](typescript.md#_lookup_in_file), [`_unique_class_method`](typescript.md#_unique_class_method)

## Functions
- `_build_shadow_locals(conn: Any)` — [`L104`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/typescript.py#L104) — Build file -> {variable / import binding names} for every TS file.
- `_import_binding_names(statement: str)` — [`L81`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/typescript.py#L81) — Extract the local binding names introduced by one TS ``import`` line.
- `_lookup_in_file(ctx: TypeScriptResolverContext, file_path: str, simple: str)` — [`L185`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/typescript.py#L185)
- `_project_owns(ctx: TypeScriptResolverContext, simple: str, caller_file: str)` — [`L216`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/typescript.py#L216) — True when a COMPATIBLE-LANGUAGE (TS/JS-family) project symbol named
- `_split_receiver(callee_full: str, callee_name: str)` — [`L176`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/typescript.py#L176) — Return ``(receiver, simple_name)`` from a TS call's full name.
- `_unique_class_method(ctx: TypeScriptResolverContext, file_path: str, simple: str)` — [`L194`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/typescript.py#L194) — Return the symbol id when EXACTLY ONE class in ``file_path`` defines a
- `build_typescript_resolver_context(*, imports_by_file: dict[str, Any], file_languages: dict[str, str], file_symbols: dict[str, Any], global_name_table: dict[str, Any], file_class_methods: Any, conn: Any = None, shadow_locals: dict[str, set[str]] | None = None, **_ignored: Any)` — [`L143`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/typescript.py#L143) — Build the TS context, or ``None`` when no TypeScript file is indexed.
- `resolve_typescript_callee(callee_name: str, callee_full: str, caller_file: str, ctx: TypeScriptResolverContext)` — [`L245`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/typescript.py#L245) — Resolve one TypeScript call edge.

## Module values
- `_IMPORT_DEFAULT_RE` — [`L73`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/typescript.py#L73)
- `_IMPORT_NAMED_BLOCK_RE` — [`L75`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/typescript.py#L75)
- `_IMPORT_NAMED_ITEM_RE` — [`L76`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/typescript.py#L76)
- `_IMPORT_NAMESPACE_RE` — [`L74`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/typescript.py#L74)
- `_SELF_RECEIVERS` — [`L40`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/typescript.py#L40)
- `_TYPESCRIPT_LANG` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/typescript.py#L35)
- `__all__` — [`L305`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/typescript.py#L305)

