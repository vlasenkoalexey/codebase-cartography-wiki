---
title: 'Module: tree_sitter_analyzer/formatters/_markdown_formatter_elements.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/formatters/_markdown_formatter_elements.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.formatters._markdown_formatter_elements`/
symbols:
  collect_markdown_groups: collect_markdown_groups().
  collect_images: collect_images().
  promoted_image_definition: promoted_image_definition().
  is_image_url: is_image_url().
  promote_image_reference_definitions: promote_image_reference_definitions().
  LINK_TYPES: LINK_TYPES.
  LIST_TYPES: LIST_TYPES.
  IMAGE_TYPES: IMAGE_TYPES.
  IMAGE_EXTENSIONS: IMAGE_EXTENSIONS.
  has_image_reference_definitions: has_image_reference_definitions().
  reference_definition_url_alt: reference_definition_url_alt().
---
# Module: [`tree_sitter_analyzer/formatters/_markdown_formatter_elements.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_markdown_formatter_elements.py)

## Functions
- `collect_images(elements: list[dict[str, Any]])` — [`L26`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_markdown_formatter_elements.py#L26) — Collect explicit images and image-like reference definitions.
- `collect_markdown_groups(elements: list[dict[str, Any]])` — [`L15`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_markdown_formatter_elements.py#L15) — Group Markdown elements by the categories used in formatter outputs.
- `has_image_reference_definitions(elements: list[dict[str, Any]])` — [`L34`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_markdown_formatter_elements.py#L34) — Return whether elements already contain image reference definitions.
- `is_image_url(url: str)` — [`L86`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_markdown_formatter_elements.py#L86) — Return whether a URL has a Markdown image-like extension.
- `promote_image_reference_definitions(elements: list[dict[str, Any]], images: list[dict[str, Any]])` — [`L39`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_markdown_formatter_elements.py#L39) — Promote reference definitions with image-like URLs into image entries.
- `promoted_image_definition(element: dict[str, Any])` — [`L54`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_markdown_formatter_elements.py#L54) — Return a promoted image definition when a reference points at an image.
- `reference_definition_url_alt(element: dict[str, Any])` — [`L71`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_markdown_formatter_elements.py#L71) — Return URL and alt text from a reference definition element.

## Module values
- `IMAGE_EXTENSIONS` — [`L12`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_markdown_formatter_elements.py#L12)
- `IMAGE_TYPES` — [`L11`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_markdown_formatter_elements.py#L11)
- `LINK_TYPES` — [`L9`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_markdown_formatter_elements.py#L9)
- `LIST_TYPES` — [`L10`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_markdown_formatter_elements.py#L10)

