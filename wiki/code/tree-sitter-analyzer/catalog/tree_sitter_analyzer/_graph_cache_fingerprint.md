---
title: 'Module: tree_sitter_analyzer/_graph_cache_fingerprint.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/_graph_cache_fingerprint.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer._graph_cache_fingerprint`/
symbols:
  compute_graph_fingerprint: compute_graph_fingerprint().
  GraphFingerprint.file_count: GraphFingerprint#file_count.
  GraphFingerprint: GraphFingerprint#
  is_ast_index_stale: is_ast_index_stale().
  GraphFingerprint.max_mtime_ns: GraphFingerprint#max_mtime_ns.
  _walk_supported_source_paths: _walk_supported_source_paths().
  _EXCLUDE_DIRS._EXCLUDE_DIRS: _EXCLUDE_DIRS._EXCLUDE_DIRS.
  _indexed_abs_and_rel_path: _indexed_abs_and_rel_path().
  _SOURCE_EXTS._SOURCE_EXTS: _SOURCE_EXTS._SOURCE_EXTS.
  GraphFingerprint.is_empty: GraphFingerprint#is_empty().
  _walk_one_directory: _walk_one_directory().
  _process_entry: _process_entry().
---
# Module: [`tree_sitter_analyzer/_graph_cache_fingerprint.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_graph_cache_fingerprint.py)

## Classes
### `GraphFingerprint`  ·  implements/extends NamedTuple
- def: [`tree_sitter_analyzer/_graph_cache_fingerprint.py:62`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_graph_cache_fingerprint.py#L62)
- doc: Cheap stable fingerprint for graph-cache invalidation.
- signature: `class GraphFingerprint(NamedTuple):`
- members:
  - `is_empty(self)` — [`L78`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_graph_cache_fingerprint.py#L78) — Return True when no source files were observed (degenerate).
  - `file_count` — [`L75`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_graph_cache_fingerprint.py#L75)
  - `max_mtime_ns` — [`L76`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_graph_cache_fingerprint.py#L76)
- used by: [`compute_graph_fingerprint`](_graph_cache_fingerprint.md#compute_graph_fingerprint), [`_cache_key_for`](project_graph.md#DependencyGraph._cache_key_for), [`_explain_fingerprint_delta`](mcp/tools/call_graph_tool.md#CodeGraphCallTool._explain_fingerprint_delta), [`_explain_fingerprint_delta`](mcp/tools/dependency_analysis_tool.md#DependencyAnalysisTool._explain_fingerprint_delta), [`_explain_fingerprint_delta`](mcp/tools/symbol_lineage_tool.md#SymbolLineageTool._explain_fingerprint_delta), [`_dep_graph_fingerprint`](mcp/tools/symbol_lineage_tool.md#SymbolLineageTool._dep_graph_fingerprint), [`_call_graph_fingerprint`](mcp/tools/call_graph_tool.md#CodeGraphCallTool._call_graph_fingerprint), [`_graph_fingerprint`](mcp/tools/dependency_analysis_tool.md#DependencyAnalysisTool._graph_fingerprint)  (3 test-only)

## Functions
- `_indexed_abs_and_rel_path(root: Path, file_path: str)` — [`L224`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_graph_cache_fingerprint.py#L224)
- `_process_entry(entry: os.DirEntry[str], exts: tuple[str, ...], stack: list[str], file_count: int, max_mtime_ns: int)` — [`L148`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_graph_cache_fingerprint.py#L148) — Sort a single entry into recurse-stack or fingerprint accumulator.
- `_walk_one_directory(path: str, exts: tuple[str, ...], stack: list[str], file_count: int, max_mtime_ns: int)` — [`L124`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_graph_cache_fingerprint.py#L124) — Iterate one ``scandir`` entry list; recurse into subdirs via the stack.
- `_walk_supported_source_paths(root: Path)` — [`L234`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_graph_cache_fingerprint.py#L234) — Yield project-relative paths accepted by the AST indexer.
- `compute_graph_fingerprint(project_root: str, *, extensions: Iterable[str] | None = None)` — [`L83`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_graph_cache_fingerprint.py#L83) — Fingerprint the project source tree under ``project_root``.
- `is_ast_index_stale(project_root: str)` — [`L172`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_graph_cache_fingerprint.py#L172) — Authoritative, language-complete staleness check for the AST index.

## Module values
- `_EXCLUDE_DIRS` — [`L39`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_graph_cache_fingerprint.py#L39)
- `_SOURCE_EXTS` — [`L43`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_graph_cache_fingerprint.py#L43)

