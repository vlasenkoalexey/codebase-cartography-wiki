---
title: 'Module: understand-anything-plugin/packages/core/src/fingerprint.ts'
type: catalog
provenance: extracted
module: understand-anything-plugin/packages/core/src/fingerprint.ts
status: fresh
symbol_base: scip-typescript npm @understand-anything/core 0.1.0 src/`fingerprint.ts`/
symbols:
  extractFileFingerprint: extractFileFingerprint().
  compareFingerprints: compareFingerprints().
  analyzeChanges: analyzeChanges().
  buildFingerprintStore: buildFingerprintStore().
  FileFingerprint.classes: FileFingerprint#classes.
  FileFingerprint.functions: FileFingerprint#functions.
  FileChangeResult.changeLevel: FileChangeResult#changeLevel.
  FileFingerprint: FileFingerprint#
  FileFingerprint.contentHash: FileFingerprint#contentHash.
  FileFingerprint.imports: FileFingerprint#imports.
  FileChangeResult.details: FileChangeResult#details.
  FileFingerprint.hasStructuralAnalysis: FileFingerprint#hasStructuralAnalysis.
  FunctionFingerprint.name: FunctionFingerprint#name.
  FileFingerprint.filePath: FileFingerprint#filePath.
  FileFingerprint.exports: FileFingerprint#exports.
  ClassFingerprint.name: ClassFingerprint#name.
  FingerprintStore: FingerprintStore#
  FunctionFingerprint.lineCount: FunctionFingerprint#lineCount.
  ClassFingerprint.methods: ClassFingerprint#methods.
  ClassFingerprint.properties: ClassFingerprint#properties.
  contentHash: contentHash().
  ImportFingerprint.specifiers: ImportFingerprint#specifiers.
  FileFingerprint.totalLines: FileFingerprint#totalLines.
  FingerprintStore.files: FingerprintStore#files.
  FunctionFingerprint.params: FunctionFingerprint#params.
  FunctionFingerprint.exported: FunctionFingerprint#exported.
  ChangeAnalysis: ChangeAnalysis#
  ChangeAnalysis.fileChanges: ChangeAnalysis#fileChanges.
  ClassFingerprint.exported: ClassFingerprint#exported.
  ChangeAnalysis.deletedFiles: ChangeAnalysis#deletedFiles.
  FunctionFingerprint.returnType: FunctionFingerprint#returnType.
  ImportFingerprint.source: ImportFingerprint#source.
  FileChangeResult.filePath: FileChangeResult#filePath.
  ChangeAnalysis.newFiles: ChangeAnalysis#newFiles.
  ClassFingerprint.lineCount: ClassFingerprint#lineCount.
  ChangeAnalysis.structurallyChangedFiles: ChangeAnalysis#structurallyChangedFiles.
  FileChangeResult: FileChangeResult#
  FunctionFingerprint: FunctionFingerprint#
  ClassFingerprint: ClassFingerprint#
  ImportFingerprint: ImportFingerprint#
  FingerprintStore.version: FingerprintStore#version.
  FingerprintStore.gitCommitHash: FingerprintStore#gitCommitHash.
  FingerprintStore.generatedAt: FingerprintStore#generatedAt.
  ChangeAnalysis.cosmeticOnlyFiles: ChangeAnalysis#cosmeticOnlyFiles.
  ChangeAnalysis.unchangedFiles: ChangeAnalysis#unchangedFiles.
  ChangeLevel: ChangeLevel#
---
# Module: [`understand-anything-plugin/packages/core/src/fingerprint.ts`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/fingerprint.ts)

## Classes
### `ChangeAnalysis`
- def: [`understand-anything-plugin/packages/core/src/fingerprint.ts:56`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/fingerprint.ts#L56)
- signature: `interface ChangeAnalysis`
- members:
  - `cosmeticOnlyFiles` — [`L61`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/fingerprint.ts#L61)
  - `deletedFiles` — [`L59`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/fingerprint.ts#L59)
  - `fileChanges` — [`L57`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/fingerprint.ts#L57)
  - `newFiles` — [`L58`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/fingerprint.ts#L58)
  - `structurallyChangedFiles` — [`L60`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/fingerprint.ts#L60)
  - `unchangedFiles` — [`L62`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/fingerprint.ts#L62)
- uses (calls/refs, reference-scoped): [`FileChangeResult`](fingerprint.ts.md#FileChangeResult)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-index.ts), [`fingerprint.test.ts`](__tests__/fingerprint.test.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-__tests__-fingerprint.test.ts), [`analyzeChanges`](fingerprint.ts.md#analyzeChanges), [`classifyUpdate`](change-classifier.ts.md#classifyUpdate), [`makeAnalysis`](__tests__/change-classifier.test.ts.md#makeAnalysis), [`change-classifier.test.ts`](__tests__/change-classifier.test.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-__tests__-change-classifier.test.ts), [`summarizeChanges`](change-classifier.ts.md#summarizeChanges), [`change-classifier.ts`](change-classifier.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-change-classifier.ts)

### `ChangeLevel`
- def: [`understand-anything-plugin/packages/core/src/fingerprint.ts:48`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/fingerprint.ts#L48)
- signature: `type ChangeLevel`
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-index.ts), [`changeLevel`](fingerprint.ts.md#FileChangeResult.changeLevel)

### `ClassFingerprint`
- def: [`understand-anything-plugin/packages/core/src/fingerprint.ts:17`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/fingerprint.ts#L17)
- signature: `interface ClassFingerprint`
- members:
  - `exported` — [`L21`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/fingerprint.ts#L21)
  - `lineCount` — [`L22`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/fingerprint.ts#L22)
  - `methods` — [`L19`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/fingerprint.ts#L19) — documented in [understand-anything-plugin-packages-core-src-fingerprint.ts](../../../../../concepts/understand-anything-plugin-packages-core-src-fingerprint.ts.md)
  - `name` — [`L18`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/fingerprint.ts#L18)
  - `properties` — [`L20`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/fingerprint.ts#L20) — documented in [understand-anything-plugin-packages-core-src-fingerprint.ts](../../../../../concepts/understand-anything-plugin-packages-core-src-fingerprint.ts.md)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-index.ts), [`fingerprint.test.ts`](__tests__/fingerprint.test.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-__tests__-fingerprint.test.ts), [`extractFileFingerprint`](fingerprint.ts.md#extractFileFingerprint), [`compareFingerprints`](fingerprint.ts.md#compareFingerprints), [`classes`](fingerprint.ts.md#FileFingerprint.classes)

### `FileChangeResult`
- def: [`understand-anything-plugin/packages/core/src/fingerprint.ts:50`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/fingerprint.ts#L50)
- signature: `interface FileChangeResult`
- members:
  - `changeLevel` — [`L52`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/fingerprint.ts#L52) — documented in [understand-anything-plugin-packages-core-src-fingerprint.ts](../../../../../concepts/understand-anything-plugin-packages-core-src-fingerprint.ts.md)
  - `details` — [`L53`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/fingerprint.ts#L53) — documented in [understand-anything-plugin-packages-core-src-fingerprint.ts](../../../../../concepts/understand-anything-plugin-packages-core-src-fingerprint.ts.md)
  - `filePath` — [`L51`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/fingerprint.ts#L51)
- uses (calls/refs, reference-scoped): [`ChangeLevel`](fingerprint.ts.md#ChangeLevel)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-index.ts), [`fingerprint.test.ts`](__tests__/fingerprint.test.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-__tests__-fingerprint.test.ts), [`analyzeChanges`](fingerprint.ts.md#analyzeChanges), [`compareFingerprints`](fingerprint.ts.md#compareFingerprints), [`fileChanges`](fingerprint.ts.md#ChangeAnalysis.fileChanges)

### `FileFingerprint`
- def: [`understand-anything-plugin/packages/core/src/fingerprint.ts:30`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/fingerprint.ts#L30) — documented in [understand-anything-plugin-packages-core-src-fingerprint.ts](../../../../../concepts/understand-anything-plugin-packages-core-src-fingerprint.ts.md)
- signature: `interface FileFingerprint`
- members:
  - `classes` — [`L34`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/fingerprint.ts#L34) — documented in [understand-anything-plugin-packages-core-src-fingerprint.ts](../../../../../concepts/understand-anything-plugin-packages-core-src-fingerprint.ts.md)
  - `contentHash` — [`L32`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/fingerprint.ts#L32) — documented in [understand-anything-plugin-packages-core-src-fingerprint.ts](../../../../../concepts/understand-anything-plugin-packages-core-src-fingerprint.ts.md)
  - `exports` — [`L36`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/fingerprint.ts#L36) — documented in [understand-anything-plugin-packages-core-src-fingerprint.ts](../../../../../concepts/understand-anything-plugin-packages-core-src-fingerprint.ts.md)
  - `filePath` — [`L31`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/fingerprint.ts#L31) — documented in [understand-anything-plugin-packages-core-src-fingerprint.ts](../../../../../concepts/understand-anything-plugin-packages-core-src-fingerprint.ts.md)
  - `functions` — [`L33`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/fingerprint.ts#L33) — documented in [understand-anything-plugin-packages-core-src-fingerprint.ts](../../../../../concepts/understand-anything-plugin-packages-core-src-fingerprint.ts.md)
  - `hasStructuralAnalysis` — [`L38`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/fingerprint.ts#L38) — documented in [understand-anything-plugin-packages-core-src-fingerprint.ts](../../../../../concepts/understand-anything-plugin-packages-core-src-fingerprint.ts.md)
  - `imports` — [`L35`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/fingerprint.ts#L35) — documented in [understand-anything-plugin-packages-core-src-fingerprint.ts](../../../../../concepts/understand-anything-plugin-packages-core-src-fingerprint.ts.md)
  - `totalLines` — [`L37`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/fingerprint.ts#L37)
- uses (calls/refs, reference-scoped): [`ClassFingerprint`](fingerprint.ts.md#ClassFingerprint), [`FunctionFingerprint`](fingerprint.ts.md#FunctionFingerprint), [`ImportFingerprint`](fingerprint.ts.md#ImportFingerprint)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-index.ts), [`persistence.test.ts`](persistence/persistence.test.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-persistence-persistence.test.ts), [`fingerprint.test.ts`](__tests__/fingerprint.test.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-__tests__-fingerprint.test.ts), [`extractFileFingerprint`](fingerprint.ts.md#extractFileFingerprint), [`analyzeChanges`](fingerprint.ts.md#analyzeChanges), [`compareFingerprints`](fingerprint.ts.md#compareFingerprints), [`buildFingerprintStore`](fingerprint.ts.md#buildFingerprintStore), [`files`](fingerprint.ts.md#FingerprintStore.files)

### `FingerprintStore`
- def: [`understand-anything-plugin/packages/core/src/fingerprint.ts:41`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/fingerprint.ts#L41) — documented in [understand-anything-plugin-packages-core-src-fingerprint.ts](../../../../../concepts/understand-anything-plugin-packages-core-src-fingerprint.ts.md)
- signature: `interface FingerprintStore`
- members:
  - `files` — [`L45`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/fingerprint.ts#L45)
  - `generatedAt` — [`L44`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/fingerprint.ts#L44)
  - `gitCommitHash` — [`L43`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/fingerprint.ts#L43)
  - `version` — [`L42`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/fingerprint.ts#L42)
- uses (calls/refs, reference-scoped): [`FileFingerprint`](fingerprint.ts.md#FileFingerprint)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-index.ts), [`persistence.test.ts`](persistence/persistence.test.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-persistence-persistence.test.ts), [`fingerprint.test.ts`](__tests__/fingerprint.test.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-__tests__-fingerprint.test.ts), [`analyzeChanges`](fingerprint.ts.md#analyzeChanges), [`buildFingerprintStore`](fingerprint.ts.md#buildFingerprintStore), [`index.ts`](persistence/index.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-persistence-index.ts), [`loadFingerprints`](persistence/index.ts.md#loadFingerprints), [`saveFingerprints`](persistence/index.ts.md#saveFingerprints)

### `FunctionFingerprint`
- def: [`understand-anything-plugin/packages/core/src/fingerprint.ts:9`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/fingerprint.ts#L9)
- signature: `interface FunctionFingerprint`
- members:
  - `exported` — [`L13`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/fingerprint.ts#L13)
  - `lineCount` — [`L14`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/fingerprint.ts#L14)
  - `name` — [`L10`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/fingerprint.ts#L10) — documented in [understand-anything-plugin-packages-core-src-fingerprint.ts](../../../../../concepts/understand-anything-plugin-packages-core-src-fingerprint.ts.md)
  - `params` — [`L11`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/fingerprint.ts#L11)
  - `returnType` — [`L12`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/fingerprint.ts#L12)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-index.ts), [`fingerprint.test.ts`](__tests__/fingerprint.test.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-__tests__-fingerprint.test.ts), [`extractFileFingerprint`](fingerprint.ts.md#extractFileFingerprint), [`compareFingerprints`](fingerprint.ts.md#compareFingerprints), [`functions`](fingerprint.ts.md#FileFingerprint.functions)

### `ImportFingerprint`
- def: [`understand-anything-plugin/packages/core/src/fingerprint.ts:25`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/fingerprint.ts#L25)
- signature: `interface ImportFingerprint`
- members:
  - `source` — [`L26`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/fingerprint.ts#L26)
  - `specifiers` — [`L27`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/fingerprint.ts#L27)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-index.ts), [`fingerprint.test.ts`](__tests__/fingerprint.test.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-__tests__-fingerprint.test.ts), [`extractFileFingerprint`](fingerprint.ts.md#extractFileFingerprint), [`compareFingerprints`](fingerprint.ts.md#compareFingerprints), [`imports`](fingerprint.ts.md#FileFingerprint.imports)

## Functions
- `analyzeChanges(projectDir: string, changedFiles: string[], existingStore: FingerprintStore, registry: PluginRegistry)` — [`L297`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/fingerprint.ts#L297) — Analyze changes between the current state of files and stored fingerprints. — documented in [understand-anything-plugin-packages-core-src-fingerprint.ts](../../../../../concepts/understand-anything-plugin-packages-core-src-fingerprint.ts.md)
- `buildFingerprintStore(projectDir: string, filePaths: string[], registry: PluginRegistry, gitCommitHash: string)` — [`L253`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/fingerprint.ts#L253) — Build a fingerprint store for a set of files. — documented in [understand-anything-plugin-packages-core-src-fingerprint.ts](../../../../../concepts/understand-anything-plugin-packages-core-src-fingerprint.ts.md)
- `compareFingerprints(oldFp: FileFingerprint, newFp: FileFingerprint)` — [`L131`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/fingerprint.ts#L131) — Compare two file fingerprints and determine the change level. — documented in [understand-anything-plugin-packages-core-src-fingerprint.ts](../../../../../concepts/understand-anything-plugin-packages-core-src-fingerprint.ts.md)
- `contentHash(content: string)` — [`L70`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/fingerprint.ts#L70) — Compute SHA-256 content hash for a file's content. — documented in [understand-anything-plugin-packages-core-src-fingerprint.ts](../../../../../concepts/understand-anything-plugin-packages-core-src-fingerprint.ts.md)
- `extractFileFingerprint(filePath: string, content: string, analysis: StructuralAnalysis)` — [`L79`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/fingerprint.ts#L79) — Extract a structural fingerprint from a file using its tree-sitter analysis. — documented in [understand-anything-plugin-packages-core-src-fingerprint.ts](../../../../../concepts/understand-anything-plugin-packages-core-src-fingerprint.ts.md)

