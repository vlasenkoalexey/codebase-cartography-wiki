---
title: 'Module: src/agent/prompt.ts'
type: catalog
provenance: extracted
module: src/agent/prompt.ts
status: fresh
symbol_base: scip-typescript npm openwiki 0.0.1 src/agent/`prompt.ts`/
symbols:
  createUserPrompt: createUserPrompt().
  createSystemPrompt: createSystemPrompt().
  createModeInstructions: createModeInstructions().
  formatLastUpdate: formatLastUpdate().
  appendUserMessage: appendUserMessage().
---
# Module: [`src/agent/prompt.ts`](../../../../../../raw/code/openwiki/src/agent/prompt.ts)

## Functions
- `appendUserMessage(prompt: string, userMessage: string | null)` — [`L219`](../../../../../../raw/code/openwiki/src/agent/prompt.ts#L219)
- `createModeInstructions(command: OpenWikiCommand)` — [`L134`](../../../../../../raw/code/openwiki/src/agent/prompt.ts#L134) — documented in [openwiki-agent-types.ts](../../../concepts/openwiki-agent-types.ts.md)
- `createSystemPrompt(command: OpenWikiCommand)` — [`L12`](../../../../../../raw/code/openwiki/src/agent/prompt.ts#L12) — documented in [openwiki-agent-index.ts](../../../concepts/openwiki-agent-index.ts.md)
- `createUserPrompt(command: OpenWikiCommand, context: RunContext, userMessage?: string | null)` — [`L178`](../../../../../../raw/code/openwiki/src/agent/prompt.ts#L178) — documented in [openwiki-agent-index.ts](../../../concepts/openwiki-agent-index.ts.md)
- `formatLastUpdate(lastUpdate: UpdateMetadata | null)` — [`L4`](../../../../../../raw/code/openwiki/src/agent/prompt.ts#L4) — documented in [openwiki-agent-types.ts](../../../concepts/openwiki-agent-types.ts.md)

