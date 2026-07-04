---
title: 'Module: tree_sitter_analyzer/languages/sql_plugin/schema_reference_extractor.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/sql_plugin/schema_reference_extractor.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.sql_plugin.schema_reference_extractor`/
symbols:
  _append_schema_reference: _append_schema_reference().
  extract_schema_references: extract_schema_references().
---
# Module: [`tree_sitter_analyzer/languages/sql_plugin/schema_reference_extractor.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/schema_reference_extractor.py)

## Functions
- `_append_schema_reference(node: tree_sitter.Node, imports: list[Import], get_node_text: Callable[..., str])` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/schema_reference_extractor.py#L28) — Append one schema reference when text has exactly two dotted parts.
- `extract_schema_references(root_node: tree_sitter.Node, imports: list[Import], traverse_nodes: Callable[..., Iterator[Any]], get_node_text: Callable[..., str])` — [`L15`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/schema_reference_extractor.py#L15) — Extract schema.table references as generic Import elements.

