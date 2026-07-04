---
title: Dynamic-Dispatch Coverage
type: doc-concept
provenance: doc
source: docs/design/dynamic-dispatch-coverage-playbook.md
updated: 2026-07-04
status: fresh
---
# Dynamic-Dispatch Coverage

## Definition
codegraph's signature job is to be **the map** — to answer structural/flow questions
("how does X reach Y", callers, impact) that grep and Read cannot, and to do it well
enough that an agent stops reading files to reconstruct a flow by hand. The obstacle is
**dynamic dispatch**: static tree-sitter extraction only sees a call when the callee's
name appears literally at the call site (`foo()`, `this.bar()`). The instant control
routes through *indirection* — a stored callback, a string-keyed event, a runtime-chosen
attribute, an interface reference, a command bus, a generated RPC stub — that literal name
vanishes and the flow **breaks in the graph even though it is fully connected at runtime**.
"Dynamic-dispatch coverage" is the standing mission of systematically finding those holes
across **every language and framework codegraph supports** and bridging each one, so
cross-symbol flows exist in the graph everywhere. The maintainers proved empirically that
**coverage is the lever** for getting agents to prefer codegraph over Read — not prompting,
hooks, or new tools: when the flow is missing the agent reads to rebuild it; when the flow
is in the graph the agent can answer completely without reading (validated on excalidraw —
2/3 headless runs answered "how does an update reach the screen" with Read 0).

## In codegraph (grounded)
Two mechanisms close two distinct classes of hole; the choice is driven by **whether a
name exists to resolve**:

- **Resolver — a named ref exists** (`self._iterable_class(self)`, `[HttpGet]` action,
  `Route::get([Ctrl::class,'m'])`). One ref, resolved one at a time. A
  [`FrameworkResolver`](../catalog/src/resolution/types.ts.md#FrameworkResolver) claims the
  otherwise-unresolvable ref through its name-exists pre-filter hook
  [`claimsReference`](../catalog/src/resolution/types.ts.md#FrameworkResolver.claimsReference)
  (consulted by [`ReferenceResolver.resolveOne`](../catalog/src/resolution/index.ts.md#ReferenceResolver.resolveOne))
  and then resolves it. The canonical example is the Django ORM: `QuerySet._fetch_all`
  calls a runtime-chosen `_iterable_class`, which
  [`djangoResolver`](../catalog/src/resolution/frameworks/python.ts.md#djangoResolver) resolves
  to [`ModelIterable.__iter__`](../catalog/src/resolution/frameworks/python.ts.md#resolveModelIterableIter),
  reconnecting `_fetch_all → __iter__ → execute_sql`.
- **Synthesizer — no name to resolve** (`cb()` is anonymous; a dispatcher and a registrar
  live in different files and must be *correlated*). This is a whole-graph pass run at the
  end of a resolution batch —
  [`synthesizeCallbackEdges`](../catalog/src/resolution/callback-synthesizer.ts.md#synthesizeCallbackEdges),
  invoked from [`ReferenceResolver.resolveAndPersistBatched`](../catalog/src/resolution/index.ts.md#ReferenceResolver.resolveAndPersistBatched)
  — that today fans out into ~30 narrow, framework-specific channels. The foundational
  three: [`fieldChannelEdges`](../catalog/src/resolution/callback-synthesizer.ts.md#fieldChannelEdges)
  (field observers — `onUpdate(cb)` + `for(cb of cbs)cb()`),
  [`eventEmitterEdges`](../catalog/src/resolution/callback-synthesizer.ts.md#eventEmitterEdges)
  (string-keyed `on('e',fn)`/`emit('e')`, correlated by the event-name literal), and
  [`closureCollectionEdges`](../catalog/src/resolution/callback-synthesizer.ts.md#closureCollectionEdges)
  (Swift/Alamofire deferred closures — a registrar appends to a field, a dispatcher drains
  it with `forEach { $0() }`, gated on the element-invoke).

Extraction plays a supporting role: named inline handlers were invisible until
[`TreeSitterExtractor.visitFunctionBody`](../catalog/src/extraction/tree-sitter.ts.md#TreeSitterExtractor.visitFunctionBody)
began emitting named nested functions as nodes (via
[`extractFunction`](../catalog/src/extraction/tree-sitter.ts.md#TreeSitterExtractor.extractFunction))
so a synthesizer has something to link *to*. Every synthesized edge is tagged
`provenance:'heuristic'` on the exact same [`Edge`](../catalog/src/types.ts.md#Edge) shape
(a fixed [`EdgeKind`](../catalog/src/types.ts.md#EdgeKind) enum) as a real static edge —
plus `metadata.synthesizedBy` (the channel name) and `registeredAt` (the wiring site) — so
downstream it is indistinguishable to trace, impact, and `codegraph_explore` from an edge
tree-sitter extracted directly. Coverage is validated only after it is *surfaced*: the
single query tool `codegraph_explore` renders the flow among a query's named symbols via
[`ToolHandler.buildFlowFromNamedSymbols`](../catalog/src/mcp/tools.ts.md#ToolHandler.buildFlowFromNamedSymbols).

## Why it matters / when it applies
The governing doctrine is **high-precision, low-recall — silent beats wrong**. A single
false edge poisons the map (an agent trusts it, follows it, and lands nowhere), so every
synthesizer is precision-first: it must emit **0 edges on a control repo that lacks the
shape** while being non-zero and precise on **≥2 repos that contain it** (a synthesizer
validated on one repo is unvalidated). Recall is deliberately sacrificed — canvas dispatch,
anonymous-arrow handlers, reactive/Proxy runtimes (Vue reactivity, MobX), and
metaprogramming finders (ActiveRecord/Eloquent/Spring-Data-JPA) are left **uncovered on
purpose** because they have no static anchor. When a flow genuinely can't be bridged
precisely, the frontier fallback is **boundary surfacing** (`dynamic-boundaries.ts`):
explore *announces* the dispatch site where the static path ends rather than fabricating an
edge. Two corollaries the docs hammer:

- **Partial coverage is worse than none.** Bridging one boundary but not the next reveals a
  hop the agent then drills and reads to finish (measured on excalidraw: react-render alone
  *raised* reads to 5–7; only completing the flow with the jsx-child hop dropped it to 0–1).
  Always close a flow end-to-end and re-measure.
- **Coverage *enables*, doesn't *force*, the no-read path.** Agents still sometimes read to
  confirm; the reliable, unconditional win is answer *completeness*, not a guaranteed cost drop.

Coverage is tracked along **two orthogonal axes**, because a single framework contains
several indirection shapes and a single shape recurs across many frameworks:

- **By language × framework** (the playbook's §6 matrix): one row per ecosystem — React,
  Vue, Django, Spring, Gin, Axum, Rails, Laravel, Vapor, Flutter, and cross-language
  bridges — each with its canonical flow, its mechanism (R = resolver, S = synthesizer,
  X = extraction), and a validated status.
- **By dispatch shape** (the synthesizer backlog): organized by *indirection shape* rather
  than framework, because "Redux" alone is ≥2 shapes (hand-written thunks vs RTK Query) and
  a name→class registry is the same problem in a trezor SDK, an n8n node loader, and a VS
  Code command palette. Shipped shape-channels include redux-thunk, object-registry, RTK
  Query, Vuex/Pinia dispatch, Celery, Sidekiq, Spring/Laravel events, MediatR/CQRS, and a
  C/systems fn-pointer-dispatch family; a Tier-C set (RxJS subscribe, MobX/Solid signals,
  Redux-Saga) is explicitly marked **do-not-build** — no static anchor, silent beats wrong.

The **roadmap/backlog framing**: prioritize by *frequency × static-resolvability ×
query-seedability* (an edge only helps if a realistic symbol-named `codegraph_explore` query
seeds a path it lies on), do the cheap resolver-shaped holes before the hard synthesizer
ones, and treat anonymous-arrow "link-through-body" dispatch as the hard, still-open frontier.

## Connections
- Code concepts:
  [resolution-callback-synthesizer.ts](../concepts/resolution-callback-synthesizer.ts.md) —
  the deep page on the ~30 heuristic synthesizer passes (this doc-concept's home);
  [resolution-index.ts](../concepts/resolution-index.ts.md) — the resolver pipeline and the
  `claimsReference` pre-filter; [resolution-types.ts](../concepts/resolution-types.ts.md) —
  the `FrameworkResolver` contract; [extraction-function-ref.ts](../concepts/extraction-function-ref.ts.md)
  — reference-candidate capture that feeds resolution; [types.ts](../concepts/types.ts.md)
  — the `provenance:'heuristic'` `Edge` / `EdgeKind` vocabulary.
- Module catalogs:
  [resolution/callback-synthesizer.ts](../catalog/src/resolution/callback-synthesizer.ts.md),
  [resolution/index.ts](../catalog/src/resolution/index.ts.md),
  [resolution/types.ts](../catalog/src/resolution/types.ts.md),
  [resolution/frameworks/python.ts](../catalog/src/resolution/frameworks/python.ts.md),
  [extraction/tree-sitter.ts](../catalog/src/extraction/tree-sitter.ts.md),
  [mcp/tools.ts](../catalog/src/mcp/tools.ts.md),
  [types.ts](../catalog/src/types.ts.md).
- Related doc-concepts:
  [cross-language-native-bridging.md](cross-language-native-bridging.md) — the cross-language
  half of dispatch coverage (Swift↔ObjC, the React Native / Expo bridges);
  [template-markup-parsing.md](template-markup-parsing.md) — template extraction (Vue SFC,
  JSX, Svelte) that feeds the template/JSX synthesizer channels;
  [chained-call-resolution.md](chained-call-resolution.md) — the chained-method route
  parsing (`.route(...).post(...)`) adjacent to this work;
  [value-reference-edges.md](value-reference-edges.md) — how reference/value edges are
  modeled, the same `Edge` machinery synthesized edges ride on.

## Source
Extracted from three overlapping design docs, all kept in place:
- `docs/design/dynamic-dispatch-coverage-playbook.md` — the primary: the top-level mission,
  the two-mechanism model, the repeatable per-framework methodology, and the language ×
  framework coverage matrix (§6).
- `docs/design/dispatch-synthesizer-backlog.md` — the cross-cutting queue organized by
  dispatch *shape* (registry / RTK Query / Vuex / MediatR / Celery / Sidekiq / events /
  fn-pointer), with the precision discipline and per-synthesizer validation protocol.
- `docs/design/callback-edge-synthesis.md` — the original design of the callback/observer/
  EventEmitter synthesizer, the "why a whole-graph pass, not a `resolve()`" rationale, and
  the as-built divergences (file+field pairing, fan-out cap, `provenance:'heuristic'`).
