---
title: Development mode & dry runs
type: doc-concept
provenance: doc
source: DEVELOPMENT.md
updated: 2026-07-04
status: fresh
---
# Development mode & dry runs

## Definition
`DEVELOPMENT.md` documents how to run OpenWiki against another local repo while hacking on it: build and
`pnpm link --global` the package, then from a target repo run `OPENWIKI_DEV=1 openwiki --dry-run` for a dry
test or `openwiki` for a real run. The target repo stays the current working directory; the global link only
saves typing the path to `dist/cli.js`.

## In openwiki (grounded)
The `OPENWIKI_DEV=1` (or `NODE_ENV=development`) switch is read by
[`isDevelopmentMode`](../catalog/src/commands.ts.md#isDevelopmentMode), which is what *unlocks* the `--dry-run`
flag in [`parseCommand`](../catalog/src/commands.ts.md#parseCommand) — outside development the flag is rejected
as unknown — and what adds the development section to the help text
([`getHelpText`](../catalog/src/commands.ts.md#getHelpText)). A dry run resolves the command but never invokes
the agent; the TUI renders a summary instead (the `DryRunView` path in the Ink app). Running against a target
repo works because the agent's filesystem tools are rooted at the current working directory via the
virtual-root shell backend set up in [`runOpenWikiAgentCore`](../catalog/src/agent/index.ts.md#runOpenWikiAgentCore).

## Why it matters / when it applies
This is purely a contributor affordance: `--dry-run` lets you see what a run *would* do (command, model,
whether it would start) without spending tokens or touching files, and the dev-gate keeps that affordance out
of the published CLI's surface. The "run against another repo" instructions are the practical consequence of
OpenWiki always treating `process.cwd()` as the project under documentation.

## Connections
- Code concepts: [CLI command parsing](../concepts/openwiki-commands.ts.md);
  [TUI orchestration](../concepts/openwiki-cli.tsx.md); [Agent runtime](../concepts/openwiki-agent-index.ts.md).
- Module catalogs: [src/commands.ts](../catalog/src/commands.ts.md), [src/cli.tsx](../catalog/src/cli.tsx.md).
- Related doc-concepts: [Documentation lifecycle](documentation-lifecycle.md).

## Source
Extracted from `DEVELOPMENT.md` (kept in place).
