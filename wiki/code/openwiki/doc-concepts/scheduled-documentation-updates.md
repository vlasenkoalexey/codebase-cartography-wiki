---
title: Scheduled documentation updates
type: doc-concept
provenance: doc
source: README.md
updated: 2026-07-04
status: fresh
---
# Scheduled documentation updates

## Definition
The README's recommended way to keep docs current is automation: add a GitHub Action
(`examples/openwiki-update.yml`) that "automatically open[s] a PR once a day with documentation updates." So
the intended steady state is not a human periodically running `openwiki --update`, but a scheduled job that
runs the update mode non-interactively and proposes the diff as a pull request.

## In openwiki (grounded)
A scheduled run is a non-interactive `update`: it needs a provider API key in the environment (the workflow
supplies one), and it exercises the print/non-interactive path rather than the Ink UI. The update itself is
[`runOpenWikiAgent`](../catalog/src/agent/index.ts.md#runOpenWikiAgent) in `update` mode, which diffs from the
`gitHead` recorded in the prior run's metadata (read by [`readLastUpdate`](../catalog/src/agent/utils.ts.md#readLastUpdate))
and re-serialized into the prompt by [`formatLastUpdate`](../catalog/src/agent/prompt.ts.md#formatLastUpdate).
Because a no-relevant-change run is a deliberate no-op (no metadata write when the content hash is unchanged),
a daily job on a quiet repo produces an empty PR-worthy diff rather than churn.

## Why it matters / when it applies
This is the operational payoff of the git-anchored reconcile: the update is cheap and bounded (only changed
files feed the model), and idempotent enough to run on a schedule. It applies to any repo that wants
always-current agent-readable docs without manual upkeep — the same "maintenance is near-zero-cost" thesis
this survey's host wiki is built on, implemented here as a cron-driven agent.

## Connections
- Code concepts: [Agent runtime](../concepts/openwiki-agent-index.ts.md);
  [TUI orchestration](../concepts/openwiki-cli.tsx.md) (the print/non-interactive entry path).
- Module catalogs: [src/agent/index.ts](../catalog/src/agent/index.ts.md),
  [src/agent/utils.ts](../catalog/src/agent/utils.ts.md).
- Related doc-concepts: [Documentation lifecycle](documentation-lifecycle.md).

## Source
Extracted from `README.md` (kept in place).
