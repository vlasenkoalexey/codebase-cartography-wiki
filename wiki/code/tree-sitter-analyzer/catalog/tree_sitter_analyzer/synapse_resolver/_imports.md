---
title: 'Module: tree_sitter_analyzer/synapse_resolver/_imports.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/synapse_resolver/_imports.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.synapse_resolver._imports`/
symbols:
  _parse_python_imports: _parse_python_imports().
  ImportEntry.local_name: ImportEntry#local_name.
  ImportEntry: ImportEntry#
  ImportEntry.module_path: ImportEntry#module_path.
  parse_imports: parse_imports().
  ImportEntry.is_relative: ImportEntry#is_relative.
  ImportEntry.is_star: ImportEntry#is_star.
  ImportEntry.file_path: ImportEntry#file_path.
  ImportEntry.alias_of: ImportEntry#alias_of.
  ImportEntry.language: ImportEntry#language.
  ImportEntry.line: ImportEntry#line.
  _split_names_clause: _split_names_clause().
  _PY_FROM_IMPORT_RE: _PY_FROM_IMPORT_RE.
  _PY_IMPORT_RE: _PY_IMPORT_RE.
  __all__: __all__.
---
# Module: [`tree_sitter_analyzer/synapse_resolver/_imports.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_imports.py)

## Classes
### `ImportEntry`
- def: [`tree_sitter_analyzer/synapse_resolver/_imports.py:20`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_imports.py#L20)
- doc: One row in `ast_imports` — a single imported name binding.
- signature: `class ImportEntry:`
- members:
  - `alias_of` — [`L29`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_imports.py#L29)
  - `file_path` — [`L23`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_imports.py#L23)
  - `is_relative` — [`L27`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_imports.py#L27)
  - `is_star` — [`L28`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_imports.py#L28)
  - `language` — [`L24`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_imports.py#L24)
  - `line` — [`L30`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_imports.py#L30)
  - `local_name` — [`L26`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_imports.py#L26)
  - `module_path` — [`L25`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_imports.py#L25)
- used by: [`_build_resolver_context_uncached`](_context.md#_build_resolver_context_uncached), [`write_graph_edges_for_file`](../_ast_cache_write.md#write_graph_edges_for_file), [`build_java_context`](_java.md#build_java_context), [`parse_java_imports`](_java.md#parse_java_imports), [`_parse_python_imports`](_imports.md#_parse_python_imports), [`_build_import_maps`](_context.md#_build_import_maps), [`_try_stdlib`](__init__.md#_try_stdlib), [`parse_imports`](_imports.md#parse_imports), [`_python_import_modules`](../mcp/tools/utils/change_impact_cached_graph.md#_python_import_modules), [`imports_by_file`](_context.md#ResolverContext.imports_by_file), [`__init__`](_context.md#ResolverContext.__init__)  (7 test-only)

## Functions
- `_parse_python_imports(text: str, file_path: str = "", line: int = 0)` — [`L72`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_imports.py#L72) — Parse one Python import statement into structured rows.
- `_split_names_clause(clause: str)` — [`L33`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_imports.py#L33) — Parse ``"a, b as c, *"`` into ``[(local_name, alias_of), ...]``.
- `parse_imports(text: str, language: str, file_path: str = "", line: int = 0)` — [`L53`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_imports.py#L53) — Parse one import statement into structured rows (language dispatch).

## Module values
- `_PY_FROM_IMPORT_RE` — [`L13`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_imports.py#L13)
- `_PY_IMPORT_RE` — [`L16`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_imports.py#L16)
- `__all__` — [`L155`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_imports.py#L155)

