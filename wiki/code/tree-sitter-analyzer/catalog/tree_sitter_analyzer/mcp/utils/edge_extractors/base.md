---
title: 'Module: tree_sitter_analyzer/mcp/utils/edge_extractors/base.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/utils/edge_extractors/base.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.utils.edge_extractors.base`/EdgeExtractor#
symbols:
  EdgeExtractor: ''
  EdgeExtractor.extract: extract().
  EdgeExtractor.detect_root_packages: detect_root_packages().
---
# Module: [`tree_sitter_analyzer/mcp/utils/edge_extractors/base.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/edge_extractors/base.py)

## Classes
### `EdgeExtractor`  ·  implements/extends ABC
- def: [`tree_sitter_analyzer/mcp/utils/edge_extractors/base.py:8`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/edge_extractors/base.py#L8)
- doc: Extract (source_class, target_class) edges from source code.
- signature: `class EdgeExtractor(ABC):`
- members:
  - `detect_root_packages(self, project_root: str)` — [`L38`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/edge_extractors/base.py#L38) — Detect project root packages for first-party filtering.
  - `extract(self, source: str, src_name: str, project_root: str)` — [`L21`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/edge_extractors/base.py#L21) — Extract edges from source code.
- uses (calls/refs, reference-scoped): [`extract`](java.md#JavaEdgeExtractor.extract), [`TypeScriptEdgeExtractor`](typescript.md#TypeScriptEdgeExtractor), [`JavaEdgeExtractor`](java.md#JavaEdgeExtractor), [`PythonEdgeExtractor`](python.md#PythonEdgeExtractor), [`detect_root_packages`](java.md#JavaEdgeExtractor.detect_root_packages), [`extract`](python.md#PythonEdgeExtractor.extract), [`extract`](typescript.md#TypeScriptEdgeExtractor.extract)
- used by: [`_extract_edges_from_file`](../project_index/_manager.md#ProjectIndexManager._extract_edges_from_file), [`REGISTRY`](__init__.md#REGISTRY.REGISTRY), [`TypeScriptEdgeExtractor`](typescript.md#TypeScriptEdgeExtractor), [`get_extractor`](__init__.md#get_extractor), [`JavaEdgeExtractor`](java.md#JavaEdgeExtractor), [`PythonEdgeExtractor`](python.md#PythonEdgeExtractor)

