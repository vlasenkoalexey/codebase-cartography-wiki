---
title: 'Module: graphify/resolver_registry.py'
type: catalog
provenance: extracted
module: graphify/resolver_registry.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `graphify.resolver_registry`/
symbols:
  run_language_resolvers: run_language_resolvers().
  LanguageResolver: LanguageResolver#
  register: register().
  registered_resolvers: registered_resolvers().
  _REGISTRY._REGISTRY: _REGISTRY._REGISTRY.
  LanguageResolver.name: LanguageResolver#name.
  _LOG: _LOG.
  LanguageResolver.suffixes: LanguageResolver#suffixes.
  LanguageResolver.resolve: LanguageResolver#resolve.
---
# Module: [`graphify/resolver_registry.py`](../../../../../raw/code/graphify/graphify/resolver_registry.py)

## Classes
### `LanguageResolver`
- def: [`graphify/resolver_registry.py:29`](../../../../../raw/code/graphify/graphify/resolver_registry.py#L29)
- doc: One cross-file, language-specific resolution pass.
- signature: `class LanguageResolver:`
- members:
  - `name` — [`L38`](../../../../../raw/code/graphify/graphify/resolver_registry.py#L38)
  - `resolve` — [`L40`](../../../../../raw/code/graphify/graphify/resolver_registry.py#L40)
  - `suffixes` — [`L39`](../../../../../raw/code/graphify/graphify/resolver_registry.py#L39)
- used by: [`run_language_resolvers`](resolver_registry.md#run_language_resolvers), [`register`](resolver_registry.md#register), [`registered_resolvers`](resolver_registry.md#registered_resolvers), [`_REGISTRY`](resolver_registry.md#_REGISTRY._REGISTRY)  (4 test-only)

## Functions
- `register(resolver: LanguageResolver)` — [`L48`](../../../../../raw/code/graphify/graphify/resolver_registry.py#L48) — Append a resolver to the global registry and return it (for inline use).
- `registered_resolvers()` — [`L54`](../../../../../raw/code/graphify/graphify/resolver_registry.py#L54) — Return a copy of the registered resolvers, in registration order.
- `run_language_resolvers(paths: Sequence[Path], per_file: list[dict], all_nodes: list[dict], all_edges: list[dict], *, resolvers: Sequence[LanguageResolver] | None = None)` — [`L59`](../../../../../raw/code/graphify/graphify/resolver_registry.py#L59) — Run every resolver whose suffix appears in ``paths``.

## Module values
- `_LOG` — [`L25`](../../../../../raw/code/graphify/graphify/resolver_registry.py#L25)
- `_REGISTRY` — [`L45`](../../../../../raw/code/graphify/graphify/resolver_registry.py#L45)

