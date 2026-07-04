---
title: 'Module: tree_sitter_analyzer/mcp/utils/edge_extractors/python.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/utils/edge_extractors/python.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.utils.edge_extractors.python`/
symbols:
  _is_first_party: _is_first_party().
  _third_party_cache._third_party_cache: _third_party_cache._third_party_cache.
  PythonEdgeExtractor: PythonEdgeExtractor#
  _get_third_party: _get_third_party().
  PythonEdgeExtractor.extract: PythonEdgeExtractor#extract().
  _STDLIB._STDLIB: _STDLIB._STDLIB.
---
# Module: [`tree_sitter_analyzer/mcp/utils/edge_extractors/python.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/edge_extractors/python.py)

## Classes
### `PythonEdgeExtractor`  ·  implements/extends EdgeExtractor
- def: [`tree_sitter_analyzer/mcp/utils/edge_extractors/python.py:39`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/edge_extractors/python.py#L39)
- doc: Python: filter stdlib and third-party imports using built-in APIs.
- signature: `class PythonEdgeExtractor(EdgeExtractor):`
- members:
  - `extract(self, source: str, src_name: str, project_root: str)` — [`L42`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/edge_extractors/python.py#L42)
- uses (calls/refs, reference-scoped): [`EdgeExtractor`](base.md#EdgeExtractor), [`_is_first_party`](python.md#_is_first_party)
- used by: [`EdgeExtractor`](base.md#EdgeExtractor), [`REGISTRY`](__init__.md#REGISTRY.REGISTRY), [`extract`](base.md#EdgeExtractor.extract)

## Functions
- `_get_third_party()` — [`L16`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/edge_extractors/python.py#L16)
- `_is_first_party(module: str)` — [`L29`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/edge_extractors/python.py#L29) — Check if a Python module is first-party (not stdlib, not third-party).

## Module values
- `_STDLIB` — [`L10`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/edge_extractors/python.py#L10)
- `_third_party_cache` — [`L13`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/edge_extractors/python.py#L13)

