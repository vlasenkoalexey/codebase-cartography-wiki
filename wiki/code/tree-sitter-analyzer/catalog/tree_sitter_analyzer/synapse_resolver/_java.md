---
title: 'Module: tree_sitter_analyzer/synapse_resolver/_java.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/synapse_resolver/_java.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.synapse_resolver._java`/
symbols:
  resolve_java_callee: resolve_java_callee().
  parse_java_imports: parse_java_imports().
  build_java_context: build_java_context().
  _project_owns: _project_owns().
  _lookup_in_file: _lookup_in_file().
  JavaResolverContext: JavaResolverContext#
  JavaResolverContext.fqn_to_file: JavaResolverContext#fqn_to_file.
  JavaResolverContext.file_package: JavaResolverContext#file_package.
  JavaResolverContext.global_name_table: JavaResolverContext#global_name_table.
  _PACKAGE_MARKER: _PACKAGE_MARKER.
  JavaResolverContext.simple_to_fqn_by_file: JavaResolverContext#simple_to_fqn_by_file.
  JavaResolverContext.static_imports_by_file: JavaResolverContext#static_imports_by_file.
  JavaResolverContext.wildcard_pkgs_by_file: JavaResolverContext#wildcard_pkgs_by_file.
  JavaResolverContext.file_class_methods: JavaResolverContext#file_class_methods.
  JavaResolverContext.file_symbols: JavaResolverContext#file_symbols.
  JavaResolverContext.file_languages: JavaResolverContext#file_languages.
  _PKG_RE: _PKG_RE.
  _IMPORT_RE: _IMPORT_RE.
  JavaResolverContext.package_to_files: JavaResolverContext#package_to_files.
  _split_receiver: _split_receiver().
  __all__: __all__.
---
# Module: [`tree_sitter_analyzer/synapse_resolver/_java.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_java.py)

## Classes
### `JavaResolverContext`
- def: [`tree_sitter_analyzer/synapse_resolver/_java.py:124`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_java.py#L124)
- doc: Per-index Java resolution maps (built once per pass).
- signature: `class JavaResolverContext:`
- members:
  - `file_class_methods` — [`L143`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_java.py#L143)
  - `file_languages` — [`L152`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_java.py#L152)
  - `file_package` — [`L141`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_java.py#L141)
  - `file_symbols` — [`L147`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_java.py#L147)
  - `fqn_to_file` — [`L133`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_java.py#L133)
  - `global_name_table` — [`L149`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_java.py#L149)
  - `package_to_files` — [`L131`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_java.py#L131)
  - `simple_to_fqn_by_file` — [`L135`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_java.py#L135)
  - `static_imports_by_file` — [`L137`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_java.py#L137)
  - `wildcard_pkgs_by_file` — [`L139`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_java.py#L139)
- used by: [`resolve_java_callee`](_java.md#resolve_java_callee), [`build_java_context`](_java.md#build_java_context), [`_project_owns`](_java.md#_project_owns), [`_lookup_in_file`](_java.md#_lookup_in_file)  (1 test-only)

## Functions
- `_lookup_in_file(ctx: JavaResolverContext, file_path: str, simple: str)` — [`L223`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_java.py#L223)
- `_project_owns(ctx: JavaResolverContext, simple: str)` — [`L361`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_java.py#L361) — True when a COMPATIBLE-LANGUAGE (Java) project symbol of name ``simple``
- `_split_receiver(callee_full: str, callee_name: str)` — [`L214`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_java.py#L214) — Return ``(receiver, simple_name)`` from a Java call's full name.
- `build_java_context(imports_by_file: dict[str, list[ImportEntry]], file_symbols: dict[str, list[tuple[str, str, int]]], file_class_methods: dict[str, dict[str, dict[str, int]]], global_name_table: dict[str, list[tuple[str, int]]], file_languages: dict[str, str] | None = None)` — [`L155`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_java.py#L155) — Assemble the Java resolution maps from already-loaded cache data.
- `parse_java_imports(text: str, file_path: str = "", line: int = 0)` — [`L48`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_java.py#L48) — Parse one Java ``import`` / ``package`` statement into rows.
- `resolve_java_callee(callee_name: str, callee_full: str, caller_file: str, ctx: JavaResolverContext)` — [`L232`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_java.py#L232) — Resolve one Java call edge per the 10-stage cascade.

## Module values
- `_IMPORT_RE` — [`L40`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_java.py#L40)
- `_PACKAGE_MARKER` — [`L45`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_java.py#L45)
- `_PKG_RE` — [`L38`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_java.py#L38)
- `__all__` — [`L386`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/_java.py#L386)

