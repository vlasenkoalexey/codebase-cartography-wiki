---
title: Supported extensions — the additive inclusion set
type: doc-concept
provenance: doc
source: raw/code/claude-context/docs/dive-deep/file-inclusion-rules.md
updated: 2026-07-04
status: fresh
---
# Supported extensions — the additive inclusion set

## Definition
The **inclusion** half of the [file-inclusion rule](files-inclusion-rules.md): a file only enters
the index if its extension is in the supported set. That set is an **additive union of three
sources**, all merged and de-duplicated:

1. **Default extensions** — the built-in list of languages and doc formats claude-context ships with.
2. **MCP custom extensions** — extras passed per-request via the MCP `customExtensions` parameter
   (e.g. *"index this codebase, and include `.vue`, `.svelte`, `.astro` files"*).
3. **Environment-variable extensions** — a comma-separated `CUSTOM_EXTENSIONS` env value.

There is no on-disk "include file" analogue to `.gitignore`; extensions only ever come from these
three sources.

## In claude-context (grounded)
**Defaults.** [`DEFAULT_SUPPORTED_EXTENSIONS`](../catalog/packages/core/src/context.ts.md#DEFAULT_SUPPORTED_EXTENSIONS)
is a module-level constant covering programming languages (`.ts .tsx .js .jsx .py .java .cpp .c .h
.hpp .cs .go .rs .php .rb .swift .kt .scala .m .mm .dart .sol`) and documentation formats (`.md
.markdown .ipynb`). Commented-out entries in the source (`.txt`, `.json`, `.yaml`, `.html`, `.css`,
…) show the maintainers deliberately keep config/markup out of the default set.

**Assembly.** The [constructor](../catalog/packages/core/src/context.ts.md#Context.-constructor)
unions the defaults with
[`ContextConfig.supportedExtensions`](../catalog/packages/core/src/context.ts.md#ContextConfig.supportedExtensions),
[`ContextConfig.customExtensions`](../catalog/packages/core/src/context.ts.md#ContextConfig.customExtensions),
and the env extensions read by
[`getCustomExtensionsFromEnv`](../catalog/packages/core/src/context.ts.md#Context.getCustomExtensionsFromEnv),
then `new Set(...)` de-dups into
[`Context.supportedExtensions`](../catalog/packages/core/src/context.ts.md#Context.supportedExtensions).

**Env parsing.** [`getCustomExtensionsFromEnv`](../catalog/packages/core/src/context.ts.md#Context.getCustomExtensionsFromEnv)
splits `CUSTOM_EXTENSIONS` on commas, trims, drops empties, and **prepends a dot** to any entry that
lacks one (so `vue` and `.vue` both work). The same trim/dot-normalize logic is factored into
[`normalizeExtensions`](../catalog/packages/core/src/context.ts.md#Context.normalizeExtensions).

**Dynamic (MCP) extensions.** Extensions supplied after construction are folded in by
[`addCustomExtensions`](../catalog/packages/core/src/context.ts.md#Context.addCustomExtensions), which
normalizes and set-merges them into `supportedExtensions` in place. For a **non-mutating** view used
during a single operation,
[`getEffectiveSupportedExtensions`](../catalog/packages/core/src/context.ts.md#Context.getEffectiveSupportedExtensions)
returns `supportedExtensions ∪ additionalExtensions` without touching the stored field. The public
read accessor is
[`getSupportedExtensions`](../catalog/packages/core/src/context.ts.md#Context.getSupportedExtensions).

**Application.** The set is consumed in
[`getCodeFiles`](../catalog/packages/core/src/context.ts.md#Context.getCodeFiles) as a membership
test: `supportedExtensions.includes(path.extname(entry.name))`. Matching is exact and
case-sensitive on the raw extension string.

> [!inferred]
> Because the test is exact string membership on `path.extname`, an uppercase `.PY` or a
> compound-looking name is not normalized — only what the walker sees as the final `.ext` is checked.

## Why it matters / when it applies
This set decides which languages get semantically indexed. Users extend it without forking source:
per-request via MCP for one-off runs, or via `CUSTOM_EXTENSIONS` to persist across a server's
lifetime. An extension that is added but has no tree-sitter grammar still gets indexed — it simply
falls back to the LangChain character splitter (see the
[splitter contract](../concepts/packages-core-src-splitter-index.ts.md)) rather than AST chunking.

## Connections
- **Code concepts:** [Context orchestrator](../concepts/packages-core-src-context.ts.md) (assembles
  and applies the set); [splitter contract + fallback](../concepts/packages-core-src-splitter-index.ts.md)
  and [AST splitter](../concepts/packages-core-src-splitter-ast-splitter.ts.md) (a supported
  extension without a grammar is still chunked, via fallback).
- **Module catalogs:** [`context.ts`](../catalog/packages/core/src/context.ts.md).
- **Related doc-concepts:** [file inclusion rules](files-inclusion-rules.md) (the master equation) ·
  [ignore patterns](files-ignore-patterns.md) (the exclusion set subtracted from this one).

## Source
[`docs/dive-deep/file-inclusion-rules.md`](../../../../raw/code/claude-context/docs/dive-deep/file-inclusion-rules.md)
</content>
