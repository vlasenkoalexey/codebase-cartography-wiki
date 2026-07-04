---
title: 'Module: tree_sitter_analyzer/languages/ruby_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/ruby_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.ruby_helpers`/
symbols:
  _make_ruby_attr_function: _make_ruby_attr_function().
  extract_require_statement: extract_require_statement().
  extract_attr_methods: extract_attr_methods().
---
# Module: [`tree_sitter_analyzer/languages/ruby_helpers.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/ruby_helpers.py)

## Functions
- `_make_ruby_attr_function(call_node: Any, parent_class: str, attr_name: str)` — [`L78`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/ruby_helpers.py#L78) — Build the synthetic ``Function`` for one ``attr_*`` symbol.
- `extract_attr_methods(node: Any, parent_class: str, get_node_text: Callable[..., str])` — [`L43`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/ruby_helpers.py#L43) — Extract attr_accessor, attr_reader, attr_writer methods.
- `extract_require_statement(node: Any, get_node_text: Callable[..., str])` — [`L10`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/ruby_helpers.py#L10) — Extract require statement.

