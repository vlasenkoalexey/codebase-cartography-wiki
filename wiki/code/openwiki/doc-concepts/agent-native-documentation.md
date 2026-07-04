---
title: Agent-native documentation
type: doc-concept
provenance: doc
source: README.md
updated: 2026-07-04
status: fresh
---
# Agent-native documentation

## Definition
OpenWiki's stated purpose is "a CLI that writes and maintains documentation for your codebase, **built
specifically for agents**." The docs it produces (under `openwiki/`) are meant to be read first by a future
coding agent so it can make changes "with less source exploration" — not just by humans. The corollary is
that OpenWiki actively wires itself into the target repo's agent-instruction files so those agents know the
wiki exists.

## In openwiki (grounded)
The whole product is one agent run: [`runOpenWikiAgent`](../catalog/src/agent/index.ts.md#runOpenWikiAgent)
builds a `deepagents` agent that reads the repo and writes Markdown into
[`OPEN_WIKI_DIR`](../catalog/src/constants.ts.md#OPEN_WIKI_DIR) (`openwiki/`). The "for agents" framing is
enforced by the system prompt, [`createSystemPrompt`](../catalog/src/agent/prompt.ts.md#createSystemPrompt),
whose "Documentation goals" and "Root agent instruction files" sections instruct the model to (a) write docs
a future agent can act on and (b) add an OpenWiki reference section to the repo's top-level `AGENTS.md` /
`CLAUDE.md` (the exact block this repo's own `AGENTS.md` carries). Grounding is a *prompt directive* — "ground
every important claim in source files, existing docs, or git evidence you have inspected" — with no separate
verification pass.

## Why it matters / when it applies
This is the design choice that places OpenWiki at the "agent-native, prompt-grounded" pole of the survey:
there is no code index, symbol graph, or citation linter; the model *is* the analyzer and the prompt *is* the
contract. That buys language-agnosticism and human-shaped organization ("like human documentation, not a raw
file inventory") at the cost of mechanical verifiability.

## Connections
- Code concepts: [Agent runtime](../concepts/openwiki-agent-index.ts.md) — the run that produces the docs;
  [Run contract](../concepts/openwiki-agent-types.ts.md) — the three modes.
- Module catalogs: [src/agent/index.ts](../catalog/src/agent/index.ts.md),
  [src/agent/prompt.ts](../catalog/src/agent/prompt.ts.md).
- Related doc-concepts: [Documentation lifecycle](documentation-lifecycle.md),
  [Scheduled documentation updates](scheduled-documentation-updates.md).

## Source
Extracted from `README.md` (kept in place).
