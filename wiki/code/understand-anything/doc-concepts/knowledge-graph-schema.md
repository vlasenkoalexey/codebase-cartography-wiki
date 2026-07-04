---
title: Knowledge graph schema (the code representation)
type: doc-concept
provenance: doc
source: docs/superpowers/specs/2026-03-14-understand-anything-design.md
updated: 2026-07-04
status: fresh
---
# Knowledge graph schema (the code representation)

## Definition
Understand-Anything represents a codebase as a single JSON **knowledge graph**:
typed nodes (file, function, class, module, concept, …), typed edges (structural
`imports`/`contains`/`inherits`, behavioral `calls`/`publishes`, data-flow
`reads_from`/`writes_to`, semantic `related`/`similar_to`), architectural
`layers`, and an ordered `tour`. The JSON is the interchange format shared by the
skill (writer) and the dashboard (reader), and it is committable to git. This is
*how the tool stores what it understands* — the comparison point against a
call-graph or an embedding store.

## In understand-anything (grounded)
The whole schema is declared in `packages/core/src/types.ts`:
[`KnowledgeGraph`](../catalog/understand-anything-plugin/packages/core/src/types.ts.md#KnowledgeGraph)
holds [`nodes`](../catalog/understand-anything-plugin/packages/core/src/types.ts.md#KnowledgeGraph.nodes),
[`edges`](../catalog/understand-anything-plugin/packages/core/src/types.ts.md#KnowledgeGraph.edges),
[`layers`](../catalog/understand-anything-plugin/packages/core/src/types.ts.md#KnowledgeGraph.layers),
a [`tour`](../catalog/understand-anything-plugin/packages/core/src/types.ts.md#KnowledgeGraph.tour),
and [`project`](../catalog/understand-anything-plugin/packages/core/src/types.ts.md#KnowledgeGraph.project)
metadata ([`ProjectMeta`](../catalog/understand-anything-plugin/packages/core/src/types.ts.md#ProjectMeta)).
A node is a [`GraphNode`](../catalog/understand-anything-plugin/packages/core/src/types.ts.md#GraphNode)
(id, [`type`](../catalog/understand-anything-plugin/packages/core/src/types.ts.md#GraphNode.type),
[`summary`](../catalog/understand-anything-plugin/packages/core/src/types.ts.md#GraphNode.summary),
[`tags`](../catalog/understand-anything-plugin/packages/core/src/types.ts.md#GraphNode.tags),
[`complexity`](../catalog/understand-anything-plugin/packages/core/src/types.ts.md#GraphNode.complexity)),
an edge a [`GraphEdge`](../catalog/understand-anything-plugin/packages/core/src/types.ts.md#GraphEdge)
(source/target/[`type`](../catalog/understand-anything-plugin/packages/core/src/types.ts.md#GraphEdge.type)/[`weight`](../catalog/understand-anything-plugin/packages/core/src/types.ts.md#GraphEdge.weight)/[`direction`](../catalog/understand-anything-plugin/packages/core/src/types.ts.md#GraphEdge.direction)).
The vocabularies are the [`NodeType`](../catalog/understand-anything-plugin/packages/core/src/types.ts.md#NodeType)
and [`EdgeType`](../catalog/understand-anything-plugin/packages/core/src/types.ts.md#EdgeType)
unions; [`Layer`](../catalog/understand-anything-plugin/packages/core/src/types.ts.md#Layer)
and [`TourStep`](../catalog/understand-anything-plugin/packages/core/src/types.ts.md#TourStep)
carry the layer grouping and guided-tour steps.

The single type has grown to cover **three graph kinds** — the schema is the
extension point later specs reuse rather than fork:
[`KnowledgeGraph.kind`](../catalog/understand-anything-plugin/packages/core/src/types.ts.md#KnowledgeGraph.kind)
selects `codebase` vs `knowledge`; the optional
[`GraphNode.domainMeta`](../catalog/understand-anything-plugin/packages/core/src/types.ts.md#GraphNode.domainMeta)
([`DomainMeta`](../catalog/understand-anything-plugin/packages/core/src/types.ts.md#DomainMeta))
and [`GraphNode.knowledgeMeta`](../catalog/understand-anything-plugin/packages/core/src/types.ts.md#GraphNode.knowledgeMeta)
([`KnowledgeMeta`](../catalog/understand-anything-plugin/packages/core/src/types.ts.md#KnowledgeMeta))
attach business-domain and knowledge-base payloads.

Every graph is validated on load. `packages/core/src/schema.ts` mirrors the
types as Zod schemas ([`KnowledgeGraphSchema`](../catalog/understand-anything-plugin/packages/core/src/schema.ts.md#KnowledgeGraphSchema),
[`GraphNodeSchema`](../catalog/understand-anything-plugin/packages/core/src/schema.ts.md#GraphNodeSchema))
and runs [`validateGraph`](../catalog/understand-anything-plugin/packages/core/src/schema.ts.md#validateGraph)
/ [`autoFixGraph`](../catalog/understand-anything-plugin/packages/core/src/schema.ts.md#autoFixGraph);
loose LLM output is coerced via
[`NODE_TYPE_ALIASES`](../catalog/understand-anything-plugin/packages/core/src/schema.ts.md#NODE_TYPE_ALIASES)
/ [`EDGE_TYPE_ALIASES`](../catalog/understand-anything-plugin/packages/core/src/schema.ts.md#EDGE_TYPE_ALIASES)
and by [`normalizeBatchOutput`](../catalog/understand-anything-plugin/packages/core/src/analyzer/normalize-graph.ts.md#normalizeBatchOutput)
(which strips ids to [`VALID_PREFIXES`](../catalog/understand-anything-plugin/packages/core/src/analyzer/normalize-graph.ts.md#VALID_PREFIXES)).

## Why it matters / when it applies
The design doc's key decisions — **JSON interchange** and **committable +
auto-sync** — hang off this one schema: because skill and dashboard share it,
search, validation, and filtering work uniformly for code, domain, and knowledge
graphs. Anyone comparing tools should read this as the substrate answer: not
embeddings, not a raw call graph, but a typed, human-summarized graph persisted
as reviewable JSON.

## Connections
- Code concepts: [core types](../concepts/understand-anything-plugin-packages-core-src-types.ts.md), [schema](../concepts/understand-anything-plugin-packages-core-src-schema.ts.md), [normalize-graph](../concepts/understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts.md)
- Module catalogs: [types.ts](../catalog/understand-anything-plugin/packages/core/src/types.ts.md), [schema.ts](../catalog/understand-anything-plugin/packages/core/src/schema.ts.md), [analyzer/normalize-graph.ts](../catalog/understand-anything-plugin/packages/core/src/analyzer/normalize-graph.ts.md)
- Related doc-concepts: [tree-sitter-llm-hybrid](tree-sitter-llm-hybrid.md), [multi-agent-pipeline](multi-agent-pipeline.md), [business-domain-extraction](business-domain-extraction.md), [knowledge-base-analysis](knowledge-base-analysis.md)

## Source
Extracted from `docs/superpowers/specs/2026-03-14-understand-anything-design.md`
(§ Knowledge Graph Schema), with schema extensions from the
`2026-04-01-business-domain-knowledge-design.md` and
`2026-04-09-understand-knowledge-design.md` specs — all kept in place.
