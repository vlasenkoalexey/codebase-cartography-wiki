---
title: 'Module: tree_sitter_analyzer/languages/javascript_plugin/_import_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/javascript_plugin/_import_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.javascript_plugin._import_helpers`/
symbols:
  _commonjs_import_from_match: _commonjs_import_from_match().
  parse_import_statement: parse_import_statement().
  extract_commonjs_requires: extract_commonjs_requires().
  extract_import_names: extract_import_names().
  _identifier_names: _identifier_names().
  ImportStatementParts: ImportStatementParts.
  _namespace_import_parts: _namespace_import_parts().
  _named_import_parts: _named_import_parts().
  _default_import_parts: _default_import_parts().
  _named_import_names: _named_import_names().
  _node_text: _node_text().
---
# Module: [`tree_sitter_analyzer/languages/javascript_plugin/_import_helpers.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_import_helpers.py)

## Functions
- `_commonjs_import_from_match(match: re.Match[str], source_code: str)` — [`L70`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_import_helpers.py#L70)
- `_default_import_parts(clean_text: str, source: str)` — [`L105`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_import_helpers.py#L105)
- `_identifier_names(nodes: list[tree_sitter.Node], source_bytes: bytes)` — [`L123`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_import_helpers.py#L123)
- `_named_import_names(nodes: list[tree_sitter.Node], source_bytes: bytes)` — [`L112`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_import_helpers.py#L112)
- `_named_import_parts(clean_text: str, source: str)` — [`L96`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_import_helpers.py#L96)
- `_namespace_import_parts(clean_text: str, source: str)` — [`L86`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_import_helpers.py#L86)
- `_node_text(node: tree_sitter.Node, source_bytes: bytes)` — [`L132`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_import_helpers.py#L132)
- `extract_commonjs_requires(source_code: str)` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_import_helpers.py#L35) — Extract CommonJS require() statements.
- `extract_import_names(import_clause_node: tree_sitter.Node, source_code: str)` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_import_helpers.py#L18) — Extract imported names from a JavaScript import clause.
- `parse_import_statement(import_text: str)` — [`L52`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_import_helpers.py#L52) — Parse import statement to extract details.

## Module values
- `ImportStatementParts` — [`L15`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_import_helpers.py#L15)

