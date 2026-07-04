---
title: Function-as-value capture — turning callback registrations into candidate references
type: concept
provenance: mixed
concept: extraction-function-ref.ts
concepts: [multi-language-extraction]
updated: 2026-07-04
status: fresh
---
# Function-as-value capture — turning callback registrations into candidate references

## Overview
Static call extraction only sees a function name where it is *invoked* — `fn()`. It is
blind to a function name used as a *value*: passed as a callback argument
(`addEventListener('click', handler)`), assigned to a field or function pointer
(`o->cb = target_cb`), or placed in a struct/table initializer
(`static cb_t table[] = { cb_a, cb_b }`). Every one of those sites is a real dependency —
"where does this callback get wired up?" is an agent's natural next question after finding
a handler — but a tree-sitter walk that only recognizes `call_expression` nodes never
produces an edge for it. This module is the **capture** half of fixing that: for each of
~20 languages it recognizes the AST shapes where a bare name is *used as data* rather than
*called*, and turns each occurrence into an [`FnRefCandidate`](../catalog/src/extraction/function-ref.ts.md#FnRefCandidate)
— a name, a position, and enough metadata for a later gating/resolution stage (outside
this module) to decide whether it becomes a real graph edge. The central design idea is a
**declarative per-language spec** ([`FnRefSpec`](../catalog/src/extraction/function-ref.ts.md#FnRefSpec))
rather than one recognizer function per language: each language's "value positions" differ
in AST shape (a C `initializer_pair`, a Kotlin `callable_reference`, a Ruby
`method(:sym)` call) but the *categories* of shape repeat across languages, so the module
factors them into a small closed vocabulary — dispatch tables, transparent wrapper layers,
unary unwrap operators, and bespoke "special" forms — and each language spec just picks
which categories it needs.

## Diagram
```mermaid
flowchart TD
    FRS["FN_REF_SPECS[language]"] -->|"picked at construction"| CTOR["`&lt;constructor&gt;` (TreeSitterExtractor)"]
    CTOR -->|"this.fnRefSpec"| MCFR[maybeCaptureFnRefs]
    MCFR -->|"dispatch.get(nodeType)"| RULE[CaptureRule]
    RULE --> CFC[captureFnRefCandidates]
    CFC -->|"mode: args/list/rhs/value/varinit"| VN["value node(s)"]
    VN --> NV[normalizeValue]
    NV -->|"type in idTypes"| BARE["bare-identifier NormalizedRef"]
    NV -->|"type in layers: peel through"| NV
    NV -->|"type in unwrap: &fn / @Fn / fn _"| NV
    NV -->|"type in special"| NS[normalizeSpecial]
    NS --> SPECIAL["method_reference / this.x / method(:sym) / ... NormalizedRef"]
    BARE --> OUT["FnRefCandidate[]"]
    SPECIAL --> OUT
```
The loop back into `normalizeValue` is real recursion (bounded to depth 4), not a
simplification — a wrapper layer's inner value can itself be another wrapper layer
(e.g. an argument holding a parenthesized reference).

## Design rationale (why it's built this way)
The module's own header comment states the guiding constraint explicitly: resolving the
*dispatch* side (`o->cb(x)` → which concrete function `cb` currently holds) "needs
data-flow through struct fields," and "a wrong edge is worse than none" — so this module
deliberately covers only the deterministic half, the **registration** site, where "the
function's name is literally in the source." Every other design choice follows from
protecting that precision bar rather than maximizing recall:

- **Per-language specs are data, not code branches.** [`FN_REF_SPECS`](../catalog/src/extraction/function-ref.ts.md#FN_REF_SPECS)
  maps a language string to an [`FnRefSpec`](../catalog/src/extraction/function-ref.ts.md#FnRefSpec)
  built by small factory functions/constants — [`cFamilySpec`](../catalog/src/extraction/function-ref.ts.md#cFamilySpec)
  shared by C/C++/ObjC, and per-language literals like [`TS_JS_SPEC`](../catalog/src/extraction/function-ref.ts.md#TS_JS_SPEC),
  [`CSHARP_SPEC`](../catalog/src/extraction/function-ref.ts.md#CSHARP_SPEC),
  [`RUBY_SPEC`](../catalog/src/extraction/function-ref.ts.md#RUBY_SPEC),
  [`SWIFT_SPEC`](../catalog/src/extraction/function-ref.ts.md#SWIFT_SPEC). Adding a
  language means describing its grammar's value-position node types, not writing a new
  walker.
- **The gate rules are precision guards bought by specific false positives, not
  speculative hardening.** The `rhs`-mode skip in [`captureFnRefCandidates`](../catalog/src/extraction/function-ref.ts.md#captureFnRefCandidates)
  — when an assignment's left-hand name equals its right-hand identifier text
  (`this.status = status`, `o->cb = cb`) — exists because a same-named function elsewhere
  would otherwise resolve to the wrong target: the right-hand side there is a
  parameter/local being *stored*, not a reference to a same-named function. The comment
  attributes this directly to an "excalidraw A/B finding," i.e. it was observed as a real
  wrong edge on a real repository, not designed defensively in the abstract. The
  labeled-argument skip in [`normalizeValue`](../catalog/src/extraction/function-ref.ts.md#normalizeValue)
  (Swift/Kotlin `value: value`) is the identical rationale one layer down (a
  parameter-forwarding label, not a reference).
- **`idTypes` is per-language, not universal**, because "is a bare identifier ever a
  function value here" is itself language-dependent: [`idTypes`](../catalog/src/extraction/function-ref.ts.md#FnRefSpec.idTypes)
  is empty for Java, Kotlin, Ruby, and PHP because those languages' method/callable
  references always carry explicit syntax (`Type::method`, `::fn`, `method(:sym)`) — a
  bare identifier in an argument position in those languages is a parameter or local, so
  admitting it would only add wrong edges, never real ones.
- **`unwrap` distinguishes operators the grammar conflates.** C's `pointer_expression`
  node covers both `&x` (address-of — a real function reference) and `*x` (dereference — a
  data read). [`normalizeValue`](../catalog/src/extraction/function-ref.ts.md#normalizeValue)
  checks the operator token itself rather than trusting the node type, because — per the
  inline comment — "fmt's `*begin` reads resolved to its free `begin()` functions" before
  the check existed.
- **Ordering of the checks inside `normalizeValue` is deliberate**: bare identifier →
  transparent layer → unary unwrap → special form, each an `if` that returns before
  falling through. A node type only ever qualifies for one category per spec, so treating
  the categories as an ordered dispatch (rather than a rule engine trying every category)
  keeps each language spec's behavior fully determined by which maps it populates.

> [!inferred] The five-value [`CaptureMode`](../catalog/src/extraction/function-ref.ts.md#CaptureMode)
> enum (`args`/`rhs`/`value`/`list`/`varinit`) reads as the smallest set that covers every
> grammar's "container holding value(s)" shapes the author found across ~20 languages —
> the module doesn't state this design goal directly, but no spec needs a sixth mode, and
> every per-language dispatch table is built entirely from these five.

## Entry points
- [`maybeCaptureFnRefs`](../catalog/src/extraction/tree-sitter.ts.md#TreeSitterExtractor.maybeCaptureFnRefs)
  — the sole call site into this module's capture logic, reached once per AST node during
  `TreeSitterExtractor`'s walk (outside this subgraph). It looks up the current node's type
  in the language's [`dispatch`](../catalog/src/extraction/function-ref.ts.md#FnRefSpec.dispatch)
  map and does nothing if there's no rule or no enclosing symbol on the node stack — so for
  a language with no [`FnRefSpec`](../catalog/src/extraction/function-ref.ts.md#FnRefSpec)
  entry in [`FN_REF_SPECS`](../catalog/src/extraction/function-ref.ts.md#FN_REF_SPECS)
  (picked once, at extractor [`<constructor>`](../catalog/src/extraction/tree-sitter.ts.md#TreeSitterExtractor.-constructor)
  time), this entire mechanism is a no-op.
- [`captureFnRefCandidates`](../catalog/src/extraction/function-ref.ts.md#captureFnRefCandidates)
  — this module's actual entry point, called by `maybeCaptureFnRefs` with the matched
  [`CaptureRule`](../catalog/src/extraction/function-ref.ts.md#CaptureRule) once per
  container node. It is also imported directly by `tree-sitter.ts` — the packet's Subgraph
  shows the whole `tree-sitter.ts`
  module pulling in `FN_REF_SPECS`, `FnRefCandidate`, `FnRefSpec`, and this function
  together, confirming it is the only consumer.
- [`FN_REF_SPECS`](../catalog/src/extraction/function-ref.ts.md#FN_REF_SPECS) — not a
  function, but the configuration surface a new language integration edits to opt in at
  all; a language key absent from this map means `maybeCaptureFnRefs` reads `undefined`
  and every node in that language's files is skipped.

## Mechanism (step-by-step)
1. **A dispatch-table lookup decides whether a node is a "value container" at all.**
   [`maybeCaptureFnRefs`](../catalog/src/extraction/tree-sitter.ts.md#TreeSitterExtractor.maybeCaptureFnRefs)
   reads the visited node's [`<get>type`](../catalog/src/web-tree-sitter.d.ts.md#Node.-get-type)
   string and looks it up in the language spec's [`dispatch`](../catalog/src/extraction/function-ref.ts.md#FnRefSpec.dispatch)
   map — a `Map<string, CaptureRule>` where the key is a grammar node type
   (`argument_list`, `assignment_expression`, `initializer_pair`, …) and the value is a
   [`CaptureRule`](../catalog/src/extraction/function-ref.ts.md#CaptureRule) naming a
   [`mode`](../catalog/src/extraction/function-ref.ts.md#CaptureRule.mode) and, optionally,
   a [`field`](../catalog/src/extraction/function-ref.ts.md#CaptureRule.field). Most node
   types in a file produce no match and the walker moves on with no extra work.
2. **The matched `mode` decides which child node(s) are candidate values.**
   [`captureFnRefCandidates`](../catalog/src/extraction/function-ref.ts.md#captureFnRefCandidates)
   switches on the rule's mode: `args`/`list` collect every
   [`namedChild`](../catalog/src/web-tree-sitter.d.ts.md#Node.namedChild) (a call's
   arguments, an array's elements); `rhs` finds the assignment's right-hand side (via
   [`getChildByField`](../catalog/src/extraction/tree-sitter-helpers.ts.md#getChildByField)
   if a `field` is given, else the last named child) and applies the param-storage skip
   described above; `value` picks a keyed pair's value field, falling back to the last
   named child for grammars with no such field (Go's `keyed_element`); `varinit` finds a
   declarator's initializer while explicitly refusing destructuring patterns
   (`object_pattern`/`array_pattern`/`tuple_pattern`/`struct_pattern`), since `const {
   center } = ellipse` extracts data, never a function alias. Each branch reads
   [`<get>namedChildCount`](../catalog/src/web-tree-sitter.d.ts.md#Node.-get-namedChildCount)
   to walk children by index.
3. **Each candidate value node is normalized to zero or more names by bounded recursion.**
   [`normalizeValue`](../catalog/src/extraction/function-ref.ts.md#normalizeValue) checks,
   in order: is the node's type a bare-identifier type for this language
   ([`idTypes`](../catalog/src/extraction/function-ref.ts.md#FnRefSpec.idTypes) — if so,
   return its [`getNodeText`](../catalog/src/extraction/tree-sitter-helpers.ts.md#getNodeText));
   is it a transparent wrapper the spec lists in
   [`layers`](../catalog/src/extraction/function-ref.ts.md#FnRefSpec.layers) (peel into the
   named field, or fan out over every named child if the layer has no fixed field — the Go
   `expression_list` multi-assign case); is it a unary reference form in
   [`unwrap`](../catalog/src/extraction/function-ref.ts.md#FnRefSpec.unwrap) (C `&fn`,
   Pascal `@Fn`, Scala `fn _` — with the `pointer_expression` operator check that rejects
   `*x` dereferences); or does it need bespoke handling via
   [`special`](../catalog/src/extraction/function-ref.ts.md#FnRefSpec.special). Recursion is
   capped at depth 4 so a pathological wrapper chain can't spin.
4. **`special` node types get whole-node, language-specific extraction in `normalizeSpecial`,
   because their reference shape isn't "peel one field."**
   [`normalizeSpecial`](../catalog/src/extraction/function-ref.ts.md#normalizeSpecial)
   handles: Java/Kotlin method references (`this::run`, `Type::method`, `::topLevelFn`) by
   walking to the rightmost identifier child; Swift/ObjC selector expressions via
   [`lastNamedOfType`](../catalog/src/extraction/function-ref.ts.md#lastNamedOfType); Ruby's
   `method(:sym)` call shape and hook-DSL symbols (`before_action :authenticate`) via
   [`rubyEnclosingCall`](../catalog/src/extraction/function-ref.ts.md#rubyEnclosingCall) and
   [`isRubyHookCall`](../catalog/src/extraction/function-ref.ts.md#isRubyHookCall); and
   PHP's string/array callables (`usort($a, 'cmp')`, `[$this, 'method']`) via
   [`phpEnclosingCallName`](../catalog/src/extraction/function-ref.ts.md#phpEnclosingCallName)
   and [`phpStringContent`](../catalog/src/extraction/function-ref.ts.md#phpStringContent),
   which walk up to the enclosing call to confirm the string sits in a known
   callable-taking position before trusting it.
5. **Every resolved [`NormalizedRef`](../catalog/src/extraction/function-ref.ts.md#NormalizedRef)
   is packaged into an [`FnRefCandidate`](../catalog/src/extraction/function-ref.ts.md#FnRefCandidate)
   carrying the metadata a later stage needs, not just the name.**
   [`captureFnRefCandidates`](../catalog/src/extraction/function-ref.ts.md#captureFnRefCandidates)
   attaches the original capture [`mode`](../catalog/src/extraction/function-ref.ts.md#FnRefCandidate.mode),
   whether the source syntax was an explicit reference form rather than a bare identifier
   (`explicitRef`, computed by checking the *outer* value node's type against `idTypes`
   before normalization), and the position from
   [`startPosition`](../catalog/src/web-tree-sitter.d.ts.md#Node.startPosition)'s
   [`row`](../catalog/src/web-tree-sitter.d.ts.md#Point.row)/[`column`](../catalog/src/web-tree-sitter.d.ts.md#Point.column).
   The candidate's [`name`](../catalog/src/extraction/function-ref.ts.md#FnRefCandidate.name)
   is the only thing a naive implementation would keep — the rest is what lets the
   out-of-subgraph gating/resolution stage apply per-mode, per-language precision rules
   without re-deriving them from the AST.

## Key data structures
- [`FnRefSpec`](../catalog/src/extraction/function-ref.ts.md#FnRefSpec) — the whole
  per-language configuration: [`idTypes`](../catalog/src/extraction/function-ref.ts.md#FnRefSpec.idTypes)
  (which bare-identifier grammar types count as a function value),
  [`dispatch`](../catalog/src/extraction/function-ref.ts.md#FnRefSpec.dispatch) (container
  node type → `CaptureRule`), [`layers`](../catalog/src/extraction/function-ref.ts.md#FnRefSpec.layers)
  (transparent wrappers to peel through), [`unwrap`](../catalog/src/extraction/function-ref.ts.md#FnRefSpec.unwrap)
  (unary reference operators), [`special`](../catalog/src/extraction/function-ref.ts.md#FnRefSpec.special)
  (whole-node bespoke forms), and [`ungatedModes`](../catalog/src/extraction/function-ref.ts.md#FnRefSpec.ungatedModes)
  (capture modes that skip the same-file/import name gate applied *outside* this module,
  because — per its own doc comment — C has no symbol imports and repo-scale callback
  tables would otherwise be invisible to a same-file/import check).
- [`CaptureRule`](../catalog/src/extraction/function-ref.ts.md#CaptureRule) /
  [`CaptureMode`](../catalog/src/extraction/function-ref.ts.md#CaptureMode) — the five-value
  closed vocabulary (`args`, `rhs`, `value`, `list`, `varinit`) every language's dispatch
  table is built from, plus the optional [`field`](../catalog/src/extraction/function-ref.ts.md#CaptureRule.field)
  a mode reads its value from.
- [`NormalizedRef`](../catalog/src/extraction/function-ref.ts.md#NormalizedRef) — the
  internal, pre-packaging result of [`normalizeValue`](../catalog/src/extraction/function-ref.ts.md#normalizeValue)/[`normalizeSpecial`](../catalog/src/extraction/function-ref.ts.md#normalizeSpecial):
  a [`name`](../catalog/src/extraction/function-ref.ts.md#NormalizedRef.name), the
  [`node`](../catalog/src/extraction/function-ref.ts.md#NormalizedRef.node) it came from
  (for position), and an optional per-candidate `skipGate` override.
- [`FnRefCandidate`](../catalog/src/extraction/function-ref.ts.md#FnRefCandidate) — this
  module's public output shape: name, line/column, the originating `mode`, `explicitRef`,
  and `skipGate`. This is deliberately richer than "a name at a position" — every extra
  field exists because a downstream precision rule keys on it.
- [`Node`](../catalog/src/web-tree-sitter.d.ts.md#Node) / [`Point`](../catalog/src/web-tree-sitter.d.ts.md#Point)
  — the tree-sitter primitives this entire module is built on top of; nearly every
  function here is, mechanically, a sequence of [`namedChild`](../catalog/src/web-tree-sitter.d.ts.md#Node.namedChild)/[`getChildByField`](../catalog/src/extraction/tree-sitter-helpers.ts.md#getChildByField)
  navigations and [`getNodeText`](../catalog/src/extraction/tree-sitter-helpers.ts.md#getNodeText)
  extractions over these types.

## Dynamics (design intent)
> [!inferred] Nothing in this subgraph is concurrent — capture is a synchronous function
> call made once per matching AST node, from whatever thread is running the extraction walk
> ([`maybeCaptureFnRefs`](../catalog/src/extraction/tree-sitter.ts.md#TreeSitterExtractor.maybeCaptureFnRefs)
> is a plain private method, not async). The only "scheduling" concern visible in the
> source is the depth cap in [`normalizeValue`](../catalog/src/extraction/function-ref.ts.md#normalizeValue)
> (`depth > 4` returns `[]`) and the 4-hop walk-up caps in
> [`phpEnclosingCallName`](../catalog/src/extraction/function-ref.ts.md#phpEnclosingCallName)
> and [`rubyEnclosingCall`](../catalog/src/extraction/function-ref.ts.md#rubyEnclosingCall) —
> all bounds against runaway recursion on adversarial or deeply-nested source, not against
> concurrent access. The Evidence section of this packet lists no tests referencing this
> subgraph directly; validation for this mechanism (per the design doc alongside this
> module, out of subgraph) is a manual before/after A/B node-count and edge-count diff
> across real repositories rather than unit tests exercising these functions in isolation.

## Edge cases
- **A container node type can appear in `dispatch` for one language and mean something
  completely different in another's grammar** — the whole point of keying
  [`FN_REF_SPECS`](../catalog/src/extraction/function-ref.ts.md#FN_REF_SPECS) by language is
  that `assignment_expression`'s `field` for the right-hand side differs in name and
  shape between grammars ([`field`](../catalog/src/extraction/function-ref.ts.md#CaptureRule.field)
  is per-rule for exactly this reason), so a spec copy-pasted from a related language
  without checking its actual grammar output is a silent miss, not an error.
- **Same-named LHS/RHS and label/value pairs are deliberately treated as "not a
  reference,"** not as "unknown, assume yes" — the `rhs`-mode and `value_argument`-layer
  skips inside [`captureFnRefCandidates`](../catalog/src/extraction/function-ref.ts.md#captureFnRefCandidates)/[`normalizeValue`](../catalog/src/extraction/function-ref.ts.md#normalizeValue)
  return early rather than falling through to emit a (likely wrong) candidate.
- **`explicitRef` is computed from the outer value node's type, not the final normalized
  name** — a bare identifier that happens to normalize the same way as an explicit form
  still reports `explicitRef: false`, because the check in
  [`captureFnRefCandidates`](../catalog/src/extraction/function-ref.ts.md#captureFnRefCandidates)
  runs against `spec.idTypes` before recursing into `normalizeValue` at all.
- **`normalizeSpecial`'s `default` case silently returns `[]`** — any node type listed in a
  spec's `special` set that this function doesn't have a `case` for produces nothing,
  with no error surfaced; adding a language to `special` without adding a matching branch
  here is a silent no-op, not a crash.

## Open questions
> [!inferred] This module's own header comment and the [`ungatedModes`](../catalog/src/extraction/function-ref.ts.md#FnRefSpec.ungatedModes)
> doc comment both describe a "same-file/import name gate" applied to candidates — but the
> function that implements that gate (referenced by name as `flushFnRefCandidates` in the
> header comment) is not part of this packet's Subgraph, so exactly how `skipGate`,
> `explicitRef`, and `ungatedModes` combine at gating time cannot be confirmed from this
> module alone.
- How does the resolution stage (outside this subgraph) actually consume `FnRefCandidate.mode`/`explicitRef` when deciding same-file-vs-cross-file matching? This module only produces the candidates and their metadata; the consumption logic isn't visible here.
- No test in the configured test paths references any symbol in this subgraph (per this
  packet's Evidence) — is this mechanism's correctness validated only by the manual
  per-repo A/B methodology, or is there test coverage elsewhere that just doesn't reference
  these exact symbols (e.g. black-box tests that only assert on final edge counts)?

## See also
- [resolution-callback-synthesizer.ts](resolution-callback-synthesizer.ts.md) — the
  framework-heuristic layer that synthesizes dispatcher→handler edges; this module's
  candidates are the registration-side half of the same "make callbacks visible" problem.
- [resolution-index.ts](resolution-index.ts.md) — `ReferenceResolver`, which turns the
  `UnresolvedReference`s this module's candidates eventually become into persisted
  `references` edges.
- [extraction-tree-sitter.ts](extraction-tree-sitter.ts.md) — the core extraction engine
  whose AST walk calls `maybeCaptureFnRefs` and owns the per-extractor `FnRefSpec`
  selection this module's specs are chosen from.
- [extraction-tree-sitter-helpers.ts](extraction-tree-sitter-helpers.ts.md) — the shared
  `getNodeText`/`getChildByField` helpers this module calls throughout to navigate and read
  tree-sitter nodes.
