---
title: 'Module: src/project-config.ts'
type: catalog
provenance: extracted
module: src/project-config.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/`project-config.ts`/
symbols:
  parseConfig: parseConfig().
  extractExtensions: extractExtensions().
  loadParsedConfig: loadParsedConfig().
  loadExtensionOverrides: loadExtensionOverrides().
  extractIncludeIgnored: extractIncludeIgnored().
  extractExclude: extractExclude().
  EMPTY_CONFIG: EMPTY_CONFIG.
  PROJECT_CONFIG_FILENAME: PROJECT_CONFIG_FILENAME.
  loadIncludeIgnoredPatterns: loadIncludeIgnoredPatterns().
  loadExcludePatterns: loadExcludePatterns().
  cache: cache.
  EMPTY_EXTENSIONS: EMPTY_EXTENSIONS.
  ParsedConfig.extensions: ParsedConfig#extensions.
  ParsedConfig: ParsedConfig#
  CacheEntry: CacheEntry#
  ProjectConfig: ProjectConfig#
  clearProjectConfigCache: clearProjectConfigCache().
  ParsedConfig.includeIgnored: ParsedConfig#includeIgnored.
  ParsedConfig.exclude: ParsedConfig#exclude.
  CacheEntry.mtimeMs: CacheEntry#mtimeMs.
  CacheEntry.config: CacheEntry#config.
  ProjectConfig.extensions: ProjectConfig#extensions.
  ProjectConfig.includeIgnored: ProjectConfig#includeIgnored.
  ProjectConfig.exclude: ProjectConfig#exclude.
  normalizeExtKey: normalizeExtKey().
---
# Module: [`src/project-config.ts`](../../../../../raw/code/codegraph/src/project-config.ts)

## Classes
### `CacheEntry`
- def: [`src/project-config.ts:65`](../../../../../raw/code/codegraph/src/project-config.ts#L65)
- signature: `interface CacheEntry`
- members:
  - `config` — [`L67`](../../../../../raw/code/codegraph/src/project-config.ts#L67)
  - `mtimeMs` — [`L66`](../../../../../raw/code/codegraph/src/project-config.ts#L66)
- uses (calls/refs, reference-scoped): [`ParsedConfig`](project-config.ts.md#ParsedConfig)
- used by: [`loadParsedConfig`](project-config.ts.md#loadParsedConfig), [`cache`](project-config.ts.md#cache)

### `ParsedConfig`
- def: [`src/project-config.ts:59`](../../../../../raw/code/codegraph/src/project-config.ts#L59)
- doc: Parsed, validated view of a project's `codegraph.json`.
- signature: `interface ParsedConfig`
- members:
  - `exclude` — [`L62`](../../../../../raw/code/codegraph/src/project-config.ts#L62)
  - `extensions` — [`L60`](../../../../../raw/code/codegraph/src/project-config.ts#L60)
  - `includeIgnored` — [`L61`](../../../../../raw/code/codegraph/src/project-config.ts#L61)
- uses (calls/refs, reference-scoped): [`Language`](types.ts.md#Language)
- used by: [`parseConfig`](project-config.ts.md#parseConfig), [`loadParsedConfig`](project-config.ts.md#loadParsedConfig), [`loadExtensionOverrides`](project-config.ts.md#loadExtensionOverrides), [`EMPTY_CONFIG`](project-config.ts.md#EMPTY_CONFIG), [`loadExcludePatterns`](project-config.ts.md#loadExcludePatterns), [`loadIncludeIgnoredPatterns`](project-config.ts.md#loadIncludeIgnoredPatterns), [`CacheEntry`](project-config.ts.md#CacheEntry)

### `ProjectConfig`
- def: [`src/project-config.ts:34`](../../../../../raw/code/codegraph/src/project-config.ts#L34)
- signature: `interface ProjectConfig`
- members:
  - `exclude` — [`L55`](../../../../../raw/code/codegraph/src/project-config.ts#L55) — Gitignore-style patterns for paths to keep OUT of the index — even when
  - `extensions` — [`L36`](../../../../../raw/code/codegraph/src/project-config.ts#L36) — Map of custom file extension (`.foo`) to a supported language id.
  - `includeIgnored` — [`L44`](../../../../../raw/code/codegraph/src/project-config.ts#L44) — Gitignore-style patterns naming gitignored directories whose embedded git
- used by: [`extractExtensions`](project-config.ts.md#extractExtensions), [`extractExclude`](project-config.ts.md#extractExclude), [`extractIncludeIgnored`](project-config.ts.md#extractIncludeIgnored)

## Functions
- `clearProjectConfigCache()` — [`L279`](../../../../../raw/code/codegraph/src/project-config.ts#L279) — Test/maintenance hook: forget cached config (e.g. after rewriting it in a test).
- `extractExclude(parsed: object, file: string)` — [`L198`](../../../../../raw/code/codegraph/src/project-config.ts#L198) — Validate the `exclude` patterns: an array of non-empty gitignore-style
- `extractExtensions(parsed: object, file: string)` — [`L145`](../../../../../raw/code/codegraph/src/project-config.ts#L145) — Validate the `extensions` map. Every failure mode degrades to "no overrides
- `extractIncludeIgnored(parsed: object, file: string)` — [`L172`](../../../../../raw/code/codegraph/src/project-config.ts#L172) — Validate the `includeIgnored` patterns: an array of non-empty gitignore-style
- `loadExcludePatterns(rootDir: string)` — [`L274`](../../../../../raw/code/codegraph/src/project-config.ts#L274) — Load the validated `exclude` patterns for a project, mtime-cached.
- `loadExtensionOverrides(rootDir: string)` — [`L250`](../../../../../raw/code/codegraph/src/project-config.ts#L250) — Load the validated extension overrides for a project, mtime-cached. — documented in [sync-watcher.ts](../../concepts/sync-watcher.ts.md)
- `loadIncludeIgnoredPatterns(rootDir: string)` — [`L262`](../../../../../raw/code/codegraph/src/project-config.ts#L262) — Load the validated `includeIgnored` patterns for a project, mtime-cached.
- `loadParsedConfig(rootDir: string)` — [`L222`](../../../../../raw/code/codegraph/src/project-config.ts#L222) — Load the parsed `codegraph.json` for a project, mtime-cached. A missing or — documented in [sync-watcher.ts](../../concepts/sync-watcher.ts.md)
- `normalizeExtKey(raw: string)` — [`L95`](../../../../../raw/code/codegraph/src/project-config.ts#L95) — Normalize a user-provided extension key to the `.ext` lowercase form used by
- `parseConfig(file: string)` — [`L111`](../../../../../raw/code/codegraph/src/project-config.ts#L111) — Read + JSON-parse a `codegraph.json` once and return its validated view. — documented in [sync-watcher.ts](../../concepts/sync-watcher.ts.md)

## Module values
- `EMPTY_CONFIG` — [`L80`](../../../../../raw/code/codegraph/src/project-config.ts#L80)
- `EMPTY_EXTENSIONS` — [`L79`](../../../../../raw/code/codegraph/src/project-config.ts#L79) — Shared frozen empties so the no-config path allocates nothing.
- `PROJECT_CONFIG_FILENAME` — [`L32`](../../../../../raw/code/codegraph/src/project-config.ts#L32) — Filename of the project-scoped config, resolved relative to the project root.
- `cache` — [`L76`](../../../../../raw/code/codegraph/src/project-config.ts#L76) — Cache keyed by project root. The loader is called once per indexing/scan/sync

