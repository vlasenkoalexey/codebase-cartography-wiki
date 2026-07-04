---
title: 'Module: tree_sitter_analyzer/import_extractors/_javascript.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/import_extractors/_javascript.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.import_extractors._javascript`/
symbols:
  _extract_js_imports: _extract_js_imports().
  _js_import_module_path: _js_import_module_path().
  _collect_require_call_imports: _collect_require_call_imports().
  extract_js_imports: extract_js_imports().
  _JS_BUILTIN: _JS_BUILTIN.
---
# Module: [`tree_sitter_analyzer/import_extractors/_javascript.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_extractors/_javascript.py)

## Functions
- `_collect_require_call_imports(node: Any, source: str, imports: list[dict[str, Any]])` — [`L58`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_extractors/_javascript.py#L58) — Walk a JS ``require('mod')`` call node, appending non-builtin imports.
- `_extract_js_imports(node: Any, source: str, imports: list[dict[str, Any]])` — [`L107`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_extractors/_javascript.py#L107) — Extract JS/TS import/require statements.
- `_js_import_module_path(node: Any, source: str)` — [`L40`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_extractors/_javascript.py#L40) — Return the module path of a JS ``import ... from "X"`` statement.
- `extract_js_imports(node: Any, source: str, imports: list[dict[str, Any]])` — [`L85`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_extractors/_javascript.py#L85) — Extract JS/TS import/require statements.

## Module values
- `_JS_BUILTIN` — [`L7`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_extractors/_javascript.py#L7)

