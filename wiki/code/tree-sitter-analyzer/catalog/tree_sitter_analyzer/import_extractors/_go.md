---
title: 'Module: tree_sitter_analyzer/import_extractors/_go.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/import_extractors/_go.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.import_extractors._go`/_
symbols:
  _extract_go_imports: extract_go_imports().
  _parse_go_spec: parse_go_spec().
  _GO_STD: GO_STD.
  _collect_go_specs: collect_go_specs().
---
# Module: [`tree_sitter_analyzer/import_extractors/_go.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_extractors/_go.py)

## Functions
- `_collect_go_specs(child: Any)` — [`L71`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_extractors/_go.py#L71) — Collect import_spec children from an import_spec_list node.
- `_extract_go_imports(node: Any, source: str, imports: list[dict[str, Any]])` — [`L78`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_extractors/_go.py#L78) — Extract Go import declarations.
- `_parse_go_spec(spec: Any, source: str)` — [`L48`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_extractors/_go.py#L48) — Return import dict from a single Go import_spec node, or None to skip.

## Module values
- `_GO_STD` — [`L7`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_extractors/_go.py#L7)

