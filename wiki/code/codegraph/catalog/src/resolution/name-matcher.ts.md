---
title: 'Module: src/resolution/name-matcher.ts'
type: catalog
provenance: extracted
module: src/resolution/name-matcher.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/resolution/`name-matcher.ts`/
symbols:
  matchMethodCall: matchMethodCall().
  matchReference: matchReference().
  resolveMethodOnType: resolveMethodOnType().
  matchFunctionRef: matchFunctionRef().
  matchByExactName: matchByExactName().
  inferJavaFieldReceiverType: inferJavaFieldReceiverType().
  findBestMatch: findBestMatch().
  matchDottedCallChain: matchDottedCallChain().
  matchByQualifiedName: matchByQualifiedName().
  inferCppReceiverType: inferCppReceiverType().
  matchFuzzy: matchFuzzy().
  matchByFilePath: matchByFilePath().
  enclosingScopeStartLine: enclosingScopeStartLine().
  inferLocalReceiverType: inferLocalReceiverType().
  lookupCalleeReturnType: lookupCalleeReturnType().
  importedFqnOf: importedFqnOf().
  pickClosestFileNode: pickClosestFileNode().
  applyLanguageGate: applyLanguageGate().
  cppClassExists: cppClassExists().
  matchScopedCallChain: matchScopedCallChain().
  resolveCppCallResultType: resolveCppCallResultType().
  matchCppCallChain: matchCppCallChain().
  preferCallSiteFile: preferCallSiteFile().
  sameLanguageFamily: sameLanguageFamily().
  inferCppAutoInitializerType: inferCppAutoInitializerType().
  crossesKnownFamily: crossesKnownFamily().
  AMBIGUOUS_NAME_CEILING: AMBIGUOUS_NAME_CEILING.
  isKnownLanguageFamily: isKnownLanguageFamily().
  normalizeCppTypeName: normalizeCppTypeName().
  computePathProximity: computePathProximity().
  resolveAmbiguousNameCeiling: resolveAmbiguousNameCeiling().
  normalizeInferredTypeName: normalizeInferredTypeName().
  localReceiverTypePatterns: localReceiverTypePatterns().
  LANGUAGE_FAMILY: LANGUAGE_FAMILY.
  cppLastSegment: cppLastSegment().
  DEFAULT_AMBIGUOUS_NAME_CEILING: DEFAULT_AMBIGUOUS_NAME_CEILING.
  splitCamelCase: splitCamelCase().
  pathProximityFromDirs: pathProximityFromDirs().
  CPP_NON_TYPE_TOKENS: CPP_NON_TYPE_TOKENS.
  buildDeclaratorRegex: buildDeclaratorRegex().
  CONSTRUCTS_VIA_BARE_CALL: CONSTRUCTS_VIA_BARE_CALL.
  NON_TYPE_RECEIVER_TOKENS: NON_TYPE_RECEIVER_TOKENS.
---
# Module: [`src/resolution/name-matcher.ts`](../../../../../../raw/code/codegraph/src/resolution/name-matcher.ts)

## Functions
- `applyLanguageGate(candidates: Node[], ref: UnresolvedRef)` — [`L187`](../../../../../../raw/code/codegraph/src/resolution/name-matcher.ts#L187) — Drop cross-language candidates from a name lookup. Two regimes:
- `buildDeclaratorRegex(escapedReceiver: string)` — [`L611`](../../../../../../raw/code/codegraph/src/resolution/name-matcher.ts#L611)
- `computePathProximity(filePath1: string, filePath2: string)` — [`L1599`](../../../../../../raw/code/codegraph/src/resolution/name-matcher.ts#L1599) — Compute directory proximity between two file paths.
- `cppClassExists(name: string, ref: UnresolvedRef, context: ResolutionContext)` — [`L732`](../../../../../../raw/code/codegraph/src/resolution/name-matcher.ts#L732) — Does the graph contain a class/struct named `name`'s last segment?
- `cppLastSegment(name: string)` — [`L683`](../../../../../../raw/code/codegraph/src/resolution/name-matcher.ts#L683) — Last `::`-separated segment of a (possibly namespace-qualified) C++ name.
- `crossesKnownFamily(a: string, b: string)` — [`L174`](../../../../../../raw/code/codegraph/src/resolution/name-matcher.ts#L174) — True when `a` and `b` are two DIFFERENT *known* language families — the
- `enclosingScopeStartLine(ref: UnresolvedRef, context: ResolutionContext)` — [`L1224`](../../../../../../raw/code/codegraph/src/resolution/name-matcher.ts#L1224) — 1-based start line of the tightest function/method enclosing the call.
- `findBestMatch(ref: UnresolvedRef, candidates: Node[], _context: ResolutionContext)` — [`L1608`](../../../../../../raw/code/codegraph/src/resolution/name-matcher.ts#L1608) — Find the best matching node when there are multiple candidates
- `importedFqnOf(typeName: string, ref: UnresolvedRef, context: ResolutionContext)` — [`L969`](../../../../../../raw/code/codegraph/src/resolution/name-matcher.ts#L969) — When several classes share a simple type name, the caller file's import of
- `inferCppAutoInitializerType(line: string, receiverName: string, ref: UnresolvedRef, context: ResolutionContext, depth: number)` — [`L786`](../../../../../../raw/code/codegraph/src/resolution/name-matcher.ts#L786) — Recover the type of an `auto`-declared local from its initializer on the
- `inferCppReceiverType(receiverName: string, ref: UnresolvedRef, context: ResolutionContext, depth?: number)` — [`L617`](../../../../../../raw/code/codegraph/src/resolution/name-matcher.ts#L617)
- `inferJavaFieldReceiverType(receiverName: string, ref: UnresolvedRef, context: ResolutionContext)` — [`L989`](../../../../../../raw/code/codegraph/src/resolution/name-matcher.ts#L989) — Java/Kotlin: infer a receiver's declared type by walking field declarations
- `inferLocalReceiverType(receiverName: string, ref: UnresolvedRef, context: ResolutionContext)` — [`L1243`](../../../../../../raw/code/codegraph/src/resolution/name-matcher.ts#L1243) — Infer a receiver's type from its local declaration/initializer in the
- `isKnownLanguageFamily(lang: string)` — [`L161`](../../../../../../raw/code/codegraph/src/resolution/name-matcher.ts#L161) — True when `lang` belongs to a known multi-language family (jvm/apple/web/c).
- `localReceiverTypePatterns(language: "typescript" | "javascript" | "tsx" | "jsx" | "python" | "go" | "rust" | "java" | "c" | "cpp" | "csharp" | "razor" | "php" | "ruby" | "swift" | "kotlin" | "dart" | "svelte" | "vue" | ... 20 more ... | "unknown", r: string)` — [`L1076`](../../../../../../raw/code/codegraph/src/resolution/name-matcher.ts#L1076) — Per-language patterns that recover a local variable's (or typed parameter's)
- `lookupCalleeReturnType(callee: string, ref: UnresolvedRef, context: ResolutionContext)` — [`L694`](../../../../../../raw/code/codegraph/src/resolution/name-matcher.ts#L694) — Return type captured at extraction for `Class::method` (or a free function),
- `matchByExactName(ref: UnresolvedRef, context: ResolutionContext)` — [`L343`](../../../../../../raw/code/codegraph/src/resolution/name-matcher.ts#L343) — Try to resolve a reference by exact name match
- `matchByFilePath(ref: UnresolvedRef, context: ResolutionContext)` — [`L41`](../../../../../../raw/code/codegraph/src/resolution/name-matcher.ts#L41) — Try to resolve a path-like reference (e.g., "snippets/drawer-menu.liquid")
- `matchByQualifiedName(ref: UnresolvedRef, context: ResolutionContext)` — [`L403`](../../../../../../raw/code/codegraph/src/resolution/name-matcher.ts#L403) — Try to resolve by qualified name
- `matchCppCallChain(ref: UnresolvedRef, context: ResolutionContext)` — [`L815`](../../../../../../raw/code/codegraph/src/resolution/name-matcher.ts#L815) — Resolve a C++ chained call whose receiver is itself a call — encoded by the
- `matchDottedCallChain(ref: UnresolvedRef, context: ResolutionContext)` — [`L876`](../../../../../../raw/code/codegraph/src/resolution/name-matcher.ts#L876) — Resolve a dotted chained call whose receiver is a static factory / fluent call —
- `matchFunctionRef(ref: UnresolvedRef, context: ResolutionContext)` — [`L206`](../../../../../../raw/code/codegraph/src/resolution/name-matcher.ts#L206) — Resolve a function-as-value reference (#756) — a function name used as a — documented in [resolution-index.ts](../../../concepts/resolution-index.ts.md)
- `matchFuzzy(ref: UnresolvedRef, context: ResolutionContext)` — [`L1712`](../../../../../../raw/code/codegraph/src/resolution/name-matcher.ts#L1712) — Fuzzy match - last resort with lower confidence
- `matchMethodCall(ref: UnresolvedRef, context: ResolutionContext)` — [`L1324`](../../../../../../raw/code/codegraph/src/resolution/name-matcher.ts#L1324) — Try to resolve by method name on a class/object — documented in [resolution-index.ts](../../../concepts/resolution-index.ts.md)
- `matchReference(ref: UnresolvedRef, context: ResolutionContext)` — [`L1745`](../../../../../../raw/code/codegraph/src/resolution/name-matcher.ts#L1745) — Match all strategies in order of confidence — documented in [resolution-index.ts](../../../concepts/resolution-index.ts.md)
- `matchScopedCallChain(ref: UnresolvedRef, context: ResolutionContext)` — [`L837`](../../../../../../raw/code/codegraph/src/resolution/name-matcher.ts#L837) — Resolve a `::`-scoped factory chain whose receiver is a scoped/static call —
- `normalizeCppTypeName(typeName: string)` — [`L590`](../../../../../../raw/code/codegraph/src/resolution/name-matcher.ts#L590)
- `normalizeInferredTypeName(raw: string)` — [`L1061`](../../../../../../raw/code/codegraph/src/resolution/name-matcher.ts#L1061) — Normalize a captured type expression to a simple type name: drop generic
- `pathProximityFromDirs(dir1: string[], filePath2: string)` — [`L1577`](../../../../../../raw/code/codegraph/src/resolution/name-matcher.ts#L1577) — Compute directory proximity from a pre-split list of directory segments
- `pickClosestFileNode(candidates: Node[], ref: UnresolvedRef)` — [`L113`](../../../../../../raw/code/codegraph/src/resolution/name-matcher.ts#L113) — Among several file nodes that all match a bare include/import by basename,
- `preferCallSiteFile(nodes: Node[], callSiteFile: string)` — [`L469`](../../../../../../raw/code/codegraph/src/resolution/name-matcher.ts#L469) — When a symbol name is ambiguous across files, prefer the candidate(s) declared
- `resolveAmbiguousNameCeiling()` — [`L29`](../../../../../../raw/code/codegraph/src/resolution/name-matcher.ts#L29)
- `resolveCppCallResultType(inner: string, ref: UnresolvedRef, context: ResolutionContext, depth?: number)` — [`L749`](../../../../../../raw/code/codegraph/src/resolution/name-matcher.ts#L749) — Infer the class produced by a C++ call/construction expression, using return
- `resolveMethodOnType(typeName: string, methodName: string, ref: UnresolvedRef, context: ResolutionContext, confidence: number, resolvedBy: "import" | "exact-match" | ... 5 more ... | "function-ref", preferredFqn?: string | undefined, depth?: number)` — [`L482`](../../../../../../raw/code/codegraph/src/resolution/name-matcher.ts#L482)
- `sameLanguageFamily(a: string, b: string)` — [`L149`](../../../../../../raw/code/codegraph/src/resolution/name-matcher.ts#L149)
- `splitCamelCase(str: string)` — [`L1560`](../../../../../../raw/code/codegraph/src/resolution/name-matcher.ts#L1560) — Split a camelCase or PascalCase string into words.

## Module values
- `AMBIGUOUS_NAME_CEILING` — [`L35`](../../../../../../raw/code/codegraph/src/resolution/name-matcher.ts#L35)
- `CONSTRUCTS_VIA_BARE_CALL` — [`L864`](../../../../../../raw/code/codegraph/src/resolution/name-matcher.ts#L864) — Languages where an unprefixed capitalized call `Foo(args)` constructs the
- `CPP_NON_TYPE_TOKENS` — [`L583`](../../../../../../raw/code/codegraph/src/resolution/name-matcher.ts#L583)
- `DEFAULT_AMBIGUOUS_NAME_CEILING` — [`L28`](../../../../../../raw/code/codegraph/src/resolution/name-matcher.ts#L28) — Ceiling on how many same-named definitions a FUZZY name-match strategy will
- `LANGUAGE_FAMILY` — [`L140`](../../../../../../raw/code/codegraph/src/resolution/name-matcher.ts#L140) — Language families that share a type system / runtime, so a same-language-only
- `NON_TYPE_RECEIVER_TOKENS` — [`L1051`](../../../../../../raw/code/codegraph/src/resolution/name-matcher.ts#L1051)

