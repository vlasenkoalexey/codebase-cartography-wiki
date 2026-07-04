---
title: 'Module: tree_sitter_analyzer/formatters/_markdown_formatter_counts.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/formatters/_markdown_formatter_counts.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.formatters._markdown_formatter_counts`/
symbols:
  compute_robust_counts_from_file: compute_robust_counts_from_file().
  count_used_image_definitions: count_used_image_definitions().
  count_markdown_links: count_markdown_links().
  count_markdown_images: count_markdown_images().
  autolink_pattern: autolink_pattern().
  image_reference_labels: image_reference_labels().
  reference_definition_pattern: reference_definition_pattern().
---
# Module: [`tree_sitter_analyzer/formatters/_markdown_formatter_counts.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_markdown_formatter_counts.py)

## Functions
- `autolink_pattern()` — [`L42`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_markdown_formatter_counts.py#L42) — Return the Markdown autolink pattern.
- `compute_robust_counts_from_file(file_path: str)` — [`L11`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_markdown_formatter_counts.py#L11) — Compute link and image counts directly from raw Markdown text.
- `count_markdown_images(content: str)` — [`L47`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_markdown_formatter_counts.py#L47) — Count inline and reference Markdown images.
- `count_markdown_links(content: str)` — [`L29`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_markdown_formatter_counts.py#L29) — Count inline, reference, and autolink Markdown links.
- `count_used_image_definitions(content: str)` — [`L54`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_markdown_formatter_counts.py#L54) — Count reference definitions used by image references or image-like URLs.
- `image_reference_labels(content: str)` — [`L66`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_markdown_formatter_counts.py#L66) — Return lowercased labels used by image references.
- `reference_definition_pattern()` — [`L74`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_markdown_formatter_counts.py#L74) — Return the Markdown reference definition pattern.

