---
title: 'Module: tree_sitter_analyzer/formatters/markdown_full_formatter.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/formatters/markdown_full_formatter.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.formatters.markdown_full_formatter`/
symbols:
  format_full: format_full().
  _filter_by_type: _filter_by_type().
  _start_line: _start_line().
  _render_blockquotes: _render_blockquotes().
  _render_html_elements: _render_html_elements().
  _render_text_formatting: _render_text_formatting().
  _render_footnotes: _render_footnotes().
  _render_references: _render_references().
  _truncate: _truncate().
  _render_headers: _render_headers().
  _render_links: _render_links().
  _render_images: _render_images().
  _render_lists: _render_lists().
  _render_tables: _render_tables().
  _render_horizontal_rules: _render_horizontal_rules().
  _strip_md_extension: _strip_md_extension().
  _render_overview: _render_overview().
  _render_code_blocks: _render_code_blocks().
---
# Module: [`tree_sitter_analyzer/formatters/markdown_full_formatter.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/markdown_full_formatter.py)

## Functions
- `_filter_by_type(elements: list[dict[str, Any]], types: tuple[str, ...])` — [`L61`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/markdown_full_formatter.py#L61) — Return elements whose ``type`` field is one of ``types``.
- `_render_blockquotes(output: list[str], blockquotes: list[dict[str, Any]])` — [`L191`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/markdown_full_formatter.py#L191) — Blockquotes table — truncated content + line.
- `_render_code_blocks(output: list[str], code_blocks: list[dict[str, Any]])` — [`L145`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/markdown_full_formatter.py#L145) — Code Blocks table — language + line count + line range.
- `_render_footnotes(output: list[str], footnotes: list[dict[str, Any]])` — [`L249`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/markdown_full_formatter.py#L249) — Footnotes table — reference + definition variants.
- `_render_headers(output: list[str], headers: list[dict[str, Any]])` — [`L97`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/markdown_full_formatter.py#L97) — Document Structure table — Markdown headings.
- `_render_horizontal_rules(output: list[str], horizontal_rules: list[dict[str, Any]])` — [`L203`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/markdown_full_formatter.py#L203) — Horizontal Rules table.
- `_render_html_elements(output: list[str], html_elements: list[dict[str, Any]])` — [`L217`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/markdown_full_formatter.py#L217) — HTML Elements table — element type + truncated name.
- `_render_images(output: list[str], images: list[dict[str, Any]])` — [`L130`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/markdown_full_formatter.py#L130) — Images table — alt text + URL.
- `_render_links(output: list[str], links: list[dict[str, Any]])` — [`L111`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/markdown_full_formatter.py#L111) — Links table — text + URL + External/Internal classification.
- `_render_lists(output: list[str], lists: list[dict[str, Any]])` — [`L163`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/markdown_full_formatter.py#L163) — Lists table — list_type + item count.
- `_render_overview(output: list[str], file_path: str, analysis_result: dict[str, Any], element_count: int)` — [`L80`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/markdown_full_formatter.py#L80) — Document Overview table — file path, language, line count, element count.
- `_render_references(output: list[str], references: list[dict[str, Any]])` — [`L263`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/markdown_full_formatter.py#L263) — Reference Definitions table — truncated name + line.
- `_render_tables(output: list[str], tables: list[dict[str, Any]])` — [`L177`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/markdown_full_formatter.py#L177) — Tables table — column + row counts.
- `_render_text_formatting(output: list[str], formatting_elements: list[dict[str, Any]])` — [`L233`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/markdown_full_formatter.py#L233) — Text Formatting table — type + truncated text.
- `_start_line(entry: dict[str, Any])` — [`L68`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/markdown_full_formatter.py#L68) — Return the ``line_range.start`` field or empty string.
- `_strip_md_extension(file_path: str)` — [`L53`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/markdown_full_formatter.py#L53) — Return the filename without its ``.md`` / ``.markdown`` extension.
- `_truncate(text: str, limit: int)` — [`L73`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/markdown_full_formatter.py#L73) — Truncate ``text`` to ``limit`` chars with a ``...`` suffix when needed.
- `format_full(analysis_result: dict[str, Any], collect_images: Callable[[list[dict[str, Any]]], list[dict[str, Any]]])` — [`L15`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/markdown_full_formatter.py#L15) — Format full table output for Markdown files.

