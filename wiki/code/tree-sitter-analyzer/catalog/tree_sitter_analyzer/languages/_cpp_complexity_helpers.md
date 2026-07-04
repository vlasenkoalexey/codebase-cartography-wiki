---
title: 'Module: tree_sitter_analyzer/languages/_cpp_complexity_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/_cpp_complexity_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages._cpp_complexity_helpers`/
symbols:
  _is_logical_operator: _is_logical_operator().
  calculate_complexity: calculate_complexity().
  _DECISION_NODES: _DECISION_NODES.
  _LOGICAL_OPERATORS: _LOGICAL_OPERATORS.
  _NON_EXECUTABLE_ANCHORS: _NON_EXECUTABLE_ANCHORS.
---
# Module: [`tree_sitter_analyzer/languages/_cpp_complexity_helpers.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_complexity_helpers.py)

## Functions
- `_is_logical_operator(node: Any)` — [`L44`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_complexity_helpers.py#L44) — True when ``node`` is a "&&"/"||" used as an executable boolean branch.
- `calculate_complexity(node: Any)` — [`L51`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_complexity_helpers.py#L51) — Calculate cyclomatic complexity for a C++ syntax node.

## Module values
- `_DECISION_NODES` — [`L11`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_complexity_helpers.py#L11)
- `_LOGICAL_OPERATORS` — [`L31`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_complexity_helpers.py#L31)
- `_NON_EXECUTABLE_ANCHORS` — [`L32`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_complexity_helpers.py#L32)

