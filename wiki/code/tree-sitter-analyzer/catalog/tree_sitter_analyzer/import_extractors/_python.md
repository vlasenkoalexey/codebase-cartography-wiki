---
title: 'Module: tree_sitter_analyzer/import_extractors/_python.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/import_extractors/_python.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.import_extractors._python`/
symbols:
  extract_python_import_from: extract_python_import_from().
  extract_python_import_simple: extract_python_import_simple().
  _extract_python_imports: _extract_python_imports().
  _parse_python_from_children: _parse_python_from_children().
  _extract_import_names: _extract_import_names().
  _parse_relative_import: _parse_relative_import().
  _collect_aliased_import_names: _collect_aliased_import_names().
  _emit_python_from_import: _emit_python_from_import().
  _STDLIB_TOP_LEVEL: _STDLIB_TOP_LEVEL.
  _emit_relative_submodule_imports: _emit_relative_submodule_imports().
---
# Module: [`tree_sitter_analyzer/import_extractors/_python.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_extractors/_python.py)

## Functions
- `_collect_aliased_import_names(aliased_node: Any, source: str, names: list[str])` — [`L96`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_extractors/_python.py#L96) — Append identifiers from ``aliased_import`` (handles ``foo as bar``).
- `_emit_python_from_import(dots_prefix: str, module_name: str, imported_names: list[str], imports: list[dict[str, Any]])` — [`L170`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_extractors/_python.py#L170) — Emit a single entry for ``from <prefix>module import a, b`` shape.
- `_emit_relative_submodule_imports(dots_prefix: str, imported_names: list[str], imports: list[dict[str, Any]])` — [`L151`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_extractors/_python.py#L151) — Emit one entry per imported name for ``from . import a, b`` shape.
- `_extract_import_names(names_node: Any, source: str)` — [`L106`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_extractors/_python.py#L106) — Extract individual names from an import_list or aliased_import node.
- `_extract_python_imports(node: Any, source: str, imports: list[dict[str, Any]])` — [`L210`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_extractors/_python.py#L210) — Extract Python import statements.
- `_parse_python_from_children(node: Any, source: str)` — [`L122`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_extractors/_python.py#L122) — Walk an ``import_from_statement``'s children; return ``(module, dots, names)``.
- `_parse_relative_import(child: Any, source: str)` — [`L83`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_extractors/_python.py#L83) — Return (dots_prefix, module_name) from a ``relative_import`` node.
- `extract_python_import_from(node: Any, source: str, imports: list[dict[str, Any]])` — [`L193`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_extractors/_python.py#L193) — Handle: from [.][.]module import name1, name2
- `extract_python_import_simple(node: Any, source: str, imports: list[dict[str, Any]])` — [`L62`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_extractors/_python.py#L62) — Handle: import os, sys

## Module values
- `_STDLIB_TOP_LEVEL` — [`L7`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_extractors/_python.py#L7)

