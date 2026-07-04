---
title: 'Module: tree_sitter_analyzer/mcp/tools/utils/anti_patterns.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/utils/anti_patterns.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.utils.anti_patterns`/
symbols:
  detect_anti_patterns: detect_anti_patterns().
  _check_python_anti_patterns: _check_python_anti_patterns().
  _check_js_anti_patterns: _check_js_anti_patterns().
  _check_java_anti_patterns: _check_java_anti_patterns().
  python_docstring_line_set: python_docstring_line_set().
  _python_mutable_default_lines: _python_mutable_default_lines().
  _record_mutable_defaults: _record_mutable_defaults().
  _is_mutable_literal: _is_mutable_literal().
  __all__: __all__.
---
# Module: [`tree_sitter_analyzer/mcp/tools/utils/anti_patterns.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/anti_patterns.py)

## Functions
- `_check_java_anti_patterns(lines: list[str], patterns: list[dict[str, Any]])` — [`L222`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/anti_patterns.py#L222)
- `_check_js_anti_patterns(lines: list[str], patterns: list[dict[str, Any]])` — [`L196`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/anti_patterns.py#L196)
- `_check_python_anti_patterns(lines: list[str], patterns: list[dict[str, Any]])` — [`L136`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/anti_patterns.py#L136)
- `_is_mutable_literal(node: ast.expr)` — [`L89`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/anti_patterns.py#L89) — Return True for ``[]`` / ``{}`` / ``{1, 2}`` / ``list()`` etc.
- `_python_mutable_default_lines(lines: list[str])` — [`L42`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/anti_patterns.py#L42) — Return 1-indexed line numbers of ``def`` defaults that are mutable.
- `_record_mutable_defaults(func: ast.FunctionDef | ast.AsyncFunctionDef | ast.Lambda, flagged: set[int])` — [`L72`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/anti_patterns.py#L72) — Append line numbers of mutable defaults on a single function node.
- `detect_anti_patterns(file_path: str, language: str | None)` — [`L18`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/anti_patterns.py#L18) — Return anti-pattern findings for ``file_path`` in ``language``.
- `python_docstring_line_set(lines: list[str])` — [`L104`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/anti_patterns.py#L104) — Return 1-indexed line numbers inside Python triple-quoted strings.

## Module values
- `__all__` — [`L247`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/anti_patterns.py#L247)

