---
title: Knowledge-base analysis (/understand-knowledge)
type: doc-concept
provenance: doc
source: docs/superpowers/specs/2026-04-09-understand-knowledge-design.md
updated: 2026-07-04
status: fresh
---
# Knowledge-base analysis (/understand-knowledge)

## Definition
`/understand-knowledge` points the same graph machinery at a folder of markdown
notes — an Obsidian vault, Logseq graph, Dendron/Foam workspace, a Karpathy-style
LLM wiki, Zettelkasten, or plain markdown — and produces a force-directed
knowledge graph with community clustering. A deterministic parser extracts
explicit structure (wikilinks, categories, frontmatter) from `index.md`, then LLM
agents discover *implicit* relationships that Obsidian/Logseq graph views miss:
typed edges (`cites`, `contradicts`, `builds_on`, `categorized_under`,
`authored_by`, `exemplifies`) over typed nodes (`article`, `entity`, `topic`,
`claim`, `source`). Format is auto-detected so parsing adapts per tool.

## In understand-anything (grounded)
It is a second graph *kind*, not a fork of the pipeline. In
`packages/core/src/types.ts`, the five knowledge node types join
[`NodeType`](../catalog/understand-anything-plugin/packages/core/src/types.ts.md#NodeType)
and the six edges join
[`EdgeType`](../catalog/understand-anything-plugin/packages/core/src/types.ts.md#EdgeType);
[`KnowledgeGraph.kind`](../catalog/understand-anything-plugin/packages/core/src/types.ts.md#KnowledgeGraph.kind)
= `"knowledge"` switches the dashboard's layout/sidebar, and the per-node payload
is [`GraphNode.knowledgeMeta`](../catalog/understand-anything-plugin/packages/core/src/types.ts.md#GraphNode.knowledgeMeta)
→ [`KnowledgeMeta`](../catalog/understand-anything-plugin/packages/core/src/types.ts.md#KnowledgeMeta)
([`wikilinks`](../catalog/understand-anything-plugin/packages/core/src/types.ts.md#KnowledgeMeta.wikilinks),
[`backlinks`](../catalog/understand-anything-plugin/packages/core/src/types.ts.md#KnowledgeMeta.backlinks),
[`category`](../catalog/understand-anything-plugin/packages/core/src/types.ts.md#KnowledgeMeta.category),
[`content`](../catalog/understand-anything-plugin/packages/core/src/types.ts.md#KnowledgeMeta.content)),
validated by
[`KnowledgeMetaSchema`](../catalog/understand-anything-plugin/packages/core/src/schema.ts.md#KnowledgeMetaSchema).

The deterministic markdown parser (no tree-sitter here) is
`skills/understand-knowledge/parse-knowledge-base.py`:
[`parse_index`](../catalog/understand-anything-plugin/skills/understand-knowledge/parse-knowledge-base.md#parse_index),
[`parse_wiki`](../catalog/understand-anything-plugin/skills/understand-knowledge/parse-knowledge-base.md#parse_wiki),
[`extract_wikilinks`](../catalog/understand-anything-plugin/skills/understand-knowledge/parse-knowledge-base.md#extract_wikilinks),
[`extract_frontmatter`](../catalog/understand-anything-plugin/skills/understand-knowledge/parse-knowledge-base.md#extract_frontmatter).
Cross-file/agent output is reconciled by
[`merge`](../catalog/understand-anything-plugin/skills/understand-knowledge/merge-knowledge-graph.md#merge)
with entity dedup and type coercion
([`normalize_node_type`](../catalog/understand-anything-plugin/skills/understand-knowledge/merge-knowledge-graph.md#normalize_node_type),
[`normalize_edge_type`](../catalog/understand-anything-plugin/skills/understand-knowledge/merge-knowledge-graph.md#normalize_edge_type),
[`normalize_entity_name`](../catalog/understand-anything-plugin/skills/understand-knowledge/merge-knowledge-graph.md#normalize_entity_name)).
The force-directed community clustering the README advertises is the dashboard's
[`detectCommunities`](../catalog/understand-anything-plugin/packages/dashboard/src/utils/louvain.ts.md#detectCommunities)
(Louvain).

## Why it matters / when it applies
The value proposition is explicitly comparative: Obsidian's graph has untyped
edges, Logseq only shows explicit links, and a flat Karpathy wiki has no
visualization — this adds typed edges, LLM-discovered implicit relationships,
cross-format support, and guided tours over a knowledge base. The agent pipeline
mirrors the codebase one (scanner → format-detector → article-analyzer →
relationship-builder → reviewer) and supports incremental `--ingest` of new
notes, so the same reconcile discipline applies to prose as to code. For this
wiki's own survey, it is the direct analog: a tool that graphs a Karpathy-pattern
wiki — the very pattern this repo instantiates.

## Connections
- Code concepts: [core types](../concepts/understand-anything-plugin-packages-core-src-types.ts.md), [schema](../concepts/understand-anything-plugin-packages-core-src-schema.ts.md)
- Module catalogs: [types.ts](../catalog/understand-anything-plugin/packages/core/src/types.ts.md), [schema.ts](../catalog/understand-anything-plugin/packages/core/src/schema.ts.md), [skills/understand-knowledge/parse-knowledge-base.py](../catalog/understand-anything-plugin/skills/understand-knowledge/parse-knowledge-base.md), [skills/understand-knowledge/merge-knowledge-graph.py](../catalog/understand-anything-plugin/skills/understand-knowledge/merge-knowledge-graph.md), [dashboard/utils/louvain.ts](../catalog/understand-anything-plugin/packages/dashboard/src/utils/louvain.ts.md)
- Related doc-concepts: [knowledge-graph-schema](knowledge-graph-schema.md), [business-domain-extraction](business-domain-extraction.md), [semantic-batching-output-chunking](semantic-batching-output-chunking.md)

## Source
Extracted from `docs/superpowers/specs/2026-04-09-understand-knowledge-design.md`
and `README.md` (§ Analyze knowledge bases) — kept in place.
