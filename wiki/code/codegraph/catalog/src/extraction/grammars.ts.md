---
title: 'Module: src/extraction/grammars.ts'
type: catalog
provenance: extracted
module: src/extraction/grammars.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/extraction/`grammars.ts`/
symbols:
  detectLanguage: detectLanguage().
  loadGrammarsForLanguages: loadGrammarsForLanguages().
  isSourceFile: isSourceFile().
  isLanguageSupported: isLanguageSupported().
  getParser: getParser().
  initGrammars: initGrammars().
  parserCache: parserCache.
  loadAllGrammars: loadAllGrammars().
  getSupportedLanguages: getSupportedLanguages().
  resetParser: resetParser().
  languageCache: languageCache.
  WASM_GRAMMAR_FILES: WASM_GRAMMAR_FILES.
  isFileLevelOnlyLanguage: isFileLevelOnlyLanguage().
  clearParserCache: clearParserCache().
  isGrammarLoaded: isGrammarLoaded().
  GrammarLanguage: GrammarLanguage#
  unavailableGrammarErrors: unavailableGrammarErrors.
  getUnavailableGrammarErrors: getUnavailableGrammarErrors().
  EXTENSION_MAP: EXTENSION_MAP.
  isPlayRoutesFile: isPlayRoutesFile().
  parserInitialized: parserInitialized.
  isGrammarsInitialized: isGrammarsInitialized().
  getLanguageDisplayName: getLanguageDisplayName().
  isShopifyLiquidJson: isShopifyLiquidJson().
  isErlangAppFile: isErlangAppFile().
  looksLikeCpp: looksLikeCpp().
  looksLikeObjc: looksLikeObjc().
---
# Module: [`src/extraction/grammars.ts`](../../../../../../raw/code/codegraph/src/extraction/grammars.ts)

## Classes
### `GrammarLanguage`
- def: [`src/extraction/grammars.ts:13`](../../../../../../raw/code/codegraph/src/extraction/grammars.ts#L13)
- signature: `type GrammarLanguage`
- uses (calls/refs, reference-scoped): [`Language`](../types.ts.md#Language)
- used by: [`loadGrammarsForLanguages`](grammars.ts.md#loadGrammarsForLanguages), [`getSupportedLanguages`](grammars.ts.md#getSupportedLanguages), [`loadAllGrammars`](grammars.ts.md#loadAllGrammars), [`WASM_GRAMMAR_FILES`](grammars.ts.md#WASM_GRAMMAR_FILES)

## Functions
- `clearParserCache()` — [`L456`](../../../../../../raw/code/codegraph/src/extraction/grammars.ts#L456) — Clear parser/grammar caches (useful for testing)
- `detectLanguage(filePath: string, source?: string | undefined, overrides?: Record<string, "typescript" | "javascript" | "tsx" | "jsx" | "python" | "go" | "rust" | "java" | "c" | "cpp" | "csharp" | "razor" | ... 27 more ... | "unknown"> | undefined)` — [`L351`](../../../../../../raw/code/codegraph/src/extraction/grammars.ts#L351) — Detect language from file extension.
- `getLanguageDisplayName(language: "typescript" | "javascript" | "tsx" | "jsx" | "python" | "go" | "rust" | "java" | "c" | "cpp" | "csharp" | "razor" | "php" | "ruby" | "swift" | "kotlin" | "dart" | "svelte" | "vue" | ... 20 more ... | "unknown")` — [`L480`](../../../../../../raw/code/codegraph/src/extraction/grammars.ts#L480) — Get language display name
- `getParser(language: "typescript" | "javascript" | "tsx" | "jsx" | "python" | "go" | "rust" | "java" | "c" | "cpp" | "csharp" | "razor" | "php" | "ruby" | "swift" | "kotlin" | "dart" | "svelte" | "vue" | ... 20 more ... | "unknown")` — [`L328`](../../../../../../raw/code/codegraph/src/extraction/grammars.ts#L328) — Get a parser for the specified language.
- `getSupportedLanguages()` — [`L434`](../../../../../../raw/code/codegraph/src/extraction/grammars.ts#L434) — Get all supported languages (those with grammar definitions).
- `getUnavailableGrammarErrors()` — [`L469`](../../../../../../raw/code/codegraph/src/extraction/grammars.ts#L469) — Report grammars that failed to load.
- `initGrammars()` — [`L236`](../../../../../../raw/code/codegraph/src/extraction/grammars.ts#L236) — Initialize the tree-sitter WASM runtime. Must be called before loading grammars.
- `isErlangAppFile(filePath: string)` — [`L205`](../../../../../../raw/code/codegraph/src/extraction/grammars.ts#L205) — OTP application resource file: `<app>.app.src` (checked into every rebar3/
- `isFileLevelOnlyLanguage(language: "typescript" | "javascript" | "tsx" | "jsx" | "python" | "go" | "rust" | "java" | "c" | "cpp" | "csharp" | "razor" | "php" | "ruby" | "swift" | "kotlin" | "dart" | "svelte" | "vue" | ... 20 more ... | "unknown")` — [`L427`](../../../../../../raw/code/codegraph/src/extraction/grammars.ts#L427) — Languages tracked at the file-record level only: parsing emits zero symbol
- `isGrammarLoaded(language: "typescript" | "javascript" | "tsx" | "jsx" | "python" | "go" | "rust" | "java" | "c" | "cpp" | "csharp" | "razor" | "php" | "ruby" | "swift" | "kotlin" | "dart" | "svelte" | "vue" | ... 20 more ... | "unknown")` — [`L411`](../../../../../../raw/code/codegraph/src/extraction/grammars.ts#L411) — Check if a grammar has been loaded and is ready for parsing.
- `isGrammarsInitialized()` — [`L320`](../../../../../../raw/code/codegraph/src/extraction/grammars.ts#L320) — Check if grammars have been initialized
- `isLanguageSupported(language: "typescript" | "javascript" | "tsx" | "jsx" | "python" | "go" | "rust" | "java" | "c" | "cpp" | "csharp" | "razor" | "php" | "ruby" | "swift" | "kotlin" | "dart" | "svelte" | "vue" | ... 20 more ... | "unknown")` — [`L394`](../../../../../../raw/code/codegraph/src/extraction/grammars.ts#L394) — Check if a language is supported (has a grammar defined).
- `isPlayRoutesFile(filePath: string)` — [`L214`](../../../../../../raw/code/codegraph/src/extraction/grammars.ts#L214) — Play Framework routes file: the extensionless `conf/routes` (and included
- `isShopifyLiquidJson(filePath: string)` — [`L191`](../../../../../../raw/code/codegraph/src/extraction/grammars.ts#L191) — Shopify OS 2.0 JSON template (`templates/*.json`) or section group
- `isSourceFile(filePath: string, overrides?: Record<string, "typescript" | "javascript" | "tsx" | "jsx" | "python" | "go" | "rust" | "java" | "c" | "cpp" | "csharp" | "razor" | "php" | "ruby" | "swift" | ... 24 more ... | "unknown"> | undefined)` — [`L176`](../../../../../../raw/code/codegraph/src/extraction/grammars.ts#L176) — Whether a file is one CodeGraph can parse, based purely on its extension. — documented in [sync-watcher.ts](../../../concepts/sync-watcher.ts.md)
- `loadAllGrammars()` — [`L312`](../../../../../../raw/code/codegraph/src/extraction/grammars.ts#L312) — Load ALL grammar WASM files. Convenience function for tests and
- `loadGrammarsForLanguages(languages: ("typescript" | "javascript" | "tsx" | "jsx" | "python" | "go" | "rust" | "java" | "c" | "cpp" | "csharp" | "razor" | "php" | "ruby" | "swift" | "kotlin" | "dart" | "svelte" | "vue" | ... 20 more ... | "unknown")[])` — [`L249`](../../../../../../raw/code/codegraph/src/extraction/grammars.ts#L249) — Load grammar WASM files for specific languages only.
- `looksLikeCpp(source: string)` — [`L377`](../../../../../../raw/code/codegraph/src/extraction/grammars.ts#L377) — Heuristic: does a .h file contain C++ constructs?
- `looksLikeObjc(source: string)` — [`L385`](../../../../../../raw/code/codegraph/src/extraction/grammars.ts#L385) — Heuristic: does a .h file contain Objective-C constructs?
- `resetParser(language: "typescript" | "javascript" | "tsx" | "jsx" | "python" | "go" | "rust" | "java" | "c" | "cpp" | "csharp" | "razor" | "php" | "ruby" | "swift" | "kotlin" | "dart" | "svelte" | "vue" | ... 20 more ... | "unknown")` — [`L445`](../../../../../../raw/code/codegraph/src/extraction/grammars.ts#L445) — Reset the cached parser for a language to reclaim WASM heap memory.

## Module values
- `EXTENSION_MAP` — [`L55`](../../../../../../raw/code/codegraph/src/extraction/grammars.ts#L55) — File extension to Language mapping
- `WASM_GRAMMAR_FILES` — [`L19`](../../../../../../raw/code/codegraph/src/extraction/grammars.ts#L19) — WASM filename map — maps each language to its .wasm grammar file
- `languageCache` — [`L226`](../../../../../../raw/code/codegraph/src/extraction/grammars.ts#L226)
- `parserCache` — [`L225`](../../../../../../raw/code/codegraph/src/extraction/grammars.ts#L225) — Caches for loaded grammars and parsers
- `parserInitialized` — [`L229`](../../../../../../raw/code/codegraph/src/extraction/grammars.ts#L229)
- `unavailableGrammarErrors` — [`L227`](../../../../../../raw/code/codegraph/src/extraction/grammars.ts#L227)

