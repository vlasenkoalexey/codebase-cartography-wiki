---
title: Adaptive explore sizing (sibling skeletonization)
type: doc-concept
provenance: doc
source: docs/design/adaptive-explore-sizing.md
updated: 2026-07-04
status: fresh
---
# Adaptive explore sizing (sibling skeletonization)

## Definition
`codegraph_explore` used to return full source for **every** relevant file up to
its char budget — the budget was a *target it filled*, not a ceiling. On a
question whose answer spans many *same-shaped* classes (e.g. OkHttp's ~14
`class … : Interceptor` implementations), that meant ~28 KB of mostly **redundant
full bodies** riding in the context window for the rest of the session — so the
WITH-codegraph arm cost *more* than plain grep/read. Adaptive sizing makes explore
size its output **to the answer**: when a file is an interchangeable *polymorphic
sibling* and off the traced flow, it is rendered as a **skeleton** (class + member
*signatures*, bodies elided) instead of full source. Default-on; escape hatch
`CODEGRAPH_ADAPTIVE_EXPLORE=0`.

## Mental model
The whole game is telling an **interchangeable sibling** apart from a **distinct
step**, cheaply. N implementations of one interface invoked polymorphically are
redundant — the agent needs the *mechanism* (the dispatch loop) + the *contract*
every sibling implements + maybe one concrete exemplar; the other bodies are
padding *because they are interchangeable*. On a diffuse flow (Excalidraw's render
pipeline) the off-spine files are *distinct steps* doing real work — eliding them
just forces the agent to reconstruct them, net costlier. So the structural signal
is "shared supertype with **≥3 implementers**" (`MIN_SIBLINGS`), read from real
`implements`/`extends` edges — a 1:1 interface→impl pair is *not* a sibling and
stays full.

## In codegraph (grounded)
Lives entirely in `src/mcp/tools.ts` — the explore tool and its output shaping:

- [`adaptiveExploreEnabled`](../catalog/src/mcp/tools.ts.md#adaptiveExploreEnabled)
  — the flag (default on; `CODEGRAPH_ADAPTIVE_EXPLORE=0` disables).
- [`ToolHandler.buildFlowFromNamedSymbols`](../catalog/src/mcp/tools.ts.md#ToolHandler.buildFlowFromNamedSymbols)
  — returns `{ text, pathNodeIds, namedNodeIds }`. `pathNodeIds` is the flow
  **spine** (always kept full); `namedNodeIds` is every callable the agent named
  (a superset of the spine) — the named-callable *spare* reads it.
- [`ToolHandler.handleExplore`](../catalog/src/mcp/tools.ts.md#ToolHandler.handleExplore)
  — gathers relevant files, sorts by relevance, fills to `maxOutputChars`, and
  applies the skeleton branch. Two **cached local helpers** implement the sibling
  test — `isPolymorphicSibling()` (a node has an outgoing `implements`/`extends`
  to a ≥3-impl supertype) and `definesPolymorphicSupertype()` (a node HAS ≥3
  *incoming* such edges — i.e. it is the family base). These are nested inside
  `handleExplore` and so have no catalog anchor of their own; the branch itself is
  `off-spine && isPolymorphicSibling && !(namedInFile && !definesSupertype)`.
- The budget these interact with is set by
  [`getExploreBudget`](../catalog/src/mcp/tools.ts.md#getExploreBudget) (call
  count) and
  [`getExploreOutputBudget`](../catalog/src/mcp/tools.ts.md#getExploreOutputBudget)
  (chars / files / per-file). Skeletonizing a family file *frees* budget for the
  sibling files the agent would otherwise Read. Skeletons still route through
  [`ToolHandler.truncateOutput`](../catalog/src/mcp/tools.ts.md#ToolHandler.truncateOutput)'s
  honest cap, and the skeleton header lists the file's symbols and says
  `Read for a full body` so the agent can still pull one specific impl.

The gate (a file skeletonizes iff **all** hold): (1) a spine exists;
(2) the file is **off** that spine; (3) it is a **polymorphic sibling** (≥3-impl
supertype); (4) it is **not spared** — where *spared = the agent named a
(near-)UNIQUE callable in it* — **UNLESS** the file itself **DEFINES a ≥3-impl
supertype** (the override: a base+subclasses "family" file is huge and Read-anyway,
so skeletonizing it frees budget). Worked cases: OkHttp's `RealCall` is spared
(named `getResponseWithInterceptorChain`, defines no supertype → kept full, 0
read-backs); the 5 redundant `: Interceptor` impls skeletonize; Django's
`compiler.py` is named but *defines* `SQLCompiler`, so the override fires and it
skeletonizes to free budget.

## Why it matters / when it applies
- Applies only to **many-impl families** (interceptor chains, strategy/visitor
  families, codec registries). Diffuse flows and 1:1 interface→impl pairs are
  untouched, so inert repos (Excalidraw / Tokio / VS Code / Gin) stay at **0
  skeletons** — the refined gate skeletonizes a strict subset of the naive gate.
- **Validated** (real-agent A/B, Opus 4.8, median cost): OkHttp `$0.45→$0.50`
  (~10% cheaper, `RealCall` full and never read back); Django `$0.56→$0.63`
  (~10% cheaper) — both were the README's cost outliers and flipped to wins.
- **Dead ends the doc warns against re-attempting:** demote/rank low-value files
  (ranking ≠ shrinking — you must skeletonize); gate on entry-node membership
  (all chain participants are named); rely on `synthesizedBy:'interface-impl'`
  synth edges (not created for Kotlin `fun interface`); a plain "core-floor" gate
  (regressed Excalidraw's distinct steps +17%); *sparing* a supertype-defining
  file (backwards — it starves budget); validating with the deterministic probe
  only (its spine differs from the real agent's — always confirm with a real A/B).

## Connections
- Code concepts: [MCP tools — the explore/node tool surface](../concepts/mcp-tools.ts.md)
  — the deep page on `handleExplore`, `buildFlowFromNamedSymbols`, and output shaping.
- Module catalogs: [src/mcp/tools.ts](../catalog/src/mcp/tools.ts.md) — full
  per-symbol index for the explore tool.
- Related doc-concepts: [Agent adoption of codegraph](agent-adoption.md) — the
  sibling doctrine ("sufficiency: make the answer complete enough that the agent
  stops reading") that adaptive sizing serves.

## Source
Extracted from `docs/design/adaptive-explore-sizing.md` (kept in place).
