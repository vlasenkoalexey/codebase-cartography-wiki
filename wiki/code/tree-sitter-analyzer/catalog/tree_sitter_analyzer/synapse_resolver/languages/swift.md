---
title: 'Module: tree_sitter_analyzer/synapse_resolver/languages/swift.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/synapse_resolver/languages/swift.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.synapse_resolver.languages.swift`/
symbols:
  resolve_swift_callee: resolve_swift_callee().
  SwiftResolverContext: SwiftResolverContext#
  _project_owns: _project_owns().
  build_swift_resolver_context: build_swift_resolver_context().
  _lookup_in_file: _lookup_in_file().
  _lookup_unique_method_in_file: _lookup_unique_method_in_file().
  SwiftResolverContext.__init__: SwiftResolverContext#__init__().
  _SELF_RECEIVERS: _SELF_RECEIVERS.
  _split_receiver: _split_receiver().
  SwiftResolverContext.__slots__: SwiftResolverContext#__slots__.
  __all__: __all__.
---
# Module: [`tree_sitter_analyzer/synapse_resolver/languages/swift.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/swift.py)

## Classes
### `SwiftResolverContext`
- def: [`tree_sitter_analyzer/synapse_resolver/languages/swift.py:31`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/swift.py#L31)
- doc: Per-index Swift resolution maps (built once per pass).
- signature: `class SwiftResolverContext:`
- protocol/private: `__init__`[`L41`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/swift.py#L41), `__slots__`[`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/swift.py#L39)
- used by: [`resolve_swift_callee`](swift.md#resolve_swift_callee), [`_project_owns`](swift.md#_project_owns), [`_lookup_in_file`](swift.md#_lookup_in_file), [`_lookup_unique_method_in_file`](swift.md#_lookup_unique_method_in_file), [`build_swift_resolver_context`](swift.md#build_swift_resolver_context)  (1 test-only)

## Functions
- `_lookup_in_file(ctx: SwiftResolverContext, file_path: str, simple: str)` — [`L90`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/swift.py#L90) — Return the symbol id of a same-file ``simple`` def, or ``None``.
- `_lookup_unique_method_in_file(ctx: SwiftResolverContext, file_path: str, simple: str)` — [`L100`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/swift.py#L100) — Return the symbol id of a same-file ``simple`` METHOD def, but ONLY when it
- `_project_owns(ctx: SwiftResolverContext, simple: str)` — [`L118`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/swift.py#L118) — True when a COMPATIBLE-LANGUAGE (Swift) project symbol named ``simple``
- `_split_receiver(callee_full: str, callee_name: str)` — [`L77`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/swift.py#L77) — Return ``(receiver, simple_name)`` from a Swift call's full name.
- `build_swift_resolver_context(*, imports_by_file: dict[str, Any], file_languages: dict[str, str], file_symbols: dict[str, Any], global_name_table: dict[str, Any], file_class_methods: Any, **_ignored: Any)` — [`L53`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/swift.py#L53) — Build the Swift context, or ``None`` when no Swift file is indexed.
- `resolve_swift_callee(callee_name: str, callee_full: str, caller_file: str, ctx: SwiftResolverContext)` — [`L135`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/swift.py#L135) — Resolve one Swift call edge.

## Module values
- `_SELF_RECEIVERS` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/swift.py#L28)
- `__all__` — [`L183`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/swift.py#L183)

