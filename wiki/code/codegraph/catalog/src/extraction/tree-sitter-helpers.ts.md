---
title: 'Module: src/extraction/tree-sitter-helpers.ts'
type: catalog
provenance: extracted
module: src/extraction/tree-sitter-helpers.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/extraction/`tree-sitter-helpers.ts`/
symbols:
  getNodeText: getNodeText().
  getChildByField: getChildByField().
  generateNodeId: generateNodeId().
  getPrecedingDocstring: getPrecedingDocstring().
  DOCSTRING_WRAPPER_TYPES: DOCSTRING_WRAPPER_TYPES.
  cleanCommentMarkers: cleanCommentMarkers().
---
# Module: [`src/extraction/tree-sitter-helpers.ts`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-helpers.ts)

## Functions
- `cleanCommentMarkers(comment: string)` — [`L77`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-helpers.ts#L77) — Strip comment-syntax markers from a raw comment so the stored docstring is
- `generateNodeId(filePath: string, kind: "function" | "file" | "module" | "class" | "struct" | "interface" | "trait" | "protocol" | "method" | "property" | "field" | "variable" | "constant" | "enum" | ... 7 more ... | "component", name: string, line: number)` — [`L18`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-helpers.ts#L18) — Generate a unique node ID — documented in [extraction-tree-sitter-helpers.ts](../../../concepts/extraction-tree-sitter-helpers.ts.md)
- `getChildByField(node: Node, fieldName: string)` — [`L42`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-helpers.ts#L42) — Find a child node by field name — documented in [extraction-function-ref.ts](../../../concepts/extraction-function-ref.ts.md)
- `getNodeText(node: Node, source: string)` — [`L35`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-helpers.ts#L35) — Extract text from a syntax node — documented in [extraction-function-ref.ts](../../../concepts/extraction-function-ref.ts.md)
- `getPrecedingDocstring(node: Node, source: string)` — [`L95`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-helpers.ts#L95) — Get the docstring/comment preceding a node — documented in [extraction-tree-sitter-helpers.ts](../../../concepts/extraction-tree-sitter-helpers.ts.md)

## Module values
- `DOCSTRING_WRAPPER_TYPES` — [`L55`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-helpers.ts#L55) — Node types that *wrap* a declaration so a leading comment is a sibling of the

