---
title: 'Module: tree_sitter_analyzer/synapse_resolver/languages/c.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/synapse_resolver/languages/c.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.synapse_resolver.languages.c`/
symbols:
  resolve_c_callee: resolve_c_callee().
  build_c_context: build_c_context().
  _project_owns: _project_owns().
  CResolverContext: CResolverContext#
  _lookup_in_file: _lookup_in_file().
  __all__: __all__.
  CResolverContext.file_languages: CResolverContext#file_languages.
  _has_receiver: _has_receiver().
  CResolverContext.global_name_table: CResolverContext#global_name_table.
  CResolverContext.file_symbols: CResolverContext#file_symbols.
  _C_LANGS._C_LANGS: _C_LANGS._C_LANGS.
  _ACCESS_OPERATORS._ACCESS_OPERATORS: _ACCESS_OPERATORS._ACCESS_OPERATORS.
  _LOCAL_KINDS._LOCAL_KINDS: _LOCAL_KINDS._LOCAL_KINDS.
---
# Module: [`tree_sitter_analyzer/synapse_resolver/languages/c.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/c.py)

## Classes
### `CResolverContext`
- def: [`tree_sitter_analyzer/synapse_resolver/languages/c.py:77`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/c.py#L77)
- doc: Per-index C resolution maps (built once per pass).
- signature: `class CResolverContext:`
- members:
  - `file_languages` — [`L91`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/c.py#L91)
  - `file_symbols` — [`L86`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/c.py#L86)
  - `global_name_table` — [`L88`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/c.py#L88)
- used by: [`resolve_c_callee`](c.md#resolve_c_callee), [`build_c_context`](c.md#build_c_context), [`_project_owns`](c.md#_project_owns), [`_lookup_in_file`](c.md#_lookup_in_file)  (3 test-only)

## Functions
- `_has_receiver(callee_full: str, callee_name: str)` — [`L119`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/c.py#L119) — True when the call carries a struct-field / pointer access operator.
- `_lookup_in_file(ctx: CResolverContext, file_path: str, simple: str)` — [`L136`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/c.py#L136) — Resolve ``simple`` to a same-file free ``function`` symbol, or ``None``.
- `_project_owns(ctx: CResolverContext, simple: str)` — [`L148`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/c.py#L148) — True when a COMPATIBLE-LANGUAGE project symbol of name ``simple`` exists.
- `build_c_context(*, imports_by_file: dict[str, Any], file_languages: dict[str, str], file_symbols: dict[str, Any], global_name_table: dict[str, Any], file_class_methods: Callable[[], dict[str, Any]], **_ignored: Any)` — [`L94`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/c.py#L94) — Build the C context, or ``None`` when no C file is indexed.
- `resolve_c_callee(callee_name: str, callee_full: str, caller_file: str, ctx: CResolverContext)` — [`L164`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/c.py#L164) — Resolve one C call edge.

## Module values
- `_ACCESS_OPERATORS` — [`L73`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/c.py#L73)
- `_C_LANGS` — [`L68`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/c.py#L68)
- `_LOCAL_KINDS` — [`L133`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/c.py#L133)
- `__all__` — [`L213`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/c.py#L213)

