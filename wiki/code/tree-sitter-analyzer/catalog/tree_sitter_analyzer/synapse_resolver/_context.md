---
title: 'Module: tree_sitter_analyzer/synapse_resolver/_context.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/synapse_resolver/_context.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.synapse_resolver._context`/
symbols:
  ResolverContext._ensure_loaded: ResolverContext#_ensure_loaded().
  ResolverContext: ResolverContext#
  _build_resolver_context_uncached: _build_resolver_context_uncached().
  build_resolver_context: build_resolver_context().
  ResolverContext.callee_resolver: ResolverContext#callee_resolver().
  _build_import_maps: _build_import_maps().
  ResolverContext.file_class_methods: ResolverContext#file_class_methods().
  ResolverContext.file_languages: ResolverContext#file_languages().
  ResolverContext.file_symbols: ResolverContext#file_symbols().
  ResolverContext._loaded: ResolverContext#_loaded.
  ResolverContext.imports_by_file: ResolverContext#imports_by_file().
  ResolverContext.lang_context: ResolverContext#lang_context().
  clear_resolver_context_cache: clear_resolver_context_cache().
  ResolverContext.name_to_source: ResolverContext#name_to_source().
  ResolverContext.import_alias_target: ResolverContext#import_alias_target().
  ResolverContext.builtins: ResolverContext#builtins().
  ResolverContext.stdlib_modules: ResolverContext#stdlib_modules().
  is_enabled: is_enabled().
  _build_file_class_methods_from_cache: _build_file_class_methods_from_cache().
  _CONTEXT_CACHE._CONTEXT_CACHE: _CONTEXT_CACHE._CONTEXT_CACHE.
  ResolverContext._file_class_methods_loaded: ResolverContext#_file_class_methods_loaded.
  ResolverContext.global_name_table: ResolverContext#global_name_table().
  ResolverContext.stdlib_methods: ResolverContext#stdlib_methods().
  _build_module_to_file: _build_module_to_file().
  ResolverContext.__init__: ResolverContext#__init__().
  ResolverContext.external_methods: ResolverContext#external_methods().
  ResolverContext.builtin_methods: ResolverContext#builtin_methods().
  ResolverContext._lang_contexts: ResolverContext#_lang_contexts.
  _resolve_relative_module: _resolve_relative_module().
  _resolve_absolute_module: _resolve_absolute_module().
  _resolve_module_to_file: _resolve_module_to_file().
  ResolverContext._file_symbols: ResolverContext#_file_symbols.
  ResolverContext._file_class_methods: ResolverContext#_file_class_methods.
  ResolverContext.cache: ResolverContext#cache.
  _cache_identity: _cache_identity().
  _build_resolver_context_uncached._file_class_methods_thunk: _build_resolver_context_uncached()._file_class_methods_thunk().
  _build_callee_resolver: _build_callee_resolver().
  ResolverContext._name_to_source: ResolverContext#_name_to_source.
  ResolverContext._global_name_table: ResolverContext#_global_name_table.
  ResolverContext._import_alias_target: ResolverContext#_import_alias_target.
  ResolverContext._imports_by_file: ResolverContext#_imports_by_file.
  ResolverContext._builtins: ResolverContext#_builtins.
  ResolverContext._stdlib_modules: ResolverContext#_stdlib_modules.
  ResolverContext._callee_resolver: ResolverContext#_callee_resolver.
  ResolverContext._file_languages: ResolverContext#_file_languages.
  ResolverContext._external_methods: ResolverContext#_external_methods.
  ResolverContext._builtin_methods: ResolverContext#_builtin_methods.
  ResolverContext.java_context: ResolverContext#java_context().
  ResolverContext._stdlib_methods: ResolverContext#_stdlib_methods.
  _build_file_class_methods: _build_file_class_methods().
  ResolverContext.project_root: ResolverContext#project_root.
  _CONTEXT_CACHE_MAX: _CONTEXT_CACHE_MAX.
  _local_name_as_submodule: _local_name_as_submodule().
  __all__: __all__.
---
# Module: [`tree_sitter_analyzer/synapse_resolver/_context.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_context.py)

## Classes
### `ResolverContext`
- def: [`tree_sitter_analyzer/synapse_resolver/_context.py:25`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_context.py#L25)
- members:
  - `builtin_methods(self)` — [`L167`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_context.py#L167)
  - `builtins(self)` — [`L147`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_context.py#L147)
  - `callee_resolver(self)` — [`L172`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_context.py#L172)
  - `external_methods(self)` — [`L162`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_context.py#L162)
  - `file_class_methods(self)` — [`L124`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_context.py#L124)
  - `file_languages(self)` — [`L100`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_context.py#L100)
  - `file_symbols(self)` — [`L114`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_context.py#L114)
  - `global_name_table(self)` — [`L132`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_context.py#L132)
  - `import_alias_target(self)` — [`L137`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_context.py#L137)
  - `imports_by_file(self)` — [`L142`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_context.py#L142)
  - `java_context(self)` — [`L105`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_context.py#L105)
  - `lang_context(self, language: str)` — [`L108`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_context.py#L108) — Return the per-language resolver context for ``language`` (RFC-0010).
  - `name_to_source(self)` — [`L119`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_context.py#L119)
  - `stdlib_methods(self)` — [`L157`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_context.py#L157)
  - `stdlib_modules(self)` — [`L152`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_context.py#L152)
  - `cache` — [`L61`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_context.py#L61)
  - `project_root` — [`L60`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_context.py#L60)
- protocol/private: `__init__`[`L39`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_context.py#L39), `_builtin_methods`[`L80`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_context.py#L80), `_builtins`[`L76`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_context.py#L76), `_callee_resolver`[`L81`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_context.py#L81), `_ensure_loaded`[`L176`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_context.py#L176), `_external_methods`[`L79`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_context.py#L79), `_file_class_methods`[`L71`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_context.py#L71), `_file_class_methods_loaded`[`L72`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_context.py#L72), `_file_languages`[`L62`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_context.py#L62), `_file_symbols`[`L69`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_context.py#L69), `_global_name_table`[`L73`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_context.py#L73), `_import_alias_target`[`L74`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_context.py#L74), `_imports_by_file`[`L75`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_context.py#L75), `_lang_contexts`[`L66`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_context.py#L66), `_loaded`[`L82`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_context.py#L82), `_name_to_source`[`L70`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_context.py#L70), `_stdlib_methods`[`L78`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_context.py#L78), `_stdlib_modules`[`L77`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_context.py#L77)
- uses (calls/refs, reference-scoped): [`ASTCache`](../ast_cache.md#ASTCache), [`build_resolver_context`](_context.md#build_resolver_context), [`CalleeResolver`](../callee_resolution.md#CalleeResolver), [`ImportEntry`](_imports.md#ImportEntry), [`_build_file_class_methods_from_cache`](_context.md#_build_file_class_methods_from_cache)
- used by: [`_build_resolver_context_uncached`](_context.md#_build_resolver_context_uncached), [`resolve_callee`](__init__.md#resolve_callee), [`_resolve_callee_python`](__init__.md#_resolve_callee_python), [`build_resolver_context`](_context.md#build_resolver_context), [`_try_stdlib_method`](__init__.md#_try_stdlib_method), [`_try_import`](__init__.md#_try_import), [`_try_builtin_method`](__init__.md#_try_builtin_method), [`_try_external_method`](__init__.md#_try_external_method), [`_try_local`](__init__.md#_try_local), [`_try_single_global`](__init__.md#_try_single_global), [`_try_stdlib`](__init__.md#_try_stdlib), [`_is_cross_language`](__init__.md#_is_cross_language), [`_try_unique_method`](__init__.md#_try_unique_method), [`_lookup_symbol_id`](__init__.md#_lookup_symbol_id), [`_table_language`](__init__.md#_table_language), [`_CONTEXT_CACHE`](_context.md#_CONTEXT_CACHE._CONTEXT_CACHE), [`_try_builtin`](__init__.md#_try_builtin), [`_try_class_method`](__init__.md#_try_class_method), [`_try_self_method`](__init__.md#_try_self_method)  (50 test-only)

## Functions
- `_build_callee_resolver(*, file_symbols: dict[str, list[tuple[str, str, int]]], global_name_table: dict[str, list[tuple[str, int]]], name_to_source: dict[str, dict[str, str]], alias_target: dict[str, dict[str, str]])` — [`L570`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_context.py#L570)
- `_build_file_class_methods(conn: Any, line_idx: dict[tuple[str, str, int], int])` — [`L333`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_context.py#L333) — Pull class→method maps from ``symbols_json``.
- `_build_file_class_methods_from_cache(cache: ASTCache)` — [`L368`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_context.py#L368)
- `_build_import_maps(imports_by_file: dict[str, list[ImportEntry]], module_to_file: dict[str, str])` — [`L384`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_context.py#L384) — Derive (name_to_source, alias_target) from per-file import entries.
- `_build_module_to_file(file_paths: list[str])` — [`L217`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_context.py#L217) — Map every indexed Python file to its module-dotted-name.
- `_build_resolver_context_uncached(cache: ASTCache)` — [`L452`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_context.py#L452) — One DB pass; populates every map the resolver needs.
- `_cache_identity(cache: ASTCache)` — [`L427`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_context.py#L427)
- `_file_class_methods_thunk()` — [`L523`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_context.py#L523)
- `_local_name_as_submodule(local_name: str, alias_of: str, module_path: str, caller_file: str, module_to_file: dict[str, str])` — [`L285`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_context.py#L285) — For ``from <pkg> import <name>``, check if ``<name>`` is itself a
- `_resolve_absolute_module(module_path: str, module_to_file: dict[str, str])` — [`L263`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_context.py#L263)
- `_resolve_module_to_file(module_path: str, is_relative: bool, caller_file: str, module_to_file: dict[str, str])` — [`L274`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_context.py#L274)
- `_resolve_relative_module(module_path: str, caller_file: str, module_to_file: dict[str, str])` — [`L231`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_context.py#L231) — Resolve a relative ``.x.y`` import to a concrete file path.
- `build_resolver_context(cache: ASTCache)` — [`L438`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_context.py#L438) — Return a loaded resolver context, reusing recent cache snapshots.
- `clear_resolver_context_cache()` — [`L205`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_context.py#L205)
- `is_enabled()` — [`L209`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_context.py#L209) — ``TSA_SYNAPSE=0`` disables; anything else enables.

## Module values
- `_CONTEXT_CACHE` — [`L202`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_context.py#L202)
- `_CONTEXT_CACHE_MAX` — [`L201`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_context.py#L201)
- `__all__` — [`L615`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_context.py#L615)

