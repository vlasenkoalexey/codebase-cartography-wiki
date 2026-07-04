---
title: 'Module: understand-anything-plugin/packages/core/src/plugins/extractors/base-extractor.ts'
type: catalog
provenance: extracted
module: understand-anything-plugin/packages/core/src/plugins/extractors/base-extractor.ts
status: fresh
symbol_base: scip-typescript npm @understand-anything/core 0.1.0 src/plugins/extractors/`base-extractor.ts`/
symbols:
  findChild: findChild().
  findChildren: findChildren().
  getStringValue: getStringValue().
  traverse: traverse().
  hasChildOfType: hasChildOfType().
---
# Module: [`understand-anything-plugin/packages/core/src/plugins/extractors/base-extractor.ts`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/base-extractor.ts)

## Functions
- `findChild(node: any, type: string)` — [`L27`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/base-extractor.ts#L27) — Find the first child matching a type. — documented in [understand-anything-plugin-packages-core-src-plugins-extractors-base-extractor.ts](../../../../../../../concepts/understand-anything-plugin-packages-core-src-plugins-extractors-base-extractor.ts.md)
- `findChildren(node: any, type: string)` — [`L36`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/base-extractor.ts#L36) — Find all children matching a type. — documented in [understand-anything-plugin-packages-core-src-plugins-extractors-base-extractor.ts](../../../../../../../concepts/understand-anything-plugin-packages-core-src-plugins-extractors-base-extractor.ts.md)
- `getStringValue(node: any)` — [`L16`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/base-extractor.ts#L16) — Extract the unquoted string value from a string-like node. — documented in [understand-anything-plugin-packages-core-src-plugins-extractors-base-extractor.ts](../../../../../../../concepts/understand-anything-plugin-packages-core-src-plugins-extractors-base-extractor.ts.md)
- `hasChildOfType(node: any, type: string)` — [`L46`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/base-extractor.ts#L46) — Check if a node has a child of the given type (used for export/visibility checks).
- `traverse(node: any, visitor: (node: any) => void)` — [`L4`](../../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/extractors/base-extractor.ts#L4) — Recursively traverse an AST tree, calling the visitor for each node. — documented in [understand-anything-plugin-packages-core-src-plugins-extractors-base-extractor.ts](../../../../../../../concepts/understand-anything-plugin-packages-core-src-plugins-extractors-base-extractor.ts.md)

