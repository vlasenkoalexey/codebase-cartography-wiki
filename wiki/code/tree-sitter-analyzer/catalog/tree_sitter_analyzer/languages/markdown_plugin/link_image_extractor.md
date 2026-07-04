---
title: 'Module: tree_sitter_analyzer/languages/markdown_plugin/link_image_extractor.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/markdown_plugin/link_image_extractor.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.markdown_plugin.link_image_extractor`/
symbols:
  _extract_image_reference_definitions: _extract_image_reference_definitions().
  _extract_inline_images: _extract_inline_images().
  _extract_reference_images: _extract_reference_images().
  extract_md_links: extract_md_links().
  extract_md_images: extract_md_images().
  extract_md_link_reference_definitions: extract_md_link_reference_definitions().
  _extract_inline_links: _extract_inline_links().
  _extract_reference_links: _extract_reference_links().
  _extract_autolinks: _extract_autolinks().
  parse_link_components: parse_link_components().
  parse_image_components: parse_image_components().
---
# Module: [`tree_sitter_analyzer/languages/markdown_plugin/link_image_extractor.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/link_image_extractor.py)

## Functions
- `_extract_autolinks(root_node: Any, links: list[Any], get_node_text: Callable[..., str], traverse_nodes: Callable[..., Iterator[Any]], extracted_links: set[str] | None = None)` — [`L138`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/link_image_extractor.py#L138) — Extract autolinks.
- `_extract_image_reference_definitions(root_node: Any, images: list[Any], get_node_text: Callable[..., str], traverse_nodes: Callable[..., Iterator[Any]])` — [`L242`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/link_image_extractor.py#L242) — Extract image reference definitions.
- `_extract_inline_images(root_node: Any, images: list[Any], get_node_text: Callable[..., str], traverse_nodes: Callable[..., Iterator[Any]])` — [`L152`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/link_image_extractor.py#L152) — Extract inline images.
- `_extract_inline_links(root_node: Any, links: list[Any], get_node_text: Callable[..., str], traverse_nodes: Callable[..., Iterator[Any]], extracted_links: set[str] | None = None)` — [`L110`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/link_image_extractor.py#L110) — Extract inline links.
- `_extract_reference_images(root_node: Any, images: list[Any], get_node_text: Callable[..., str], traverse_nodes: Callable[..., Iterator[Any]])` — [`L198`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/link_image_extractor.py#L198) — Extract reference images.
- `_extract_reference_links(root_node: Any, links: list[Any], get_node_text: Callable[..., str], traverse_nodes: Callable[..., Iterator[Any]])` — [`L124`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/link_image_extractor.py#L124) — Extract reference links.
- `extract_md_images(root_node: Any, get_node_text: Callable[..., str], traverse_nodes: Callable[..., Iterator[Any]])` — [`L59`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/link_image_extractor.py#L59) — Extract all image types (inline, reference, ref definitions) from markdown.
- `extract_md_link_reference_definitions(root_node: Any, get_node_text: Callable[..., str], traverse_nodes: Callable[..., Iterator[Any]])` — [`L78`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/link_image_extractor.py#L78) — Extract link reference definitions from markdown.
- `extract_md_links(root_node: Any, get_node_text: Callable[..., str], traverse_nodes: Callable[..., Iterator[Any]], extracted_links: set[str] | None = None)` — [`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/link_image_extractor.py#L39) — Extract all link types (inline, reference, autolinks) from markdown.
- `parse_image_components(raw_text: str)` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/link_image_extractor.py#L29) — Parse ``![alt](url "title")`` components from raw Markdown text.
- `parse_link_components(raw_text: str)` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/link_image_extractor.py#L20) — Parse ``[text](url "title")`` components from raw Markdown text.

