---
title: 'Module: src/resolution/import-resolver.ts'
type: catalog
provenance: extracted
module: src/resolution/import-resolver.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/resolution/`import-resolver.ts`/
symbols:
  resolveViaImport: resolveViaImport().
  resolvePythonModuleMember: resolvePythonModuleMember().
  resolveModuleImportToFile: resolveModuleImportToFile().
  findExportedSymbol.want-typeLiteral677.memberName: findExportedSymbol().(want)typeLiteral677:memberName.
  resolveGoCrossPackageReference: resolveGoCrossPackageReference().
  resolveJavaImportedReference: resolveJavaImportedReference().
  resolveImportPath: resolveImportPath().
  resolveJvmImport: resolveJvmImport().
  isExternalImport: isExternalImport().
  resolveRustPathReference: resolveRustPathReference().
  resolveStaticMember: resolveStaticMember().
  resolveLuaRequire: resolveLuaRequire().
  extractImportMappings: extractImportMappings().
  resolveAliasedImport: resolveAliasedImport().
  resolvePythonAbsoluteModule: resolvePythonAbsoluteModule().
  extractJSImports: extractJSImports().
  extractPythonImports: extractPythonImports().
  extractGoImports: extractGoImports().
  extractJavaImports: extractJavaImports().
  extractPHPImports: extractPHPImports().
  extractCppImports: extractCppImports().
  findPythonModuleFile: findPythonModuleFile().
  resolveRelativeImport: resolveRelativeImport().
  resolveCppIncludePath: resolveCppIncludePath().
  resolveRustModuleFile: resolveRustModuleFile().
  isPhpIncludePathRef: isPhpIncludePathRef().
  resolveCobolCopybook: resolveCobolCopybook().
  resolvePhpIncludePath: resolvePhpIncludePath().
  isCobolCopybookRef: isCobolCopybookRef().
  loadCppIncludeDirs: loadCppIncludeDirs().
  extractReExports: extractReExports().
  rustCrateRootDir: rustCrateRootDir().
  pickClosestJvmCandidate: pickClosestJvmCandidate().
  STATIC_MEMBER_CONTAINERS: STATIC_MEMBER_CONTAINERS.
  clearImportMappingCache: clearImportMappingCache().
  cobolCopybookIndexes: cobolCopybookIndexes.
  EXTENSION_RESOLUTION: EXTENSION_RESOLUTION.
  cppIncludeDirCache: cppIncludeDirCache.
  findExportedSymbol.want-typeLiteral677.isDefault: findExportedSymbol().(want)typeLiteral677:isDefault.
  findExportedSymbol.want-typeLiteral677.exportedName: findExportedSymbol().(want)typeLiteral677:exportedName.
  loadCppIncludeDirsFromCompileDB: loadCppIncludeDirsFromCompileDB().
  importMappingCache: importMappingCache.
  rustSelfModuleDir: rustSelfModuleDir().
  findExportedSymbol: findExportedSymbol().
  findExportedSymbol.want-typeLiteral677.isNamespace: findExportedSymbol().(want)typeLiteral677:isNamespace.
  clearCppIncludeDirCache: clearCppIncludeDirCache().
  C_CPP_STDLIB_HEADERS: C_CPP_STDLIB_HEADERS.
  shlexSplit: shlexSplit().
  loadCppIncludeDirsHeuristic: loadCppIncludeDirsHeuristic().
  stripJsComments: stripJsComments().
  REEXPORT_MAX_DEPTH: REEXPORT_MAX_DEPTH.
---
# Module: [`src/resolution/import-resolver.ts`](../../../../../../raw/code/codegraph/src/resolution/import-resolver.ts)

## Functions
- `clearCppIncludeDirCache()` — [`L393`](../../../../../../raw/code/codegraph/src/resolution/import-resolver.ts#L393) — Clear the C/C++ include directory cache (call between indexing runs)
- `clearImportMappingCache()` — [`L988`](../../../../../../raw/code/codegraph/src/resolution/import-resolver.ts#L988) — Clear the import mapping cache (call between indexing runs)
- `extractCppImports(content: string)` — [`L959`](../../../../../../raw/code/codegraph/src/resolution/import-resolver.ts#L959) — Extract C/C++ import mappings from #include directives.
- `extractGoImports(content: string)` — [`L840`](../../../../../../raw/code/codegraph/src/resolution/import-resolver.ts#L840) — Extract Go import mappings
- `extractImportMappings(_filePath: string, content: string, language: "typescript" | "javascript" | "tsx" | "jsx" | "python" | "go" | "rust" | "java" | "c" | "cpp" | "csharp" | "razor" | "php" | "ruby" | "swift" | ... 24 more ... | "unknown")` — [`L645`](../../../../../../raw/code/codegraph/src/resolution/import-resolver.ts#L645) — Extract import mappings from a file
- `extractJSImports(content: string)` — [`L683`](../../../../../../raw/code/codegraph/src/resolution/import-resolver.ts#L683) — Extract JS/TS import mappings
- `extractJavaImports(content: string)` — [`L896`](../../../../../../raw/code/codegraph/src/resolution/import-resolver.ts#L896) — Extract Java / Kotlin import mappings.
- `extractPHPImports(content: string)` — [`L928`](../../../../../../raw/code/codegraph/src/resolution/import-resolver.ts#L928) — Extract PHP import mappings (use statements)
- `extractPythonImports(content: string)` — [`L787`](../../../../../../raw/code/codegraph/src/resolution/import-resolver.ts#L787) — Extract Python import mappings
- `extractReExports(content: string, language: "typescript" | "javascript" | "tsx" | "jsx" | "python" | "go" | "rust" | "java" | "c" | "cpp" | "csharp" | "razor" | "php" | "ruby" | "swift" | "kotlin" | "dart" | ... 22 more ... | "unknown")` — [`L1059`](../../../../../../raw/code/codegraph/src/resolution/import-resolver.ts#L1059) — Extract JS/TS re-export declarations from `content`.
- `findExportedSymbol(filePath: string, want: { isDefault: boolean; isNamespace: boolean; exportedName: string; memberName: string | null; }, language: "typescript" | "javascript" | "tsx" | "jsx" | "python" | ... 34 more ... | "unknown", context: ResolutionContext, visited: Set<...>, depth?: number)` — [`L1922`](../../../../../../raw/code/codegraph/src/resolution/import-resolver.ts#L1922) — Find an exported symbol in `filePath`, following `export { x } from
- `findPythonModuleFile(mod: string, context: ResolutionContext, excludeFilePath: string)` — [`L1609`](../../../../../../raw/code/codegraph/src/resolution/import-resolver.ts#L1609) — Find the file node for a Python dotted module path `a.b.c` — a module file
- `isCobolCopybookRef(ref: UnresolvedRef)` — [`L614`](../../../../../../raw/code/codegraph/src/resolution/import-resolver.ts#L614) — Is this a COBOL COPY / EXEC SQL INCLUDE copybook reference? These resolve
- `isExternalImport(importPath: string, language: "typescript" | "javascript" | "tsx" | "jsx" | "python" | "go" | "rust" | "java" | "c" | "cpp" | "csharp" | "razor" | "php" | "ruby" | "swift" | "kotlin" | ... 23 more ... | "unknown", context?: ResolutionContext | undefined)` — [`L183`](../../../../../../raw/code/codegraph/src/resolution/import-resolver.ts#L183) — Check if an import is external (npm package, etc.)
- `isPhpIncludePathRef(ref: UnresolvedRef)` — [`L601`](../../../../../../raw/code/codegraph/src/resolution/import-resolver.ts#L601) — Is this reference a PHP include/require PATH (vs a namespace `use` symbol)?
- `loadCppIncludeDirs(projectRoot: string)` — [`L410`](../../../../../../raw/code/codegraph/src/resolution/import-resolver.ts#L410) — Discover C/C++ include search directories for a project.
- `loadCppIncludeDirsFromCompileDB(projectRoot: string)` — [`L426`](../../../../../../raw/code/codegraph/src/resolution/import-resolver.ts#L426) — Try to load include directories from compile_commands.json.
- `loadCppIncludeDirsHeuristic(projectRoot: string)` — [`L535`](../../../../../../raw/code/codegraph/src/resolution/import-resolver.ts#L535) — Heuristic include directory discovery when no compile_commands.json exists.
- `pickClosestJvmCandidate(candidates: Node[], fromPath: string)` — [`L1166`](../../../../../../raw/code/codegraph/src/resolution/import-resolver.ts#L1166) — Pick the same-FQN candidate closest to `fromPath` by shared directory
- `resolveAliasedImport(importPath: string, projectRoot: string, language: "typescript" | "javascript" | "tsx" | "jsx" | "python" | "go" | "rust" | "java" | "c" | "cpp" | "csharp" | "razor" | "php" | "ruby" | ... 25 more ... | "unknown", context: ResolutionContext)` — [`L325`](../../../../../../raw/code/codegraph/src/resolution/import-resolver.ts#L325) — Resolve an aliased/absolute import.
- `resolveCobolCopybook(member: string, fromFile: string, context: ResolutionContext)` — [`L97`](../../../../../../raw/code/codegraph/src/resolution/import-resolver.ts#L97)
- `resolveCppIncludePath(importPath: string, language: "typescript" | "javascript" | "tsx" | "jsx" | "python" | "go" | "rust" | "java" | "c" | "cpp" | "csharp" | "razor" | "php" | "ruby" | "swift" | "kotlin" | ... 23 more ... | "unknown", context: ResolutionContext)` — [`L570`](../../../../../../raw/code/codegraph/src/resolution/import-resolver.ts#L570) — Resolve a C/C++ include path by searching include directories.
- `resolveGoCrossPackageReference(ref: UnresolvedRef, imports: ImportMapping[], context: ResolutionContext)` — [`L1857`](../../../../../../raw/code/codegraph/src/resolution/import-resolver.ts#L1857) — Resolve a Go cross-package qualified reference (`pkga.FuncX`) by matching
- `resolveImportPath(importPath: string, fromFile: string, language: "typescript" | "javascript" | "tsx" | "jsx" | "python" | "go" | "rust" | "java" | "c" | "cpp" | "csharp" | "razor" | "php" | "ruby" | "swift" | ... 24 more ... | "unknown", context: ResolutionContext)` — [`L43`](../../../../../../raw/code/codegraph/src/resolution/import-resolver.ts#L43) — Resolve an import path to an actual file
- `resolveJavaImportedReference(ref: UnresolvedRef, imports: ImportMapping[], context: ResolutionContext)` — [`L1783`](../../../../../../raw/code/codegraph/src/resolution/import-resolver.ts#L1783) — Resolve a Java/Kotlin reference whose receiver is the simple name of
- `resolveJvmImport(ref: UnresolvedRef, context: ResolutionContext)` — [`L1126`](../../../../../../raw/code/codegraph/src/resolution/import-resolver.ts#L1126) — JVM (Java / Kotlin) imports use fully-qualified names (`import
- `resolveLuaRequire(ref: UnresolvedRef, context: ResolutionContext)` — [`L1520`](../../../../../../raw/code/codegraph/src/resolution/import-resolver.ts#L1520) — Resolve a Lua/Luau `require(...)` to its module file. The reference name is
- `resolveModuleImportToFile(ref: UnresolvedRef, imports: ImportMapping[], context: ResolutionContext)` — [`L1548`](../../../../../../raw/code/codegraph/src/resolution/import-resolver.ts#L1548)
- `resolvePhpIncludePath(includePath: string, fromFile: string, context: ResolutionContext)` — [`L625`](../../../../../../raw/code/codegraph/src/resolution/import-resolver.ts#L625) — Resolve a PHP include/require path to a project-relative file path.
- `resolvePythonAbsoluteModule(ref: UnresolvedRef, context: ResolutionContext)` — [`L1633`](../../../../../../raw/code/codegraph/src/resolution/import-resolver.ts#L1633) — Resolve a Python ABSOLUTE dotted module import (`import a.b.c`) to its file —
- `resolvePythonModuleMember(ref: UnresolvedRef, imports: ImportMapping[], context: ResolutionContext)` — [`L1439`](../../../../../../raw/code/codegraph/src/resolution/import-resolver.ts#L1439) — Resolve a Python qualified reference whose receiver is an imported MODULE:
- `resolveRelativeImport(importPath: string, fromDir: string, language: "typescript" | "javascript" | "tsx" | "jsx" | "python" | "go" | "rust" | "java" | "c" | "cpp" | "csharp" | "razor" | "php" | "ruby" | "swift" | ... 24 more ... | "unknown", context: ResolutionContext)` — [`L267`](../../../../../../raw/code/codegraph/src/resolution/import-resolver.ts#L267) — Resolve a relative import
- `resolveRustModuleFile(segments: string[], fromFile: string, context: ResolutionContext)` — [`L1718`](../../../../../../raw/code/codegraph/src/resolution/import-resolver.ts#L1718) — Resolve a Rust module path (segments WITHOUT the leaf symbol) to the file of
- `resolveRustPathReference(ref: UnresolvedRef, context: ResolutionContext)` — [`L1656`](../../../../../../raw/code/codegraph/src/resolution/import-resolver.ts#L1656) — Resolve a Rust qualified reference `A::B::C` by mapping the MODULE prefix
- `resolveStaticMember(container: Node, ref: UnresolvedRef, localName: string, context: ResolutionContext)` — [`L2028`](../../../../../../raw/code/codegraph/src/resolution/import-resolver.ts#L2028) — Resolve `Container.member` — a static method/property access on a NAMED class
- `resolveViaImport(ref: UnresolvedRef, context: ResolutionContext)` — [`L1191`](../../../../../../raw/code/codegraph/src/resolution/import-resolver.ts#L1191) — documented in [resolution-index.ts](../../../concepts/resolution-index.ts.md)
- `rustCrateRootDir(fromFileAbs: string, context: ResolutionContext)` — [`L1688`](../../../../../../raw/code/codegraph/src/resolution/import-resolver.ts#L1688) — The crate-root directory (holds `lib.rs`/`main.rs`), walking up from a file.
- `rustSelfModuleDir(fromFileAbs: string)` — [`L1705`](../../../../../../raw/code/codegraph/src/resolution/import-resolver.ts#L1705) — Directory under which the current file's module declares its SUBMODULES.
- `shlexSplit(cmd: string)` — [`L498`](../../../../../../raw/code/codegraph/src/resolution/import-resolver.ts#L498) — Minimal shlex-style split for compiler command strings.
- `stripJsComments(content: string)` — [`L1005`](../../../../../../raw/code/codegraph/src/resolution/import-resolver.ts#L1005) — Strip JS line + block comments from `content` while preserving

## Module values
- `C_CPP_STDLIB_HEADERS` — [`L142`](../../../../../../raw/code/codegraph/src/resolution/import-resolver.ts#L142) — C and C++ standard library header names (without delimiters).
- `EXTENSION_RESOLUTION` — [`L17`](../../../../../../raw/code/codegraph/src/resolution/import-resolver.ts#L17) — Extension resolution order by language
- `REEXPORT_MAX_DEPTH` — [`L1910`](../../../../../../raw/code/codegraph/src/resolution/import-resolver.ts#L1910) — Recursive depth cap for re-export chain following. Real codebases
- `STATIC_MEMBER_CONTAINERS` — [`L2011`](../../../../../../raw/code/codegraph/src/resolution/import-resolver.ts#L2011) — Node kinds that own static members reachable as `Container.member`.
- `cobolCopybookIndexes` — [`L95`](../../../../../../raw/code/codegraph/src/resolution/import-resolver.ts#L95) — COBOL copybook lookup: `COPY CVACT01Y` (or `EXEC SQL INCLUDE X`) names a
- `cppIncludeDirCache` — [`L388`](../../../../../../raw/code/codegraph/src/resolution/import-resolver.ts#L388) — C/C++ include directory cache (keyed by project root).
- `exportedName` — [`L1927`](../../../../../../raw/code/codegraph/src/resolution/import-resolver.ts#L1927)
- `importMappingCache` — [`L983`](../../../../../../raw/code/codegraph/src/resolution/import-resolver.ts#L983)
- `isDefault` — [`L1925`](../../../../../../raw/code/codegraph/src/resolution/import-resolver.ts#L1925)
- `isNamespace` — [`L1926`](../../../../../../raw/code/codegraph/src/resolution/import-resolver.ts#L1926)
- `memberName` — [`L1928`](../../../../../../raw/code/codegraph/src/resolution/import-resolver.ts#L1928)

