---
title: Ignore patterns — the additive exclusion set
type: doc-concept
provenance: doc
source: raw/code/claude-context/docs/dive-deep/file-inclusion-rules.md
updated: 2026-07-04
status: fresh
---
# Ignore patterns — the additive exclusion set

## Definition
The **exclusion** half of the [file-inclusion rule](files-inclusion-rules.md): a glob-pattern set
subtracted from the supported-extension set. Unlike the extension set, ignores come from **six
additive sources**, spanning both in-memory config and on-disk files:

1. **Default ignore patterns** — built-in globs for build output, IDE files, VCS dirs, caches, logs,
   env/secret files, and minified bundles.
2. **MCP custom ignore patterns** — per-request patterns via the MCP `ignorePatterns` parameter.
3. **Environment-variable patterns** — comma-separated `CUSTOM_IGNORE_PATTERNS`.
4. **`.gitignore`** — standard Git ignore file in the codebase root.
5. **`.xxxignore` files** — any dot-file in the root whose name ends in `ignore` (`.cursorignore`,
   `.codeiumignore`, `.contextignore`, …).
6. **Global `.contextignore`** — user-wide patterns at `~/.context/.contextignore`.

## In claude-context (grounded)
**Defaults + config + env (the base set).** The
[constructor](../catalog/packages/core/src/context.ts.md#Context.-constructor) unions
[`DEFAULT_IGNORE_PATTERNS`](../catalog/packages/core/src/context.ts.md#DEFAULT_IGNORE_PATTERNS) with
[`ContextConfig.ignorePatterns`](../catalog/packages/core/src/context.ts.md#ContextConfig.ignorePatterns),
[`ContextConfig.customIgnorePatterns`](../catalog/packages/core/src/context.ts.md#ContextConfig.customIgnorePatterns),
and the env value parsed by
[`getCustomIgnorePatternsFromEnv`](../catalog/packages/core/src/context.ts.md#Context.getCustomIgnorePatternsFromEnv)
(comma-split, trimmed, empties dropped), de-duplicating via
[`dedupePatterns`](../catalog/packages/core/src/context.ts.md#Context.dedupePatterns) into
[`Context.baseIgnorePatterns`](../catalog/packages/core/src/context.ts.md#Context.baseIgnorePatterns).
`DEFAULT_IGNORE_PATTERNS` includes `node_modules/**`, `dist/**`, `build/**`, `.git/**`,
`__pycache__/**`, `*.log`, `.env`, `.env.*`, `*.min.js`, `*.map`, and bare-directory-name variants.

**On-disk ignore files (the per-codebase set).**
[`loadIgnorePatterns`](../catalog/packages/core/src/context.ts.md#Context.loadIgnorePatterns) is run
per codebase and layers file-based patterns on top of `baseIgnorePatterns` plus any per-request
patterns, then re-dedups. It gathers file patterns from:
- [`findIgnoreFiles`](../catalog/packages/core/src/context.ts.md#Context.findIgnoreFiles) — reads the
  codebase root and returns every entry that **starts with `.` and ends with `ignore`**. This single
  rule is what makes `.gitignore`, `.cursorignore`, `.codeiumignore`, and `.contextignore` all
  first-class — there is no hard-coded list of ignore-file names.
- [`loadGlobalIgnoreFile`](../catalog/packages/core/src/context.ts.md#Context.loadGlobalIgnoreFile) —
  loads `~/.context/.contextignore` (via `os.homedir()`); silently returns `[]` if absent.

Each file is parsed by
[`loadIgnoreFile`](../catalog/packages/core/src/context.ts.md#Context.loadIgnoreFile) →
[`getIgnorePatternsFromFile`](../catalog/packages/core/src/context.ts.md#Context.getIgnorePatternsFromFile),
which splits on newlines, trims, and **drops blank lines and `#` comments**. On any read error
`loadIgnorePatterns` falls back to `baseIgnorePatterns + request patterns` — file-based patterns from
a *previous* codebase are never allowed to leak forward.

**Application.** The merged pattern list is handed to an
[`IgnoreMatcher`](../catalog/packages/core/src/utils/ignore-matcher.ts.md#IgnoreMatcher) inside
[`getCodeFiles`](../catalog/packages/core/src/context.ts.md#Context.getCodeFiles);
[`IgnoreMatcher.ignores`](../catalog/packages/core/src/utils/ignore-matcher.ts.md#IgnoreMatcher.ignores)
tests each relative path (with an `isDirectory` flag) and matched directories are never descended.

> [!inferred]
> The doc lists `.gitignore` and `.xxxignore` as separate sources, but the code treats them
> uniformly: `.gitignore` is simply the `.xxxignore` entry named `.gitignore`. Its patterns are read
> verbatim as globs and de-duped with the rest — there is no separate Git-semantics parser, so
> gitignore features like negation (`!`) or nested `.gitignore` files below the root are not given
> special handling here.

## Why it matters / when it applies
Ignores are the guardrail that keeps the index clean and fast: they exclude dependency trees, build
artifacts, minified bundles, and — importantly — `.env` secrets, so credentials are not embedded and
made searchable. Because a matched directory prunes the whole subtree, tuning ignores is the primary
speed lever on large monorepos. The six-source design lets a pattern be set globally (env / global
`.contextignore`), per-repo (`.gitignore` / `.contextignore` in root), or per-request (MCP
`ignorePatterns`) without editing claude-context itself.

## Connections
- **Code concepts:** [Context orchestrator](../concepts/packages-core-src-context.ts.md) (loads and
  applies patterns); [FileSynchronizer](../concepts/packages-core-src-sync-synchronizer.ts.md) (uses
  the same `IgnoreMatcher` so incremental sync sees the identical file set).
- **Module catalogs:** [`context.ts`](../catalog/packages/core/src/context.ts.md) ·
  [`ignore-matcher.ts`](../catalog/packages/core/src/utils/ignore-matcher.ts.md).
- **Related doc-concepts:** [file inclusion rules](files-inclusion-rules.md) (the master equation) ·
  [supported extensions](files-supported-extensions.md) (the inclusion set this is subtracted from).

## Source
[`docs/dive-deep/file-inclusion-rules.md`](../../../../raw/code/claude-context/docs/dive-deep/file-inclusion-rules.md)
</content>
