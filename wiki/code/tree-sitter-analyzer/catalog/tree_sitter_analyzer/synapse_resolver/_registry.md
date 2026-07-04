---
title: 'Module: tree_sitter_analyzer/synapse_resolver/_registry.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/synapse_resolver/_registry.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.synapse_resolver._registry`/
symbols:
  register_language: register_language().
  get_language_resolver: get_language_resolver().
  registered_languages: registered_languages().
  _REGISTRY._REGISTRY: _REGISTRY._REGISTRY.
  ResolveCalleeFn: ResolveCalleeFn.
  LanguageResolver.build_context: LanguageResolver#build_context.
  LanguageResolver.resolve_callee: LanguageResolver#resolve_callee.
  LanguageResolver: LanguageResolver#
  LanguageResolver.language: LanguageResolver#language.
  BuildContextFn: BuildContextFn.
  ResolveResult: ResolveResult.
---
# Module: [`tree_sitter_analyzer/synapse_resolver/_registry.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_registry.py)

## Classes
### `LanguageResolver`  ·  implements/extends NamedTuple
- def: [`tree_sitter_analyzer/synapse_resolver/_registry.py:33`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_registry.py#L33)
- doc: One registered language's build + resolve hooks.
- signature: `class LanguageResolver(NamedTuple):`
- members:
  - `build_context` — [`L37`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_registry.py#L37)
  - `language` — [`L36`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_registry.py#L36)
  - `resolve_callee` — [`L38`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_registry.py#L38)
- uses (calls/refs, reference-scoped): [`ResolveCalleeFn`](_registry.md#ResolveCalleeFn), [`BuildContextFn`](_registry.md#BuildContextFn)
- used by: [`_build_resolver_context_uncached`](_context.md#_build_resolver_context_uncached), [`resolve_callee`](__init__.md#resolve_callee), [`register_language`](_registry.md#register_language), [`get_language_resolver`](_registry.md#get_language_resolver), [`_REGISTRY`](_registry.md#_REGISTRY._REGISTRY)  (3 test-only)

## Functions
- `get_language_resolver(language: str | None)` — [`L53`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_registry.py#L53) — Return the registered resolver for ``language``, or ``None``.
- `register_language(language: str, build_context: BuildContextFn, resolve_callee: ResolveCalleeFn)` — [`L44`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_registry.py#L44) — Register (or replace) the resolver hooks for ``language``.
- `registered_languages()` — [`L60`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_registry.py#L60) — Return the list of registered language names (registration order).

## Module values
- `BuildContextFn` — [`L29`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_registry.py#L29)
- `ResolveCalleeFn` — [`L30`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_registry.py#L30)
- `ResolveResult` — [`L27`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_registry.py#L27)
- `_REGISTRY` — [`L41`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_registry.py#L41)

