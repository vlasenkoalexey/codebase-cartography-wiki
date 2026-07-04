---
title: 'Module: src/extraction/tree-sitter-types.ts'
type: catalog
provenance: extracted
module: src/extraction/tree-sitter-types.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/extraction/`tree-sitter-types.ts`/
symbols:
  ExtractorContext.source: ExtractorContext#source.
  LanguageExtractor: LanguageExtractor#
  LanguageExtractor.bodyField: LanguageExtractor#bodyField.
  ExtractorContext.createNode: ExtractorContext#createNode().
  LanguageExtractor.getVisibility: LanguageExtractor#getVisibility.
  ExtractorContext: ExtractorContext#
  LanguageExtractor.functionTypes: LanguageExtractor#functionTypes.
  LanguageExtractor.structTypes: LanguageExtractor#structTypes.
  LanguageExtractor.enumTypes: LanguageExtractor#enumTypes.
  LanguageExtractor.callTypes: LanguageExtractor#callTypes.
  LanguageExtractor.classTypes: LanguageExtractor#classTypes.
  LanguageExtractor.methodTypes: LanguageExtractor#methodTypes.
  LanguageExtractor.interfaceTypes: LanguageExtractor#interfaceTypes.
  LanguageExtractor.typeAliasTypes: LanguageExtractor#typeAliasTypes.
  LanguageExtractor.variableTypes: LanguageExtractor#variableTypes.
  LanguageExtractor.importTypes: LanguageExtractor#importTypes.
  LanguageExtractor.nameField: LanguageExtractor#nameField.
  LanguageExtractor.paramsField: LanguageExtractor#paramsField.
  LanguageExtractor.extractImport: LanguageExtractor#extractImport.
  LanguageExtractor.visitNode: LanguageExtractor#visitNode.
  ExtractorContext.nodeStack: ExtractorContext#nodeStack.
  ExtractorContext.popScope: ExtractorContext#popScope().
  LanguageExtractor.getSignature: LanguageExtractor#getSignature.
  ExtractorContext.addUnresolvedReference: ExtractorContext#addUnresolvedReference().
  LanguageExtractor.isStatic: LanguageExtractor#isStatic.
  LanguageExtractor.resolveBody: LanguageExtractor#resolveBody.
  ExtractorContext.pushScope: ExtractorContext#pushScope().
  LanguageExtractor.getReturnType: LanguageExtractor#getReturnType.
  ExtractorContext.visitNode: ExtractorContext#visitNode().
  LanguageExtractor.enumMemberTypes: LanguageExtractor#enumMemberTypes.
  LanguageExtractor.isExported: LanguageExtractor#isExported.
  LanguageExtractor.isAsync: LanguageExtractor#isAsync.
  LanguageExtractor.returnField: LanguageExtractor#returnField.
  LanguageExtractor.isConst: LanguageExtractor#isConst.
  ExtractorContext.filePath: ExtractorContext#filePath.
  LanguageExtractor.classifyClassNode: LanguageExtractor#classifyClassNode.
  LanguageExtractor.resolveTypeAliasKind: LanguageExtractor#resolveTypeAliasKind.
  ExtractorContext.nodes: ExtractorContext#nodes.
  LanguageExtractor.resolveName: LanguageExtractor#resolveName.
  LanguageExtractor.getReceiverType: LanguageExtractor#getReceiverType.
  LanguageExtractor.fieldTypes: LanguageExtractor#fieldTypes.
  LanguageExtractor.synthesizeMembers: LanguageExtractor#synthesizeMembers.
  LanguageExtractor.extractPackage: LanguageExtractor#extractPackage.
  ExtractorContext.visitFunctionBody: ExtractorContext#visitFunctionBody().
  LanguageExtractor.interfaceKind: LanguageExtractor#interfaceKind.
  LanguageExtractor.preParse: LanguageExtractor#preParse.
  LanguageExtractor.packageTypes: LanguageExtractor#packageTypes.
  LanguageExtractor.isMisparsedFunction: LanguageExtractor#isMisparsedFunction.
  LanguageExtractor.extractBareCall: LanguageExtractor#extractBareCall.
  LanguageExtractor.classifyMethodNode: LanguageExtractor#classifyMethodNode.
  LanguageExtractor.propertyTypes: LanguageExtractor#propertyTypes.
  LanguageExtractor.extractVariables: LanguageExtractor#extractVariables.
  LanguageExtractor.extractPropertyName: LanguageExtractor#extractPropertyName.
  LanguageExtractor.extractModifiers: LanguageExtractor#extractModifiers.
  LanguageExtractor.recoverMangledName: LanguageExtractor#recoverMangledName.
  LanguageExtractor.extraClassNodeTypes: LanguageExtractor#extraClassNodeTypes.
  ImportInfo.moduleName: ImportInfo#moduleName.
  VariableInfo.kind: VariableInfo#kind.
  VariableInfo.delegateToFunction: VariableInfo#delegateToFunction.
  VariableInfo.positionNode: VariableInfo#positionNode.
  LanguageExtractor.methodsAreTopLevel: LanguageExtractor#methodsAreTopLevel.
  LanguageExtractor.skipBodilessClass: LanguageExtractor#skipBodilessClass.
  ImportInfo: ImportInfo#
  ImportInfo.signature: ImportInfo#signature.
  ImportInfo.handledRefs: ImportInfo#handledRefs.
  VariableInfo: VariableInfo#
  VariableInfo.name: VariableInfo#name.
  VariableInfo.signature: VariableInfo#signature.
---
# Module: [`src/extraction/tree-sitter-types.ts`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-types.ts)

## Classes
### `ExtractorContext`
- def: [`src/extraction/tree-sitter-types.ts:50`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-types.ts#L50)
- doc: Context object passed to language hooks that need to call back into the core extractor.
- signature: `interface ExtractorContext`
- members:
  - `addUnresolvedReference(method)` — [`L58`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-types.ts#L58) — Add an unresolved reference
  - `createNode(method)` — [`L52`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-types.ts#L52) — Create a node and add it to the extraction result — documented in [extraction-tree-sitter-types.ts](../../../concepts/extraction-tree-sitter-types.ts.md)
  - `popScope(method)` — [`L62`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-types.ts#L62) — Pop the last node ID from the scope stack
  - `pushScope(method)` — [`L60`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-types.ts#L60) — Push a node ID onto the scope stack (for containment/qualified name building)
  - `visitFunctionBody(method)` — [`L56`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-types.ts#L56) — Visit a function body to extract calls
  - `visitNode(method)` — [`L54`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-types.ts#L54) — Visit a child node (dispatches through the standard visitNode logic)
  - `filePath` — [`L64`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-types.ts#L64) — Current file path
  - `nodeStack` — [`L68`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-types.ts#L68) — Stack of parent node IDs (current scope)
  - `nodes` — [`L70`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-types.ts#L70) — All nodes extracted so far
  - `source` — [`L66`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-types.ts#L66) — Current source text — documented in [extraction-tree-sitter-types.ts](../../../concepts/extraction-tree-sitter-types.ts.md)
- uses (calls/refs, reference-scoped): [`Node`](../web-tree-sitter.d.ts.md#Node), [`Node`](../types.ts.md#Node), [`NodeKind`](../types.ts.md#NodeKind), [`UnresolvedReference`](../types.ts.md#UnresolvedReference)
- used by: [`kotlin.ts`](languages/kotlin.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-extraction-languages-kotlin.ts), [`tree-sitter.ts`](tree-sitter.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-extraction-tree-sitter.ts), [`php.ts`](languages/php.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-extraction-languages-php.ts), [`objc.ts`](languages/objc.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-extraction-languages-objc.ts), [`r.ts`](languages/r.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-extraction-languages-r.ts), [`solidity.ts`](languages/solidity.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-extraction-languages-solidity.ts), [`ruby.ts`](languages/ruby.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-extraction-languages-ruby.ts), [`terraformExtractor`](languages/terraform.ts.md#terraformExtractor), [`dart.ts`](languages/dart.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-extraction-languages-dart.ts), [`vbnet.ts`](languages/vbnet.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-extraction-languages-vbnet.ts), [`scala.ts`](languages/scala.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-extraction-languages-scala.ts), [`java.ts`](languages/java.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-extraction-languages-java.ts), [`cobol.ts`](languages/cobol.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-extraction-languages-cobol.ts), [`erlang.ts`](languages/erlang.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-extraction-languages-erlang.ts), [`lua.ts`](languages/lua.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-extraction-languages-lua.ts), [`handleFunDecl`](languages/erlang.ts.md#handleFunDecl), [`synthesizeLombokMembers`](languages/java.ts.md#synthesizeLombokMembers), [`extractClassMembers`](languages/r.ts.md#extractClassMembers), [`makeExtractorContext`](tree-sitter.ts.md#TreeSitterExtractor.makeExtractorContext), [`emitModuleWiring`](languages/terraform.ts.md#emitModuleWiring), [`emitLocals`](languages/terraform.ts.md#emitLocals), [`emitModuleProvidersRefs`](languages/terraform.ts.md#emitModuleProvidersRefs), [`emitReferencesInBody`](languages/terraform.ts.md#emitReferencesInBody), [`emitProviderSelectionRef`](languages/terraform.ts.md#emitProviderSelectionRef), [`handleAppResourceTuple`](languages/erlang.ts.md#handleAppResourceTuple), [`handleBehaviour`](languages/erlang.ts.md#handleBehaviour), [`walkDataEntries`](languages/cobol.ts.md#walkDataEntries), [`walkProcedureChildren`](languages/cobol.ts.md#walkProcedureChildren), [`handleRecordDecl`](languages/erlang.ts.md#handleRecordDecl), [`addRef`](languages/cobol.ts.md#addRef), [`collectRefs`](languages/cobol.ts.md#collectRefs), [`handleExec`](languages/cobol.ts.md#handleExec), [`emitMethodArg`](languages/r.ts.md#emitMethodArg), [`handlePpDefine`](languages/erlang.ts.md#handlePpDefine), [`handleCopy`](languages/cobol.ts.md#handleCopy), [`visitNode`](tree-sitter-types.ts.md#LanguageExtractor.visitNode), [`emitWriteRefs`](languages/cobol.ts.md#emitWriteRefs), [`derefSameFileValue`](languages/cobol.ts.md#derefSameFileValue), [`handleTypeAlias`](languages/erlang.ts.md#handleTypeAlias), [`currentScope`](languages/cobol.ts.md#currentScope)  (+1 more)

### `ImportInfo`
- def: [`src/extraction/tree-sitter-types.ts:19`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-types.ts#L19)
- doc: Information returned by a language's extractImport hook.
- signature: `interface ImportInfo`
- members:
  - `handledRefs` — [`L25`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-types.ts#L25) — If true, the hook already created unresolved references itself
  - `moduleName` — [`L21`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-types.ts#L21) — The module/package name being imported
  - `signature` — [`L23`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-types.ts#L23) — Full import statement text for display
- used by: [`extractImport`](tree-sitter.ts.md#TreeSitterExtractor.extractImport), [`extractImport`](tree-sitter-types.ts.md#LanguageExtractor.extractImport)

### `LanguageExtractor`
- def: [`src/extraction/tree-sitter-types.ts:80`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-types.ts#L80) — documented in [extraction-tree-sitter-types.ts](../../../concepts/extraction-tree-sitter-types.ts.md)
- doc: Language-specific extraction configuration.
- signature: `interface LanguageExtractor`
- members:
  - `bodyField` — [`L127`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-types.ts#L127) — Field name for body — documented in [extraction-tree-sitter-types.ts](../../../concepts/extraction-tree-sitter-types.ts.md)
  - `callTypes` — [`L114`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-types.ts#L114) — Node types that represent function calls
  - `classTypes` — [`L98`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-types.ts#L98) — Node types that represent classes
  - `classifyClassNode` — [`L215`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-types.ts#L215) — Classify a class_declaration node when the grammar reuses one node type
  - `classifyMethodNode` — [`L224`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-types.ts#L224) — Classify a methodTypes node when the grammar reuses one node type for
  - `enumMemberTypes` — [`L108`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-types.ts#L108) — Node types that represent enum members/cases (e.g. Swift: 'enum_entry', Rust: 'enum_variant')
  - `enumTypes` — [`L106`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-types.ts#L106) — Node types that represent enums
  - `extraClassNodeTypes` — [`L175`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-types.ts#L175) — Additional node types to treat as class declarations (e.g. Dart: 'mixin_declaration')
  - `extractBareCall` — [`L284`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-types.ts#L284) — Detect bare method calls that don't use call expression syntax.
  - `extractImport` — [`L236`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-types.ts#L236) — Extract import information from an import node.
  - `extractModifiers` — [`L170`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-types.ts#L170) — Extract extra symbol-level modifier keywords to persist on the node's
  - `extractPackage` — [`L296`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-types.ts#L296) — Extract the dotted package name from a package declaration node.
  - `extractPropertyName` — [`L149`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-types.ts#L149) — Extract property name when the generic name walk fails (e.g. ObjC
  - `extractVariables` — [`L242`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-types.ts#L242) — Extract variable declarations from a variable declaration node.
  - `fieldTypes` — [`L118`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-types.ts#L118) — Node types that represent class fields (extracted as 'field' kind inside class bodies)
  - `functionTypes` — [`L96`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-types.ts#L96) — Node types that represent functions
  - `getReceiverType` — [`L249`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-types.ts#L249) — Extract receiver/owner type name from a method declaration.
  - `getReturnType` — [`L258`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-types.ts#L258) — Extract a function/method's normalized return type name (bare class name,
  - `getSignature` — [`L152`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-types.ts#L152) — Extract signature from node
  - `getVisibility` — [`L154`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-types.ts#L154) — Extract visibility from node
  - `importTypes` — [`L112`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-types.ts#L112) — Node types that represent imports
  - `interfaceKind` — [`L187`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-types.ts#L187) — NodeKind to use for interface-like declarations (Rust: 'trait'). Default: 'interface'
  - `interfaceTypes` — [`L102`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-types.ts#L102) — Node types that represent interfaces/protocols/traits
  - `isAsync` — [`L158`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-types.ts#L158) — Check if node is async
  - `isConst` — [`L162`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-types.ts#L162) — Check if variable declaration is a constant (const vs let/var)
  - `isExported` — [`L156`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-types.ts#L156) — Check if node is exported
  - `isMisparsedFunction` — [`L276`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-types.ts#L276) — Check if a function/method name is a misparse artifact that should be skipped.
  - `isStatic` — [`L160`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-types.ts#L160) — Check if node is static
  - `methodTypes` — [`L100`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-types.ts#L100) — Node types that represent methods
  - `methodsAreTopLevel` — [`L177`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-types.ts#L177) — Whether methods can be top-level without enclosing class (Go: true)
  - `nameField` — [`L125`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-types.ts#L125) — Field name for identifier/name
  - `packageTypes` — [`L293`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-types.ts#L293) — Node types representing a file-level package/namespace declaration
  - `paramsField` — [`L129`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-types.ts#L129) — Field name for parameters
  - `preParse` — [`L91`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-types.ts#L91) — Optional source transform applied immediately before the grammar parses the
  - `propertyTypes` — [`L120`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-types.ts#L120) — Node types that represent class properties (extracted as 'property' kind inside class bodies)
  - `recoverMangledName` — [`L146`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-types.ts#L146) — Post-process an already-extracted name to recover a real identifier from a
  - `resolveBody` — [`L230`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-types.ts#L230) — Resolve the body node for a function/method/class when it's not a child field.
  - `resolveName` — [`L136`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-types.ts#L136) — Override symbol name extraction (e.g. ObjC multi-part selectors).
  - `resolveTypeAliasKind` — [`L267`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-types.ts#L267) — Resolve the actual node kind for a type alias declaration.
  - `returnField` — [`L131`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-types.ts#L131) — Field name for return type
  - `skipBodilessClass` — [`L185`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-types.ts#L185) — Skip a bodiless class node as a forward declaration / elaborated type,
  - `structTypes` — [`L104`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-types.ts#L104) — Node types that represent structs
  - `synthesizeMembers` — [`L209`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-types.ts#L209) — Synthesize members that exist at compile time but not in the source AST,
  - `typeAliasTypes` — [`L110`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-types.ts#L110) — Node types that represent type aliases (e.g. `type X = ...`)
  - `variableTypes` — [`L116`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-types.ts#L116) — Node types that represent variable declarations (const, let, var, etc.)
  - `visitNode` — [`L195`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-types.ts#L195) — Custom node visitor. Return true if the node was fully handled (skip default dispatch).
- uses (calls/refs, reference-scoped): [`Node`](../web-tree-sitter.d.ts.md#Node), [`NodeKind`](../types.ts.md#NodeKind), [`ExtractorContext`](tree-sitter-types.ts.md#ExtractorContext), [`ImportInfo`](tree-sitter-types.ts.md#ImportInfo), [`VariableInfo`](tree-sitter-types.ts.md#VariableInfo)
- used by: [`visitNode`](tree-sitter.ts.md#TreeSitterExtractor.visitNode), [`extractor`](tree-sitter.ts.md#TreeSitterExtractor.extractor), [`kotlin.ts`](languages/kotlin.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-extraction-languages-kotlin.ts), [`index.ts`](languages/index.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-extraction-languages-index.ts), [`tree-sitter.ts`](tree-sitter.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-extraction-tree-sitter.ts), [`createNode`](tree-sitter.ts.md#TreeSitterExtractor.createNode), [`php.ts`](languages/php.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-extraction-languages-php.ts), [`objc.ts`](languages/objc.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-extraction-languages-objc.ts), [`r.ts`](languages/r.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-extraction-languages-r.ts), [`solidity.ts`](languages/solidity.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-extraction-languages-solidity.ts), [`ruby.ts`](languages/ruby.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-extraction-languages-ruby.ts), [`visitFunctionBody`](tree-sitter.ts.md#TreeSitterExtractor.visitFunctionBody), [`terraformExtractor`](languages/terraform.ts.md#terraformExtractor), [`dart.ts`](languages/dart.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-extraction-languages-dart.ts), [`c-cpp.ts`](languages/c-cpp.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-extraction-languages-c-cpp.ts), [`vbnet.ts`](languages/vbnet.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-extraction-languages-vbnet.ts), [`scala.ts`](languages/scala.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-extraction-languages-scala.ts), [`extract`](tree-sitter.ts.md#TreeSitterExtractor.extract), [`extractVariable`](tree-sitter.ts.md#TreeSitterExtractor.extractVariable), [`extractMethod`](tree-sitter.ts.md#TreeSitterExtractor.extractMethod), [`csharp.ts`](languages/csharp.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-extraction-languages-csharp.ts), [`typescript.ts`](languages/typescript.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-extraction-languages-typescript.ts), [`java.ts`](languages/java.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-extraction-languages-java.ts), [`cobol.ts`](languages/cobol.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-extraction-languages-cobol.ts), [`erlang.ts`](languages/erlang.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-extraction-languages-erlang.ts), [`rust.ts`](languages/rust.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-extraction-languages-rust.ts), [`lua.ts`](languages/lua.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-extraction-languages-lua.ts), [`swift.ts`](languages/swift.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-extraction-languages-swift.ts), [`javascript.ts`](languages/javascript.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-extraction-languages-javascript.ts), [`cExtractor`](languages/c-cpp.ts.md#cExtractor), [`pascal.ts`](languages/pascal.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-extraction-languages-pascal.ts), [`cfscript.ts`](languages/cfscript.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-extraction-languages-cfscript.ts), [`extractTypeAlias`](tree-sitter.ts.md#TreeSitterExtractor.extractTypeAlias), [`extractImport`](tree-sitter.ts.md#TreeSitterExtractor.extractImport), [`python.ts`](languages/python.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-extraction-languages-python.ts), [`extractFunction`](tree-sitter.ts.md#TreeSitterExtractor.extractFunction), [`go.ts`](languages/go.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-extraction-languages-go.ts), [`extractClass`](tree-sitter.ts.md#TreeSitterExtractor.extractClass), [`extractEnum`](tree-sitter.ts.md#TreeSitterExtractor.extractEnum), [`extractInterface`](tree-sitter.ts.md#TreeSitterExtractor.extractInterface)  (+22 more)

### `VariableInfo`
- def: [`src/extraction/tree-sitter-types.ts:32`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-types.ts#L32)
- doc: Information about a single variable within a declaration.
- signature: `interface VariableInfo`
- members:
  - `delegateToFunction` — [`L40`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-types.ts#L40) — If set, this declarator is actually a function and should be extracted as such
  - `kind` — [`L36`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-types.ts#L36) — Node kind: 'variable' or 'constant'
  - `name` — [`L34`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-types.ts#L34) — Variable name
  - `positionNode` — [`L42`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-types.ts#L42) — The AST node to use for positioning (may differ from the declaration node)
  - `signature` — [`L38`](../../../../../../raw/code/codegraph/src/extraction/tree-sitter-types.ts#L38) — Optional signature string
- uses (calls/refs, reference-scoped): [`Node`](../web-tree-sitter.d.ts.md#Node), [`NodeKind`](../types.ts.md#NodeKind)
- used by: [`extractVariables`](tree-sitter-types.ts.md#LanguageExtractor.extractVariables)

