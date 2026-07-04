---
title: 'Module: src/resolution/frameworks/java.ts'
type: catalog
provenance: extracted
module: src/resolution/frameworks/java.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/resolution/frameworks/`java.ts`/
symbols:
  springResolver: springResolver.
  extractSpringValueBindings: extractSpringValueBindings().
  extractSpringConfig: extractSpringConfig().
  resolveByNameAndKind: resolveByNameAndKind().
  canonicalConfigKey: canonicalConfigKey().
  extractSpringConfig.typeLiteral171.nodes: extractSpringConfig().typeLiteral171:nodes.
  CLASS_KINDS: CLASS_KINDS.
  parseMappingPath: parseMappingPath().
  extractSpringConfig.typeLiteral171.references: extractSpringConfig().typeLiteral171:references.
  SERVICE_KINDS: SERVICE_KINDS.
  joinPath: joinPath().
  isSpringConfigFile: isSpringConfigFile().
  SERVICE_DIRS: SERVICE_DIRS.
  REPO_DIRS: REPO_DIRS.
  CONTROLLER_DIRS: CONTROLLER_DIRS.
  ENTITY_DIRS: ENTITY_DIRS.
  COMPONENT_DIRS: COMPONENT_DIRS.
---
# Module: [`src/resolution/frameworks/java.ts`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/java.ts)

## Functions
- `canonicalConfigKey(key: string)` — [`L493`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/java.ts#L493) — Spring's relaxed binding (`cache-list` ↔ `cacheList` ↔ `cache_list` ↔
- `extractSpringConfig(filePath: string, content: string)` — [`L315`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/java.ts#L315) — Parse a Spring config file (YAML or .properties) and emit one `constant`
- `extractSpringValueBindings(filePath: string, safe: string, lang: "java" | "kotlin", now: number, nodes: Node[], references: UnresolvedRef[])` — [`L416`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/java.ts#L416) — Append `@Value("${k}")` and `@ConfigurationProperties(prefix=...)`
- `isSpringConfigFile(filePath: string)` — [`L303`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/java.ts#L303) — Spring config file patterns: application(-profile)?.{yml,yaml,properties} +
- `joinPath(prefix: string, sub: string)` — [`L514`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/java.ts#L514) — Join a class-level prefix and a method sub-path into one normalized `/path`.
- `parseMappingPath(args: string)` — [`L508`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/java.ts#L508) — Path string from a mapping's args (`"/x"`, `value = "/x"`, `path = "/x"`); '' if bare.
- `resolveByNameAndKind(name: string, kinds: Set<string>, preferredDirPatterns: string[], context: ResolutionContext)` — [`L522`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/java.ts#L522) — Resolve a symbol by name using indexed queries instead of scanning all files.

## Module values
- `CLASS_KINDS` — [`L504`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/java.ts#L504)
- `COMPONENT_DIRS` — [`L502`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/java.ts#L502)
- `CONTROLLER_DIRS` — [`L500`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/java.ts#L500)
- `ENTITY_DIRS` — [`L501`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/java.ts#L501)
- `REPO_DIRS` — [`L499`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/java.ts#L499)
- `SERVICE_DIRS` — [`L498`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/java.ts#L498)
- `SERVICE_KINDS` — [`L505`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/java.ts#L505)
- `nodes` — [`L318`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/java.ts#L318)
- `references` — [`L318`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/java.ts#L318)
- `springResolver` — [`L11`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/java.ts#L11) — documented in [extraction-index.ts](../../../../concepts/extraction-index.ts.md)

