---
title: 'Module: tree_sitter_analyzer/mcp/utils/file_metrics.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/utils/file_metrics.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.utils.file_metrics`/
symbols:
  compute_file_metrics: compute_file_metrics().
  FileMetrics.as_dict: FileMetrics#as_dict().
  _compute_line_metrics: _compute_line_metrics().
  _estimate_tokens: _estimate_tokens().
  FileMetrics.total_lines: FileMetrics#total_lines.
  _compute_max_nesting_depth: _compute_max_nesting_depth().
  FileMetrics.code_lines: FileMetrics#code_lines.
  FileMetrics.comment_lines: FileMetrics#comment_lines.
  FileMetrics.blank_lines: FileMetrics#blank_lines.
  FileMetrics.estimated_tokens: FileMetrics#estimated_tokens.
  FileMetrics.file_size_bytes: FileMetrics#file_size_bytes.
  FileMetrics.content_hash: FileMetrics#content_hash.
  FileMetrics: FileMetrics#
  logger: logger.
  FileMetrics.max_nesting_depth: FileMetrics#max_nesting_depth.
  _TOKEN_RE: _TOKEN_RE.
---
# Module: [`tree_sitter_analyzer/mcp/utils/file_metrics.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/file_metrics.py)

## Classes
### `FileMetrics`
- def: [`tree_sitter_analyzer/mcp/utils/file_metrics.py:15`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/file_metrics.py#L15)
- signature: `class FileMetrics:`
- members:
  - `as_dict(self)` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/file_metrics.py#L25)
  - `blank_lines` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/file_metrics.py#L19)
  - `code_lines` — [`L17`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/file_metrics.py#L17)
  - `comment_lines` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/file_metrics.py#L18)
  - `content_hash` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/file_metrics.py#L22)
  - `estimated_tokens` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/file_metrics.py#L20)
  - `file_size_bytes` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/file_metrics.py#L21)
  - `max_nesting_depth` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/file_metrics.py#L23)
  - `total_lines` — [`L16`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/file_metrics.py#L16)
- used by: [`compute_file_metrics`](file_metrics.md#compute_file_metrics)  (3 test-only)

## Functions
- `_compute_line_metrics(content: str, language: str | None)` — [`L66`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/file_metrics.py#L66) — Compute (total_lines, code_lines, comment_lines, blank_lines).
- `_compute_max_nesting_depth(content: str)` — [`L50`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/file_metrics.py#L50) — Return the deepest block-nesting depth (feature #580).
- `_estimate_tokens(content: str)` — [`L44`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/file_metrics.py#L44)
- `compute_file_metrics(file_path: str, *, language: str | None = None, project_root: str | None = None)` — [`L148`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/file_metrics.py#L148) — Compute file metrics and cache the result by (project_root, file_path, content_hash).

## Module values
- `_TOKEN_RE` — [`L41`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/file_metrics.py#L41)
- `logger` — [`L11`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/file_metrics.py#L11)

