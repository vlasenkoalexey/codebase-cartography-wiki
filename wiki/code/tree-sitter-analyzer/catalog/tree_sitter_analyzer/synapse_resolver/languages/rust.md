---
title: 'Module: tree_sitter_analyzer/synapse_resolver/languages/rust.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/synapse_resolver/languages/rust.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.synapse_resolver.languages.rust`/
symbols:
  resolve_rust_callee: resolve_rust_callee().
  RustResolverContext: RustResolverContext#
  build_rust_resolver_context: build_rust_resolver_context().
  _project_owns: _project_owns().
  _lookup_in_file: _lookup_in_file().
  _lookup_unique_method_in_file: _lookup_unique_method_in_file().
  RustResolverContext.__init__: RustResolverContext#__init__().
  _split_receiver: _split_receiver().
  RustResolverContext.__slots__: RustResolverContext#__slots__.
  __all__: __all__.
---
# Module: [`tree_sitter_analyzer/synapse_resolver/languages/rust.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/rust.py)

## Classes
### `RustResolverContext`
- def: [`tree_sitter_analyzer/synapse_resolver/languages/rust.py:36`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/rust.py#L36)
- doc: Per-index Rust resolution maps (built once per pass).
- signature: `class RustResolverContext:`
- protocol/private: `__init__`[`L46`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/rust.py#L46), `__slots__`[`L44`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/rust.py#L44)
- used by: [`resolve_rust_callee`](rust.md#resolve_rust_callee), [`build_rust_resolver_context`](rust.md#build_rust_resolver_context), [`_project_owns`](rust.md#_project_owns), [`_lookup_in_file`](rust.md#_lookup_in_file), [`_lookup_unique_method_in_file`](rust.md#_lookup_unique_method_in_file)

## Functions
- `_lookup_in_file(ctx: RustResolverContext, file_path: str, simple: str)` — [`L106`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/rust.py#L106) — Return the symbol id of a same-file ``simple`` def, or ``None``.
- `_lookup_unique_method_in_file(ctx: RustResolverContext, file_path: str, simple: str)` — [`L116`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/rust.py#L116) — Return the symbol id of a same-file ``simple`` METHOD def, but ONLY when
- `_project_owns(ctx: RustResolverContext, simple: str)` — [`L150`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/rust.py#L150) — True when a COMPATIBLE-LANGUAGE (Rust) project symbol of name ``simple``
- `_split_receiver(callee_full: str, callee_name: str)` — [`L88`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/rust.py#L88) — Return ``(receiver, simple_name)`` from a Rust call's full name.
- `build_rust_resolver_context(*, imports_by_file: dict[str, Any], file_languages: dict[str, str], file_symbols: dict[str, Any], global_name_table: dict[str, Any], file_class_methods: Any, **_ignored: Any)` — [`L63`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/rust.py#L63) — Build the Rust context, or ``None`` when no Rust file is indexed.
- `resolve_rust_callee(callee_name: str, callee_full: str, caller_file: str, ctx: RustResolverContext)` — [`L171`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/rust.py#L171) — Resolve one Rust call edge.

## Module values
- `__all__` — [`L233`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/rust.py#L233)

