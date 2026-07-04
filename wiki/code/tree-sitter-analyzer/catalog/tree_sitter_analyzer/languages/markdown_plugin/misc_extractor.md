---
title: 'Module: tree_sitter_analyzer/languages/markdown_plugin/misc_extractor.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/markdown_plugin/misc_extractor.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.markdown_plugin.misc_extractor`/extract_
symbols:
  extract_block_quotes: block_quotes().
  extract_thematic_breaks: thematic_breaks().
  extract_html_blocks: html_blocks().
  extract_inline_html: inline_html().
  extract_emphasis_elements: emphasis_elements().
  extract_inline_code_spans: inline_code_spans().
  extract_strikethrough_elements: strikethrough_elements().
  extract_footnote_elements: footnote_elements().
---
# Module: [`tree_sitter_analyzer/languages/markdown_plugin/misc_extractor.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/misc_extractor.py)

## Functions
- `extract_block_quotes(root_node: Any, blockquotes: list[Any], get_node_text: Callable[..., str], traverse_nodes: Callable[..., Iterator[Any]])` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/misc_extractor.py#L23) — Extract blockquotes.
- `extract_emphasis_elements(root_node: Any, formatting_elements: list[Any], get_node_text: Callable[..., str], traverse_nodes: Callable[..., Iterator[Any]])` — [`L75`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/misc_extractor.py#L75) — Extract emphasis and strong emphasis elements.
- `extract_footnote_elements(root_node: Any, footnotes: list[Any], get_node_text: Callable[..., str], traverse_nodes: Callable[..., Iterator[Any]])` — [`L114`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/misc_extractor.py#L114) — Extract footnote elements.
- `extract_html_blocks(root_node: Any, html_elements: list[Any], get_node_text: Callable[..., str], traverse_nodes: Callable[..., Iterator[Any]])` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/misc_extractor.py#L49) — Extract HTML block elements.
- `extract_inline_code_spans(root_node: Any, formatting_elements: list[Any], get_node_text: Callable[..., str], traverse_nodes: Callable[..., Iterator[Any]])` — [`L88`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/misc_extractor.py#L88) — Extract inline code spans.
- `extract_inline_html(root_node: Any, html_elements: list[Any], get_node_text: Callable[..., str], traverse_nodes: Callable[..., Iterator[Any]])` — [`L62`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/misc_extractor.py#L62) — Extract inline HTML elements.
- `extract_strikethrough_elements(root_node: Any, formatting_elements: list[Any], get_node_text: Callable[..., str], traverse_nodes: Callable[..., Iterator[Any]])` — [`L101`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/misc_extractor.py#L101) — Extract strikethrough elements.
- `extract_thematic_breaks(root_node: Any, horizontal_rules: list[Any], get_node_text: Callable[..., str], traverse_nodes: Callable[..., Iterator[Any]])` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/misc_extractor.py#L36) — Extract thematic breaks (horizontal rules).

