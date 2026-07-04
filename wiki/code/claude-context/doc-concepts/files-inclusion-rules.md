---
title: File inclusion rules — extensions minus ignores
type: doc-concept
provenance: doc
source: raw/code/claude-context/docs/dive-deep/file-inclusion-rules.md
updated: 2026-07-04
status: fresh
---
# File inclusion rules — extensions minus ignores

## Definition
Before claude-context can chunk, embed, and index a codebase, it must decide **which files even
enter the pipeline**. The doc states the whole policy as one set equation:

```
Final Files = (All Supported Extensions) − (All Ignore Patterns)
```

An *inclusion* set (file extensions the indexer understands) is intersected with the directory
tree, and an *exclusion* set (glob patterns for junk, build output, secrets) is subtracted. Both
sides are **additive unions of several sources** — built-in defaults, MCP request parameters,
environment variables, and (for ignores only) on-disk ignore files. A file is indexed iff its
extension is in the supported set **and** its path is not matched by any ignore pattern.

## In claude-context (grounded)
The two sets are assembled in the [`Context` constructor](../catalog/packages/core/src/context.ts.md#Context.-constructor).
The **extension** set unions the built-in
[`DEFAULT_SUPPORTED_EXTENSIONS`](../catalog/packages/core/src/context.ts.md#DEFAULT_SUPPORTED_EXTENSIONS)
with [`ContextConfig.supportedExtensions`](../catalog/packages/core/src/context.ts.md#ContextConfig.supportedExtensions),
[`ContextConfig.customExtensions`](../catalog/packages/core/src/context.ts.md#ContextConfig.customExtensions),
and any `CUSTOM_EXTENSIONS` env value, then de-dups into
[`Context.supportedExtensions`](../catalog/packages/core/src/context.ts.md#Context.supportedExtensions).
The **ignore** set unions
[`DEFAULT_IGNORE_PATTERNS`](../catalog/packages/core/src/context.ts.md#DEFAULT_IGNORE_PATTERNS) with
[`ContextConfig.ignorePatterns`](../catalog/packages/core/src/context.ts.md#ContextConfig.ignorePatterns),
[`ContextConfig.customIgnorePatterns`](../catalog/packages/core/src/context.ts.md#ContextConfig.customIgnorePatterns),
and any `CUSTOM_IGNORE_PATTERNS` env value into
[`Context.baseIgnorePatterns`](../catalog/packages/core/src/context.ts.md#Context.baseIgnorePatterns)
(via [`dedupePatterns`](../catalog/packages/core/src/context.ts.md#Context.dedupePatterns)). See the
[extensions](files-supported-extensions.md) and [ignore-patterns](files-ignore-patterns.md) pages
for the per-source detail.

The equation is **evaluated during directory traversal**, not as a literal set difference over a
pre-listed file set. [`getCodeFiles`](../catalog/packages/core/src/context.ts.md#Context.getCodeFiles)
recursively walks the codebase and, for each entry, first tests the **ignore** side with an
[`IgnoreMatcher`](../catalog/packages/core/src/utils/ignore-matcher.ts.md#IgnoreMatcher):
`ignoreMatcher.ignores(relativePath, entry.isDirectory())` prunes matched files **and whole
directories** (a matched directory is never descended, so ignoring is the fast path). Surviving
files then pass the **inclusion** side — a plain `supportedExtensions.includes(path.extname(name))`
membership test. Only entries that clear both gates are collected for chunking.

> [!inferred]
> The doc's `Final = Extensions − Ignores` is a mental model; operationally the ignore test runs
> **first** (and short-circuits directory descent), then the extension test filters the remaining
> files. The observable result matches the equation, but the ordering means an ignored directory's
> supported files are never even stat-ed.

The file-level ignore set is loaded fresh per codebase by
[`loadIgnorePatterns`](../catalog/packages/core/src/context.ts.md#Context.loadIgnorePatterns), which
merges `baseIgnorePatterns` with the on-disk ignore files (`.gitignore`, `.xxxignore`, global
`~/.context/.contextignore`) and any per-request patterns — see the
[ignore-patterns page](files-ignore-patterns.md).

## Why it matters / when it applies
This gate is the very first filter in the index pipeline: nothing outside `Final Files` is ever
chunked by the [AST splitter](../concepts/packages-core-src-splitter-ast-splitter.ts.md), embedded,
or written to the vector store. Getting it right is what keeps `node_modules`, build output,
minified bundles, and `.env` secrets out of the semantic index — and what lets a user opt an unusual
extension (`.vue`, `.svelte`) into it without editing source. Because the ignore side prunes whole
directories, it is also the main lever for indexing speed on large repos.

## Connections
- **Code concepts:** [Context orchestrator](../concepts/packages-core-src-context.ts.md) (owns file
  walking and the index pipeline this gate feeds);
  [AST splitter](../concepts/packages-core-src-splitter-ast-splitter.ts.md) and
  [splitter contract](../concepts/packages-core-src-splitter-index.ts.md) (consume the surviving
  files); [FileSynchronizer](../concepts/packages-core-src-sync-synchronizer.ts.md) (shares the same
  `IgnoreMatcher` for incremental change detection).
- **Module catalogs:** [`context.ts`](../catalog/packages/core/src/context.ts.md) ·
  [`ignore-matcher.ts`](../catalog/packages/core/src/utils/ignore-matcher.ts.md).
- **Related doc-concepts:** [supported extensions](files-supported-extensions.md) (the inclusion
  set) · [ignore patterns](files-ignore-patterns.md) (the exclusion set).

## Source
[`docs/dive-deep/file-inclusion-rules.md`](../../../../raw/code/claude-context/docs/dive-deep/file-inclusion-rules.md)
</content>
