---
title: 'Module: src/extraction/languages/vbnet.ts'
type: catalog
provenance: extracted
module: src/extraction/languages/vbnet.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/extraction/languages/`vbnet.ts`/
symbols:
  hasModifier: hasModifier().
  extractVbnetReturnType: extractVbnetReturnType().
  vbnetExtractor: vbnetExtractor.
  ensureTrailingNewline: ensureTrailingNewline().
---
# Module: [`src/extraction/languages/vbnet.ts`](../../../../../../../raw/code/codegraph/src/extraction/languages/vbnet.ts)

## Functions
- `ensureTrailingNewline(source: string)` — [`L12`](../../../../../../../raw/code/codegraph/src/extraction/languages/vbnet.ts#L12) — The vendored VB.NET grammar has no true end-of-file token (its `_eof` rule is
- `extractVbnetReturnType(node: Node, source: string)` — [`L33`](../../../../../../../raw/code/codegraph/src/extraction/languages/vbnet.ts#L33) — A VB.NET method's declared return type (`Function Foo(...) As Bar`),
- `hasModifier(node: Node, re: RegExp)` — [`L17`](../../../../../../../raw/code/codegraph/src/extraction/languages/vbnet.ts#L17) — Case-insensitive member-modifier scan (VB keywords are case-insensitive).

## Module values
- `vbnetExtractor` — [`L46`](../../../../../../../raw/code/codegraph/src/extraction/languages/vbnet.ts#L46)

