---
title: 'Module: tree_sitter_analyzer/synapse_resolver/languages/go.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/synapse_resolver/languages/go.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.synapse_resolver.languages.go`/
symbols:
  resolve_go_callee: resolve_go_callee().
  build_go_resolver_context: build_go_resolver_context().
  GoResolverContext: GoResolverContext#
  _lookup_in_file: _lookup_in_file().
  GoResolverContext.file_symbols: GoResolverContext#file_symbols.
  GoResolverContext.project_names: GoResolverContext#project_names.
  GoResolverContext.imported_stdlib_by_file: GoResolverContext#imported_stdlib_by_file.
  _go_import_blocks_from_conn: _go_import_blocks_from_conn().
  _split_receiver: _split_receiver().
  __all__: __all__.
---
# Module: [`tree_sitter_analyzer/synapse_resolver/languages/go.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/go.py)

## Classes
### `GoResolverContext`
- def: [`tree_sitter_analyzer/synapse_resolver/languages/go.py:39`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/go.py#L39)
- doc: Per-index Go resolution maps (built once per pass).
- signature: `class GoResolverContext:`
- members:
  - `file_symbols` — [`L47`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/go.py#L47)
  - `imported_stdlib_by_file` — [`L58`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/go.py#L58)
  - `project_names` — [`L50`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/go.py#L50)
- used by: [`resolve_go_callee`](go.md#resolve_go_callee), [`build_go_resolver_context`](go.md#build_go_resolver_context), [`_lookup_in_file`](go.md#_lookup_in_file)  (2 test-only)

## Functions
- `_go_import_blocks_from_conn(conn: Any, file_languages: dict[str, str])` — [`L61`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/go.py#L61) — Read each Go file's raw ``import`` text from the AST cache.
- `_lookup_in_file(ctx: GoResolverContext, file_path: str, simple: str)` — [`L162`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/go.py#L162) — Find a same-file symbol id for ``simple`` in ``file_path`` only.
- `_split_receiver(callee_full: str, callee_name: str)` — [`L147`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/go.py#L147) — Return ``(qualifier, simple_name)`` from a Go call's full name.
- `build_go_resolver_context(*, imports_by_file: dict[str, Any], file_languages: dict[str, str], file_symbols: dict[str, Any], global_name_table: dict[str, Any], file_class_methods: Any, conn: Any = None, go_import_blocks: dict[str, str] | None = None, **_ignored: Any)` — [`L90`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/go.py#L90) — Build the Go context, or ``None`` when no Go file is indexed.
- `resolve_go_callee(callee_name: str, callee_full: str, caller_file: str, ctx: GoResolverContext)` — [`L170`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/go.py#L170) — Resolve one Go call edge.

## Module values
- `__all__` — [`L218`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/go.py#L218)

