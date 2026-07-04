---
title: 'Module: src/extraction/languages/c-cpp.ts'
type: catalog
provenance: extracted
module: src/extraction/languages/c-cpp.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/extraction/languages/`c-cpp.ts`/
symbols:
  cExtractor: cExtractor.
  recoverCppMacroDefinedName: recoverCppMacroDefinedName().
  extractCppQualifiedMethodName: extractCppQualifiedMethodName().
  preParseCppSource: preParseCppSource().
  findDeclaratorQualifiedId: findDeclaratorQualifiedId().
  extractCppReturnType: extractCppReturnType().
  extractCppReceiverType: extractCppReceiverType().
  isMacroMisparsedTypeDecl: isMacroMisparsedTypeDecl().
  blankCudaConstructs: blankCudaConstructs().
  blankCppInlineMacros: blankCppInlineMacros().
  preParseCSource: preParseCSource().
  recoverMangledCppName: recoverMangledCppName().
  stripCppTemplateArgs: stripCppTemplateArgs().
  normalizeCppReturnType: normalizeCppReturnType().
  CPP_INLINE_MACRO_RE: CPP_INLINE_MACRO_RE.
  blankMetalAttributes: blankMetalAttributes().
  CPP_INLINE_MACROS: CPP_INLINE_MACROS.
  looksLikeCudaSource: looksLikeCudaSource().
  cppExtractor: cppExtractor.
  CPP_NON_CLASS_RETURN: CPP_NON_CLASS_RETURN.
  blankCppExportMacros: blankCppExportMacros().
  CPP_PRIMITIVE_NAMES: CPP_PRIMITIVE_NAMES.
  METAL_ATTRIBUTE_RE: METAL_ATTRIBUTE_RE.
  CUDA_LAUNCH_BOUNDS_RE: CUDA_LAUNCH_BOUNDS_RE.
  CUDA_SPECIFIER_RE: CUDA_SPECIFIER_RE.
  CUDA_LAUNCH_CONFIG_RE: CUDA_LAUNCH_CONFIG_RE.
---
# Module: [`src/extraction/languages/c-cpp.ts`](../../../../../../../raw/code/codegraph/src/extraction/languages/c-cpp.ts)

## Functions
- `blankCppExportMacros(source: string)` — [`L285`](../../../../../../../raw/code/codegraph/src/extraction/languages/c-cpp.ts#L285) — Blank an export/visibility macro in a `class/struct EXPORT_MACRO Name …`
- `blankCppInlineMacros(source: string)` — [`L369`](../../../../../../../raw/code/codegraph/src/extraction/languages/c-cpp.ts#L369)
- `blankCudaConstructs(source: string)` — [`L483`](../../../../../../../raw/code/codegraph/src/extraction/languages/c-cpp.ts#L483)
- `blankMetalAttributes(source: string)` — [`L431`](../../../../../../../raw/code/codegraph/src/extraction/languages/c-cpp.ts#L431)
- `extractCppQualifiedMethodName(node: Node, source: string)` — [`L75`](../../../../../../../raw/code/codegraph/src/extraction/languages/c-cpp.ts#L75)
- `extractCppReceiverType(node: Node, source: string)` — [`L86`](../../../../../../../raw/code/codegraph/src/extraction/languages/c-cpp.ts#L86)
- `extractCppReturnType(node: Node, source: string)` — [`L166`](../../../../../../../raw/code/codegraph/src/extraction/languages/c-cpp.ts#L166) — A function/method's return type lives in the `function_definition`'s `type`
- `findDeclaratorQualifiedId(declarator: Node)` — [`L13`](../../../../../../../raw/code/codegraph/src/extraction/languages/c-cpp.ts#L13) — Find the function NAME's `qualified_identifier` (`Foo::bar`) inside a
- `isMacroMisparsedTypeDecl(node: Node)` — [`L253`](../../../../../../../raw/code/codegraph/src/extraction/languages/c-cpp.ts#L253) — Detect tree-sitter's misparse of a macro-annotated class/struct, e.g.
- `looksLikeCudaSource(source: string)` — [`L509`](../../../../../../../raw/code/codegraph/src/extraction/languages/c-cpp.ts#L509) — Strong content markers for CUDA source in files without a CUDA extension
- `normalizeCppReturnType(raw: string)` — [`L114`](../../../../../../../raw/code/codegraph/src/extraction/languages/c-cpp.ts#L114) — Normalize a C++ return type to the bare class name a method could be called
- `preParseCSource(source: string)` — [`L536`](../../../../../../../raw/code/codegraph/src/extraction/languages/c-cpp.ts#L536) — C source pre-processing: C-detected headers in CUDA projects (llm.c keeps
- `preParseCppSource(source: string, filePath?: string | undefined)` — [`L523`](../../../../../../../raw/code/codegraph/src/extraction/languages/c-cpp.ts#L523) — C/C++ source pre-processing before tree-sitter: recover both macro-annotated
- `recoverCppMacroDefinedName(node: Node, source: string)` — [`L49`](../../../../../../../raw/code/codegraph/src/extraction/languages/c-cpp.ts#L49) — Recover the real function name from the macro-definition idiom
- `recoverMangledCppName(name: string)` — [`L398`](../../../../../../../raw/code/codegraph/src/extraction/languages/c-cpp.ts#L398) — Universal fallback (any macro, no list) for a C/C++ function name still mangled
- `stripCppTemplateArgs(name: string)` — [`L149`](../../../../../../../raw/code/codegraph/src/extraction/languages/c-cpp.ts#L149) — Strip C++ template arguments from a base-type reference name so it matches the

## Module values
- `CPP_INLINE_MACROS` — [`L318`](../../../../../../../raw/code/codegraph/src/extraction/languages/c-cpp.ts#L318) — Blank a known inline-specifier macro sitting in front of a function's return
- `CPP_INLINE_MACRO_RE` — [`L365`](../../../../../../../raw/code/codegraph/src/extraction/languages/c-cpp.ts#L365)
- `CPP_NON_CLASS_RETURN` — [`L100`](../../../../../../../raw/code/codegraph/src/extraction/languages/c-cpp.ts#L100) — Built-in / non-class return types that can never be a method receiver. We
- `CPP_PRIMITIVE_NAMES` — [`L377`](../../../../../../../raw/code/codegraph/src/extraction/languages/c-cpp.ts#L377)
- `CUDA_LAUNCH_BOUNDS_RE` — [`L473`](../../../../../../../raw/code/codegraph/src/extraction/languages/c-cpp.ts#L473) — Blank CUDA-specific constructs before parsing `.cu`/`.cuh` files (parsed with
- `CUDA_LAUNCH_CONFIG_RE` — [`L482`](../../../../../../../raw/code/codegraph/src/extraction/languages/c-cpp.ts#L482)
- `CUDA_SPECIFIER_RE` — [`L474`](../../../../../../../raw/code/codegraph/src/extraction/languages/c-cpp.ts#L474)
- `METAL_ATTRIBUTE_RE` — [`L429`](../../../../../../../raw/code/codegraph/src/extraction/languages/c-cpp.ts#L429) — Blank Metal Shading Language `[[attribute]]` annotations before parsing.
- `cExtractor` — [`L172`](../../../../../../../raw/code/codegraph/src/extraction/languages/c-cpp.ts#L172)
- `cppExtractor` — [`L540`](../../../../../../../raw/code/codegraph/src/extraction/languages/c-cpp.ts#L540)

