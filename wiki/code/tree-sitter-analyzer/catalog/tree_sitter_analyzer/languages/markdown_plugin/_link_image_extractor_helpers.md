---
title: 'Module: tree_sitter_analyzer/languages/markdown_plugin/_link_image_extractor_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/markdown_plugin/_link_image_extractor_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.markdown_plugin._link_image_extractor_helpers`/_
symbols:
  _append_inline_link_match: append_inline_link_match().
  _append_autolink_match: append_autolink_match().
  _append_reference_link_match: append_reference_link_match().
  _extract_inline_links_process_items: extract_inline_links_process_items().
  _extract_reference_links_process_items: extract_reference_links_process_items().
  _extract_autolinks_process_items: extract_autolinks_process_items().
  _remember_signature: remember_signature().
---
# Module: [`tree_sitter_analyzer/languages/markdown_plugin/_link_image_extractor_helpers.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/_link_image_extractor_helpers.py)

## Functions
- `_append_autolink_match(node: Any, raw_text: str, match: re.Match[str], links: list[Any], extracted_links: set[str] | None)` — [`L129`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/_link_image_extractor_helpers.py#L129)
- `_append_inline_link_match(node: Any, match: re.Match[str], links: list[Any], extracted_links: set[str] | None)` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/_link_image_extractor_helpers.py#L22)
- `_append_reference_link_match(node: Any, raw_text: str, match: re.Match[str], links: list[Any], processed_ref_links: set[tuple[str, str, int]])` — [`L73`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/_link_image_extractor_helpers.py#L73)
- `_extract_autolinks_process_items(root_node: Any, links: list[Any], get_node_text: Callable[..., str], traverse_nodes: Callable[..., Iterator[Any]], extracted_links: set[str] | None)` — [`L159`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/_link_image_extractor_helpers.py#L159)
- `_extract_inline_links_process_items(root_node: Any, links: list[Any], get_node_text: Callable[..., str], traverse_nodes: Callable[..., Iterator[Any]], extracted_links: set[str] | None)` — [`L53`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/_link_image_extractor_helpers.py#L53)
- `_extract_reference_links_process_items(root_node: Any, links: list[Any], get_node_text: Callable[..., str], traverse_nodes: Callable[..., Iterator[Any]], processed_ref_links: set[tuple[str, str, int]])` — [`L107`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/_link_image_extractor_helpers.py#L107)
- `_remember_signature(signature: str, seen: set[str] | None)` — [`L12`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/_link_image_extractor_helpers.py#L12) — Return true when a signature has not been processed before.

