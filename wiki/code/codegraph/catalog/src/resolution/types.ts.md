---
title: 'Module: src/resolution/types.ts'
type: catalog
provenance: extracted
module: src/resolution/types.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/resolution/`types.ts`/
symbols:
  UnresolvedRef.referenceName: UnresolvedRef#referenceName.
  ResolutionContext: ResolutionContext#
  UnresolvedRef.language: UnresolvedRef#language.
  UnresolvedRef: UnresolvedRef#
  UnresolvedRef.filePath: UnresolvedRef#filePath.
  ResolutionContext.readFile: ResolutionContext#readFile().
  ResolvedRef: ResolvedRef#
  ResolutionContext.getNodesByName: ResolutionContext#getNodesByName().
  UnresolvedRef.referenceKind: UnresolvedRef#referenceKind.
  FrameworkResolver: FrameworkResolver#
  ResolutionContext.getNodesInFile: ResolutionContext#getNodesInFile().
  ResolutionContext.getAllFiles: ResolutionContext#getAllFiles().
  FrameworkExtractionResult.nodes: FrameworkExtractionResult#nodes.
  UnresolvedRef.fromNodeId: UnresolvedRef#fromNodeId.
  FrameworkExtractionResult.references: FrameworkExtractionResult#references.
  ResolutionContext.fileExists: ResolutionContext#fileExists().
  UnresolvedRef.line: UnresolvedRef#line.
  ImportMapping.localName: ImportMapping#localName.
  FrameworkResolver.resolve: FrameworkResolver#resolve().
  FrameworkResolver.name: FrameworkResolver#name.
  ImportMapping.source: ImportMapping#source.
  FrameworkResolver.detect: FrameworkResolver#detect().
  FrameworkResolver.languages: FrameworkResolver#languages.
  UnresolvedRef.column: UnresolvedRef#column.
  FrameworkResolver.extract: FrameworkResolver#extract().
  ResolutionContext.getNodesByKind: ResolutionContext#getNodesByKind().
  ImportMapping: ImportMapping#
  ImportMapping.isNamespace: ImportMapping#isNamespace.
  ImportMapping.isDefault: ImportMapping#isDefault.
  ResolvedRef.original: ResolvedRef#original.
  ImportMapping.exportedName: ImportMapping#exportedName.
  ResolutionContext.getNodesByQualifiedName: ResolutionContext#getNodesByQualifiedName().
  ResolutionContext.getImportMappings: ResolutionContext#getImportMappings().
  FrameworkResolver.claimsReference: FrameworkResolver#claimsReference().
  ResolutionResult.resolved: ResolutionResult#resolved.
  FrameworkExtractionResult: FrameworkExtractionResult#
  ResolutionResult: ResolutionResult#
  ResolvedRef.confidence: ResolvedRef#confidence.
  ResolutionContext.getFileLines: ResolutionContext#getFileLines().
  ResolutionContext.getMethodMatches: ResolutionContext#getMethodMatches().
  ResolutionContext.getProjectAliases: ResolutionContext#getProjectAliases().
  ResolutionContext.getGoModule: ResolutionContext#getGoModule().
  ResolutionContext.getWorkspacePackages: ResolutionContext#getWorkspacePackages().
  FrameworkResolver.postExtract: FrameworkResolver#postExtract().
  ResolvedRef.targetNodeId: ResolvedRef#targetNodeId.
  ResolvedRef.resolvedBy: ResolvedRef#resolvedBy.
  ResolutionContext.getProjectRoot: ResolutionContext#getProjectRoot().
  ResolutionContext.getReExports: ResolutionContext#getReExports().
  ResolutionResult.unresolved: ResolutionResult#unresolved.
  ReExport: ReExport#
  ResolutionContext.getNodesByLowerName: ResolutionContext#getNodesByLowerName().
  ResolutionContext.getSupertypes: ResolutionContext#getSupertypes().
  ResolutionResult.stats: ResolutionResult#stats.
  ResolutionContext.listDirectories: ResolutionContext#listDirectories().
  ResolutionContext.getNodeById: ResolutionContext#getNodeById().
  ResolutionResult.stats.typeLiteral0.total: ResolutionResult#stats.typeLiteral0:total.
  ResolutionResult.stats.typeLiteral0.resolved: ResolutionResult#stats.typeLiteral0:resolved.
  ResolutionResult.stats.typeLiteral0.unresolved: ResolutionResult#stats.typeLiteral0:unresolved.
  ResolutionResult.stats.typeLiteral0.byMethod: ResolutionResult#stats.typeLiteral0:byMethod.
  ResolutionContext.getCppIncludeDirs: ResolutionContext#getCppIncludeDirs().
  UnresolvedRef.candidates: UnresolvedRef#candidates.
  ImportMapping.resolvedPath: ImportMapping#resolvedPath.
---
# Module: [`src/resolution/types.ts`](../../../../../../raw/code/codegraph/src/resolution/types.ts)

## Classes
### `FrameworkExtractionResult`
- def: [`src/resolution/types.ts:174`](../../../../../../raw/code/codegraph/src/resolution/types.ts#L174)
- doc: Result of framework-specific file extraction.
- signature: `interface FrameworkExtractionResult`
- members:
  - `nodes` — [`L176`](../../../../../../raw/code/codegraph/src/resolution/types.ts#L176) — Framework-specific nodes (e.g. routes)
  - `references` — [`L178`](../../../../../../raw/code/codegraph/src/resolution/types.ts#L178) — Framework-specific unresolved references (e.g. route -> handler)
- uses (calls/refs, reference-scoped): [`Node`](../types.ts.md#Node), [`UnresolvedRef`](types.ts.md#UnresolvedRef)
- used by: [`nestjsResolver`](frameworks/nestjs.ts.md#nestjsResolver), [`springResolver`](frameworks/java.ts.md#springResolver), [`railsResolver`](frameworks/ruby.ts.md#railsResolver), [`aspnetResolver`](frameworks/csharp.ts.md#aspnetResolver), [`rustResolver`](frameworks/rust.ts.md#rustResolver), [`expressResolver`](frameworks/express.ts.md#expressResolver), [`djangoResolver`](frameworks/python.ts.md#djangoResolver), [`goResolver`](frameworks/go.ts.md#goResolver), [`react-native.ts`](frameworks/react-native.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-resolution-frameworks-react-native.ts), [`vaporResolver`](frameworks/swift.ts.md#vaporResolver), [`extractFromSource`](../extraction/tree-sitter.ts.md#extractFromSource), [`reactResolver`](frameworks/react.ts.md#reactResolver), [`svelteResolver`](frameworks/svelte.ts.md#svelteResolver), [`laravelResolver`](frameworks/laravel.ts.md#laravelResolver), [`vueResolver`](frameworks/vue.ts.md#vueResolver), [`swiftUIResolver`](frameworks/swift.ts.md#swiftUIResolver), [`goframe.ts`](frameworks/goframe.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-resolution-frameworks-goframe.ts), [`uikitResolver`](frameworks/swift.ts.md#uikitResolver), [`astroResolver`](frameworks/astro.ts.md#astroResolver), [`extractDecoratorRoutes`](frameworks/python.ts.md#extractDecoratorRoutes), [`fastapiResolver`](frameworks/python.ts.md#fastapiResolver), [`extractFlaskRestful`](frameworks/python.ts.md#extractFlaskRestful), [`flaskResolver`](frameworks/python.ts.md#flaskResolver), [`fabric.ts`](frameworks/fabric.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-resolution-frameworks-fabric.ts), [`expo-modules.ts`](frameworks/expo-modules.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-resolution-frameworks-expo-modules.ts), [`extract`](types.ts.md#FrameworkResolver.extract), [`python.ts`](frameworks/python.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-resolution-frameworks-python.ts)

### `FrameworkResolver`
- def: [`src/resolution/types.ts:184`](../../../../../../raw/code/codegraph/src/resolution/types.ts#L184) — documented in [resolution-index.ts](../../../concepts/resolution-index.ts.md)
- doc: Framework-specific resolver
- signature: `interface FrameworkResolver`
- members:
  - `claimsReference(method)` — [`L200`](../../../../../../raw/code/codegraph/src/resolution/types.ts#L200) — Opt a reference NAME through the resolver's name-exists pre-filter, even when
  - `detect(method)` — [`L190`](../../../../../../raw/code/codegraph/src/resolution/types.ts#L190) — Detect if project uses this framework (project-level, called once at startup)
  - `extract(method)` — [`L209`](../../../../../../raw/code/codegraph/src/resolution/types.ts#L209) — Extract framework-specific nodes and references from a file.
  - `postExtract(method)` — [`L223`](../../../../../../raw/code/codegraph/src/resolution/types.ts#L223) — Cross-file finalization pass, called once after all per-file extraction
  - `resolve(method)` — [`L192`](../../../../../../raw/code/codegraph/src/resolution/types.ts#L192) — Resolve a reference using framework-specific patterns
  - `languages` — [`L188`](../../../../../../raw/code/codegraph/src/resolution/types.ts#L188) — Languages this framework applies to. If omitted, applies to all languages.
  - `name` — [`L186`](../../../../../../raw/code/codegraph/src/resolution/types.ts#L186) — Framework name
- uses (calls/refs, reference-scoped): [`Node`](../types.ts.md#Node), [`ResolutionContext`](types.ts.md#ResolutionContext), [`UnresolvedRef`](types.ts.md#UnresolvedRef), [`Language`](../types.ts.md#Language), [`ResolvedRef`](types.ts.md#ResolvedRef), [`FrameworkExtractionResult`](types.ts.md#FrameworkExtractionResult)
- used by: [`nestjsResolver`](frameworks/nestjs.ts.md#nestjsResolver), [`index.ts`](frameworks/index.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-resolution-frameworks-index.ts), [`index.ts`](index.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-resolution-index.ts), [`springResolver`](frameworks/java.ts.md#springResolver), [`railsResolver`](frameworks/ruby.ts.md#railsResolver), [`aspnetResolver`](frameworks/csharp.ts.md#aspnetResolver), [`rustResolver`](frameworks/rust.ts.md#rustResolver), [`expressResolver`](frameworks/express.ts.md#expressResolver), [`djangoResolver`](frameworks/python.ts.md#djangoResolver), [`goResolver`](frameworks/go.ts.md#goResolver), [`play.ts`](frameworks/play.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-resolution-frameworks-play.ts), [`react-native.ts`](frameworks/react-native.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-resolution-frameworks-react-native.ts), [`vaporResolver`](frameworks/swift.ts.md#vaporResolver), [`extractFromSource`](../extraction/tree-sitter.ts.md#extractFromSource), [`reactResolver`](frameworks/react.ts.md#reactResolver), [`svelteResolver`](frameworks/svelte.ts.md#svelteResolver), [`laravelResolver`](frameworks/laravel.ts.md#laravelResolver), [`vueResolver`](frameworks/vue.ts.md#vueResolver), [`swiftUIResolver`](frameworks/swift.ts.md#swiftUIResolver), [`goframe.ts`](frameworks/goframe.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-resolution-frameworks-goframe.ts), [`uikitResolver`](frameworks/swift.ts.md#uikitResolver), [`astroResolver`](frameworks/astro.ts.md#astroResolver), [`resolveOne`](index.ts.md#ReferenceResolver.resolveOne), [`FRAMEWORK_RESOLVERS`](frameworks/index.ts.md#FRAMEWORK_RESOLVERS), [`drupal.ts`](frameworks/drupal.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-resolution-frameworks-drupal.ts), [`fastapiResolver`](frameworks/python.ts.md#fastapiResolver), [`flaskResolver`](frameworks/python.ts.md#flaskResolver), [`terraformResolver`](frameworks/terraform.ts.md#terraformResolver), [`swift-objc.ts`](frameworks/swift-objc.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-resolution-frameworks-swift-objc.ts), [`cics.ts`](frameworks/cics.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-resolution-frameworks-cics.ts), [`fabric.ts`](frameworks/fabric.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-resolution-frameworks-fabric.ts), [`expo-modules.ts`](frameworks/expo-modules.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-resolution-frameworks-expo-modules.ts), [`rust.ts`](frameworks/rust.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-resolution-frameworks-rust.ts), [`csharp.ts`](frameworks/csharp.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-resolution-frameworks-csharp.ts), [`express.ts`](frameworks/express.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-resolution-frameworks-express.ts), [`go.ts`](frameworks/go.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-resolution-frameworks-go.ts), [`java.ts`](frameworks/java.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-resolution-frameworks-java.ts), [`laravel.ts`](frameworks/laravel.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-resolution-frameworks-laravel.ts), [`nestjs.ts`](frameworks/nestjs.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-resolution-frameworks-nestjs.ts), [`python.ts`](frameworks/python.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-resolution-frameworks-python.ts)  (+16 more)

### `ImportMapping`
- def: [`src/resolution/types.ts:229`](../../../../../../raw/code/codegraph/src/resolution/types.ts#L229)
- doc: Import mapping from a file
- signature: `interface ImportMapping`
- members:
  - `exportedName` — [`L233`](../../../../../../raw/code/codegraph/src/resolution/types.ts#L233) — Original exported name (may differ due to aliasing)
  - `isDefault` — [`L237`](../../../../../../raw/code/codegraph/src/resolution/types.ts#L237) — Whether it's a default import
  - `isNamespace` — [`L239`](../../../../../../raw/code/codegraph/src/resolution/types.ts#L239) — Whether it's a namespace import (import * as X)
  - `localName` — [`L231`](../../../../../../raw/code/codegraph/src/resolution/types.ts#L231) — Local name used in the file
  - `resolvedPath` — [`L241`](../../../../../../raw/code/codegraph/src/resolution/types.ts#L241) — Resolved file path (if local)
  - `source` — [`L235`](../../../../../../raw/code/codegraph/src/resolution/types.ts#L235) — Source module/path
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-resolution-index.ts), [`resolveViaImport`](import-resolver.ts.md#resolveViaImport), [`matchMethodCall`](name-matcher.ts.md#matchMethodCall), [`resolveModuleImportToFile`](import-resolver.ts.md#resolveModuleImportToFile), [`resolvePythonModuleMember`](import-resolver.ts.md#resolvePythonModuleMember), [`resolveGoCrossPackageReference`](import-resolver.ts.md#resolveGoCrossPackageReference), [`import-resolver.ts`](import-resolver.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-resolution-import-resolver.ts), [`resolveJavaImportedReference`](import-resolver.ts.md#resolveJavaImportedReference), [`importedFqnOf`](name-matcher.ts.md#importedFqnOf), [`extractImportMappings`](import-resolver.ts.md#extractImportMappings), [`matchesAnyImport`](index.ts.md#ReferenceResolver.matchesAnyImport), [`extractJSImports`](import-resolver.ts.md#extractJSImports), [`extractCppImports`](import-resolver.ts.md#extractCppImports), [`extractGoImports`](import-resolver.ts.md#extractGoImports), [`extractJavaImports`](import-resolver.ts.md#extractJavaImports), [`extractPHPImports`](import-resolver.ts.md#extractPHPImports), [`extractPythonImports`](import-resolver.ts.md#extractPythonImports), [`getImportMappings`](types.ts.md#ResolutionContext.getImportMappings), [`importMappingCache`](index.ts.md#ReferenceResolver.importMappingCache), [`importMappingCache`](import-resolver.ts.md#importMappingCache)

### `ReExport`
- def: [`src/resolution/types.ts:249`](../../../../../../raw/code/codegraph/src/resolution/types.ts#L249)
- doc: Re-export from a file: `export { x } from './other'` or
- signature: `type ReExport`
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-resolution-index.ts), [`import-resolver.ts`](import-resolver.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-resolution-import-resolver.ts), [`reExportCache`](index.ts.md#ReferenceResolver.reExportCache), [`extractReExports`](import-resolver.ts.md#extractReExports), [`getReExports`](types.ts.md#ResolutionContext.getReExports)

### `ResolutionContext`
- def: [`src/resolution/types.ts:65`](../../../../../../raw/code/codegraph/src/resolution/types.ts#L65) — documented in [extraction-index.ts](../../../concepts/extraction-index.ts.md)
- doc: Context for resolution - provides access to the graph
- signature: `interface ResolutionContext`
- members:
  - `fileExists(method)` — [`L75`](../../../../../../raw/code/codegraph/src/resolution/types.ts#L75) — Check if a file exists
  - `getAllFiles(method)` — [`L101`](../../../../../../raw/code/codegraph/src/resolution/types.ts#L101) — Get all files — documented in [resolution-callback-synthesizer.ts](../../../concepts/resolution-callback-synthesizer.ts.md)
  - `getCppIncludeDirs(method)` — [`L168`](../../../../../../raw/code/codegraph/src/resolution/types.ts#L168) — C/C++ include search directories (relative to project root),
  - `getFileLines(method)` — [`L86`](../../../../../../raw/code/codegraph/src/resolution/types.ts#L86) — `readFile(filePath)` split into lines, LRU-cached per file. Receiver-type
  - `getGoModule(method)` — [`L138`](../../../../../../raw/code/codegraph/src/resolution/types.ts#L138) — Go module info from `go.mod` at the project root. Returns `null`
  - `getImportMappings(method)` — [`L122`](../../../../../../raw/code/codegraph/src/resolution/types.ts#L122) — Get cached import mappings for a file
  - `getMethodMatches(method)` — [`L97`](../../../../../../raw/code/codegraph/src/resolution/types.ts#L97) — The method-definition nodes matching `typeName::methodName` in `language` —
  - `getNodeById(method)` — [`L120`](../../../../../../raw/code/codegraph/src/resolution/types.ts#L120) — Look up a node by its id. Lets matchers derive the FROM-symbol's
  - `getNodesByKind(method)` — [`L73`](../../../../../../raw/code/codegraph/src/resolution/types.ts#L73) — Get all nodes of a kind
  - `getNodesByLowerName(method)` — [`L103`](../../../../../../raw/code/codegraph/src/resolution/types.ts#L103) — Get nodes by lowercase name (O(1) lookup for fuzzy matching)
  - `getNodesByName(method)` — [`L69`](../../../../../../raw/code/codegraph/src/resolution/types.ts#L69) — Get all nodes by name — documented in [index.ts](../../../concepts/index.ts.md)
  - `getNodesByQualifiedName(method)` — [`L71`](../../../../../../raw/code/codegraph/src/resolution/types.ts#L71) — Get all nodes by qualified name
  - `getNodesInFile(method)` — [`L67`](../../../../../../raw/code/codegraph/src/resolution/types.ts#L67) — Get all nodes in a file — documented in [resolution-callback-synthesizer.ts](../../../concepts/resolution-callback-synthesizer.ts.md)
  - `getProjectAliases(method)` — [`L130`](../../../../../../raw/code/codegraph/src/resolution/types.ts#L130) — Project import-path aliases (tsconfig/jsconfig `paths`). Returns
  - `getProjectRoot(method)` — [`L99`](../../../../../../raw/code/codegraph/src/resolution/types.ts#L99) — Get project root
  - `getReExports(method)` — [`L152`](../../../../../../raw/code/codegraph/src/resolution/types.ts#L152) — Re-exports declared by a file (`export { x } from './other'`,
  - `getSupertypes(method)` — [`L113`](../../../../../../raw/code/codegraph/src/resolution/types.ts#L113) — Direct supertypes of the type named `typeName` (same language): the classes
  - `getWorkspacePackages(method)` — [`L145`](../../../../../../raw/code/codegraph/src/resolution/types.ts#L145) — Monorepo workspace member packages, keyed by declared package name.
  - `listDirectories(method)` — [`L161`](../../../../../../raw/code/codegraph/src/resolution/types.ts#L161) — List immediate subdirectories of `relativePath` (relative to the
  - `readFile(method)` — [`L77`](../../../../../../raw/code/codegraph/src/resolution/types.ts#L77) — Read file content — documented in [extraction-index.ts](../../../concepts/extraction-index.ts.md)
- uses (calls/refs, reference-scoped): [`Node`](../types.ts.md#Node), [`kind`](../types.ts.md#Node.kind), [`Language`](../types.ts.md#Language), [`ImportMapping`](types.ts.md#ImportMapping), [`path-aliases.ts`](path-aliases.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-resolution-path-aliases.ts), [`workspace-packages.ts`](workspace-packages.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-resolution-workspace-packages.ts), [`AliasMap`](path-aliases.ts.md#AliasMap), [`ReExport`](types.ts.md#ReExport), [`WorkspacePackages`](workspace-packages.ts.md#WorkspacePackages), [`GoModule`](go-module.ts.md#GoModule), [`go-module.ts`](go-module.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-resolution-go-module.ts)
- used by: [`createContext`](index.ts.md#ReferenceResolver.createContext), [`nestjsResolver`](frameworks/nestjs.ts.md#nestjsResolver), [`index.ts`](frameworks/index.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-resolution-frameworks-index.ts), [`index.ts`](index.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-resolution-index.ts), [`springResolver`](frameworks/java.ts.md#springResolver), [`cFnPointerDispatchEdges`](c-fnptr-synthesizer.ts.md#cFnPointerDispatchEdges), [`railsResolver`](frameworks/ruby.ts.md#railsResolver), [`aspnetResolver`](frameworks/csharp.ts.md#aspnetResolver), [`rustResolver`](frameworks/rust.ts.md#rustResolver), [`expressResolver`](frameworks/express.ts.md#expressResolver), [`synthesizeCallbackEdges`](callback-synthesizer.ts.md#synthesizeCallbackEdges), [`djangoResolver`](frameworks/python.ts.md#djangoResolver), [`goResolver`](frameworks/go.ts.md#goResolver), [`play.ts`](frameworks/play.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-resolution-frameworks-play.ts), [`react-native.ts`](frameworks/react-native.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-resolution-frameworks-react-native.ts), [`index.ts`](../extraction/index.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-extraction-index.ts), [`vaporResolver`](frameworks/swift.ts.md#vaporResolver), [`reactResolver`](frameworks/react.ts.md#reactResolver), [`svelteResolver`](frameworks/svelte.ts.md#svelteResolver), [`laravelResolver`](frameworks/laravel.ts.md#laravelResolver), [`vueResolver`](frameworks/vue.ts.md#vueResolver), [`resolveViaImport`](import-resolver.ts.md#resolveViaImport), [`swiftUIResolver`](frameworks/swift.ts.md#swiftUIResolver), [`goframe.ts`](frameworks/goframe.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-resolution-frameworks-goframe.ts), [`uikitResolver`](frameworks/swift.ts.md#uikitResolver), [`astroResolver`](frameworks/astro.ts.md#astroResolver), [`drupal.ts`](frameworks/drupal.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-resolution-frameworks-drupal.ts), [`resolveDeferredThisMemberRefs`](index.ts.md#ReferenceResolver.resolveDeferredThisMemberRefs), [`erlangBehaviourDispatchEdges`](callback-synthesizer.ts.md#erlangBehaviourDispatchEdges), [`laravelEventEdges`](callback-synthesizer.ts.md#laravelEventEdges), [`fieldChannelEdges`](callback-synthesizer.ts.md#fieldChannelEdges), [`ginMiddlewareChainEdges`](callback-synthesizer.ts.md#ginMiddlewareChainEdges), [`mediatrDispatchEdges`](callback-synthesizer.ts.md#mediatrDispatchEdges), [`sidekiqDispatchEdges`](callback-synthesizer.ts.md#sidekiqDispatchEdges), [`springEventEdges`](callback-synthesizer.ts.md#springEventEdges), [`reduxThunkEdges`](callback-synthesizer.ts.md#reduxThunkEdges), [`vueTemplateEdges`](callback-synthesizer.ts.md#vueTemplateEdges), [`celeryDispatchEdges`](callback-synthesizer.ts.md#celeryDispatchEdges), [`matchMethodCall`](name-matcher.ts.md#matchMethodCall), [`fastapiResolver`](frameworks/python.ts.md#fastapiResolver)  (+135 more)

### `ResolutionResult`
- def: [`src/resolution/types.ts:48`](../../../../../../raw/code/codegraph/src/resolution/types.ts#L48)
- doc: Result of resolution attempt
- signature: `interface ResolutionResult`
- members:
  - `byMethod` — [`L58`](../../../../../../raw/code/codegraph/src/resolution/types.ts#L58)
  - `resolved` — [`L50`](../../../../../../raw/code/codegraph/src/resolution/types.ts#L50) — Successfully resolved references
  - `resolved` — [`L56`](../../../../../../raw/code/codegraph/src/resolution/types.ts#L56)
  - `stats` — [`L54`](../../../../../../raw/code/codegraph/src/resolution/types.ts#L54) — Statistics
  - `total` — [`L55`](../../../../../../raw/code/codegraph/src/resolution/types.ts#L55)
  - `unresolved` — [`L52`](../../../../../../raw/code/codegraph/src/resolution/types.ts#L52) — References that couldn't be resolved
  - `unresolved` — [`L57`](../../../../../../raw/code/codegraph/src/resolution/types.ts#L57)
- uses (calls/refs, reference-scoped): [`UnresolvedRef`](types.ts.md#UnresolvedRef), [`ResolvedRef`](types.ts.md#ResolvedRef)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-index.ts), [`index.ts`](index.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-resolution-index.ts), [`resolveBatchYielding`](index.ts.md#ReferenceResolver.resolveBatchYielding), [`resolveAll`](index.ts.md#ReferenceResolver.resolveAll), [`resolveAndPersistBatched`](index.ts.md#ReferenceResolver.resolveAndPersistBatched), [`resolveAndPersist`](index.ts.md#ReferenceResolver.resolveAndPersist), [`resolveReferences`](../index.ts.md#CodeGraph.resolveReferences), [`resolveReferencesBatched`](../index.ts.md#CodeGraph.resolveReferencesBatched)

### `ResolvedRef`
- def: [`src/resolution/types.ts:34`](../../../../../../raw/code/codegraph/src/resolution/types.ts#L34) — documented in [index.ts](../../../concepts/index.ts.md)
- doc: A resolved reference
- signature: `interface ResolvedRef`
- members:
  - `confidence` — [`L40`](../../../../../../raw/code/codegraph/src/resolution/types.ts#L40) — Confidence score (0-1)
  - `original` — [`L36`](../../../../../../raw/code/codegraph/src/resolution/types.ts#L36) — Original unresolved reference
  - `resolvedBy` — [`L42`](../../../../../../raw/code/codegraph/src/resolution/types.ts#L42) — How it was resolved
  - `targetNodeId` — [`L38`](../../../../../../raw/code/codegraph/src/resolution/types.ts#L38) — ID of the target node
- uses (calls/refs, reference-scoped): [`UnresolvedRef`](types.ts.md#UnresolvedRef)
- used by: [`nestjsResolver`](frameworks/nestjs.ts.md#nestjsResolver), [`index.ts`](index.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-resolution-index.ts), [`springResolver`](frameworks/java.ts.md#springResolver), [`railsResolver`](frameworks/ruby.ts.md#railsResolver), [`aspnetResolver`](frameworks/csharp.ts.md#aspnetResolver), [`rustResolver`](frameworks/rust.ts.md#rustResolver), [`expressResolver`](frameworks/express.ts.md#expressResolver), [`goResolver`](frameworks/go.ts.md#goResolver), [`play.ts`](frameworks/play.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-resolution-frameworks-play.ts), [`vaporResolver`](frameworks/swift.ts.md#vaporResolver), [`reactResolver`](frameworks/react.ts.md#reactResolver), [`svelteResolver`](frameworks/svelte.ts.md#svelteResolver), [`laravelResolver`](frameworks/laravel.ts.md#laravelResolver), [`vueResolver`](frameworks/vue.ts.md#vueResolver), [`resolveViaImport`](import-resolver.ts.md#resolveViaImport), [`swiftUIResolver`](frameworks/swift.ts.md#swiftUIResolver), [`goframe.ts`](frameworks/goframe.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-resolution-frameworks-goframe.ts), [`uikitResolver`](frameworks/swift.ts.md#uikitResolver), [`astroResolver`](frameworks/astro.ts.md#astroResolver), [`resolveOne`](index.ts.md#ReferenceResolver.resolveOne), [`drupal.ts`](frameworks/drupal.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-resolution-frameworks-drupal.ts), [`resolveDeferredThisMemberRefs`](index.ts.md#ReferenceResolver.resolveDeferredThisMemberRefs), [`resolveBatchYielding`](index.ts.md#ReferenceResolver.resolveBatchYielding), [`matchMethodCall`](name-matcher.ts.md#matchMethodCall), [`resolveAll`](index.ts.md#ReferenceResolver.resolveAll), [`resolveAndPersistBatched`](index.ts.md#ReferenceResolver.resolveAndPersistBatched), [`matchReference`](name-matcher.ts.md#matchReference), [`terraformResolver`](frameworks/terraform.ts.md#terraformResolver), [`resolveMethodOnType`](name-matcher.ts.md#resolveMethodOnType), [`swift-objc.ts`](frameworks/swift-objc.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-resolution-frameworks-swift-objc.ts), [`cics.ts`](frameworks/cics.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-resolution-frameworks-cics.ts), [`resolveModuleImportToFile`](import-resolver.ts.md#resolveModuleImportToFile), [`resolvePythonModuleMember`](import-resolver.ts.md#resolvePythonModuleMember), [`matchFunctionRef`](name-matcher.ts.md#matchFunctionRef), [`resolveThisMemberFnRef`](index.ts.md#ReferenceResolver.resolveThisMemberFnRef), [`matchByExactName`](name-matcher.ts.md#matchByExactName), [`createEdges`](index.ts.md#ReferenceResolver.createEdges), [`resolveGoCrossPackageReference`](import-resolver.ts.md#resolveGoCrossPackageReference), [`resolveScopedModuleRef`](frameworks/terraform.ts.md#resolveScopedModuleRef), [`resolve`](types.ts.md#FrameworkResolver.resolve)  (+36 more)

### `UnresolvedRef`
- def: [`src/resolution/types.ts:12`](../../../../../../raw/code/codegraph/src/resolution/types.ts#L12) — documented in [extraction-index.ts](../../../concepts/extraction-index.ts.md)
- doc: An unresolved reference from extraction
- signature: `interface UnresolvedRef`
- members:
  - `candidates` — [`L28`](../../../../../../raw/code/codegraph/src/resolution/types.ts#L28) — Possible qualified names it might resolve to
  - `column` — [`L22`](../../../../../../raw/code/codegraph/src/resolution/types.ts#L22) — Column where reference occurs
  - `filePath` — [`L24`](../../../../../../raw/code/codegraph/src/resolution/types.ts#L24) — File path where reference occurs — documented in [index.ts](../../../concepts/index.ts.md)
  - `fromNodeId` — [`L14`](../../../../../../raw/code/codegraph/src/resolution/types.ts#L14) — ID of the source node containing the reference — documented in [resolution-index.ts](../../../concepts/resolution-index.ts.md)
  - `language` — [`L26`](../../../../../../raw/code/codegraph/src/resolution/types.ts#L26) — Language of the source file — documented in [index.ts](../../../concepts/index.ts.md)
  - `line` — [`L20`](../../../../../../raw/code/codegraph/src/resolution/types.ts#L20) — Line where reference occurs
  - `referenceKind` — [`L18`](../../../../../../raw/code/codegraph/src/resolution/types.ts#L18) — Type of reference — documented in [index.ts](../../../concepts/index.ts.md)
  - `referenceName` — [`L16`](../../../../../../raw/code/codegraph/src/resolution/types.ts#L16) — The name being referenced — documented in [index.ts](../../../concepts/index.ts.md)
- uses (calls/refs, reference-scoped): [`Language`](../types.ts.md#Language), [`ReferenceKind`](../types.ts.md#ReferenceKind)
- used by: [`nestjsResolver`](frameworks/nestjs.ts.md#nestjsResolver), [`index.ts`](index.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-resolution-index.ts), [`springResolver`](frameworks/java.ts.md#springResolver), [`railsResolver`](frameworks/ruby.ts.md#railsResolver), [`aspnetResolver`](frameworks/csharp.ts.md#aspnetResolver), [`rustResolver`](frameworks/rust.ts.md#rustResolver), [`expressResolver`](frameworks/express.ts.md#expressResolver), [`djangoResolver`](frameworks/python.ts.md#djangoResolver), [`goResolver`](frameworks/go.ts.md#goResolver), [`play.ts`](frameworks/play.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-resolution-frameworks-play.ts), [`react-native.ts`](frameworks/react-native.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-resolution-frameworks-react-native.ts), [`vaporResolver`](frameworks/swift.ts.md#vaporResolver), [`reactResolver`](frameworks/react.ts.md#reactResolver), [`svelteResolver`](frameworks/svelte.ts.md#svelteResolver), [`laravelResolver`](frameworks/laravel.ts.md#laravelResolver), [`vueResolver`](frameworks/vue.ts.md#vueResolver), [`resolveViaImport`](import-resolver.ts.md#resolveViaImport), [`swiftUIResolver`](frameworks/swift.ts.md#swiftUIResolver), [`goframe.ts`](frameworks/goframe.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-resolution-frameworks-goframe.ts), [`uikitResolver`](frameworks/swift.ts.md#uikitResolver), [`astroResolver`](frameworks/astro.ts.md#astroResolver), [`extractDecoratorRoutes`](frameworks/python.ts.md#extractDecoratorRoutes), [`resolveOne`](index.ts.md#ReferenceResolver.resolveOne), [`drupal.ts`](frameworks/drupal.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-resolution-frameworks-drupal.ts), [`resolveDeferredThisMemberRefs`](index.ts.md#ReferenceResolver.resolveDeferredThisMemberRefs), [`resolveBatchYielding`](index.ts.md#ReferenceResolver.resolveBatchYielding), [`matchMethodCall`](name-matcher.ts.md#matchMethodCall), [`fastapiResolver`](frameworks/python.ts.md#fastapiResolver), [`extractFlaskRestful`](frameworks/python.ts.md#extractFlaskRestful), [`resolveAll`](index.ts.md#ReferenceResolver.resolveAll), [`resolveAndPersistBatched`](index.ts.md#ReferenceResolver.resolveAndPersistBatched), [`flaskResolver`](frameworks/python.ts.md#flaskResolver), [`extractDrupalRoutes`](frameworks/drupal.ts.md#extractDrupalRoutes), [`matchReference`](name-matcher.ts.md#matchReference), [`terraformResolver`](frameworks/terraform.ts.md#terraformResolver), [`extractSpringValueBindings`](frameworks/java.ts.md#extractSpringValueBindings), [`resolveMethodOnType`](name-matcher.ts.md#resolveMethodOnType), [`swift-objc.ts`](frameworks/swift-objc.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-resolution-frameworks-swift-objc.ts), [`cics.ts`](frameworks/cics.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-resolution-frameworks-cics.ts), [`resolveModuleImportToFile`](import-resolver.ts.md#resolveModuleImportToFile)  (+69 more)

