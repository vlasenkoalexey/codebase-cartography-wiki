---
title: 'Module: tree_sitter_analyzer/languages/css_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/css_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.css_helpers`/
symbols:
  create_style_element: create_style_element().
  extract_css_properties: extract_css_properties().
  _collect_css_block_declarations: _collect_css_block_declarations().
  parse_declaration: parse_declaration().
  extract_at_rule_name: extract_at_rule_name().
  classify_rule: classify_rule().
  extract_css_selector: extract_css_selector().
  extract_node_text: extract_node_text().
---
# Module: [`tree_sitter_analyzer/languages/css_helpers.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/css_helpers.py)

## Functions
- `_collect_css_block_declarations(block_node: Any, get_node_text: Callable[..., str], properties: dict[str, str])` — [`L140`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/css_helpers.py#L140) — Append each ``declaration`` child to ``properties``.
- `classify_rule(properties: dict[str, str], property_categories: dict[str, list[str]])` — [`L84`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/css_helpers.py#L84) — Classify CSS rule based on properties.
- `create_style_element(node: Any, get_node_text: Callable[..., str], property_categories: dict[str, list[str]])` — [`L158`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/css_helpers.py#L158) — Create StyleElement from tree-sitter node. — documented in [tree_sitter_analyzer-models-markup_models](../../../concepts/tree_sitter_analyzer-models-markup_models.md)
- `extract_at_rule_name(node: Any, get_node_text: Callable[..., str])` — [`L57`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/css_helpers.py#L57) — Extract at-rule name from CSS at-rule node.
- `extract_css_properties(node: Any, get_node_text: Callable[..., str])` — [`L120`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/css_helpers.py#L120) — Extract properties from CSS rule_set node.
- `extract_css_selector(node: Any, get_node_text: Callable[..., str])` — [`L104`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/css_helpers.py#L104) — Extract selector from CSS rule_set node.
- `extract_node_text(node: Any, source_code: str)` — [`L10`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/css_helpers.py#L10) — Extract text content from a tree-sitter node.
- `parse_declaration(decl_node: Any, get_node_text: Callable[..., str])` — [`L23`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/css_helpers.py#L23) — Parse individual CSS declaration.

