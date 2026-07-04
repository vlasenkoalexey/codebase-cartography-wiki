---
title: 'Module: understand-anything-plugin/packages/core/src/analyzer/graph-builder.ts'
type: catalog
provenance: extracted
module: understand-anything-plugin/packages/core/src/analyzer/graph-builder.ts
status: fresh
symbol_base: scip-typescript npm @understand-anything/core 0.1.0 src/analyzer/`graph-builder.ts`/
symbols:
  GraphBuilder.addNonCodeFileWithAnalysis: GraphBuilder#addNonCodeFileWithAnalysis().
  GraphBuilder.addFileWithAnalysis: GraphBuilder#addFileWithAnalysis().
  GraphBuilder.build: GraphBuilder#build().
  GraphBuilder.addFile: GraphBuilder#addFile().
  GraphBuilder.addNonCodeFile: GraphBuilder#addNonCodeFile().
  FileMeta.complexity: FileMeta#complexity.
  GraphBuilder.-constructor: GraphBuilder#`<constructor>`().
  GraphBuilder.addChildNode: GraphBuilder#addChildNode().
  FileMeta.tags: FileMeta#tags.
  FileMeta.summary: FileMeta#summary.
  GraphBuilder.addImportEdge: GraphBuilder#addImportEdge().
  GraphBuilder.addCallEdge: GraphBuilder#addCallEdge().
  NonCodeFileMeta.nodeType: NonCodeFileMeta#nodeType.
  NonCodeFileMeta: NonCodeFileMeta#
  GraphBuilder.nodes: GraphBuilder#nodes.
  GraphBuilder.edges: GraphBuilder#edges.
  GraphBuilder.mapKindToNodeType: GraphBuilder#mapKindToNodeType().
  GraphBuilder.detectLanguage: GraphBuilder#detectLanguage().
  GraphBuilder.nodeIds: GraphBuilder#nodeIds.
  NonCodeFileAnalysisMeta.definitions: NonCodeFileAnalysisMeta#definitions.
  KIND_TO_NODE_TYPE: KIND_TO_NODE_TYPE.
  NonCodeFileAnalysisMeta.services: NonCodeFileAnalysisMeta#services.
  GraphBuilder: GraphBuilder#
  NonCodeFileAnalysisMeta.endpoints: NonCodeFileAnalysisMeta#endpoints.
  NonCodeFileAnalysisMeta.steps: NonCodeFileAnalysisMeta#steps.
  NonCodeFileAnalysisMeta.resources: NonCodeFileAnalysisMeta#resources.
  GraphBuilder.languageRegistry: GraphBuilder#languageRegistry.
  FileAnalysisMeta.summaries: FileAnalysisMeta#summaries.
  GraphBuilder.languages: GraphBuilder#languages.
  GraphBuilder.edgeKeys: GraphBuilder#edgeKeys.
  FileAnalysisMeta: FileAnalysisMeta#
  NonCodeFileAnalysisMeta: NonCodeFileAnalysisMeta#
  FileMeta: FileMeta#
  FileAnalysisMeta.fileSummary: FileAnalysisMeta#fileSummary.
  GraphBuilder.basename: GraphBuilder#basename().
  NonCodeFileAnalysisMeta.sections: NonCodeFileAnalysisMeta#sections.
  GraphBuilder.projectName: GraphBuilder#projectName.
  GraphBuilder.gitHash: GraphBuilder#gitHash.
---
# Module: [`understand-anything-plugin/packages/core/src/analyzer/graph-builder.ts`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/graph-builder.ts)

## Classes
### `FileAnalysisMeta`
- def: [`understand-anything-plugin/packages/core/src/analyzer/graph-builder.ts:21`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/graph-builder.ts#L21)
- signature: `interface FileAnalysisMeta`
- members:
  - `fileSummary` — [`L23`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/graph-builder.ts#L23)
  - `summaries` — [`L22`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/graph-builder.ts#L22)
- uses (calls/refs, reference-scoped): [`FileMeta`](graph-builder.ts.md#FileMeta)
- used by: [`graph-builder.test.ts`](graph-builder.test.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-analyzer-graph-builder.test.ts), [`addFileWithAnalysis`](graph-builder.ts.md#GraphBuilder.addFileWithAnalysis)

### `FileMeta`
- def: [`understand-anything-plugin/packages/core/src/analyzer/graph-builder.ts:15`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/graph-builder.ts#L15)
- signature: `interface FileMeta`
- members:
  - `complexity` — [`L18`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/graph-builder.ts#L18)
  - `summary` — [`L16`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/graph-builder.ts#L16)
  - `tags` — [`L17`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/graph-builder.ts#L17)
- used by: [`graph-builder.test.ts`](graph-builder.test.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-analyzer-graph-builder.test.ts), [`addNonCodeFileWithAnalysis`](graph-builder.ts.md#GraphBuilder.addNonCodeFileWithAnalysis), [`addFileWithAnalysis`](graph-builder.ts.md#GraphBuilder.addFileWithAnalysis), [`addFile`](graph-builder.ts.md#GraphBuilder.addFile), [`addNonCodeFile`](graph-builder.ts.md#GraphBuilder.addNonCodeFile), [`NonCodeFileMeta`](graph-builder.ts.md#NonCodeFileMeta), [`FileAnalysisMeta`](graph-builder.ts.md#FileAnalysisMeta)

### `GraphBuilder`
- def: [`understand-anything-plugin/packages/core/src/analyzer/graph-builder.ts:60`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/graph-builder.ts#L60)
- signature: `class GraphBuilder`
- members:
  - `<constructor>(projectName: string, gitHash: string, languageRegistry?: LanguageRegistry | undefined)` — [`L70`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/graph-builder.ts#L70)
  - `addCallEdge(method)` — [`L192`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/graph-builder.ts#L192)
  - `addChildNode(method)` — [`L302`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/graph-builder.ts#L302) — documented in [understand-anything-plugin-packages-core-src-analyzer-graph-builder.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-analyzer-graph-builder.ts.md)
  - `addFile(method)` — [`L84`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/graph-builder.ts#L84) — documented in [understand-anything-plugin-packages-core-src-analyzer-graph-builder.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-analyzer-graph-builder.ts.md)
  - `addFileWithAnalysis(method)` — [`L105`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/graph-builder.ts#L105) — documented in [understand-anything-plugin-packages-core-src-analyzer-graph-builder.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-analyzer-graph-builder.ts.md)
  - `addImportEdge(method)` — [`L179`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/graph-builder.ts#L179)
  - `addNonCodeFile(method)` — [`L210`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/graph-builder.ts#L210) — documented in [understand-anything-plugin-packages-core-src-analyzer-graph-builder.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-analyzer-graph-builder.ts.md)
  - `addNonCodeFileWithAnalysis(method)` — [`L228`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/graph-builder.ts#L228) — documented in [understand-anything-plugin-packages-core-src-analyzer-graph-builder.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-analyzer-graph-builder.ts.md)
  - `basename(method)` — [`L80`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/graph-builder.ts#L80)
  - `build(method)` — [`L320`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/graph-builder.ts#L320) — documented in [understand-anything-plugin-packages-core-src-analyzer-graph-builder.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-analyzer-graph-builder.ts.md)
  - `detectLanguage(method)` — [`L76`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/graph-builder.ts#L76)
  - `mapKindToNodeType(method)` — [`L312`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/graph-builder.ts#L312) — documented in [understand-anything-plugin-packages-core-src-analyzer-graph-builder.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-analyzer-graph-builder.ts.md)
  - `edgeKeys` — [`L65`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/graph-builder.ts#L65)
  - `edges` — [`L62`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/graph-builder.ts#L62) — documented in [understand-anything-plugin-packages-core-src-analyzer-graph-builder.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-analyzer-graph-builder.ts.md)
  - `gitHash` — [`L67`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/graph-builder.ts#L67)
  - `languageRegistry` — [`L68`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/graph-builder.ts#L68)
  - `languages` — [`L63`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/graph-builder.ts#L63)
  - `nodeIds` — [`L64`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/graph-builder.ts#L64)
  - `nodes` — [`L61`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/graph-builder.ts#L61) — documented in [understand-anything-plugin-packages-core-src-analyzer-graph-builder.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-analyzer-graph-builder.ts.md)
  - `projectName` — [`L66`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/graph-builder.ts#L66)
- uses (calls/refs, reference-scoped): [`functions`](../types.ts.md#StructuralAnalysis.functions), [`classes`](../types.ts.md#StructuralAnalysis.classes), [`StructuralAnalysis`](../types.ts.md#StructuralAnalysis), [`name`](../types.ts.md#StructuralAnalysis.functions.Array.typeLiteral0.name), [`name`](../types.ts.md#StructuralAnalysis.classes.Array.typeLiteral1.name), [`id`](../types.ts.md#GraphNode.id), [`name`](../types.ts.md#GraphNode.name), [`type`](../types.ts.md#GraphNode.type), [`filePath`](../types.ts.md#GraphNode.filePath), [`nodes`](../types.ts.md#KnowledgeGraph.nodes), [`summary`](../types.ts.md#GraphNode.summary), [`lineRange`](../types.ts.md#StructuralAnalysis.functions.Array.typeLiteral0.lineRange), [`GraphNode`](../types.ts.md#GraphNode), [`KnowledgeGraph`](../types.ts.md#KnowledgeGraph), [`tags`](../types.ts.md#GraphNode.tags), [`lineRange`](../types.ts.md#StructuralAnalysis.classes.Array.typeLiteral1.lineRange), [`complexity`](../types.ts.md#GraphNode.complexity), [`target`](../types.ts.md#GraphEdge.target), [`complexity`](graph-builder.ts.md#FileMeta.complexity), [`source`](../types.ts.md#GraphEdge.source), [`project`](../types.ts.md#KnowledgeGraph.project), [`type`](../types.ts.md#GraphEdge.type), [`LanguageRegistry`](../languages/language-registry.ts.md#LanguageRegistry), [`fields`](../types.ts.md#DefinitionInfo.fields), [`name`](../types.ts.md#DefinitionInfo.name), [`tags`](graph-builder.ts.md#FileMeta.tags), [`edges`](../types.ts.md#KnowledgeGraph.edges), [`getForFile`](../languages/language-registry.ts.md#LanguageRegistry.getForFile), [`summary`](graph-builder.ts.md#FileMeta.summary), [`kind`](../types.ts.md#DefinitionInfo.kind), [`weight`](../types.ts.md#GraphEdge.weight), [`direction`](../types.ts.md#GraphEdge.direction), [`createDefault`](../languages/language-registry.ts.md#LanguageRegistry.createDefault), [`layers`](../types.ts.md#KnowledgeGraph.layers), [`GraphEdge`](../types.ts.md#GraphEdge), [`languages`](../types.ts.md#ProjectMeta.languages), [`lineRange`](../types.ts.md#DefinitionInfo.lineRange), [`lineRange`](../types.ts.md#GraphNode.lineRange), [`tour`](../types.ts.md#KnowledgeGraph.tour), [`analyzedAt`](../types.ts.md#ProjectMeta.analyzedAt)  (+28 more)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-index.ts), [`graph-builder.test.ts`](graph-builder.test.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-analyzer-graph-builder.test.ts)

### `NonCodeFileAnalysisMeta`
- def: [`understand-anything-plugin/packages/core/src/analyzer/graph-builder.ts:30`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/graph-builder.ts#L30)
- signature: `interface NonCodeFileAnalysisMeta`
- members:
  - `definitions` — [`L31`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/graph-builder.ts#L31)
  - `endpoints` — [`L33`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/graph-builder.ts#L33)
  - `resources` — [`L35`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/graph-builder.ts#L35)
  - `sections` — [`L36`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/graph-builder.ts#L36)
  - `services` — [`L32`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/graph-builder.ts#L32)
  - `steps` — [`L34`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/graph-builder.ts#L34)
- uses (calls/refs, reference-scoped): [`DefinitionInfo`](../types.ts.md#DefinitionInfo), [`SectionInfo`](../types.ts.md#SectionInfo), [`NonCodeFileMeta`](graph-builder.ts.md#NonCodeFileMeta), [`EndpointInfo`](../types.ts.md#EndpointInfo), [`StepInfo`](../types.ts.md#StepInfo), [`ServiceInfo`](../types.ts.md#ServiceInfo), [`ResourceInfo`](../types.ts.md#ResourceInfo)
- used by: [`graph-builder.test.ts`](graph-builder.test.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-analyzer-graph-builder.test.ts), [`addNonCodeFileWithAnalysis`](graph-builder.ts.md#GraphBuilder.addNonCodeFileWithAnalysis)

### `NonCodeFileMeta`
- def: [`understand-anything-plugin/packages/core/src/analyzer/graph-builder.ts:26`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/graph-builder.ts#L26)
- signature: `interface NonCodeFileMeta`
- members:
  - `nodeType` — [`L27`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/graph-builder.ts#L27)
- uses (calls/refs, reference-scoped): [`type`](../types.ts.md#GraphNode.type), [`GraphNode`](../types.ts.md#GraphNode), [`FileMeta`](graph-builder.ts.md#FileMeta)
- used by: [`graph-builder.test.ts`](graph-builder.test.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-analyzer-graph-builder.test.ts), [`addNonCodeFile`](graph-builder.ts.md#GraphBuilder.addNonCodeFile), [`NonCodeFileAnalysisMeta`](graph-builder.ts.md#NonCodeFileAnalysisMeta)

## Module values
- `KIND_TO_NODE_TYPE` — [`L39`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/graph-builder.ts#L39)

