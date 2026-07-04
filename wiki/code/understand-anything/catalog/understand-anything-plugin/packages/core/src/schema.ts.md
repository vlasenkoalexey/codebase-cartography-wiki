---
title: 'Module: understand-anything-plugin/packages/core/src/schema.ts'
type: catalog
provenance: extracted
module: understand-anything-plugin/packages/core/src/schema.ts
status: fresh
symbol_base: scip-typescript npm @understand-anything/core 0.1.0 src/`schema.ts`/
symbols:
  validateGraph: validateGraph().
  ValidationResult.success: ValidationResult#success.
  ValidationResult.data: ValidationResult#data.
  autoFixGraph: autoFixGraph().
  ValidationResult.issues: ValidationResult#issues.
  GraphIssue.level: GraphIssue#level.
  GraphIssue.message: GraphIssue#message.
  GraphIssue.category: GraphIssue#category.
  GraphIssue.path: GraphIssue#path.
  autoFixGraph.typeLiteral28.data: autoFixGraph().typeLiteral28:data.
  KnowledgeGraphSchema: KnowledgeGraphSchema.
  autoFixGraph.typeLiteral28.issues: autoFixGraph().typeLiteral28:issues.
  buildInvalidCollectionIssue: buildInvalidCollectionIssue().
  ValidationResult.fatal: ValidationResult#fatal.
  sanitizeGraph: sanitizeGraph().
  buildErrors: buildErrors().
  GraphNodeSchema: GraphNodeSchema.
  ValidationResult.errors: ValidationResult#errors.
  NODE_TYPE_ALIASES: NODE_TYPE_ALIASES.
  EDGE_TYPE_ALIASES: EDGE_TYPE_ALIASES.
  GraphIssue: GraphIssue#
  normalizeGraph: normalizeGraph().
  GraphEdgeSchema: GraphEdgeSchema.
  COMPLEXITY_ALIASES: COMPLEXITY_ALIASES.
  DIRECTION_ALIASES: DIRECTION_ALIASES.
  LayerSchema: LayerSchema.
  TourStepSchema: TourStepSchema.
  ProjectMetaSchema: ProjectMetaSchema.
  ValidationResult: ValidationResult#
  EdgeTypeSchema: EdgeTypeSchema.
  DomainMetaSchema: DomainMetaSchema.
  KnowledgeMetaSchema: KnowledgeMetaSchema.
---
# Module: [`understand-anything-plugin/packages/core/src/schema.ts`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/schema.ts)

## Classes
### `GraphIssue`
- def: [`understand-anything-plugin/packages/core/src/schema.ts:431`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/schema.ts#L431) — documented in [understand-anything-plugin-packages-core-src-persistence-index.ts](../../../../../concepts/understand-anything-plugin-packages-core-src-persistence-index.ts.md)
- signature: `interface GraphIssue`
- members:
  - `category` — [`L433`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/schema.ts#L433) — documented in [understand-anything-plugin-packages-core-src-persistence-index.ts](../../../../../concepts/understand-anything-plugin-packages-core-src-persistence-index.ts.md)
  - `level` — [`L432`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/schema.ts#L432) — documented in [understand-anything-plugin-packages-core-src-persistence-index.ts](../../../../../concepts/understand-anything-plugin-packages-core-src-persistence-index.ts.md)
  - `message` — [`L434`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/schema.ts#L434) — documented in [understand-anything-plugin-packages-core-src-persistence-index.ts](../../../../../concepts/understand-anything-plugin-packages-core-src-persistence-index.ts.md)
  - `path` — [`L435`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/schema.ts#L435) — documented in [understand-anything-plugin-packages-core-src-persistence-index.ts](../../../../../concepts/understand-anything-plugin-packages-core-src-persistence-index.ts.md)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-index.ts), [`schema.test.ts`](__tests__/schema.test.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-__tests__-schema.test.ts), [`validateGraph`](schema.ts.md#validateGraph), [`autoFixGraph`](schema.ts.md#autoFixGraph), [`issues`](schema.ts.md#ValidationResult.issues), [`buildInvalidCollectionIssue`](schema.ts.md#buildInvalidCollectionIssue), [`buildErrors`](schema.ts.md#buildErrors)

### `ValidationResult`
- def: [`understand-anything-plugin/packages/core/src/schema.ts:438`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/schema.ts#L438) — documented in [understand-anything-plugin-packages-core-src-persistence-index.ts](../../../../../concepts/understand-anything-plugin-packages-core-src-persistence-index.ts.md)
- signature: `interface ValidationResult`
- members:
  - `data` — [`L440`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/schema.ts#L440) — documented in [understand-anything-plugin-packages-core-src-persistence-index.ts](../../../../../concepts/understand-anything-plugin-packages-core-src-persistence-index.ts.md)
  - `errors` — [`L442`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/schema.ts#L442) — documented in [understand-anything-plugin-packages-core-src-schema.ts](../../../../../concepts/understand-anything-plugin-packages-core-src-schema.ts.md)
  - `fatal` — [`L444`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/schema.ts#L444) — documented in [understand-anything-plugin-packages-core-src-persistence-index.ts](../../../../../concepts/understand-anything-plugin-packages-core-src-persistence-index.ts.md)
  - `issues` — [`L443`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/schema.ts#L443) — documented in [understand-anything-plugin-packages-core-src-persistence-index.ts](../../../../../concepts/understand-anything-plugin-packages-core-src-persistence-index.ts.md)
  - `success` — [`L439`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/schema.ts#L439) — documented in [understand-anything-plugin-packages-core-src-persistence-index.ts](../../../../../concepts/understand-anything-plugin-packages-core-src-persistence-index.ts.md)
- uses (calls/refs, reference-scoped): [`KnowledgeGraphSchema`](schema.ts.md#KnowledgeGraphSchema), [`GraphIssue`](schema.ts.md#GraphIssue)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-index.ts), [`schema.test.ts`](__tests__/schema.test.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-__tests__-schema.test.ts), [`validateGraph`](schema.ts.md#validateGraph), [`domain-types.test.ts`](__tests__/domain-types.test.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-__tests__-domain-types.test.ts), [`normalize-graph.test.ts`](__tests__/normalize-graph.test.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-__tests__-normalize-graph.test.ts), [`loadGraph`](persistence/index.ts.md#loadGraph), [`loadDomainGraph`](persistence/index.ts.md#loadDomainGraph)

## Functions
- `autoFixGraph(data: Record<string, unknown>)` — [`L196`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/schema.ts#L196) — documented in [understand-anything-plugin-packages-core-src-persistence-index.ts](../../../../../concepts/understand-anything-plugin-packages-core-src-persistence-index.ts.md)
- `buildErrors(issues: GraphIssue[], fatal?: string | undefined)` — [`L456`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/schema.ts#L456) — documented in [understand-anything-plugin-packages-core-src-schema.ts](../../../../../concepts/understand-anything-plugin-packages-core-src-schema.ts.md)
- `buildInvalidCollectionIssue(name: string)` — [`L447`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/schema.ts#L447) — documented in [understand-anything-plugin-packages-core-src-persistence-index.ts](../../../../../concepts/understand-anything-plugin-packages-core-src-persistence-index.ts.md)
- `normalizeGraph(data: unknown)` — [`L462`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/schema.ts#L462) — documented in [understand-anything-plugin-packages-core-src-persistence-index.ts](../../../../../concepts/understand-anything-plugin-packages-core-src-persistence-index.ts.md)
- `sanitizeGraph(data: Record<string, unknown>)` — [`L148`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/schema.ts#L148) — documented in [understand-anything-plugin-packages-core-src-persistence-index.ts](../../../../../concepts/understand-anything-plugin-packages-core-src-persistence-index.ts.md)
- `validateGraph(data: unknown)` — [`L499`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/schema.ts#L499) — documented in [understand-anything-plugin-packages-core-src-persistence-index.ts](../../../../../concepts/understand-anything-plugin-packages-core-src-persistence-index.ts.md)

## Module values
- `COMPLEXITY_ALIASES` — [`L128`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/schema.ts#L128) — documented in [understand-anything-plugin-packages-core-src-schema.ts](../../../../../concepts/understand-anything-plugin-packages-core-src-schema.ts.md)
- `DIRECTION_ALIASES` — [`L139`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/schema.ts#L139) — documented in [understand-anything-plugin-packages-core-src-schema.ts](../../../../../concepts/understand-anything-plugin-packages-core-src-schema.ts.md)
- `DomainMetaSchema` — [`L353`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/schema.ts#L353)
- `EDGE_TYPE_ALIASES` — [`L78`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/schema.ts#L78) — documented in [understand-anything-plugin-packages-core-src-persistence-index.ts](../../../../../concepts/understand-anything-plugin-packages-core-src-persistence-index.ts.md)
- `EdgeTypeSchema` — [`L4`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/schema.ts#L4)
- `GraphEdgeSchema` — [`L388`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/schema.ts#L388) — documented in [understand-anything-plugin-packages-core-src-schema.ts](../../../../../concepts/understand-anything-plugin-packages-core-src-schema.ts.md)
- `GraphNodeSchema` — [`L368`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/schema.ts#L368) — documented in [understand-anything-plugin-packages-core-src-schema.ts](../../../../../concepts/understand-anything-plugin-packages-core-src-schema.ts.md)
- `KnowledgeGraphSchema` — [`L421`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/schema.ts#L421) — documented in [understand-anything-plugin-packages-core-src-schema.ts](../../../../../concepts/understand-anything-plugin-packages-core-src-schema.ts.md)
- `KnowledgeMetaSchema` — [`L361`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/schema.ts#L361)
- `LayerSchema` — [`L397`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/schema.ts#L397) — documented in [understand-anything-plugin-packages-core-src-schema.ts](../../../../../concepts/understand-anything-plugin-packages-core-src-schema.ts.md)
- `NODE_TYPE_ALIASES` — [`L17`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/schema.ts#L17) — documented in [understand-anything-plugin-packages-core-src-persistence-index.ts](../../../../../concepts/understand-anything-plugin-packages-core-src-persistence-index.ts.md)
- `ProjectMetaSchema` — [`L412`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/schema.ts#L412) — documented in [understand-anything-plugin-packages-core-src-schema.ts](../../../../../concepts/understand-anything-plugin-packages-core-src-schema.ts.md)
- `TourStepSchema` — [`L404`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/schema.ts#L404) — documented in [understand-anything-plugin-packages-core-src-schema.ts](../../../../../concepts/understand-anything-plugin-packages-core-src-schema.ts.md)
- `data` — [`L197`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/schema.ts#L197) — documented in [understand-anything-plugin-packages-core-src-schema.ts](../../../../../concepts/understand-anything-plugin-packages-core-src-schema.ts.md)
- `issues` — [`L198`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/schema.ts#L198) — documented in [understand-anything-plugin-packages-core-src-schema.ts](../../../../../concepts/understand-anything-plugin-packages-core-src-schema.ts.md)

