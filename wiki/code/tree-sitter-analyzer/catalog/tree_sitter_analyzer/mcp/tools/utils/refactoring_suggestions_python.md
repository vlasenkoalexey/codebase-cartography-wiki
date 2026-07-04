---
title: 'Module: tree_sitter_analyzer/mcp/tools/utils/refactoring_suggestions_python.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/utils/refactoring_suggestions_python.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.utils.refactoring_suggestions_python`/
symbols:
  python_bonus_analysis: python_bonus_analysis().
  _check_static_extraction: _check_static_extraction().
  _check_depth: _check_depth().
  _is_framework_hook: _is_framework_hook().
  _check_param_count: _check_param_count().
  MCP_TOOL_HOOK_METHODS: MCP_TOOL_HOOK_METHODS.
  _attach_class_parents: _attach_class_parents().
  _base_name: _base_name().
---
# Module: [`tree_sitter_analyzer/mcp/tools/utils/refactoring_suggestions_python.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/refactoring_suggestions_python.py)

## Functions
- `_attach_class_parents(tree: ast.AST)` — [`L53`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/refactoring_suggestions_python.py#L53) — Attach class parent references to immediate class children.
- `_base_name(base: ast.expr)` — [`L150`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/refactoring_suggestions_python.py#L150) — Return the visible name for a class base expression.
- `_check_depth(node: ast.AST, name: str, start: int, end: int, suggestions: list[dict[str, Any]], pattern_rules: list[dict[str, Any]])` — [`L62`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/refactoring_suggestions_python.py#L62) — Check and flag functions exceeding nesting depth threshold.
- `_check_param_count(node: ast.AST, name: str, start: int, suggestions: list[dict[str, Any]], pattern_rules: list[dict[str, Any]])` — [`L86`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/refactoring_suggestions_python.py#L86) — Check and flag functions with too many parameters.
- `_check_static_extraction(node: ast.FunctionDef, name: str, start: int, end: int, suggestions: list[dict[str, Any]], extractable_patterns: list[dict[str, Any]])` — [`L116`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/refactoring_suggestions_python.py#L116) — Check and flag methods that do not use self or cls.
- `_is_framework_hook(parent: ast.ClassDef, method_name: str)` — [`L143`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/refactoring_suggestions_python.py#L143) — Return True for required framework hook methods that may not use self.
- `python_bonus_analysis(source: str, suggestions: list[dict[str, Any]], include_extractions: bool, pattern_rules: list[dict[str, Any]], extractable_patterns: list[dict[str, Any]])` — [`L24`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/refactoring_suggestions_python.py#L24) — Run Python-specific bonus analysis using AST.

## Module values
- `MCP_TOOL_HOOK_METHODS` — [`L15`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/refactoring_suggestions_python.py#L15)

