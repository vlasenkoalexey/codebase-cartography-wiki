---
title: MCP tool surface — one codegraph_explore call
type: doc-concept
provenance: doc
source: README.md
updated: 2026-07-04
status: fresh
---
# MCP tool surface — one codegraph_explore call

## Definition
CodeGraph's whole retrieval value-prop is compressed into a **single MCP tool, `codegraph_explore`**. Instead of the agent rebuilding structure the slow way — grep, glob, Read, one file at a time — it asks one question and gets back the relevant source (grouped by file), the call paths between those symbols (including dynamic-dispatch hops grep can't follow), and the blast radius of a change. The README frames this as **surgical context, not a file-by-file search** — fewer tool calls, faster answers. The deliberate design choice is *one strong tool*: measured agent behavior showed one tool steers agents better than a menu of narrower ones (fewer mis-picks, less context spent every session).

## In codegraph (grounded)
The tool surface lives in the **`src/mcp/tools.ts`** module. `codegraph_explore` is served by [`ToolHandler.handleExplore`](../catalog/src/mcp/tools.ts.md#ToolHandler.handleExplore), which leads its output with the call flow assembled by [`ToolHandler.buildFlowFromNamedSymbols`](../catalog/src/mcp/tools.ts.md#ToolHandler.buildFlowFromNamedSymbols) (it finds the path among the symbol names in the query, riding synthesized edges) and appends the change-impact summary from [`ToolHandler.buildBlastRadiusSection`](../catalog/src/mcp/tools.ts.md#ToolHandler.buildBlastRadiusSection).

- **One listed tool, the rest unlisted-but-live.** The default MCP list comes from [`getStaticTools`](../catalog/src/mcp/tools.ts.md#getStaticTools) / the [`tools`](../catalog/src/mcp/tools.ts.md#tools) definitions; the other handlers ([`ToolHandler.handleNode`](../catalog/src/mcp/tools.ts.md#ToolHandler.handleNode), `handleSearch`, `handleCallers`, `handleCallees`, `handleImpact`, `handleFiles`, `handleStatus`) stay fully functional but hidden — everything they return already arrives inline on explore. Re-enable them for the MCP surface via `CODEGRAPH_MCP_TOOLS`, or use the CLI equivalents.
- **Output sized to the answer, scaled to the repo.** The per-call output budget comes from [`getExploreOutputBudget`](../catalog/src/mcp/tools.ts.md#getExploreOutputBudget) (chars / files / per-file), which grows monotonically with indexed file count so a god-file repo still returns a usable slice.
- **Never fails loudly.** [`ToolHandler.execute`](../catalog/src/mcp/tools.ts.md#ToolHandler.execute) turns every expected condition (project not indexed, symbol not found) into a *success-shaped* response carrying guidance rather than an error — so one bad response doesn't teach the agent to abandon CodeGraph. The tool surface stays exposed even at an un-indexed root; pass `projectPath` to query any indexed project in the same session.
- **First contact.** The usage guidance the agent sees in the MCP `initialize` response is the single source of truth in **`src/mcp/server-instructions.ts`** — [`SERVER_INSTRUCTIONS`](../catalog/src/mcp/server-instructions.ts.md#SERVER_INSTRUCTIONS) (and [`SERVER_INSTRUCTIONS_NO_ROOT_INDEX`](../catalog/src/mcp/server-instructions.ts.md#SERVER_INSTRUCTIONS_NO_ROOT_INDEX) for an un-indexed root). It tells the agent to answer structural questions directly and treat returned source as already read.

## Why it matters / when it applies
The README's benchmark claim — across 7 real repos, **58% fewer tool calls, 22% faster, file reads cut to ~zero** — rests entirely on the agent *stopping* after an explore call instead of falling back to a grep/Read crawl. So the point of the single-tool surface is sufficiency: the response has to be complete enough (source + flow + blast radius) that the agent doesn't re-verify. This applies to almost any structural question: "how does X work", a flow ("how does X reach Y"), or surveying an area. Naming a file or symbol in the query returns its current line-numbered source, the same shape Read gives.

## Connections
- Code concepts: [mcp-tools.ts](../concepts/mcp-tools.ts.md) — the deep page on the tool handlers, budgets, and flow assembly; [mcp-daemon.ts](../concepts/mcp-daemon.ts.md) and [mcp-transport.ts](../concepts/mcp-transport.ts.md) — how the tools are served to the agent; [mcp-query-pool.ts](../concepts/mcp-query-pool.ts.md) — the worker pool answering queries.
- Module catalogs: [mcp/tools.ts](../catalog/src/mcp/tools.ts.md), [mcp/server-instructions.ts](../catalog/src/mcp/server-instructions.ts.md).
- Related doc-concepts: [local-first-grounding](local-first-grounding.md) — where the graph explore reads from comes from; [init-and-autosync](init-and-autosync.md) — how that graph is built and kept fresh.

## Source
Extracted from `README.md` (kept in place) — the "Why CodeGraph?", "MCP Tools", "Agent Tool Guidance", and "How It Works" sections.
