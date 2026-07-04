---
title: 'Module: tree_sitter_analyzer/languages/_swift_plugin_nodes.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/_swift_plugin_nodes.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages._swift_plugin_nodes`/
symbols:
  visibility: visibility().
  named_child_text: named_child_text().
  modifier_words: modifier_words().
  binding_kind: binding_kind().
  decode_node_text: decode_node_text().
  type_name: type_name().
  variable_name: variable_name().
  class_type: class_type().
  first_descendant_text: first_descendant_text().
  TYPE_DECLARATION_KINDS: TYPE_DECLARATION_KINDS.
  extract_matching_nodes: extract_matching_nodes().
  VISIBILITY_MODIFIERS: VISIBILITY_MODIFIERS.
  walk: walk().
  base_element_fields: base_element_fields().
  inherited_types: inherited_types().
  superclass: superclass().
  interfaces: interfaces().
  type_annotation: type_annotation().
  fallback_name: fallback_name().
---
# Module: [`tree_sitter_analyzer/languages/_swift_plugin_nodes.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_swift_plugin_nodes.py)

## Functions
- `base_element_fields(node: tree_sitter.Node, raw_text: str, name: str)` — [`L94`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_swift_plugin_nodes.py#L94) — Return fields common to all extracted Swift elements.
- `binding_kind(node: tree_sitter.Node, raw_text: str)` — [`L77`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_swift_plugin_nodes.py#L77) — Return let/var binding kind for a Swift property.
- `class_type(node: tree_sitter.Node)` — [`L64`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_swift_plugin_nodes.py#L64) — Return Swift type declaration kind.
- `decode_node_text(node: tree_sitter.Node)` — [`L43`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_swift_plugin_nodes.py#L43) — Decode a node's byte text safely.
- `extract_matching_nodes(root: tree_sitter.Node, node_types: set[str], extractor: Callable[[tree_sitter.Node], Any | None])` — [`L27`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_swift_plugin_nodes.py#L27) — Extract model elements for matching Swift AST node types.
- `fallback_name(node: tree_sitter.Node)` — [`L180`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_swift_plugin_nodes.py#L180) — Return a deterministic fallback name for anonymous Swift nodes.
- `first_descendant_text(extractor: Any, node: tree_sitter.Node, node_types: tuple[str, ...])` — [`L118`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_swift_plugin_nodes.py#L118) — Return the first matching descendant text.
- `inherited_types(raw_text: str)` — [`L159`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_swift_plugin_nodes.py#L159) — Return inherited class/protocol names from a Swift declaration header.
- `interfaces(inherited: list[str], superclass_name: str | None)` — [`L175`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_swift_plugin_nodes.py#L175) — Return protocol/interface names after removing superclass.
- `modifier_words(node: tree_sitter.Node)` — [`L51`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_swift_plugin_nodes.py#L51) — Return Swift modifier tokens attached to a declaration.
- `named_child_text(extractor: Any, node: tree_sitter.Node, node_types: tuple[str, ...])` — [`L109`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_swift_plugin_nodes.py#L109) — Return the first descendant text matching any node type.
- `superclass(class_type_name: str, inherited: list[str])` — [`L168`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_swift_plugin_nodes.py#L168) — Return superclass for class declarations.
- `type_annotation(extractor: Any, node: tree_sitter.Node)` — [`L151`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_swift_plugin_nodes.py#L151) — Return a Swift type annotation without the leading colon.
- `type_name(extractor: Any, node: tree_sitter.Node)` — [`L130`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_swift_plugin_nodes.py#L130) — Return the declared Swift type name.
- `variable_name(extractor: Any, node: tree_sitter.Node)` — [`L139`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_swift_plugin_nodes.py#L139) — Return the declared Swift property name.
- `visibility(modifiers: list[str])` — [`L86`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_swift_plugin_nodes.py#L86) — Return Swift visibility, defaulting to internal.
- `walk(root: tree_sitter.Node)` — [`L16`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_swift_plugin_nodes.py#L16) — Return root and descendants in source order.

## Module values
- `TYPE_DECLARATION_KINDS` — [`L13`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_swift_plugin_nodes.py#L13)
- `VISIBILITY_MODIFIERS` — [`L12`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_swift_plugin_nodes.py#L12)

