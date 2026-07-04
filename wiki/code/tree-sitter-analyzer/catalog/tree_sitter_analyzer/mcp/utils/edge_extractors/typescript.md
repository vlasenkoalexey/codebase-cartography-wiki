---
title: 'Module: tree_sitter_analyzer/mcp/utils/edge_extractors/typescript.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/utils/edge_extractors/typescript.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.utils.edge_extractors.typescript`/TypeScriptEdgeExtractor#
symbols:
  TypeScriptEdgeExtractor: ''
  TypeScriptEdgeExtractor.extract: extract().
---
# Module: [`tree_sitter_analyzer/mcp/utils/edge_extractors/typescript.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/edge_extractors/typescript.py)

## Classes
### `TypeScriptEdgeExtractor`  ·  implements/extends EdgeExtractor
- def: [`tree_sitter_analyzer/mcp/utils/edge_extractors/typescript.py:10`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/edge_extractors/typescript.py#L10)
- doc: TypeScript/JS: only relative imports (./ ../) are first-party.
- signature: `class TypeScriptEdgeExtractor(EdgeExtractor):`
- members:
  - `extract(self, source: str, src_name: str, project_root: str)` — [`L13`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/edge_extractors/typescript.py#L13)
- uses (calls/refs, reference-scoped): [`EdgeExtractor`](base.md#EdgeExtractor)
- used by: [`EdgeExtractor`](base.md#EdgeExtractor), [`REGISTRY`](__init__.md#REGISTRY.REGISTRY), [`extract`](base.md#EdgeExtractor.extract)

