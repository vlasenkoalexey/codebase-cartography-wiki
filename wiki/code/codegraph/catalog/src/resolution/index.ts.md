---
title: 'Module: src/resolution/index.ts'
type: catalog
provenance: extracted
module: src/resolution/index.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/resolution/`index.ts`/
symbols:
  ReferenceResolver.createContext: ReferenceResolver#createContext().
  ReferenceResolver.resolveOne: ReferenceResolver#resolveOne().
  ReferenceResolver.resolveDeferredThisMemberRefs: ReferenceResolver#resolveDeferredThisMemberRefs().
  ReferenceResolver.resolveBatchYielding: ReferenceResolver#resolveBatchYielding().
  ReferenceResolver.resolveAll: ReferenceResolver#resolveAll().
  ReferenceResolver.resolveAndPersistBatched: ReferenceResolver#resolveAndPersistBatched().
  ReferenceResolver.-constructor: ReferenceResolver#`<constructor>`().
  ReferenceResolver.isBuiltInOrExternal: ReferenceResolver#isBuiltInOrExternal().
  ReferenceResolver.resolveThisMemberFnRef: ReferenceResolver#resolveThisMemberFnRef().
  ReferenceResolver.queries: ReferenceResolver#queries.
  ReferenceResolver.clearCaches: ReferenceResolver#clearCaches().
  ReferenceResolver.createEdges: ReferenceResolver#createEdges().
  ReferenceResolver.resolveChainedCallsViaConformance: ReferenceResolver#resolveChainedCallsViaConformance().
  ReferenceResolver.resolveAndPersist: ReferenceResolver#resolveAndPersist().
  ReferenceResolver.resolveCfmlComponentPath: ReferenceResolver#resolveCfmlComponentPath().
  ReferenceResolver.gateLanguage: ReferenceResolver#gateLanguage().
  ReferenceResolver.context: ReferenceResolver#context.
  ReferenceResolver.resolveRazorUsing: ReferenceResolver#resolveRazorUsing().
  ReferenceResolver.runPostExtract: ReferenceResolver#runPostExtract().
  ReferenceResolver.matchesAnyImport: ReferenceResolver#matchesAnyImport().
  ReferenceResolver.gateFrameworkLanguage: ReferenceResolver#gateFrameworkLanguage().
  ReferenceResolver.warmCaches: ReferenceResolver#warmCaches().
  ReferenceResolver.knownNames: ReferenceResolver#knownNames.
  ReferenceResolver.readFileCached: ReferenceResolver#readFileCached().
  ReferenceResolver.getLanguageFromNodeId: ReferenceResolver#getLanguageFromNodeId().
  ReferenceResolver.initialize: ReferenceResolver#initialize().
  createResolver: createResolver().
  SUPERTYPE_BEARING_KINDS: SUPERTYPE_BEARING_KINDS.
  ReferenceResolver.nameCache: ReferenceResolver#nameCache.
  ReferenceResolver.projectRoot: ReferenceResolver#projectRoot.
  ReferenceResolver.nodeCache: ReferenceResolver#nodeCache.
  ReferenceResolver.importMappingCache: ReferenceResolver#importMappingCache.
  ReferenceResolver.reExportCache: ReferenceResolver#reExportCache.
  ReferenceResolver.getFilePathFromNodeId: ReferenceResolver#getFilePathFromNodeId().
  ReferenceResolver.lowerNameCache: ReferenceResolver#lowerNameCache.
  ReferenceResolver.qualifiedNameCache: ReferenceResolver#qualifiedNameCache.
  ReferenceResolver.methodMatchCache: ReferenceResolver#methodMatchCache.
  ReferenceResolver.fileCache: ReferenceResolver#fileCache.
  ReferenceResolver.getRazorUsings: ReferenceResolver#getRazorUsings().
  ReferenceResolver.frameworks: ReferenceResolver#frameworks.
  ReferenceResolver.fileLinesCache: ReferenceResolver#fileLinesCache.
  ReferenceResolver.getDetectedFrameworks: ReferenceResolver#getDetectedFrameworks().
  ReferenceResolver.deferredChainRefs: ReferenceResolver#deferredChainRefs.
  ReferenceResolver.deferredThisMemberRefs: ReferenceResolver#deferredThisMemberRefs.
  ReferenceResolver.projectAliases: ReferenceResolver#projectAliases.
  ReferenceResolver.goModule: ReferenceResolver#goModule.
  ReferenceResolver.workspacePackages: ReferenceResolver#workspacePackages.
  ReferenceResolver.knownFiles: ReferenceResolver#knownFiles.
  ReferenceResolver.hasAnyPossibleMatch: ReferenceResolver#hasAnyPossibleMatch().
  resolveCacheLimit: resolveCacheLimit().
  ReferenceResolver: ReferenceResolver#
  ReferenceResolver.cachesWarmed: ReferenceResolver#cachesWarmed.
  DEFAULT_CACHE_LIMIT: DEFAULT_CACHE_LIMIT.
  PYTHON_BUILT_IN_METHODS: PYTHON_BUILT_IN_METHODS.
  ReferenceResolver.razorUsingsCache: ReferenceResolver#razorUsingsCache.
  CHAIN_LANGUAGES: CHAIN_LANGUAGES.
  SCOPED_CHAIN_LANGUAGES: SCOPED_CHAIN_LANGUAGES.
  CHAIN_SHAPE: CHAIN_SHAPE.
  JS_BUILT_INS: JS_BUILT_INS.
  REACT_HOOKS: REACT_HOOKS.
  PYTHON_BUILT_INS: PYTHON_BUILT_INS.
  PYTHON_BUILT_IN_TYPES: PYTHON_BUILT_IN_TYPES.
  GO_STDLIB_PACKAGES: GO_STDLIB_PACKAGES.
  GO_BUILT_INS: GO_BUILT_INS.
  PASCAL_UNIT_PREFIXES: PASCAL_UNIT_PREFIXES.
  PASCAL_BUILT_INS: PASCAL_BUILT_INS.
  C_BUILT_INS: C_BUILT_INS.
  CPP_BUILT_INS: CPP_BUILT_INS.
---
# Module: [`src/resolution/index.ts`](../../../../../../raw/code/codegraph/src/resolution/index.ts)

## Classes
### `ReferenceResolver`
- def: [`src/resolution/index.ts:200`](../../../../../../raw/code/codegraph/src/resolution/index.ts#L200)
- doc: Reference Resolver
- signature: `class ReferenceResolver`
- members:
  - `<constructor>(projectRoot: string, queries: QueryBuilder)` — [`L244`](../../../../../../raw/code/codegraph/src/resolution/index.ts#L244) — Reference Resolver — documented in [resolution-index.ts](../../../concepts/resolution-index.ts.md)
  - `clearCaches(method)` — [`L325`](../../../../../../raw/code/codegraph/src/resolution/index.ts#L325) — Clear internal caches
  - `createContext(method)` — [`L360`](../../../../../../raw/code/codegraph/src/resolution/index.ts#L360) — Create the resolution context — documented in [resolution-index.ts](../../../concepts/resolution-index.ts.md)
  - `createEdges(method)` — [`L859`](../../../../../../raw/code/codegraph/src/resolution/index.ts#L859) — Create edges from resolved references — documented in [resolution-index.ts](../../../concepts/resolution-index.ts.md)
  - `gateFrameworkLanguage(method)` — [`L1623`](../../../../../../raw/code/codegraph/src/resolution/index.ts#L1623) — Drop a FRAMEWORK-strategy resolution that crosses two *known* language
  - `gateLanguage(method)` — [`L1601`](../../../../../../raw/code/codegraph/src/resolution/index.ts#L1601)
  - `getDetectedFrameworks(method)` — [`L1162`](../../../../../../raw/code/codegraph/src/resolution/index.ts#L1162) — Get detected frameworks
  - `getFilePathFromNodeId(method)` — [`L1273`](../../../../../../raw/code/codegraph/src/resolution/index.ts#L1273) — Get file path from node ID
  - `getLanguageFromNodeId(method)` — [`L1281`](../../../../../../raw/code/codegraph/src/resolution/index.ts#L1281) — Get language from node ID
  - `getRazorUsings(method)` — [`L1303`](../../../../../../raw/code/codegraph/src/resolution/index.ts#L1303) — Collect the `@using` namespaces in scope for a `.razor`/`.cshtml` file: its
  - `hasAnyPossibleMatch(method)` — [`L629`](../../../../../../raw/code/codegraph/src/resolution/index.ts#L629) — Check if a reference name has any possible match in the codebase.
  - `initialize(method)` — [`L270`](../../../../../../raw/code/codegraph/src/resolution/index.ts#L270) — Initialize the resolver (detect frameworks, etc.)
  - `isBuiltInOrExternal(method)` — [`L1169`](../../../../../../raw/code/codegraph/src/resolution/index.ts#L1169) — Check if reference is to a built-in or external symbol — documented in [resolution-index.ts](../../../concepts/resolution-index.ts.md)
  - `matchesAnyImport(method)` — [`L701`](../../../../../../raw/code/codegraph/src/resolution/index.ts#L701) — Does `ref.referenceName` match an import declared in its containing
  - `readFileCached(method)` — [`L341`](../../../../../../raw/code/codegraph/src/resolution/index.ts#L341) — `readFile` through the LRU content cache (null = read failed, also cached).
  - `resolveAll(method)` — [`L561`](../../../../../../raw/code/codegraph/src/resolution/index.ts#L561) — Resolve all unresolved references — documented in [resolution-index.ts](../../../concepts/resolution-index.ts.md)
  - `resolveAndPersist(method)` — [`L914`](../../../../../../raw/code/codegraph/src/resolution/index.ts#L914) — Resolve and persist edges to database
  - `resolveAndPersistBatched(method)` — [`L1049`](../../../../../../raw/code/codegraph/src/resolution/index.ts#L1049) — Resolve and persist in batches to keep memory bounded. — documented in [resolution-callback-synthesizer.ts](../../../concepts/resolution-callback-synthesizer.ts.md)
  - `resolveBatchYielding(method)` — [`L1002`](../../../../../../raw/code/codegraph/src/resolution/index.ts#L1002) — Resolve one batch with a yield checkpoint between EVERY ref so the #850 — documented in [resolution-index.ts](../../../concepts/resolution-index.ts.md)
  - `resolveCfmlComponentPath(method)` — [`L1369`](../../../../../../raw/code/codegraph/src/resolution/index.ts#L1369) — Resolve a CFML inheritance reference written as a component path (#1152).
  - `resolveChainedCallsViaConformance(method)` — [`L955`](../../../../../../raw/code/codegraph/src/resolution/index.ts#L955) — Second resolution pass for chained static-factory / fluent calls whose
  - `resolveDeferredThisMemberRefs(method)` — [`L1499`](../../../../../../raw/code/codegraph/src/resolution/index.ts#L1499) — Second pass for `this.<member>` refs whose member wasn't on the enclosing — documented in [index.ts](../../../concepts/index.ts.md)
  - `resolveOne(method)` — [`L718`](../../../../../../raw/code/codegraph/src/resolution/index.ts#L718) — Resolve a single reference — documented in [resolution-index.ts](../../../concepts/resolution-index.ts.md)
  - `resolveRazorUsing(method)` — [`L1332`](../../../../../../raw/code/codegraph/src/resolution/index.ts#L1332) — Resolve a Razor/Blazor simple type ref through the file's `@using`
  - `resolveThisMemberFnRef(method)` — [`L1449`](../../../../../../raw/code/codegraph/src/resolution/index.ts#L1449) — Resolve a `this.<member>` function-as-value reference (#756/#808) to the — documented in [resolution-index.ts](../../../concepts/resolution-index.ts.md)
  - `runPostExtract(method)` — [`L283`](../../../../../../raw/code/codegraph/src/resolution/index.ts#L283) — Run each framework resolver's cross-file finalization pass and persist
  - `warmCaches(method)` — [`L310`](../../../../../../raw/code/codegraph/src/resolution/index.ts#L310) — Pre-build lightweight caches for resolution.
  - `cachesWarmed` — [`L234`](../../../../../../raw/code/codegraph/src/resolution/index.ts#L234)
  - `context` — [`L203`](../../../../../../raw/code/codegraph/src/resolution/index.ts#L203)
  - `deferredChainRefs` — [`L210`](../../../../../../raw/code/codegraph/src/resolution/index.ts#L210)
  - `deferredThisMemberRefs` — [`L215`](../../../../../../raw/code/codegraph/src/resolution/index.ts#L215)
  - `fileCache` — [`L224`](../../../../../../raw/code/codegraph/src/resolution/index.ts#L224)
  - `fileLinesCache` — [`L230`](../../../../../../raw/code/codegraph/src/resolution/index.ts#L230)
  - `frameworks` — [`L204`](../../../../../../raw/code/codegraph/src/resolution/index.ts#L204)
  - `goModule` — [`L240`](../../../../../../raw/code/codegraph/src/resolution/index.ts#L240)
  - `importMappingCache` — [`L225`](../../../../../../raw/code/codegraph/src/resolution/index.ts#L225)
  - `knownFiles` — [`L233`](../../../../../../raw/code/codegraph/src/resolution/index.ts#L233)
  - `knownNames` — [`L232`](../../../../../../raw/code/codegraph/src/resolution/index.ts#L232)
  - `lowerNameCache` — [`L228`](../../../../../../raw/code/codegraph/src/resolution/index.ts#L228)
  - `methodMatchCache` — [`L231`](../../../../../../raw/code/codegraph/src/resolution/index.ts#L231)
  - `nameCache` — [`L227`](../../../../../../raw/code/codegraph/src/resolution/index.ts#L227)
  - `nodeCache` — [`L223`](../../../../../../raw/code/codegraph/src/resolution/index.ts#L223)
  - `projectAliases` — [`L238`](../../../../../../raw/code/codegraph/src/resolution/index.ts#L238)
  - `projectRoot` — [`L201`](../../../../../../raw/code/codegraph/src/resolution/index.ts#L201)
  - `qualifiedNameCache` — [`L229`](../../../../../../raw/code/codegraph/src/resolution/index.ts#L229)
  - `queries` — [`L202`](../../../../../../raw/code/codegraph/src/resolution/index.ts#L202) — documented in [resolution-index.ts](../../../concepts/resolution-index.ts.md)
  - `razorUsingsCache` — [`L219`](../../../../../../raw/code/codegraph/src/resolution/index.ts#L219)
  - `reExportCache` — [`L226`](../../../../../../raw/code/codegraph/src/resolution/index.ts#L226)
  - `workspacePackages` — [`L242`](../../../../../../raw/code/codegraph/src/resolution/index.ts#L242)
- uses (calls/refs, reference-scoped): [`id`](../types.ts.md#Node.id), [`Node`](../types.ts.md#Node), [`kind`](../types.ts.md#Node.kind), [`filePath`](../types.ts.md#Node.filePath), [`name`](../types.ts.md#Node.name), [`referenceName`](types.ts.md#UnresolvedRef.referenceName), [`startLine`](../types.ts.md#Node.startLine), [`ResolutionContext`](types.ts.md#ResolutionContext), [`Edge`](../types.ts.md#Edge), [`language`](types.ts.md#UnresolvedRef.language), [`language`](../types.ts.md#Node.language), [`target`](../types.ts.md#Edge.target), [`qualifiedName`](../types.ts.md#Node.qualifiedName), [`UnresolvedRef`](types.ts.md#UnresolvedRef), [`kind`](../types.ts.md#Edge.kind), [`fromNodeId`](../types.ts.md#UnresolvedReference.fromNodeId), [`synthesizeCallbackEdges`](callback-synthesizer.ts.md#synthesizeCallbackEdges), [`line`](../types.ts.md#UnresolvedReference.line), [`referenceName`](../types.ts.md#UnresolvedReference.referenceName), [`referenceKind`](../types.ts.md#UnresolvedReference.referenceKind), [`column`](../types.ts.md#UnresolvedReference.column), [`Language`](../types.ts.md#Language), [`resolveViaImport`](import-resolver.ts.md#resolveViaImport), [`filePath`](types.ts.md#UnresolvedRef.filePath), [`readFile`](types.ts.md#ResolutionContext.readFile), [`ResolvedRef`](types.ts.md#ResolvedRef), [`updateNode`](../db/queries.ts.md#QueryBuilder.updateNode), [`getNodesByName`](types.ts.md#ResolutionContext.getNodesByName), [`referenceKind`](types.ts.md#UnresolvedRef.referenceKind), [`getNodeById`](../db/queries.ts.md#QueryBuilder.getNodeById), [`FrameworkResolver`](types.ts.md#FrameworkResolver), [`getNodesInFile`](types.ts.md#ResolutionContext.getNodesInFile), [`matchReference`](name-matcher.ts.md#matchReference), [`getOutgoingEdges`](../db/queries.ts.md#QueryBuilder.getOutgoingEdges), [`getAllFiles`](types.ts.md#ResolutionContext.getAllFiles), [`fromNodeId`](types.ts.md#UnresolvedRef.fromNodeId), [`getUnresolvedReferencesBatch`](../db/queries.ts.md#QueryBuilder.getUnresolvedReferencesBatch), [`QueryBuilder`](../db/queries.ts.md#QueryBuilder), [`matchFunctionRef`](name-matcher.ts.md#matchFunctionRef), [`loadProjectAliases`](path-aliases.ts.md#loadProjectAliases)  (+91 more)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-index.ts), [`indexAll`](../index.ts.md#CodeGraph.indexAll), [`sync`](../index.ts.md#CodeGraph.sync), [`resolver`](../index.ts.md#CodeGraph.resolver), [`resolveReferences`](../index.ts.md#CodeGraph.resolveReferences), [`createResolver`](index.ts.md#createResolver), [`resolveReferencesBatched`](../index.ts.md#CodeGraph.resolveReferencesBatched), [`getDetectedFrameworks`](../index.ts.md#CodeGraph.getDetectedFrameworks), [`reinitializeResolver`](../index.ts.md#CodeGraph.reinitializeResolver)

## Functions
- `createResolver(projectRoot: string, queries: QueryBuilder)` — [`L1635`](../../../../../../raw/code/codegraph/src/resolution/index.ts#L1635) — Create a reference resolver instance
- `resolveCacheLimit()` — [`L56`](../../../../../../raw/code/codegraph/src/resolution/index.ts#L56)

## Module values
- `CHAIN_LANGUAGES` — [`L41`](../../../../../../raw/code/codegraph/src/resolution/index.ts#L41) — Languages whose chained static-factory/fluent calls defer to the conformance
- `CHAIN_SHAPE` — [`L45`](../../../../../../raw/code/codegraph/src/resolution/index.ts#L45) — The extractor's chained-receiver encoding: `<inner>().<method>`.
- `CPP_BUILT_INS` — [`L184`](../../../../../../raw/code/codegraph/src/resolution/index.ts#L184)
- `C_BUILT_INS` — [`L152`](../../../../../../raw/code/codegraph/src/resolution/index.ts#L152)
- `DEFAULT_CACHE_LIMIT` — [`L55`](../../../../../../raw/code/codegraph/src/resolution/index.ts#L55) — Cache size limits. Each per-resolver cache is bounded so memory
- `GO_BUILT_INS` — [`L116`](../../../../../../raw/code/codegraph/src/resolution/index.ts#L116)
- `GO_STDLIB_PACKAGES` — [`L102`](../../../../../../raw/code/codegraph/src/resolution/index.ts#L102)
- `JS_BUILT_INS` — [`L68`](../../../../../../raw/code/codegraph/src/resolution/index.ts#L68)
- `PASCAL_BUILT_INS` — [`L132`](../../../../../../raw/code/codegraph/src/resolution/index.ts#L132)
- `PASCAL_UNIT_PREFIXES` — [`L126`](../../../../../../raw/code/codegraph/src/resolution/index.ts#L126)
- `PYTHON_BUILT_INS` — [`L81`](../../../../../../raw/code/codegraph/src/resolution/index.ts#L81)
- `PYTHON_BUILT_IN_METHODS` — [`L92`](../../../../../../raw/code/codegraph/src/resolution/index.ts#L92)
- `PYTHON_BUILT_IN_TYPES` — [`L87`](../../../../../../raw/code/codegraph/src/resolution/index.ts#L87)
- `REACT_HOOKS` — [`L76`](../../../../../../raw/code/codegraph/src/resolution/index.ts#L76)
- `SCOPED_CHAIN_LANGUAGES` — [`L42`](../../../../../../raw/code/codegraph/src/resolution/index.ts#L42)
- `SUPERTYPE_BEARING_KINDS` — [`L32`](../../../../../../raw/code/codegraph/src/resolution/index.ts#L32) — Node kinds that can declare supertypes (extends/implements).

