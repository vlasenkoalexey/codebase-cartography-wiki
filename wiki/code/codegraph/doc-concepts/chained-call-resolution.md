---
title: Chained static-factory / fluent call resolution
type: doc-concept
provenance: doc
source: docs/design/chained-call-resolution.md
updated: 2026-07-04
status: fresh
---
# Chained static-factory / fluent call resolution

## Definition
When a call's **receiver is itself a call** — a factory, singleton, or builder that
returns an object, as in `Foo.getInstance().bar()` — the outer method (`bar`) should
resolve to a `calls` edge on the type the inner call *returns* (`Foo::bar`), never to a
same-named decoy on an unrelated type. CodeGraph has no real type checker, so it recovers
the receiver's type from the factory's **declared return type** and then **validates** that
the method actually exists on that type before emitting an edge. Before this work every
statically-typed language dropped the receiver and bare-name-matched `bar`, which in 7 of 9
languages silently attached to the wrong type — a correctness bug, not just a coverage gap.
SHIPPED for 13 languages (C++, C, PHP, Java, Kotlin, C#, Swift, Rust, Go, Scala,
Objective-C, Dart, Pascal/Delphi); TypeScript and Luau were evaluated and intentionally
skipped (see below).

## The mental model — infer, then prove
The mechanism runs in three stages, split across extraction and resolution:

1. **Capture the factory's return type (extraction).** A per-language `getReturnType` hook
   normalizes the declared return into a bare type name — `*Foo`→`Foo`, `List<Bar>`→`List`,
   `-> Self` / `: self` / `this.type` → the declaring type — and writes it to
   `nodes.return_type` (schema v5). This is the only place the receiver's type can come
   from without a type checker, which is exactly why the mechanism needs a **reliably
   declared** return type.
2. **Preserve the chained receiver (extraction).** The extractor encodes
   `Foo.getInstance().bar()` as the marker string `Foo.getInstance().bar` — the `().`
   marker never appears in an ordinary reference — so the chain survives to the resolver
   intact instead of collapsing to bare `bar`. A per-language **node-type gate** keeps
   ordinary *instance* chains (`list.map().filter()`) bare so their existing resolution is
   untouched; only capitalized-receiver / factory chains re-encode.
3. **Resolve AND validate (resolution).** The receiver's type is inferred from what the
   inner call returns, the outer method is resolved **on that type**, and the result is
   validated: the method must exist on the type (or a supertype it conforms to). A wrong
   inference therefore yields **no edge**, never a wrong one. This validation — not
   guessing — is the decoy / absent-method guarantee that makes the feature safe to ship.

## In codegraph (grounded)
- **The `getReturnType` hook** is part of the per-language extractor interface —
  [`LanguageExtractor.getReturnType`](../catalog/src/extraction/tree-sitter-types.ts.md#LanguageExtractor.getReturnType)
  — implemented per language under `src/extraction/languages/`; its output lands on the
  node's `return_type` field. Receiver re-encoding happens in the tree-sitter extraction
  layer (`src/extraction/tree-sitter.ts`) behind the per-language node-type gate.
- **Three shared chain resolvers** live in `src/resolution/name-matcher.ts`, split by
  receiver syntax, all funneling into one validated type lookup:
  - [`matchCppCallChain`](../catalog/src/resolution/name-matcher.ts.md#matchCppCallChain) —
    `field_expression` receivers (`Foo::instance().bar`) — C++, C.
  - [`matchScopedCallChain`](../catalog/src/resolution/name-matcher.ts.md#matchScopedCallChain) —
    `::`-scoped receivers (`Cls::for($x)->m`, `Foo::new().bar`) — PHP, Rust.
  - [`matchDottedCallChain`](../catalog/src/resolution/name-matcher.ts.md#matchDottedCallChain) —
    dotted receivers (`Foo.create().bar`) — Java, Kotlin, C#, Swift, Go, Scala, Dart.
- **The validation core** every resolver ends in is
  [`resolveMethodOnType`](../catalog/src/resolution/name-matcher.ts.md#resolveMethodOnType),
  which does the "method must exist on the type or a conforming supertype" check (the
  supertype/conformance walk). These resolvers are dispatched from the strategy ladder in
  [`matchReference`](../catalog/src/resolution/name-matcher.ts.md#matchReference).
- **The capitalized-bare-call gate**
  [`CONSTRUCTS_VIA_BARE_CALL`](../catalog/src/resolution/name-matcher.ts.md#CONSTRUCTS_VIA_BARE_CALL)
  marks languages where an unprefixed capitalized call `Foo(args)` constructs the class, so
  such a chain resolves on that class.
- **The conformance second pass (#754).** When the chained method lives on a *supertype*
  the return type conforms to (inherited / default-interface / trait / mixin / embedded
  method), the first pass can't see it because `implements`/`extends` edges aren't built
  yet. Failed chain refs for languages in
  [`CHAIN_LANGUAGES`](../catalog/src/resolution/index.ts.md#CHAIN_LANGUAGES) are deferred
  and re-resolved after edges exist by
  [`ReferenceResolver.resolveChainedCallsViaConformance`](../catalog/src/resolution/index.ts.md#ReferenceResolver.resolveChainedCallsViaConformance),
  which walks the supertype chain. This is what enables Swift protocol-extension, Rust
  trait-default, Go embedded, Dart mixin, and Java/Kotlin/C# inherited chained methods.
- Per-reference resolution flows through
  [`ReferenceResolver.resolveOne`](../catalog/src/resolution/index.ts.md#ReferenceResolver.resolveOne);
  the whole feature is a coverage/precision improvement to the static reference resolver
  (see [resolution-index.ts](../concepts/resolution-index.ts.md)). Owning modules:
  `src/resolution/index.ts`, `src/resolution/name-matcher.ts`, `src/extraction/tree-sitter.ts`.

## Why it matters / when it applies
- **Precision, not just recall.** The prior bare-name match wasn't merely missing edges —
  it produced *wrong* ones (Kotlin arrow: +49 / −438; Rust clap: +937 / −775, ~622 wrong→right
  retargets; Scala gatling stdlib `Option.map` mis-tied to `Validation::*`). Because every
  resolver validates, the A/B "removed" counts are wrong-edge corrections, not losses.
- **Needs a reliably declared return type.** This is the real requirement — not "statically
  typed": PHP qualifies via its `: self` / `: Type` return declarations. The mechanism fits
  the 13 shipped languages precisely because their return types are dependably declared.
- **Why TypeScript was skipped.** TS leans on type *inference* — e.g. NestJS's
  `Test.createTestingModule(m) { return new TestingModuleBuilder(...) }` has no
  `: TestingModuleBuilder` annotation — so the factory's type can't be recovered, the
  re-encoded chain can't resolve, and it *drops* the bare-name edge the existing resolver
  found. Real-repo A/B was +0 added on typeorm and nest with a net recall regression
  (−164 on nest, mostly `Test.createTestingModule({…}).compile()`). That violates the
  recall-first invariant while adding nothing where it doesn't hurt (TS method names are
  unique enough that bare-name already lands them). Luau was likewise evaluated and skipped
  (gradually typed; additive-safe but +0 on real repos). The lesson: gradually-typed
  languages omit declared return types too often, and dynamically-typed ones have none.
- **Single-hop only.** A chain re-encodes exactly one hop; deeper hops (`a.b().c().d()`)
  keep the bare name because the inner `()` defeats the `Class::method` split.
- **When re-indexing.** The extractor changes are gated by `EXTRACTION_VERSION` (now 18); an
  existing graph must be rebuilt with `codegraph index -f` to pick up the newer extractor.

## Connections
- Code concepts:
  [resolution-index.ts](../concepts/resolution-index.ts.md) — the `ReferenceResolver`
  orchestrator that owns the deferred conformance pass (home concept);
  [resolution-types.ts](../concepts/resolution-types.ts.md) — the `UnresolvedRef` /
  `ResolutionContext` types the resolvers operate on;
  [resolution-callback-synthesizer.ts](../concepts/resolution-callback-synthesizer.ts.md) —
  the *separate* dynamic-dispatch / callback edge mechanism this doc contrasts itself with;
  [extraction-tree-sitter.ts](../concepts/extraction-tree-sitter.ts.md) and
  [extraction-tree-sitter-types.ts](../concepts/extraction-tree-sitter-types.ts.md) — where
  the receiver marker is encoded and `getReturnType` is declared;
  [types.ts](../concepts/types.ts.md) — the `NodeKind` / `EdgeKind` (`calls`, `returns`,
  `instantiates`) vocabulary these edges use.
- Module catalogs:
  [resolution/index.ts](../catalog/src/resolution/index.ts.md),
  [resolution/name-matcher.ts](../catalog/src/resolution/name-matcher.ts.md),
  [extraction/tree-sitter-types.ts](../catalog/src/extraction/tree-sitter-types.ts.md).
- Related doc-concepts:
  [dynamic-dispatch-coverage](dynamic-dispatch-coverage.md) — the complementary mechanism
  (callback / observer / EventEmitter / React-render / JSX-child / ORM edge synthesis) that
  bridges *dynamic* dispatch, as opposed to this doc's *static* chained-receiver resolution;
  [value-reference-edges](value-reference-edges.md).

## Source
Extracted from `docs/design/chained-call-resolution.md` (kept in place).
