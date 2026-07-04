---
title: 'Module: src/agent/index.ts'
type: catalog
provenance: extracted
module: src/agent/index.ts
status: fresh
symbol_base: scip-typescript npm openwiki 0.0.1 src/agent/`index.ts`/
symbols:
  runOpenWikiAgentCore: runOpenWikiAgentCore().
  runOpenWikiAgent: runOpenWikiAgent().
  runOpenWikiAgentWithModelFallbacks: runOpenWikiAgentWithModelFallbacks().
  summarizeOpenRouterRequest: summarizeOpenRouterRequest().
  emitDebug: emitDebug().
  installOpenRouterDebugFetch: installOpenRouterDebugFetch().
  extractMessageTextValue: extractMessageTextValue().
  formatEnvironmentDebug: formatEnvironmentDebug().
  isRecord: isRecord().
  resolveModelId: resolveModelId().
  createModel: createModel().
  parseStreamEvent: parseStreamEvent().
  createRunUserMessage: createRunUserMessage().
  normalizeStreamEvent: normalizeStreamEvent().
  parseToolStreamEvent: parseToolStreamEvent().
  extractContentBlockText: extractContentBlockText().
  getStringRecordValue: getStringRecordValue().
  extractContentDeltaText: extractContentDeltaText().
  getMessageRole: getMessageRole().
  attachOpenRouterDebugInfo: attachOpenRouterDebugInfo().
  createOpenWikiThreadId: createOpenWikiThreadId().
  createCheckpointer: createCheckpointer().
  ensureProviderKey: ensureProviderKey().
  shouldRetryOpenRouterServerError: shouldRetryOpenRouterServerError().
  isMessageLikeRecord: isMessageLikeRecord().
  extractProtocolMessageText: extractProtocolMessageText().
  formatToolArgs: formatToolArgs().
  formatDebugValue: formatDebugValue().
  createModelRoute: createModelRoute().
  countMessageContentChars: countMessageContentChars().
  extractContentText: extractContentText().
  createAttemptOptions: createAttemptOptions().
  isStreamMessageTuplePayload: isStreamMessageTuplePayload().
  isOpenRouterFetchInput: isOpenRouterFetchInput().
  getOpenRouterMessageChars: getOpenRouterMessageChars().
  readResponseBodyPreview: readResponseBodyPreview().
  checkpointPath: checkpointPath.
  OpenRouterFetchCapture.typeLiteral25.getLastFailure: OpenRouterFetchCapture#typeLiteral25:getLastFailure.
  chmodIfExists: chmodIfExists().
  createSyntheticToolCallId: createSyntheticToolCallId().
  describeValueShape: describeValueShape().
  OpenRouterFetchFailure.typeLiteral47.response: OpenRouterFetchFailure#typeLiteral47:response.
  formatToolValue: formatToolValue().
  OpenRouterFetchFailure: OpenRouterFetchFailure#
  extractMessageText: extractMessageText().
  shouldReadMessageRecord: shouldReadMessageRecord().
  hasSerializedMessageId: hasSerializedMessageId().
  getProtocolEventPayload: getProtocolEventPayload().
  describeStreamChunkShape: describeStreamChunkShape().
  parseJsonRecord: parseJsonRecord().
  getOpenRouterToolNames: getOpenRouterToolNames().
  OpenRouterFetchFailure.typeLiteral47.request: OpenRouterFetchFailure#typeLiteral47:request.
  createThreadId: createThreadId().
  createRunThreadId: createRunThreadId().
  NormalizedStreamEvent.typeLiteral115.mode: NormalizedStreamEvent#typeLiteral115:mode.
  NormalizedStreamEvent.typeLiteral115.payload: NormalizedStreamEvent#typeLiteral115:payload.
  getSerializedMessageType: getSerializedMessageType().
  isMessageRole: isMessageRole().
  OpenRouterFetchCapture: OpenRouterFetchCapture#
  OpenRouterFetchCapture.typeLiteral25.clearLastFailure: OpenRouterFetchCapture#typeLiteral25:clearLastFailure.
  OpenRouterFetchCapture.typeLiteral25.restore: OpenRouterFetchCapture#typeLiteral25:restore.
  OpenRouterRequestSummary: OpenRouterRequestSummary#
  OpenRouterResponseSummary.typeLiteral48.status: OpenRouterResponseSummary#typeLiteral48:status.
  OPENROUTER_DEBUG_BODY_LIMIT: OPENROUTER_DEBUG_BODY_LIMIT.
  getFetchInputUrl: getFetchInputUrl().
  formatUrlDebugValue: formatUrlDebugValue().
  isFileNotFoundError: isFileNotFoundError().
  NormalizedStreamEvent: NormalizedStreamEvent#
  NormalizedStreamEvent.typeLiteral115.isSubgraph: NormalizedStreamEvent#typeLiteral115:isSubgraph.
  normalizeStreamChunk: normalizeStreamChunk().
  isSubgraphStreamChunk: isSubgraphStreamChunk().
  formatToolCallName: formatToolCallName().
  parseStringifiedJson: parseStringifiedJson().
  OpenRouterRequestSummary.typeLiteral253.bodyBytes: OpenRouterRequestSummary#typeLiteral253:bodyBytes.
  OpenRouterRequestSummary.typeLiteral253.messageChars: OpenRouterRequestSummary#typeLiteral253:messageChars.
  OpenRouterRequestSummary.typeLiteral253.messageCount: OpenRouterRequestSummary#typeLiteral253:messageCount.
  OpenRouterRequestSummary.typeLiteral253.method: OpenRouterRequestSummary#typeLiteral253:method.
  OpenRouterRequestSummary.typeLiteral253.model: OpenRouterRequestSummary#typeLiteral253:model.
  OpenRouterRequestSummary.typeLiteral253.stream: OpenRouterRequestSummary#typeLiteral253:stream.
  OpenRouterRequestSummary.typeLiteral253.toolCount: OpenRouterRequestSummary#typeLiteral253:toolCount.
  OpenRouterRequestSummary.typeLiteral253.toolNames: OpenRouterRequestSummary#typeLiteral253:toolNames.
  OpenRouterRequestSummary.typeLiteral253.url: OpenRouterRequestSummary#typeLiteral253:url.
  OpenRouterResponseSummary: OpenRouterResponseSummary#
  OPENROUTER_DEBUG_PROPERTY: OPENROUTER_DEBUG_PROPERTY.
  sanitizeOpenRouterResponseBody: sanitizeOpenRouterResponseBody().
  getSafeResponseHeaders: getSafeResponseHeaders().
  formatOpenRouterDebugUrl: formatOpenRouterDebugUrl().
  OpenRouterFetchFailure.typeLiteral47.fetchError: OpenRouterFetchFailure#typeLiteral47:fetchError.
  OpenRouterResponseSummary.typeLiteral48.bodyPreview: OpenRouterResponseSummary#typeLiteral48:bodyPreview.
  OpenRouterResponseSummary.typeLiteral48.headers: OpenRouterResponseSummary#typeLiteral48:headers.
  OpenRouterResponseSummary.typeLiteral48.statusText: OpenRouterResponseSummary#typeLiteral48:statusText.
---
# Module: [`src/agent/index.ts`](../../../../../../raw/code/openwiki/src/agent/index.ts)

## Classes
### `NormalizedStreamEvent`
- def: [`src/agent/index.ts:439`](../../../../../../raw/code/openwiki/src/agent/index.ts#L439)
- signature: `type NormalizedStreamEvent`
- members:
  - `isSubgraph` — [`L440`](../../../../../../raw/code/openwiki/src/agent/index.ts#L440)
  - `mode` — [`L441`](../../../../../../raw/code/openwiki/src/agent/index.ts#L441)
  - `payload` — [`L442`](../../../../../../raw/code/openwiki/src/agent/index.ts#L442)
- used by: [`parseStreamEvent`](index.ts.md#parseStreamEvent), [`normalizeStreamEvent`](index.ts.md#normalizeStreamEvent)

### `OpenRouterFetchCapture`
- def: [`src/agent/index.ts:993`](../../../../../../raw/code/openwiki/src/agent/index.ts#L993)
- signature: `type OpenRouterFetchCapture`
- members:
  - `clearLastFailure` — [`L994`](../../../../../../raw/code/openwiki/src/agent/index.ts#L994)
  - `getLastFailure` — [`L995`](../../../../../../raw/code/openwiki/src/agent/index.ts#L995)
  - `restore` — [`L996`](../../../../../../raw/code/openwiki/src/agent/index.ts#L996)
- uses (calls/refs, reference-scoped): [`OpenRouterFetchFailure`](index.ts.md#OpenRouterFetchFailure)
- used by: [`runOpenWikiAgent`](index.ts.md#runOpenWikiAgent), [`runOpenWikiAgentWithModelFallbacks`](index.ts.md#runOpenWikiAgentWithModelFallbacks), [`installOpenRouterDebugFetch`](index.ts.md#installOpenRouterDebugFetch)

### `OpenRouterFetchFailure`
- def: [`src/agent/index.ts:999`](../../../../../../raw/code/openwiki/src/agent/index.ts#L999)
- signature: `type OpenRouterFetchFailure`
- members:
  - `fetchError` — [`L1000`](../../../../../../raw/code/openwiki/src/agent/index.ts#L1000)
  - `request` — [`L1001`](../../../../../../raw/code/openwiki/src/agent/index.ts#L1001)
  - `response` — [`L1002`](../../../../../../raw/code/openwiki/src/agent/index.ts#L1002)
- uses (calls/refs, reference-scoped): [`OpenRouterRequestSummary`](index.ts.md#OpenRouterRequestSummary), [`OpenRouterResponseSummary`](index.ts.md#OpenRouterResponseSummary)
- used by: [`runOpenWikiAgentWithModelFallbacks`](index.ts.md#runOpenWikiAgentWithModelFallbacks), [`installOpenRouterDebugFetch`](index.ts.md#installOpenRouterDebugFetch), [`attachOpenRouterDebugInfo`](index.ts.md#attachOpenRouterDebugInfo), [`shouldRetryOpenRouterServerError`](index.ts.md#shouldRetryOpenRouterServerError), [`getLastFailure`](index.ts.md#OpenRouterFetchCapture.typeLiteral25.getLastFailure)

### `OpenRouterRequestSummary`
- def: [`src/agent/index.ts:1005`](../../../../../../raw/code/openwiki/src/agent/index.ts#L1005)
- signature: `type OpenRouterRequestSummary`
- members:
  - `bodyBytes` — [`L1006`](../../../../../../raw/code/openwiki/src/agent/index.ts#L1006)
  - `messageChars` — [`L1007`](../../../../../../raw/code/openwiki/src/agent/index.ts#L1007)
  - `messageCount` — [`L1008`](../../../../../../raw/code/openwiki/src/agent/index.ts#L1008)
  - `method` — [`L1009`](../../../../../../raw/code/openwiki/src/agent/index.ts#L1009)
  - `model` — [`L1010`](../../../../../../raw/code/openwiki/src/agent/index.ts#L1010)
  - `stream` — [`L1011`](../../../../../../raw/code/openwiki/src/agent/index.ts#L1011)
  - `toolCount` — [`L1012`](../../../../../../raw/code/openwiki/src/agent/index.ts#L1012)
  - `toolNames` — [`L1013`](../../../../../../raw/code/openwiki/src/agent/index.ts#L1013)
  - `url` — [`L1014`](../../../../../../raw/code/openwiki/src/agent/index.ts#L1014)
- used by: [`summarizeOpenRouterRequest`](index.ts.md#summarizeOpenRouterRequest), [`request`](index.ts.md#OpenRouterFetchFailure.typeLiteral47.request)

### `OpenRouterResponseSummary`
- def: [`src/agent/index.ts:1017`](../../../../../../raw/code/openwiki/src/agent/index.ts#L1017)
- signature: `type OpenRouterResponseSummary`
- members:
  - `bodyPreview` — [`L1018`](../../../../../../raw/code/openwiki/src/agent/index.ts#L1018)
  - `headers` — [`L1019`](../../../../../../raw/code/openwiki/src/agent/index.ts#L1019)
  - `status` — [`L1020`](../../../../../../raw/code/openwiki/src/agent/index.ts#L1020)
  - `statusText` — [`L1021`](../../../../../../raw/code/openwiki/src/agent/index.ts#L1021)
- used by: [`runOpenWikiAgentWithModelFallbacks`](index.ts.md#runOpenWikiAgentWithModelFallbacks), [`shouldRetryOpenRouterServerError`](index.ts.md#shouldRetryOpenRouterServerError), [`response`](index.ts.md#OpenRouterFetchFailure.typeLiteral47.response)

## Functions
- `attachOpenRouterDebugInfo(error: unknown, failure: OpenRouterFetchFailure | null)` — [`L1082`](../../../../../../raw/code/openwiki/src/agent/index.ts#L1082) — documented in [openwiki-agent-index.ts](../../../concepts/openwiki-agent-index.ts.md)
- `chmodIfExists(filePath: string, mode: number)` — [`L306`](../../../../../../raw/code/openwiki/src/agent/index.ts#L306)
- `countMessageContentChars(content: unknown)` — [`L1183`](../../../../../../raw/code/openwiki/src/agent/index.ts#L1183)
- `createAttemptOptions(options: OpenWikiRunOptions, attemptIndex: number)` — [`L252`](../../../../../../raw/code/openwiki/src/agent/index.ts#L252)
- `createCheckpointer()` — [`L296`](../../../../../../raw/code/openwiki/src/agent/index.ts#L296) — documented in [openwiki-agent-index.ts](../../../concepts/openwiki-agent-index.ts.md)
- `createModel(provider: OpenWikiProvider, modelId: string)` — [`L380`](../../../../../../raw/code/openwiki/src/agent/index.ts#L380) — documented in [openwiki-agent-index.ts](../../../concepts/openwiki-agent-index.ts.md)
- `createModelRoute(provider: OpenWikiProvider, modelId: string)` — [`L413`](../../../../../../raw/code/openwiki/src/agent/index.ts#L413) — documented in [openwiki-agent-index.ts](../../../concepts/openwiki-agent-index.ts.md)
- `createOpenWikiThreadId(cwd?: any)` — [`L316`](../../../../../../raw/code/openwiki/src/agent/index.ts#L316)
- `createRunThreadId()` — [`L326`](../../../../../../raw/code/openwiki/src/agent/index.ts#L326)
- `createRunUserMessage(command: OpenWikiCommand, cwd: string, context: RunContext, options: OpenWikiRunOptions)` — [`L270`](../../../../../../raw/code/openwiki/src/agent/index.ts#L270) — documented in [openwiki-agent-index.ts](../../../concepts/openwiki-agent-index.ts.md)
- `createSyntheticToolCallId(name: string, input: unknown)` — [`L952`](../../../../../../raw/code/openwiki/src/agent/index.ts#L952)
- `createThreadId(cwd: string, runId: string)` — [`L320`](../../../../../../raw/code/openwiki/src/agent/index.ts#L320)
- `describeStreamChunkShape(chunk: unknown)` — [`L967`](../../../../../../raw/code/openwiki/src/agent/index.ts#L967)
- `describeValueShape(value: unknown)` — [`L978`](../../../../../../raw/code/openwiki/src/agent/index.ts#L978)
- `emitDebug(options: OpenWikiRunOptions, message: string)` — [`L332`](../../../../../../raw/code/openwiki/src/agent/index.ts#L332) — documented in [openwiki-agent-types.ts](../../../concepts/openwiki-agent-types.ts.md)
- `ensureProviderKey(provider: OpenWikiProvider)` — [`L351`](../../../../../../raw/code/openwiki/src/agent/index.ts#L351) — documented in [openwiki-agent-index.ts](../../../concepts/openwiki-agent-index.ts.md)
- `extractContentBlockText(block: unknown, seen: Set<object>)` — [`L729`](../../../../../../raw/code/openwiki/src/agent/index.ts#L729)
- `extractContentDeltaText(delta: unknown, seen: Set<object>)` — [`L699`](../../../../../../raw/code/openwiki/src/agent/index.ts#L699)
- `extractContentText(content: unknown, seen: Set<object>)` — [`L681`](../../../../../../raw/code/openwiki/src/agent/index.ts#L681)
- `extractMessageText(payload: unknown)` — [`L531`](../../../../../../raw/code/openwiki/src/agent/index.ts#L531)
- `extractMessageTextValue(payload: unknown, seen: Set<object>)` — [`L535`](../../../../../../raw/code/openwiki/src/agent/index.ts#L535) — documented in [openwiki-agent-index.ts](../../../concepts/openwiki-agent-index.ts.md)
- `extractProtocolMessageText(payload: Record<string, unknown>, seen: Set<object>)` — [`L651`](../../../../../../raw/code/openwiki/src/agent/index.ts#L651)
- `formatDebugValue(key: string, value: string | undefined)` — [`L1278`](../../../../../../raw/code/openwiki/src/agent/index.ts#L1278)
- `formatEnvironmentDebug()` — [`L1259`](../../../../../../raw/code/openwiki/src/agent/index.ts#L1259)
- `formatOpenRouterDebugUrl(value: string)` — [`L1244`](../../../../../../raw/code/openwiki/src/agent/index.ts#L1244)
- `formatToolArgs(input: unknown)` — [`L912`](../../../../../../raw/code/openwiki/src/agent/index.ts#L912)
- `formatToolCallName(name: string)` — [`L908`](../../../../../../raw/code/openwiki/src/agent/index.ts#L908)
- `formatToolValue(value: unknown)` — [`L932`](../../../../../../raw/code/openwiki/src/agent/index.ts#L932)
- `formatUrlDebugValue(value: string)` — [`L1304`](../../../../../../raw/code/openwiki/src/agent/index.ts#L1304)
- `getFetchInputUrl(input: any)` — [`L1103`](../../../../../../raw/code/openwiki/src/agent/index.ts#L1103)
- `getMessageRole(value: Record<string, unknown>)` — [`L769`](../../../../../../raw/code/openwiki/src/agent/index.ts#L769)
- `getOpenRouterMessageChars(messages: unknown)` — [`L1169`](../../../../../../raw/code/openwiki/src/agent/index.ts#L1169)
- `getOpenRouterToolNames(tools: unknown)` — [`L1153`](../../../../../../raw/code/openwiki/src/agent/index.ts#L1153)
- `getProtocolEventPayload(event: Record<string, unknown>)` — [`L835`](../../../../../../raw/code/openwiki/src/agent/index.ts#L835)
- `getSafeResponseHeaders(headers: Headers)` — [`L1230`](../../../../../../raw/code/openwiki/src/agent/index.ts#L1230)
- `getSerializedMessageType(value: Record<string, unknown>)` — [`L811`](../../../../../../raw/code/openwiki/src/agent/index.ts#L811)
- `getStringRecordValue(value: Record<string, unknown>, key: string)` — [`L956`](../../../../../../raw/code/openwiki/src/agent/index.ts#L956)
- `hasSerializedMessageId(value: Record<string, unknown>)` — [`L807`](../../../../../../raw/code/openwiki/src/agent/index.ts#L807)
- `installOpenRouterDebugFetch(options: OpenWikiRunOptions)` — [`L1027`](../../../../../../raw/code/openwiki/src/agent/index.ts#L1027) — documented in [openwiki-agent-index.ts](../../../concepts/openwiki-agent-index.ts.md)
- `isFileNotFoundError(error: unknown)` — [`L343`](../../../../../../raw/code/openwiki/src/agent/index.ts#L343)
- `isMessageLikeRecord(value: unknown)` — [`L635`](../../../../../../raw/code/openwiki/src/agent/index.ts#L635)
- `isMessageRole(value: unknown)` — [`L825`](../../../../../../raw/code/openwiki/src/agent/index.ts#L825)
- `isOpenRouterFetchInput(input: any)` — [`L1093`](../../../../../../raw/code/openwiki/src/agent/index.ts#L1093)
- `isRecord(value: unknown)` — [`L963`](../../../../../../raw/code/openwiki/src/agent/index.ts#L963)
- `isStreamMessageTuplePayload(payload: unknown[])` — [`L612`](../../../../../../raw/code/openwiki/src/agent/index.ts#L612)
- `isSubgraphStreamChunk(chunk: unknown[])` — [`L523`](../../../../../../raw/code/openwiki/src/agent/index.ts#L523)
- `normalizeStreamChunk(chunk: unknown[])` — [`L515`](../../../../../../raw/code/openwiki/src/agent/index.ts#L515)
- `normalizeStreamEvent(chunk: unknown)` — [`L471`](../../../../../../raw/code/openwiki/src/agent/index.ts#L471) — documented in [openwiki-agent-index.ts](../../../concepts/openwiki-agent-index.ts.md)
- `parseJsonRecord(value: string | null)` — [`L1139`](../../../../../../raw/code/openwiki/src/agent/index.ts#L1139)
- `parseStreamEvent(chunk: unknown)` — [`L445`](../../../../../../raw/code/openwiki/src/agent/index.ts#L445) — documented in [openwiki-agent-index.ts](../../../concepts/openwiki-agent-index.ts.md)
- `parseStringifiedJson(value: unknown)` — [`L940`](../../../../../../raw/code/openwiki/src/agent/index.ts#L940)
- `parseToolStreamEvent(payload: unknown)` — [`L853`](../../../../../../raw/code/openwiki/src/agent/index.ts#L853) — documented in [openwiki-agent-index.ts](../../../concepts/openwiki-agent-index.ts.md)
- `readResponseBodyPreview(response: Response)` — [`L1208`](../../../../../../raw/code/openwiki/src/agent/index.ts#L1208)
- `resolveModelId(options: OpenWikiRunOptions, provider: OpenWikiProvider)` — [`L361`](../../../../../../raw/code/openwiki/src/agent/index.ts#L361) — documented in [openwiki-agent-index.ts](../../../concepts/openwiki-agent-index.ts.md)
- `runOpenWikiAgent(command: OpenWikiCommand, cwd?: any, options?: OpenWikiRunOptions)` — [`L42`](../../../../../../raw/code/openwiki/src/agent/index.ts#L42) — documented in [openwiki-agent-index.ts](../../../concepts/openwiki-agent-index.ts.md)
- `runOpenWikiAgentCore(command: OpenWikiCommand, cwd: string, options: OpenWikiRunOptions, provider: OpenWikiProvider, modelId: string)` — [`L153`](../../../../../../raw/code/openwiki/src/agent/index.ts#L153) — documented in [openwiki-agent-index.ts](../../../concepts/openwiki-agent-index.ts.md)
- `runOpenWikiAgentWithModelFallbacks(command: OpenWikiCommand, cwd: string, options: OpenWikiRunOptions, provider: OpenWikiProvider, modelId: string, debugFetchCapture: OpenRouterFetchCapture)` — [`L92`](../../../../../../raw/code/openwiki/src/agent/index.ts#L92) — documented in [openwiki-agent-index.ts](../../../concepts/openwiki-agent-index.ts.md)
- `sanitizeOpenRouterResponseBody(body: string)` — [`L1223`](../../../../../../raw/code/openwiki/src/agent/index.ts#L1223)
- `shouldReadMessageRecord(value: Record<string, unknown>)` — [`L763`](../../../../../../raw/code/openwiki/src/agent/index.ts#L763)
- `shouldRetryOpenRouterServerError(failure: OpenRouterFetchFailure | null, attemptIndex: number, attemptCount: number)` — [`L424`](../../../../../../raw/code/openwiki/src/agent/index.ts#L424) — documented in [openwiki-agent-index.ts](../../../concepts/openwiki-agent-index.ts.md)
- `summarizeOpenRouterRequest(input: any, init: any)` — [`L1115`](../../../../../../raw/code/openwiki/src/agent/index.ts#L1115) — documented in [openwiki-agent-index.ts](../../../concepts/openwiki-agent-index.ts.md)

## Module values
- `OPENROUTER_DEBUG_BODY_LIMIT` — [`L1025`](../../../../../../raw/code/openwiki/src/agent/index.ts#L1025)
- `OPENROUTER_DEBUG_PROPERTY` — [`L1024`](../../../../../../raw/code/openwiki/src/agent/index.ts#L1024)
- `checkpointPath` — [`L268`](../../../../../../raw/code/openwiki/src/agent/index.ts#L268)

