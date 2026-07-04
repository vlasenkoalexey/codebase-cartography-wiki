---
title: Zero-trust deployment and the licensing business model
type: doc-concept
provenance: doc
source: README.md
updated: 2026-07-04
status: fresh
---
# Zero-trust deployment and the licensing business model

## Definition
The README dedicates two full sections to positioning independent of any single feature: "Zero-Trust
Data Security" ("Your code never leaves your machine... No Data Transmission... Ephemeral Memory
Processing... Privacy-by-Design") and "⚖️ Licensing & Usage" (PolyForm Noncommercial License 1.0.0;
free for academic/hobbyist use via a `GITGALAXY_LICENSE_KEY=COMMUNITY_FREE_TIER` env var; commercial
use requires a paid key, and "unlicensed corporate pipelines will experience intentional execution
friction").

## In gitgalaxy (grounded)
The licensing mechanics are already fully grounded by [the existing Licensing concept page](../concepts/gitgalaxy-licensing.md):
[`enforce_licensing_guard`](../catalog/gitgalaxy/licensing.md#enforce_licensing_guard) is the real
function every tool's `main()` calls, `COMMUNITY_FREE_TIER` really does short-circuit to a free pass,
and the "intentional execution friction" the README threatens is a real, measured `time.sleep()`
penalty (not a hard block) on an invalid or forged key — that page's own framing ("never actually
blocks execution") is the honest reading of this README section's more assertive marketing language.
This page adds the "why," which the licensing page deliberately declines to editorialize on (it opens
by stating licensing "has nothing to do with code comprehension").

The "your code never leaves your machine" claim is not separately enforced by a single function —
it is the *absence* of a capability across everything this survey's packets cover: neither the
Aperture Filter, the Detector, `NetworkRiskSensor`, nor either recorder (`llm_recorder.py`,
`record_keeper.py`) opens a network socket or an HTTP client anywhere in the code read for this
survey; every artifact (`{target}_galaxy_graph.sqlite`, the markdown brief, the primary mission
database) is written to a local path passed in by the caller. This is an inference from absence
across the modules this survey has actually read, not a single asserted guarantee — flagged
honestly rather than treated as proven by one code path.

> [!inferred]
> No networking library import (`requests`, `httpx`, `socket`, `urllib`) was observed in any of the
> `gitgalaxy/core`, `gitgalaxy/metrics`, or `gitgalaxy/recorders` files read across this survey's
> packets and this ingest's own source reading. This is consistent with, but does not exhaustively
> prove, the "100% air-gapped execution" claim — the full repository (all 50+ language tools, the
> `site/` visualizer, and every `tools/` Spoke) was not read line-by-line to rule out a network call
> anywhere.

## Why it matters / when it applies
This section directly explains a design choice the [structural-rag-graph](structural-rag-graph.md)
page grounds mechanically but doesn't editorialize on: why the "queryable knowledge graph" ships as a
local SQLite file rather than being pushed into a hosted graph database. `docs/wiki/01-06-the-structural-rag-graph.md`
itself argues the point directly — "trapped in ... heavy graph databases (like Neo4j) that AI agents
struggle to query" is framed as a usability complaint, but the zero-trust/air-gapped positioning here
supplies the other half of the motivation: a hosted graph service is also a data-exfiltration surface
a zero-trust pipeline can't accept. The commercial-license friction, in turn, is the monetization
model that funds maintaining the 50+ language regex tables (`docs/wiki/`'s "how to add a language in
1 minute" pitch) without charging the academic/OSS users this survey's own use case falls under.

## Connections
- Code concepts: [Licensing guard](../concepts/gitgalaxy-licensing.md) — the mechanism this page adds
  business-model context to.
- Module catalogs: [licensing](../catalog/gitgalaxy/licensing.md).
- Related doc-concepts: [structural-rag-graph](structural-rag-graph.md) — the local-SQLite-vs-Neo4j
  argument this page's zero-trust framing completes; [blast-paradigm](blast-paradigm.md) — the
  broader "why not send code to an LLM" privacy argument this page's networking claim extends to the
  whole tool suite, not just the core engine.

## Source
Extracted from `README.md` §"Local Browser-Based 3D Codebase Visualization" (Zero-Trust Data
Security) and §"⚖️ Licensing & Usage" (kept in place).
