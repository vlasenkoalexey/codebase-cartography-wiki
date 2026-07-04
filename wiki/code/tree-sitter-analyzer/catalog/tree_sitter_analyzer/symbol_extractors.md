---
title: 'Module: tree_sitter_analyzer/symbol_extractors.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/symbol_extractors.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.symbol_extractors`/
symbols:
  extract_top_level_defs_from_file: extract_top_level_defs_from_file().
  _python_top_level_names: _python_top_level_names().
  _decorated_inner_def: _decorated_inner_def().
  _name_of_def: _name_of_def().
  _PY_FUNCTION_DEF: _PY_FUNCTION_DEF.
  _PY_CLASS_DEF: _PY_CLASS_DEF.
  _PY_DECORATED_DEF: _PY_DECORATED_DEF.
  _node_text: _node_text().
  logger: logger.
  __all__: __all__.
---
# Module: [`tree_sitter_analyzer/symbol_extractors.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/symbol_extractors.py)

## Functions
- `_decorated_inner_def(decorated_node: Any)` — [`L101`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/symbol_extractors.py#L101) — Return the wrapped ``function_definition`` / ``class_definition``.
- `_name_of_def(def_node: Any, source: bytes | str)` — [`L116`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/symbol_extractors.py#L116) — Extract the identifier name from a function/class definition node.
- `_node_text(node: Any, source: bytes | str)` — [`L143`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/symbol_extractors.py#L143) — Return the literal source text of a tree-sitter node.
- `_python_top_level_names(root_node: Any, source: bytes | str)` — [`L69`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/symbol_extractors.py#L69) — Collect names of top-level ``def`` and ``class`` declarations.
- `extract_top_level_defs_from_file(file_path: str, language: str)` — [`L39`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/symbol_extractors.py#L39) — Return top-level function and class names defined in ``file_path``.

## Module values
- `_PY_CLASS_DEF` — [`L35`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/symbol_extractors.py#L35)
- `_PY_DECORATED_DEF` — [`L36`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/symbol_extractors.py#L36)
- `_PY_FUNCTION_DEF` — [`L34`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/symbol_extractors.py#L34)
- `__all__` — [`L166`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/symbol_extractors.py#L166)
- `logger` — [`L27`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/symbol_extractors.py#L27)

