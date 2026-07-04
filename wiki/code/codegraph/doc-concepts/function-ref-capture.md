---
title: Function-as-value capture — "where is this callback wired up?"
type: doc-concept
provenance: doc
source: docs/design/function-ref-capture.md
updated: 2026-07-04
status: fresh
---
# Function-as-value capture — "where is this callback wired up?"

## Definition
When a function is used as a **value** — passed as an argument, assigned to a function pointer
or field, placed in a struct initializer or handler table — static extraction produced **no
edge** (0/19 tree-sitter languages before #756). `callers(my_recv_cb)` on a C callback showed
only direct calls, so every registered callback looked dead and the **registration sites** — the
agent's actual next question, *"where is this wired up?"* — were invisible. Function-ref capture
emits a `references` edge (`metadata: { fnRef: true, resolvedBy, confidence }`) from the
registration site to the function. It is the **function** half of "a symbol used as a value, not
called"; the **data** half (a const/config/table a symbol reads) is
[value-reference edges](value-reference-edges.md).

## The registration-vs-dispatch distinction (the design's core boundary)
The feature covers **registration** and deliberately *not* **dispatch**:
- **Registration** — `register(my_cb)`, `handlers[FOO] = do_foo`, `OnClick := Handler`. The
  function's name is *literally in the source* at the wiring site, so linking it is
  **deterministic**.
- **Dispatch** — resolving `o->cb(x)` back to the concretely-registered function needs data-flow
  through struct fields; even an LSP needs fallbacks. **A wrong edge is worse than silence**, so
  dispatch resolution stays uncovered here — it is the job of the separate
  [callback/dispatch edge synthesizer](../concepts/resolution-callback-synthesizer.ts.md).
Reading a getter/callback into a local still yields the true registration-flavored dependency;
the imperfect "registration" label is accepted.

## The capture → gate → resolve flow (grounded)
Because `getCallers`/`getCallees`/`getImpactRadius` already traverse `references` edges,
registration sites surface with no graph-layer change (the MCP callers/callees lists label them
"via callback registration").

1. **Capture** — table-driven per language in
   [`src/extraction/function-ref.ts`](../catalog/src/extraction/function-ref.ts.md): each
   language's value positions (arg, assignment RHS, keyed init, list/table, wrapper forms) are a
   declarative [`FnRefSpec`](../catalog/src/extraction/function-ref.ts.md#FnRefSpec)
   (a [`CaptureRule`](../catalog/src/extraction/function-ref.ts.md#CaptureRule) per
   [`CaptureMode`](../catalog/src/extraction/function-ref.ts.md#CaptureMode)) in
   [`FN_REF_SPECS`](../catalog/src/extraction/function-ref.ts.md#FN_REF_SPECS), with
   [`cFamilySpec`](../catalog/src/extraction/function-ref.ts.md#cFamilySpec) sharing the
   C/C++/ObjC shapes.
   [`captureFnRefCandidates`](../catalog/src/extraction/function-ref.ts.md#captureFnRefCandidates)
   +
   [`normalizeValue`](../catalog/src/extraction/function-ref.ts.md#normalizeValue) turn a value
   expression into zero-or-more names as
   [`FnRefCandidate`](../catalog/src/extraction/function-ref.ts.md#FnRefCandidate)s. Capture
   fires from three walkers in
   [`tree-sitter.ts`](../catalog/src/extraction/tree-sitter.ts.md) (a node is visited by exactly
   one): `visitNode` (file/class scope), `visitForCallsAndStructure` (function bodies), and
   [`visitPascalBlock`](../catalog/src/extraction/tree-sitter.ts.md#TreeSitterExtractor.visitPascalBlock);
   subtrees the walkers don't descend get a candidates-only
   [`scanFnRefSubtree`](../catalog/src/extraction/tree-sitter.ts.md#TreeSitterExtractor.scanFnRefSubtree).
2. **Gate** —
   [`flushFnRefCandidates`](../catalog/src/extraction/tree-sitter.ts.md#TreeSitterExtractor.flushFnRefCandidates)
   keeps a candidate only if its name matches a same-file function/method **or** an *imported*
   binding. C-family **file-scope initializers skip the gate** — a bare identifier in a C
   constant-expression context can only be a function address (redis's command table names
   handlers from other `.c` files). The candidate becomes an unresolved ref with an
   internal-only `referenceKind` of `'function_ref'`.
3. **Resolve** — in
   [`src/resolution/index.ts`](../catalog/src/resolution/index.ts.md):
   [`resolveOne`](../catalog/src/resolution/index.ts.md#ReferenceResolver.resolveOne) tries
   [`resolveViaImport`](../catalog/src/resolution/import-resolver.ts.md#resolveViaImport) first,
   then
   [`matchFunctionRef`](../catalog/src/resolution/name-matcher.ts.md#matchFunctionRef) — exact
   name, function/method kinds only, same language family, same-file first, cross-file **only
   when the name is UNIQUE**, never fuzzy. TS/JS `this.X` and Java/Kotlin `Type::m` forms resolve
   class-scoped via
   [`resolveThisMemberFnRef`](../catalog/src/resolution/index.ts.md#ReferenceResolver.resolveThisMemberFnRef)
   /
   [`resolveDeferredThisMemberRefs`](../catalog/src/resolution/index.ts.md#ReferenceResolver.resolveDeferredThisMemberRefs)
   (a supertype BFS after edges persist). The result is an edge of `kind: 'references'` with
   `metadata: { fnRef: true }`.

## Precision rules — each bought by a real-repo false positive
The design lists ten; the load-bearing ones: **the extraction-time gate** (same-file fn/method
∪ imported binding); **C++ is `&`-explicit** (`addressOfOnly` — generic free-function names
collide with locals, so only `&fn` / `&Cls::method` qualify outside file-scope tables);
**TS/JS/Python bare ids resolve to `function` kind only** (a method needs a receiver);
**Swift overload-family refusal** and **param-forward / destructuring skips**; generated/minified
files ([`isGeneratedFile`](../catalog/src/extraction/generated-detection.ts.md#isGeneratedFile))
produce no candidates; and the **unique-or-drop, never-fuzzy** resolution rule. Language-specific
capture idioms live in specs like
[`PHP_CALLABLE_HOFS`](../catalog/src/extraction/function-ref.ts.md#PHP_CALLABLE_HOFS) (string
callables only in known HOF positions) and the Ruby hook DSLs
([`RUBY_HOOK_RE`](../catalog/src/extraction/function-ref.ts.md#RUBY_HOOK_RE) /
[`isRubyHookCall`](../catalog/src/extraction/function-ref.ts.md#isRubyHookCall)), with
[`NAME_STOPLIST`](../catalog/src/extraction/function-ref.ts.md#NAME_STOPLIST) excluding
never-a-function identifiers. Validated across 17 public-OSS repos: node count and `calls` edges
identical, `references` strictly additive (redis +1918, excalidraw +121), precision spot-checked.

## Why it matters / when it applies
It answers *"where is this callback registered?"* — the question `callers` used to answer with
silence. Because the edges ride the existing `references` traversal, they surface in
`codegraph_explore`'s flow, the `codegraph_node` trail, and impact radius automatically. Known
deliberate limits: dispatch resolution (deferred to the dynamic-dispatch synthesizer);
local/param shadowing an imported/same-file function (needs local-scope tracking); `obj.method`
where `obj` isn't `this`/`self`; and Java/Kotlin method refs through a variable
(`subscriber::onNext`).

## Connections
- Code concepts:
  [extraction-function-ref.ts](../concepts/extraction-function-ref.ts.md) — the capture side
  (specs, candidates, normalization);
  [extraction-tree-sitter.ts](../concepts/extraction-tree-sitter.ts.md) — the walkers +
  `flushFnRefCandidates` gate;
  [resolution-index.ts](../concepts/resolution-index.ts.md) — `resolveOne` /
  `matchFunctionRef` / the `this.member` resolution;
  [resolution-callback-synthesizer.ts](../concepts/resolution-callback-synthesizer.ts.md) — the
  **dispatch** counterpart this feature deliberately leaves to it.
- Module catalogs:
  [extraction/function-ref.ts](../catalog/src/extraction/function-ref.ts.md),
  [extraction/tree-sitter.ts](../catalog/src/extraction/tree-sitter.ts.md),
  [resolution/index.ts](../catalog/src/resolution/index.ts.md),
  [resolution/name-matcher.ts](../catalog/src/resolution/name-matcher.ts.md),
  [types.ts](../catalog/src/types.ts.md).
- Related doc-concepts:
  [value-reference-edges](value-reference-edges.md) — the data (const/var) half of
  "used as a value, not called";
  [dynamic-dispatch-coverage](dynamic-dispatch-coverage.md) — the dispatch edges that complete
  a flow once registration is captured.

## Source
Extracted from `docs/design/function-ref-capture.md` (#756 — mechanism, per-language value
positions, the ten precision rules, and the 17-repo validation). Kept in place.
