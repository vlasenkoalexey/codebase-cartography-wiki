---
title: 'Module: tree_sitter_analyzer/languages/javascript_plugin/_export_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/javascript_plugin/_export_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.javascript_plugin._export_helpers`/
symbols:
  parse_export_statement: parse_export_statement().
  extract_commonjs_exports: extract_commonjs_exports().
  ExportStatementParts: ExportStatementParts.
  _default_export_parts: _default_export_parts().
  _named_export_parts: _named_export_parts().
  _direct_export_parts: _direct_export_parts().
  _commonjs_export_from_match: _commonjs_export_from_match().
---
# Module: [`tree_sitter_analyzer/languages/javascript_plugin/_export_helpers.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_export_helpers.py)

## Functions
- `_commonjs_export_from_match(match: re.Match[str], source_code: str)` — [`L51`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_export_helpers.py#L51)
- `_default_export_parts(clean_text: str)` — [`L67`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_export_helpers.py#L67)
- `_direct_export_parts(clean_text: str)` — [`L83`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_export_helpers.py#L83)
- `_named_export_parts(clean_text: str)` — [`L74`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_export_helpers.py#L74)
- `extract_commonjs_exports(source_code: str)` — [`L13`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_export_helpers.py#L13) — Extract CommonJS module.exports statements.
- `parse_export_statement(export_text: str)` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_export_helpers.py#L33) — Parse export statement to extract details.

## Module values
- `ExportStatementParts` — [`L10`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_export_helpers.py#L10)

