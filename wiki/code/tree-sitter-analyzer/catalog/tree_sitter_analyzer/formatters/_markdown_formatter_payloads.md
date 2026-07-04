---
title: 'Module: tree_sitter_analyzer/formatters/_markdown_formatter_payloads.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/formatters/_markdown_formatter_payloads.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.formatters._markdown_formatter_payloads`/
symbols:
  build_summary_result: build_summary_result().
  build_structure_result: build_structure_result().
  build_advanced_result: build_advanced_result().
  build_content_analysis: build_content_analysis().
  links_with_robust_placeholders: links_with_robust_placeholders().
  images_with_robust_placeholders: images_with_robust_placeholders().
  summary_headers: summary_headers().
  summary_links: summary_links().
  summary_images: summary_images().
  summary_code_blocks: summary_code_blocks().
  summary_lists: summary_lists().
  structure_headers: structure_headers().
  structure_links: structure_links().
  structure_images: structure_images().
  structure_code_blocks: structure_code_blocks().
  structure_lists: structure_lists().
  structure_tables: structure_tables().
  build_structure_statistics: build_structure_statistics().
  partition_external_links: partition_external_links().
  build_document_metrics: build_document_metrics().
---
# Module: [`tree_sitter_analyzer/formatters/_markdown_formatter_payloads.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_markdown_formatter_payloads.py)

## Functions
- `build_advanced_result(analysis_result: dict[str, Any], images: list[dict[str, Any]], robust_counts: dict[str, int])` — [`L207`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_markdown_formatter_payloads.py#L207) — Build the JSON advanced-analysis payload for Markdown analysis.
- `build_content_analysis(groups: dict[str, list[Any]], images: list[dict[str, Any]], external_links: list[dict[str, Any]])` — [`L279`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_markdown_formatter_payloads.py#L279) — Build qualitative Markdown content-analysis flags.
- `build_document_metrics(groups: dict[str, list[Any]], images: list[dict[str, Any]], external_links: list[dict[str, Any]], internal_links: list[dict[str, Any]], robust_counts: dict[str, int])` — [`L250`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_markdown_formatter_payloads.py#L250) — Build aggregate Markdown document metrics.
- `build_structure_result(analysis_result: dict[str, Any], images: list[dict[str, Any]], robust_counts: dict[str, int])` — [`L94`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_markdown_formatter_payloads.py#L94) — Build the JSON structure payload for Markdown analysis.
- `build_structure_statistics(analysis_result: dict[str, Any], groups: dict[str, list[Any]], images: list[dict[str, Any]], robust_counts: dict[str, int])` — [`L189`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_markdown_formatter_payloads.py#L189) — Build structure statistics with parser-count fallbacks.
- `build_summary_result(file_path: str, elements: list[dict[str, Any]], images: list[dict[str, Any]], robust_counts: dict[str, int])` — [`L12`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_markdown_formatter_payloads.py#L12) — Build the JSON summary payload for Markdown analysis.
- `images_with_robust_placeholders(images: list[dict[str, Any]], robust_counts: dict[str, int])` — [`L46`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_markdown_formatter_payloads.py#L46) — Pad images when raw Markdown scanning found parser-undetected images.
- `links_with_robust_placeholders(links: list[dict[str, Any]], robust_counts: dict[str, int])` — [`L36`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_markdown_formatter_payloads.py#L36) — Pad links when raw Markdown scanning found parser-undetected links.
- `partition_external_links(links: list[dict[str, Any]])` — [`L231`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_markdown_formatter_payloads.py#L231) — Split links into external HTTP(S) links and the remaining internal links.
- `structure_code_blocks(code_blocks: list[dict[str, Any]])` — [`L153`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_markdown_formatter_payloads.py#L153) — Build structure code block entries.
- `structure_headers(headers: list[dict[str, Any]])` — [`L117`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_markdown_formatter_payloads.py#L117) — Build structure header entries.
- `structure_images(images: list[dict[str, Any]])` — [`L141`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_markdown_formatter_payloads.py#L141) — Build structure image entries.
- `structure_links(links: list[dict[str, Any]])` — [`L129`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_markdown_formatter_payloads.py#L129) — Build structure link entries.
- `structure_lists(lists: list[dict[str, Any]])` — [`L165`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_markdown_formatter_payloads.py#L165) — Build structure list entries.
- `structure_tables(tables: list[dict[str, Any]])` — [`L177`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_markdown_formatter_payloads.py#L177) — Build structure table entries.
- `summary_code_blocks(code_blocks: list[dict[str, Any]])` — [`L78`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_markdown_formatter_payloads.py#L78) — Build summary code block entries.
- `summary_headers(headers: list[dict[str, Any]])` — [`L56`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_markdown_formatter_payloads.py#L56) — Build summary header entries.
- `summary_images(images: list[dict[str, Any]])` — [`L71`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_markdown_formatter_payloads.py#L71) — Build summary image entries.
- `summary_links(links: list[dict[str, Any]])` — [`L64`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_markdown_formatter_payloads.py#L64) — Build summary link entries.
- `summary_lists(lists: list[dict[str, Any]])` — [`L86`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_markdown_formatter_payloads.py#L86) — Build summary list entries.

