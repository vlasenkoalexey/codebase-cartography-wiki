---
title: 'Module: tree_sitter_analyzer/languages/markdown_plugin/_misc_block_extractor_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/markdown_plugin/_misc_block_extractor_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.markdown_plugin._misc_block_extractor_helpers`/_
symbols:
  _extract_block_quotes_process_items: extract_block_quotes_process_items().
  _extract_html_blocks_process_items: extract_html_blocks_process_items().
  _extract_thematic_breaks_process_items: extract_thematic_breaks_process_items().
  _tag_name: tag_name().
  _clean_blockquote_content: clean_blockquote_content().
  _blockquote_name: blockquote_name().
---
# Module: [`tree_sitter_analyzer/languages/markdown_plugin/_misc_block_extractor_helpers.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/_misc_block_extractor_helpers.py)

## Functions
- `_blockquote_name(content: str)` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/_misc_block_extractor_helpers.py#L48)
- `_clean_blockquote_content(raw_text: str)` — [`L42`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/_misc_block_extractor_helpers.py#L42)
- `_extract_block_quotes_process_items(root_node: Any, blockquotes: list[Any], get_node_text: Callable[..., str], traverse_nodes: Callable[..., Iterator[Any]])` — [`L12`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/_misc_block_extractor_helpers.py#L12)
- `_extract_html_blocks_process_items(root_node: Any, html_elements: list[Any], get_node_text: Callable[..., str], traverse_nodes: Callable[..., Iterator[Any]])` — [`L82`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/_misc_block_extractor_helpers.py#L82)
- `_extract_thematic_breaks_process_items(root_node: Any, horizontal_rules: list[Any], get_node_text: Callable[..., str], traverse_nodes: Callable[..., Iterator[Any]])` — [`L54`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/_misc_block_extractor_helpers.py#L54)
- `_tag_name(raw_text: str)` — [`L111`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/_misc_block_extractor_helpers.py#L111)

