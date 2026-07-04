---
title: 'Module: packages/core/src/splitter/ast-splitter.ts'
type: catalog
provenance: extracted
module: packages/core/src/splitter/ast-splitter.ts
status: fresh
symbol_base: scip-typescript npm @zilliz/claude-context-core 0.1.15 src/splitter/`ast-splitter.ts`/
symbols:
  AstCodeSplitter.getLanguageConfig: AstCodeSplitter#getLanguageConfig().
  AstCodeSplitter.splitLargeChunk: AstCodeSplitter#splitLargeChunk().
  AstCodeSplitter.extractChunks: AstCodeSplitter#extractChunks().
  SPLITTABLE_NODE_TYPES: SPLITTABLE_NODE_TYPES.
  AstCodeSplitter.addOverlap: AstCodeSplitter#addOverlap().
  AstCodeSplitter.-constructor: AstCodeSplitter#`<constructor>`().
  AstCodeSplitter.split: AstCodeSplitter#split().
  AstCodeSplitter.refineChunks: AstCodeSplitter#refineChunks().
  AstCodeSplitter: AstCodeSplitter#
  AstCodeSplitter.langchainFallback: AstCodeSplitter#langchainFallback.
  AstCodeSplitter.chunkOverlap: AstCodeSplitter#chunkOverlap.
  AstCodeSplitter.setChunkSize: AstCodeSplitter#setChunkSize().
  AstCodeSplitter.setChunkOverlap: AstCodeSplitter#setChunkOverlap().
  AstCodeSplitter.chunkSize: AstCodeSplitter#chunkSize.
  Cpp: Cpp.
  AstCodeSplitter.parser: AstCodeSplitter#parser.
  JavaScript: JavaScript.
  TypeScript: TypeScript.
  Python: Python.
  Rust: Rust.
  CSharp: CSharp.
  Java: Java.
  Go: Go.
  Scala: Scala.
  AstCodeSplitter.getLineCount: AstCodeSplitter#getLineCount().
  AstCodeSplitter.isLanguageSupported: AstCodeSplitter#isLanguageSupported().
---
# Module: [`packages/core/src/splitter/ast-splitter.ts`](../../../../../../../../raw/code/claude-context/packages/core/src/splitter/ast-splitter.ts)

## Classes
### `AstCodeSplitter`  ·  implements/extends Splitter
- def: [`packages/core/src/splitter/ast-splitter.ts:28`](../../../../../../../../raw/code/claude-context/packages/core/src/splitter/ast-splitter.ts#L28) — documented in [packages-core-src-splitter-index.ts](../../../../../concepts/packages-core-src-splitter-index.ts.md)
- signature: `class AstCodeSplitter`
- members:
  - `<constructor>(chunkSize?: number | undefined, chunkOverlap?: number | undefined)` — [`L34`](../../../../../../../../raw/code/claude-context/packages/core/src/splitter/ast-splitter.ts#L34)
  - `addOverlap(method)` — [`L228`](../../../../../../../../raw/code/claude-context/packages/core/src/splitter/ast-splitter.ts#L228) — documented in [packages-core-src-splitter-index.ts](../../../../../concepts/packages-core-src-splitter-index.ts.md)
  - `extractChunks(method)` — [`L109`](../../../../../../../../raw/code/claude-context/packages/core/src/splitter/ast-splitter.ts#L109) — documented in [packages-core-src-splitter-ast-splitter.ts](../../../../../concepts/packages-core-src-splitter-ast-splitter.ts.md)
  - `getLanguageConfig(method)` — [`L86`](../../../../../../../../raw/code/claude-context/packages/core/src/splitter/ast-splitter.ts#L86) — documented in [packages-core-src-splitter-ast-splitter.ts](../../../../../concepts/packages-core-src-splitter-ast-splitter.ts.md)
  - `getLineCount(method)` — [`L256`](../../../../../../../../raw/code/claude-context/packages/core/src/splitter/ast-splitter.ts#L256)
  - `isLanguageSupported(method)` — [`L263`](../../../../../../../../raw/code/claude-context/packages/core/src/splitter/ast-splitter.ts#L263) — Check if AST splitting is supported for the given language
  - `refineChunks(method)` — [`L164`](../../../../../../../../raw/code/claude-context/packages/core/src/splitter/ast-splitter.ts#L164) — documented in [packages-core-src-splitter-ast-splitter.ts](../../../../../concepts/packages-core-src-splitter-ast-splitter.ts.md)
  - `setChunkOverlap(method)` — [`L81`](../../../../../../../../raw/code/claude-context/packages/core/src/splitter/ast-splitter.ts#L81) — Set chunk overlap size
  - `setChunkSize(method)` — [`L76`](../../../../../../../../raw/code/claude-context/packages/core/src/splitter/ast-splitter.ts#L76) — Set chunk size
  - `split(method)` — [`L44`](../../../../../../../../raw/code/claude-context/packages/core/src/splitter/ast-splitter.ts#L44) — Split code into code chunks — documented in [packages-core-src-splitter-ast-splitter.ts](../../../../../concepts/packages-core-src-splitter-ast-splitter.ts.md)
  - `splitLargeChunk(method)` — [`L180`](../../../../../../../../raw/code/claude-context/packages/core/src/splitter/ast-splitter.ts#L180) — documented in [packages-core-src-splitter-ast-splitter.ts](../../../../../concepts/packages-core-src-splitter-ast-splitter.ts.md)
  - `chunkOverlap` — [`L30`](../../../../../../../../raw/code/claude-context/packages/core/src/splitter/ast-splitter.ts#L30)
  - `chunkSize` — [`L29`](../../../../../../../../raw/code/claude-context/packages/core/src/splitter/ast-splitter.ts#L29) — documented in [packages-core-src-splitter-ast-splitter.ts](../../../../../concepts/packages-core-src-splitter-ast-splitter.ts.md)
  - `langchainFallback` — [`L32`](../../../../../../../../raw/code/claude-context/packages/core/src/splitter/ast-splitter.ts#L32)
  - `parser` — [`L31`](../../../../../../../../raw/code/claude-context/packages/core/src/splitter/ast-splitter.ts#L31)
- uses (calls/refs, reference-scoped): [`Splitter`](index.ts.md#Splitter), [`metadata`](index.ts.md#CodeChunk.metadata), [`CodeChunk`](index.ts.md#CodeChunk), [`content`](index.ts.md#CodeChunk.content), [`filePath`](index.ts.md#CodeChunk.metadata.typeLiteral52.filePath), [`startLine`](index.ts.md#CodeChunk.metadata.typeLiteral52.startLine), [`SPLITTABLE_NODE_TYPES`](ast-splitter.ts.md#SPLITTABLE_NODE_TYPES), [`endLine`](index.ts.md#CodeChunk.metadata.typeLiteral52.endLine), [`language`](index.ts.md#CodeChunk.metadata.typeLiteral52.language), [`Cpp`](ast-splitter.ts.md#Cpp), [`CSharp`](ast-splitter.ts.md#CSharp), [`JavaScript`](ast-splitter.ts.md#JavaScript), [`Python`](ast-splitter.ts.md#Python), [`Rust`](ast-splitter.ts.md#Rust), [`TypeScript`](ast-splitter.ts.md#TypeScript), [`Go`](ast-splitter.ts.md#Go), [`Java`](ast-splitter.ts.md#Java), [`Scala`](ast-splitter.ts.md#Scala)
- used by: [`<constructor>`](../context.ts.md#Context.-constructor), [`reloadContextConfiguration`](../../../vscode-extension/src/extension.ts.md#reloadContextConfiguration), [`context.ts`](../context.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-context.ts), [`createContextWithConfig`](../../../vscode-extension/src/extension.ts.md#createContextWithConfig), [`extension.ts`](../../../vscode-extension/src/extension.ts.md#scip-typescript-npm-semanticcodesearch-0.1.11-src-extension.ts), [`configManager.ts`](../../../vscode-extension/src/config/configManager.ts.md#scip-typescript-npm-semanticcodesearch-0.1.11-src-config-configManager.ts), [`Splitter`](index.ts.md#Splitter), [`SPLITTER_PROVIDERS`](../../../vscode-extension/src/config/configManager.ts.md#SPLITTER_PROVIDERS), [`split`](index.ts.md#Splitter.split), [`setChunkOverlap`](index.ts.md#Splitter.setChunkOverlap), [`setChunkSize`](index.ts.md#Splitter.setChunkSize)

## Module values
- `CSharp` — [`L12`](../../../../../../../../raw/code/claude-context/packages/core/src/splitter/ast-splitter.ts#L12) — documented in [packages-core-src-splitter-ast-splitter.ts](../../../../../concepts/packages-core-src-splitter-ast-splitter.ts.md)
- `Cpp` — [`L9`](../../../../../../../../raw/code/claude-context/packages/core/src/splitter/ast-splitter.ts#L9) — documented in [packages-core-src-splitter-ast-splitter.ts](../../../../../concepts/packages-core-src-splitter-ast-splitter.ts.md)
- `Go` — [`L10`](../../../../../../../../raw/code/claude-context/packages/core/src/splitter/ast-splitter.ts#L10) — documented in [packages-core-src-splitter-ast-splitter.ts](../../../../../concepts/packages-core-src-splitter-ast-splitter.ts.md)
- `Java` — [`L8`](../../../../../../../../raw/code/claude-context/packages/core/src/splitter/ast-splitter.ts#L8) — documented in [packages-core-src-splitter-ast-splitter.ts](../../../../../concepts/packages-core-src-splitter-ast-splitter.ts.md)
- `JavaScript` — [`L5`](../../../../../../../../raw/code/claude-context/packages/core/src/splitter/ast-splitter.ts#L5) — documented in [packages-core-src-splitter-ast-splitter.ts](../../../../../concepts/packages-core-src-splitter-ast-splitter.ts.md)
- `Python` — [`L7`](../../../../../../../../raw/code/claude-context/packages/core/src/splitter/ast-splitter.ts#L7) — documented in [packages-core-src-splitter-ast-splitter.ts](../../../../../concepts/packages-core-src-splitter-ast-splitter.ts.md)
- `Rust` — [`L11`](../../../../../../../../raw/code/claude-context/packages/core/src/splitter/ast-splitter.ts#L11) — documented in [packages-core-src-splitter-ast-splitter.ts](../../../../../concepts/packages-core-src-splitter-ast-splitter.ts.md)
- `SPLITTABLE_NODE_TYPES` — [`L16`](../../../../../../../../raw/code/claude-context/packages/core/src/splitter/ast-splitter.ts#L16) — documented in [packages-core-src-splitter-ast-splitter.ts](../../../../../concepts/packages-core-src-splitter-ast-splitter.ts.md)
- `Scala` — [`L13`](../../../../../../../../raw/code/claude-context/packages/core/src/splitter/ast-splitter.ts#L13) — documented in [packages-core-src-splitter-ast-splitter.ts](../../../../../concepts/packages-core-src-splitter-ast-splitter.ts.md)
- `TypeScript` — [`L6`](../../../../../../../../raw/code/claude-context/packages/core/src/splitter/ast-splitter.ts#L6) — documented in [packages-core-src-splitter-ast-splitter.ts](../../../../../concepts/packages-core-src-splitter-ast-splitter.ts.md)

