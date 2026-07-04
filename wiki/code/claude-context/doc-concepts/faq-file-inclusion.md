---
title: What gets embedded — extensions minus ignore patterns
type: doc-concept
provenance: doc
source: docs/troubleshooting/faq.md
updated: 2026-07-04
status: fresh
---
# What gets embedded — extensions minus ignore patterns

## Definition
The FAQ states the file-selection rule as a one-liner: `Final Files = (All Supported Extensions) - (All
Ignore Patterns)`. Both sides of the subtraction are **additive** — the effective extension set is
*default extensions + MCP custom + environment variables*, and the effective ignore set is *default
patterns + MCP custom + environment variables + `.gitignore` + `.xxxignore` files + a global
`.contextignore`. A file is embedded only if its extension is in the (unioned) allow-set **and** its
path is not caught by any (unioned) ignore rule.

## In claude-context (grounded)
The subtraction is implemented on the [`Context`](../concepts/packages-core-src-context.ts.md)
orchestrator. The "supported extensions" side starts from
[`DEFAULT_SUPPORTED_EXTENSIONS`](../catalog/packages/core/src/context.ts.md#DEFAULT_SUPPORTED_EXTENSIONS)
and is widened by env-supplied extensions
([`getCustomExtensionsFromEnv`](../catalog/packages/core/src/context.ts.md#Context.getCustomExtensionsFromEnv))
and per-request MCP custom extensions
([`addCustomExtensions`](../catalog/packages/core/src/context.ts.md#Context.addCustomExtensions)),
resolved to one effective set by
[`getEffectiveSupportedExtensions`](../catalog/packages/core/src/context.ts.md#Context.getEffectiveSupportedExtensions).
The "ignore patterns" side starts from
[`DEFAULT_IGNORE_PATTERNS`](../catalog/packages/core/src/context.ts.md#DEFAULT_IGNORE_PATTERNS) and is
grown by env patterns
([`getCustomIgnorePatternsFromEnv`](../catalog/packages/core/src/context.ts.md#Context.getCustomIgnorePatternsFromEnv)),
per-request patterns
([`addCustomIgnorePatterns`](../catalog/packages/core/src/context.ts.md#Context.addCustomIgnorePatterns)),
and on-disk ignore files loaded by
[`loadIgnorePatterns`](../catalog/packages/core/src/context.ts.md#Context.loadIgnorePatterns) and the
global-file loader
[`loadGlobalIgnoreFile`](../catalog/packages/core/src/context.ts.md#Context.loadGlobalIgnoreFile),
merged by
[`getEffectiveIgnorePatterns`](../catalog/packages/core/src/context.ts.md#Context.getEffectiveIgnorePatterns).
The two sides meet in
[`getCodeFiles`](../catalog/packages/core/src/context.ts.md#Context.getCodeFiles), which walks the tree,
keeps files whose extension is supported, and drops those matched by the
[`IgnoreMatcher.ignores`](../catalog/packages/core/src/utils/ignore-matcher.ts.md#IgnoreMatcher.ignores)
predicate (a gitignore-semantics matcher). The MCP request surface for the custom inputs is
[`CodebaseIndexOptions.requestCustomExtensions`](../catalog/packages/mcp/src/config.ts.md#CodebaseIndexOptions.requestCustomExtensions)
and
[`CodebaseIndexOptions.requestIgnorePatterns`](../catalog/packages/mcp/src/config.ts.md#CodebaseIndexOptions.requestIgnorePatterns).

## Why it matters / when it applies
This rule is the front gate of the whole pipeline: a file that fails it is never chunked, never
embedded, and never searchable — so "why isn't my file showing up in search?" almost always resolves
here (wrong extension, or caught by an ignore rule) rather than in the vector store. Because both sets
are **additive unions**, adding a custom extension can only widen coverage and adding an ignore pattern
can only narrow it; there is no subtractive override that re-includes an ignored path. Understanding the
gate also explains index size and cost: shrinking the ignore set or widening extensions directly
increases the number of chunks embedded and stored.

## Connections
- Code concepts: [Context orchestrator](../concepts/packages-core-src-context.ts.md) — owns the
  extension/ignore resolution and the file walk; [MCP config resolution](../concepts/packages-mcp-src-config.ts.md)
  — where the request-level extensions/patterns arrive.
- Module catalogs: [context.ts](../catalog/packages/core/src/context.ts.md) ·
  [ignore-matcher.ts](../catalog/packages/core/src/utils/ignore-matcher.ts.md) ·
  [config.ts](../catalog/packages/mcp/src/config.ts.md)
- Related doc-concepts: [faq-codebase-path-keying](faq-codebase-path-keying.md) ·
  [faq-indexing-status](faq-indexing-status.md)

## Source
Extracted from `docs/troubleshooting/faq.md` (kept in place).
