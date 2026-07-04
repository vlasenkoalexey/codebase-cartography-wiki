---
title: 'Module: src/agent/types.ts'
type: catalog
provenance: extracted
module: src/agent/types.ts
status: fresh
symbol_base: scip-typescript npm openwiki 0.0.1 src/agent/`types.ts`/
symbols:
  OpenWikiCommand: OpenWikiCommand#
  OpenWikiRunEvent: OpenWikiRunEvent#
  OpenWikiRunOptions: OpenWikiRunOptions#
  UpdateMetadata: UpdateMetadata#
  OpenWikiRunResult: OpenWikiRunResult#
  UpdateMetadata.typeLiteral23.updatedAt: UpdateMetadata#typeLiteral23:updatedAt.
  UpdateMetadata.typeLiteral23.gitHead: UpdateMetadata#typeLiteral23:gitHead.
  UpdateMetadata.typeLiteral23.command: UpdateMetadata#typeLiteral23:command.
  OpenWikiRunOptions.typeLiteral20.onEvent: OpenWikiRunOptions#typeLiteral20:onEvent.
  OpenWikiRunOptions.typeLiteral20.threadId: OpenWikiRunOptions#typeLiteral20:threadId.
  OpenWikiRunOptions.typeLiteral20.userMessage: OpenWikiRunOptions#typeLiteral20:userMessage.
  RunContext: RunContext#
  OpenWikiRunResult.typeLiteral0.command: OpenWikiRunResult#typeLiteral0:command.
  RunContext.typeLiteral24.lastUpdate: RunContext#typeLiteral24:lastUpdate.
  UpdateMetadata.typeLiteral23.model: UpdateMetadata#typeLiteral23:model.
  OpenWikiRunOptions.typeLiteral20.debug: OpenWikiRunOptions#typeLiteral20:debug.
  OpenWikiRunOptions.typeLiteral20.isFollowup: OpenWikiRunOptions#typeLiteral20:isFollowup.
  RunContext.typeLiteral24.gitSummary: RunContext#typeLiteral24:gitSummary.
  OpenWikiRunResult.typeLiteral0.model: OpenWikiRunResult#typeLiteral0:model.
  OpenWikiRunOptions.typeLiteral20.modelId: OpenWikiRunOptions#typeLiteral20:modelId.
---
# Module: [`src/agent/types.ts`](../../../../../../raw/code/openwiki/src/agent/types.ts)

## Classes
### `OpenWikiCommand`
- def: [`src/agent/types.ts:1`](../../../../../../raw/code/openwiki/src/agent/types.ts#L1) — documented in [openwiki-agent-types.ts](../../../concepts/openwiki-agent-types.ts.md)
- signature: `type OpenWikiCommand`
- used by: [`App`](../cli.tsx.md#App), [`cli.tsx`](../cli.tsx.md#scip-typescript-npm-openwiki-0.0.1-src-cli.tsx), [`index.ts`](index.ts.md#scip-typescript-npm-openwiki-0.0.1-src-agent-index.ts), [`runOpenWikiAgentCore`](index.ts.md#runOpenWikiAgentCore), [`runOpenWikiAgent`](index.ts.md#runOpenWikiAgent), [`runOpenWikiAgentWithModelFallbacks`](index.ts.md#runOpenWikiAgentWithModelFallbacks), [`createUserPrompt`](prompt.ts.md#createUserPrompt), [`writeLastUpdateMetadata`](utils.ts.md#writeLastUpdateMetadata), [`createGitSummary`](utils.ts.md#createGitSummary), [`prompt.ts`](prompt.ts.md#scip-typescript-npm-openwiki-0.0.1-src-agent-prompt.ts), [`utils.ts`](utils.ts.md#scip-typescript-npm-openwiki-0.0.1-src-agent-utils.ts), [`RunState`](../cli.tsx.md#RunState), [`createRunUserMessage`](index.ts.md#createRunUserMessage), [`parseCommand`](../commands.ts.md#parseCommand), [`commands.ts`](../commands.ts.md#scip-typescript-npm-openwiki-0.0.1-src-commands.ts), [`createRunContext`](utils.ts.md#createRunContext), [`CliCommand`](../commands.ts.md#CliCommand), [`createSystemPrompt`](prompt.ts.md#createSystemPrompt), [`createModeInstructions`](prompt.ts.md#createModeInstructions), [`command`](../cli.tsx.md#RunViewProps.typeLiteral229.command), [`command`](types.ts.md#UpdateMetadata.typeLiteral23.command), [`onCommandRun`](../cli.tsx.md#ChatInputProps.typeLiteral236.onCommandRun), [`command`](../cli.tsx.md#DryRunView.-command-modelId-shouldStart-userMessage-.typeLiteral209.command), [`command`](../cli.tsx.md#CompletedRun.typeLiteral35.command), [`command`](types.ts.md#OpenWikiRunResult.typeLiteral0.command)

### `OpenWikiRunEvent`
- def: [`src/agent/types.ts:8`](../../../../../../raw/code/openwiki/src/agent/types.ts#L8) — documented in [openwiki-agent-types.ts](../../../concepts/openwiki-agent-types.ts.md)
- signature: `type OpenWikiRunEvent`
- used by: [`cli.tsx`](../cli.tsx.md#scip-typescript-npm-openwiki-0.0.1-src-cli.tsx), [`index.ts`](index.ts.md#scip-typescript-npm-openwiki-0.0.1-src-agent-index.ts), [`createToolDisplay`](../cli.tsx.md#createToolDisplay), [`appendRunLogEvent`](../cli.tsx.md#appendRunLogEvent), [`parseStreamEvent`](index.ts.md#parseStreamEvent), [`parseToolStreamEvent`](index.ts.md#parseToolStreamEvent), [`appendToolStartLogItem`](../cli.tsx.md#appendToolStartLogItem), [`completeToolGroupItem`](../cli.tsx.md#completeToolGroupItem), [`completeToolLogItem`](../cli.tsx.md#completeToolLogItem), [`onEvent`](types.ts.md#OpenWikiRunOptions.typeLiteral20.onEvent)

### `OpenWikiRunOptions`
- def: [`src/agent/types.ts:32`](../../../../../../raw/code/openwiki/src/agent/types.ts#L32) — documented in [openwiki-agent-types.ts](../../../concepts/openwiki-agent-types.ts.md)
- signature: `type OpenWikiRunOptions`
- members:
  - `debug` — [`L33`](../../../../../../raw/code/openwiki/src/agent/types.ts#L33)
  - `isFollowup` — [`L34`](../../../../../../raw/code/openwiki/src/agent/types.ts#L34)
  - `modelId` — [`L35`](../../../../../../raw/code/openwiki/src/agent/types.ts#L35)
  - `onEvent` — [`L36`](../../../../../../raw/code/openwiki/src/agent/types.ts#L36) — documented in [openwiki-agent-types.ts](../../../concepts/openwiki-agent-types.ts.md)
  - `threadId` — [`L37`](../../../../../../raw/code/openwiki/src/agent/types.ts#L37)
  - `userMessage` — [`L38`](../../../../../../raw/code/openwiki/src/agent/types.ts#L38)
- uses (calls/refs, reference-scoped): [`OpenWikiRunEvent`](types.ts.md#OpenWikiRunEvent)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-openwiki-0.0.1-src-agent-index.ts), [`runOpenWikiAgentCore`](index.ts.md#runOpenWikiAgentCore), [`runOpenWikiAgent`](index.ts.md#runOpenWikiAgent), [`runOpenWikiAgentWithModelFallbacks`](index.ts.md#runOpenWikiAgentWithModelFallbacks), [`emitDebug`](index.ts.md#emitDebug), [`installOpenRouterDebugFetch`](index.ts.md#installOpenRouterDebugFetch), [`resolveModelId`](index.ts.md#resolveModelId), [`createRunUserMessage`](index.ts.md#createRunUserMessage), [`createAttemptOptions`](index.ts.md#createAttemptOptions)

### `OpenWikiRunResult`
- def: [`src/agent/types.ts:3`](../../../../../../raw/code/openwiki/src/agent/types.ts#L3)
- signature: `type OpenWikiRunResult`
- members:
  - `command` — [`L4`](../../../../../../raw/code/openwiki/src/agent/types.ts#L4) — documented in [openwiki-agent-types.ts](../../../concepts/openwiki-agent-types.ts.md)
  - `model` — [`L5`](../../../../../../raw/code/openwiki/src/agent/types.ts#L5)
- uses (calls/refs, reference-scoped): [`OpenWikiCommand`](types.ts.md#OpenWikiCommand)
- used by: [`App`](../cli.tsx.md#App), [`cli.tsx`](../cli.tsx.md#scip-typescript-npm-openwiki-0.0.1-src-cli.tsx), [`index.ts`](index.ts.md#scip-typescript-npm-openwiki-0.0.1-src-agent-index.ts), [`runOpenWikiAgentCore`](index.ts.md#runOpenWikiAgentCore), [`runOpenWikiAgent`](index.ts.md#runOpenWikiAgent), [`runOpenWikiAgentWithModelFallbacks`](index.ts.md#runOpenWikiAgentWithModelFallbacks), [`ChatHistory`](../cli.tsx.md#ChatHistory), [`RunState`](../cli.tsx.md#RunState), [`result`](../cli.tsx.md#CompletedRun.typeLiteral35.result)

### `RunContext`
- def: [`src/agent/types.ts:48`](../../../../../../raw/code/openwiki/src/agent/types.ts#L48)
- signature: `type RunContext`
- members:
  - `gitSummary` — [`L50`](../../../../../../raw/code/openwiki/src/agent/types.ts#L50)
  - `lastUpdate` — [`L49`](../../../../../../raw/code/openwiki/src/agent/types.ts#L49) — documented in [openwiki-agent-types.ts](../../../concepts/openwiki-agent-types.ts.md)
- uses (calls/refs, reference-scoped): [`UpdateMetadata`](types.ts.md#UpdateMetadata)
- used by: [`createUserPrompt`](prompt.ts.md#createUserPrompt), [`prompt.ts`](prompt.ts.md#scip-typescript-npm-openwiki-0.0.1-src-agent-prompt.ts), [`utils.ts`](utils.ts.md#scip-typescript-npm-openwiki-0.0.1-src-agent-utils.ts), [`createRunContext`](utils.ts.md#createRunContext)

### `UpdateMetadata`
- def: [`src/agent/types.ts:41`](../../../../../../raw/code/openwiki/src/agent/types.ts#L41) — documented in [openwiki-agent-types.ts](../../../concepts/openwiki-agent-types.ts.md)
- signature: `type UpdateMetadata`
- members:
  - `command` — [`L43`](../../../../../../raw/code/openwiki/src/agent/types.ts#L43) — documented in [openwiki-agent-types.ts](../../../concepts/openwiki-agent-types.ts.md)
  - `gitHead` — [`L44`](../../../../../../raw/code/openwiki/src/agent/types.ts#L44)
  - `model` — [`L45`](../../../../../../raw/code/openwiki/src/agent/types.ts#L45)
  - `updatedAt` — [`L42`](../../../../../../raw/code/openwiki/src/agent/types.ts#L42)
- uses (calls/refs, reference-scoped): [`OpenWikiCommand`](types.ts.md#OpenWikiCommand)
- used by: [`writeLastUpdateMetadata`](utils.ts.md#writeLastUpdateMetadata), [`createGitSummary`](utils.ts.md#createGitSummary), [`prompt.ts`](prompt.ts.md#scip-typescript-npm-openwiki-0.0.1-src-agent-prompt.ts), [`readLastUpdate`](utils.ts.md#readLastUpdate), [`utils.ts`](utils.ts.md#scip-typescript-npm-openwiki-0.0.1-src-agent-utils.ts), [`formatLastUpdate`](prompt.ts.md#formatLastUpdate), [`lastUpdate`](types.ts.md#RunContext.typeLiteral24.lastUpdate)

