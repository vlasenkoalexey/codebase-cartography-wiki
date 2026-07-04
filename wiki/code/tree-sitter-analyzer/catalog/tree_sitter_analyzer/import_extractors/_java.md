---
title: 'Module: tree_sitter_analyzer/import_extractors/_java.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/import_extractors/_java.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.import_extractors._java`/_
symbols:
  _extract_java_imports: extract_java_imports().
  _is_java_stdlib_path: is_java_stdlib_path().
  _strip_java_import_keywords: strip_java_import_keywords().
  _JAVA_STD_ROOTS._JAVA_STD_ROOTS: JAVA_STD_ROOTS._JAVA_STD_ROOTS.
---
# Module: [`tree_sitter_analyzer/import_extractors/_java.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_extractors/_java.py)

## Functions
- `_extract_java_imports(node: Any, source: str, imports: list[dict[str, Any]])` — [`L40`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_extractors/_java.py#L40) — Extract Java import declarations.
- `_is_java_stdlib_path(path: str)` — [`L34`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_extractors/_java.py#L34) — True if ``path`` is rooted at one of ``_JAVA_STD_ROOTS``.
- `_strip_java_import_keywords(raw: str)` — [`L21`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_extractors/_java.py#L21) — Strip ``import`` / ``import static`` prefix, trailing ``;`` and ``.*`` glob.

## Module values
- `_JAVA_STD_ROOTS` — [`L7`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_extractors/_java.py#L7)

