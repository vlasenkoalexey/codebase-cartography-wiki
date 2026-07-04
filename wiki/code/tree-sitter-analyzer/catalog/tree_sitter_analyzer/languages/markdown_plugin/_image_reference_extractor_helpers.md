---
title: 'Module: tree_sitter_analyzer/languages/markdown_plugin/_image_reference_extractor_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/markdown_plugin/_image_reference_extractor_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.markdown_plugin._image_reference_extractor_helpers`/
symbols:
  _append_image_reference_definition: _append_image_reference_definition().
  _extract_image_reference_definitions_process_items: _extract_image_reference_definitions_process_items().
  _collect_image_reference_labels: _collect_image_reference_labels().
  ImageReferenceDefinitionContext: ImageReferenceDefinitionContext#
  ImageReferenceDefinitionContext.root_node: ImageReferenceDefinitionContext#root_node.
  ImageReferenceDefinitionContext.images: ImageReferenceDefinitionContext#images.
  ImageReferenceDefinitionContext.get_node_text: ImageReferenceDefinitionContext#get_node_text.
  ImageReferenceDefinitionContext.traverse_nodes: ImageReferenceDefinitionContext#traverse_nodes.
  ImageReferenceDefinitionContext.image_refs_used: ImageReferenceDefinitionContext#image_refs_used.
  ImageReferenceDefinitionContext.image_extensions: ImageReferenceDefinitionContext#image_extensions.
---
# Module: [`tree_sitter_analyzer/languages/markdown_plugin/_image_reference_extractor_helpers.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/_image_reference_extractor_helpers.py)

## Classes
### `ImageReferenceDefinitionContext`
- def: [`tree_sitter_analyzer/languages/markdown_plugin/_image_reference_extractor_helpers.py:14`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/_image_reference_extractor_helpers.py#L14)
- doc: Inputs needed to extract image reference definitions.
- signature: `class ImageReferenceDefinitionContext:`
- members:
  - `get_node_text` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/_image_reference_extractor_helpers.py#L19)
  - `image_extensions` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/_image_reference_extractor_helpers.py#L22)
  - `image_refs_used` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/_image_reference_extractor_helpers.py#L21)
  - `images` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/_image_reference_extractor_helpers.py#L18)
  - `root_node` — [`L17`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/_image_reference_extractor_helpers.py#L17)
  - `traverse_nodes` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/_image_reference_extractor_helpers.py#L20)
- used by: [`_extract_image_reference_definitions`](link_image_extractor.md#_extract_image_reference_definitions), [`_append_image_reference_definition`](_image_reference_extractor_helpers.md#_append_image_reference_definition), [`_extract_image_reference_definitions_process_items`](_image_reference_extractor_helpers.md#_extract_image_reference_definitions_process_items)

## Functions
- `_append_image_reference_definition(node: Any, raw_text: str, ref_pattern: str, context: ImageReferenceDefinitionContext)` — [`L47`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/_image_reference_extractor_helpers.py#L47)
- `_collect_image_reference_labels(root_node: Any, get_node_text: Callable[..., str], traverse_nodes: Callable[..., Iterator[Any]])` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/_image_reference_extractor_helpers.py#L25)
- `_extract_image_reference_definitions_process_items(context: ImageReferenceDefinitionContext)` — [`L85`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/markdown_plugin/_image_reference_extractor_helpers.py#L85)

