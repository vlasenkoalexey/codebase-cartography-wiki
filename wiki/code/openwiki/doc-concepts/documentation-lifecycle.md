---
title: Documentation lifecycle — init, update, chat
type: doc-concept
provenance: doc
source: README.md
updated: 2026-07-04
status: fresh
---
# Documentation lifecycle — init, update, chat

## Definition
The README describes OpenWiki's core behavior in one rule: "`openwiki` creates initial documentation in
`openwiki/` when no wiki exists. If `openwiki/` already exists, it refreshes that documentation from
repository changes." That is the two-mode lifecycle — **init** (build from scratch) and **update** (surgical,
diff-driven refresh) — plus an interactive **chat** mode. The CLI also stays open after each run for follow-up
messages unless `-p/--print` is used for a one-shot non-interactive run.

## In openwiki (grounded)
The three modes are the [`OpenWikiCommand`](../catalog/src/agent/types.ts.md#OpenWikiCommand) union
(`chat | init | update`), and each selects different prompt behavior via
[`createModeInstructions`](../catalog/src/agent/prompt.ts.md#createModeInstructions): init "builds the
documentation structure from scratch" (≤8 pages), update is "a maintenance update run" that must be
"surgical" and "may be a no-op," and chat answers without writing docs. The README's "refreshes from
repository changes" is implemented as the git-anchored incremental reconcile — the update prompt is fed a
`git log <lastHead>..HEAD` summary built in [`createGitSummary`](../catalog/src/agent/utils.ts.md#createGitSummary),
and the run only records new metadata (via [`writeLastUpdateMetadata`](../catalog/src/agent/utils.ts.md#writeLastUpdateMetadata))
when a content-hash snapshot proves the docs actually changed.

## Why it matters / when it applies
The init/update split is what makes the wiki *maintainable* rather than a one-shot generation: update runs
diff against the last successful run's `gitHead` (stored in `openwiki/.last-update.json`) and touch only the
pages implicated by the changed source. Because the surgical discipline lives in the prompt, not in a build
gate, the model is trusted to keep edits minimal.

## Connections
- Code concepts: [Agent runtime](../concepts/openwiki-agent-index.ts.md) (Incremental reconcile section);
  [Run contract](../concepts/openwiki-agent-types.ts.md).
- Cross-repo: [`incremental-reconcile`](../../../concepts/incremental-reconcile.md).
- Module catalogs: [src/agent/prompt.ts](../catalog/src/agent/prompt.ts.md),
  [src/agent/utils.ts](../catalog/src/agent/utils.ts.md).
- Related doc-concepts: [Agent-native documentation](agent-native-documentation.md),
  [Scheduled documentation updates](scheduled-documentation-updates.md).

## Source
Extracted from `README.md` (kept in place).
