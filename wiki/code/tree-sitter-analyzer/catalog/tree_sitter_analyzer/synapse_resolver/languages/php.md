---
title: 'Module: tree_sitter_analyzer/synapse_resolver/languages/php.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/synapse_resolver/languages/php.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.synapse_resolver.languages.php`/
symbols:
  resolve_php_callee: resolve_php_callee().
  build_php_context: build_php_context().
  _project_owns_function: _project_owns_function().
  PhpResolverContext: PhpResolverContext#
  _lookup_in_file: _lookup_in_file().
  _unique_class_method: _unique_class_method().
  _split_receiver: _split_receiver().
  _PHP_LANG: _PHP_LANG.
  PhpResolverContext.file_symbols: PhpResolverContext#file_symbols.
  PhpResolverContext.file_class_methods: PhpResolverContext#file_class_methods.
  PhpResolverContext.global_name_table: PhpResolverContext#global_name_table.
  PhpResolverContext.file_languages: PhpResolverContext#file_languages.
  _SELF_RECEIVERS: _SELF_RECEIVERS.
  _BARE_CALLABLE_KINDS: _BARE_CALLABLE_KINDS.
  _RECEIVER_SPLIT: _RECEIVER_SPLIT.
  __all__: __all__.
---
# Module: [`tree_sitter_analyzer/synapse_resolver/languages/php.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/php.py)

## Classes
### `PhpResolverContext`
- def: [`tree_sitter_analyzer/synapse_resolver/languages/php.py:75`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/php.py#L75)
- doc: Per-index PHP resolution maps (built once per pass).
- signature: `class PhpResolverContext:`
- members:
  - `file_class_methods` — [`L87`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/php.py#L87)
  - `file_languages` — [`L95`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/php.py#L95)
  - `file_symbols` — [`L85`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/php.py#L85)
  - `global_name_table` — [`L93`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/php.py#L93)
- used by: [`resolve_php_callee`](php.md#resolve_php_callee), [`build_php_context`](php.md#build_php_context), [`_project_owns_function`](php.md#_project_owns_function), [`_lookup_in_file`](php.md#_lookup_in_file), [`_unique_class_method`](php.md#_unique_class_method)  (2 test-only)

## Functions
- `_lookup_in_file(ctx: PhpResolverContext, file_path: str, simple: str)` — [`L150`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/php.py#L150) — Symbol id of a same-file BARE-CALLABLE named ``simple`` in ``file_path``.
- `_project_owns_function(ctx: PhpResolverContext, simple: str)` — [`L186`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/php.py#L186) — True when a SAME-LANGUAGE (PHP) project symbol named ``simple`` exists.
- `_split_receiver(callee_full: str, callee_name: str)` — [`L124`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/php.py#L124) — Return ``(receiver, simple_name, separator)`` from a PHP call's full name.
- `_unique_class_method(ctx: PhpResolverContext, file_path: str, simple: str)` — [`L165`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/php.py#L165) — Symbol id when EXACTLY ONE class in ``file_path`` defines ``simple``.
- `build_php_context(*, imports_by_file: dict[str, Any], file_languages: dict[str, str], file_symbols: dict[str, Any], global_name_table: dict[str, Any], file_class_methods: Any, **_ignored: Any)` — [`L98`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/php.py#L98) — Build the PHP context, or ``None`` when no PHP file is indexed.
- `resolve_php_callee(callee_name: str, callee_full: str, caller_file: str, lang_ctx: PhpResolverContext)` — [`L203`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/php.py#L203) — Resolve one PHP call edge.

## Module values
- `_BARE_CALLABLE_KINDS` — [`L63`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/php.py#L63)
- `_PHP_LANG` — [`L50`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/php.py#L50)
- `_RECEIVER_SPLIT` — [`L71`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/php.py#L71)
- `_SELF_RECEIVERS` — [`L57`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/php.py#L57)
- `__all__` — [`L260`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/php.py#L260)

