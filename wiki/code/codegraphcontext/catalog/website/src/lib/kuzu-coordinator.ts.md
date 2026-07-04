---
title: 'Module: website/src/lib/kuzu-coordinator.ts'
type: catalog
provenance: extracted
module: website/src/lib/kuzu-coordinator.ts
status: fresh
symbol_base: scip-typescript npm vite_react_shadcn_ts 0.0.0 src/lib/`kuzu-coordinator.ts`/
symbols:
  KuzuCoordinator.start: KuzuCoordinator#start().
  KuzuCoordinator.stop: KuzuCoordinator#stop().
  KuzuCoordinator.-constructor: KuzuCoordinator#`<constructor>`().
  KuzuCoordinator.maybeReconnectAfterVisibility: KuzuCoordinator#maybeReconnectAfterVisibility().
  KuzuCoordinator.handleVisibilityChange: KuzuCoordinator#handleVisibilityChange.
  KuzuCoordinator.channel: KuzuCoordinator#channel.
  KuzuCoordinator.visibilityDebounceTimer: KuzuCoordinator#visibilityDebounceTimer.
  KuzuCoordinator.isTunnelHealthy: KuzuCoordinator#isTunnelHealthy().
  KuzuCoordinator.channelName: KuzuCoordinator#channelName.
  KuzuCoordinator.keepaliveInterval: KuzuCoordinator#keepaliveInterval.
  KuzuCoordinator.setupChannelListeners: KuzuCoordinator#setupChannelListeners().
  KuzuCoordinator.isStarted: KuzuCoordinator#isStarted.
  KuzuCoordinator.executeQueryCallback: KuzuCoordinator#executeQueryCallback.
  KuzuCoordinator.executeToolCallback: KuzuCoordinator#executeToolCallback.
  KuzuCoordinator.getToolsCallback: KuzuCoordinator#getToolsCallback.
  KuzuCoordinator.isReconnecting: KuzuCoordinator#isReconnecting.
  QueryExecutionCallback: QueryExecutionCallback#
  ToolsListCallback: ToolsListCallback#
  ToolCallCallback: ToolCallCallback#
  VISIBILITY_RECONNECT_DEBOUNCE_MS: VISIBILITY_RECONNECT_DEBOUNCE_MS.
  isChannelJoined: isChannelJoined().
  KuzuCoordinator: KuzuCoordinator#
---
# Module: [`website/src/lib/kuzu-coordinator.ts`](../../../../../../../raw/code/codegraphcontext/website/src/lib/kuzu-coordinator.ts)

## Classes
### `KuzuCoordinator`
- def: [`website/src/lib/kuzu-coordinator.ts:21`](../../../../../../../raw/code/codegraphcontext/website/src/lib/kuzu-coordinator.ts#L21)
- signature: `class KuzuCoordinator`
- members:
  - `<constructor>(_supabaseUrl: string, _supabaseAnonKey: string, channelName: string, executeQueryCallback: QueryExecutionCallback, getToolsCallback: ToolsListCallback, executeToolCallback: ToolCallCallback)` — [`L34`](../../../../../../../raw/code/codegraphcontext/website/src/lib/kuzu-coordinator.ts#L34)
  - `isTunnelHealthy(method)` — [`L48`](../../../../../../../raw/code/codegraphcontext/website/src/lib/kuzu-coordinator.ts#L48)
  - `maybeReconnectAfterVisibility(method)` — [`L65`](../../../../../../../raw/code/codegraphcontext/website/src/lib/kuzu-coordinator.ts#L65)
  - `setupChannelListeners(method)` — [`L126`](../../../../../../../raw/code/codegraphcontext/website/src/lib/kuzu-coordinator.ts#L126)
  - `start(method)` — [`L85`](../../../../../../../raw/code/codegraphcontext/website/src/lib/kuzu-coordinator.ts#L85) — Subscribes to the real-time signaling channel and listens for queries/MCP events.
  - `stop(method)` — [`L188`](../../../../../../../raw/code/codegraphcontext/website/src/lib/kuzu-coordinator.ts#L188)
  - `channel` — [`L23`](../../../../../../../raw/code/codegraphcontext/website/src/lib/kuzu-coordinator.ts#L23)
  - `channelName` — [`L22`](../../../../../../../raw/code/codegraphcontext/website/src/lib/kuzu-coordinator.ts#L22)
  - `executeQueryCallback` — [`L25`](../../../../../../../raw/code/codegraphcontext/website/src/lib/kuzu-coordinator.ts#L25)
  - `executeToolCallback` — [`L27`](../../../../../../../raw/code/codegraphcontext/website/src/lib/kuzu-coordinator.ts#L27)
  - `getToolsCallback` — [`L26`](../../../../../../../raw/code/codegraphcontext/website/src/lib/kuzu-coordinator.ts#L26)
  - `handleVisibilityChange` — [`L52`](../../../../../../../raw/code/codegraphcontext/website/src/lib/kuzu-coordinator.ts#L52)
  - `isReconnecting` — [`L30`](../../../../../../../raw/code/codegraphcontext/website/src/lib/kuzu-coordinator.ts#L30)
  - `isStarted` — [`L29`](../../../../../../../raw/code/codegraphcontext/website/src/lib/kuzu-coordinator.ts#L29)
  - `keepaliveInterval` — [`L32`](../../../../../../../raw/code/codegraphcontext/website/src/lib/kuzu-coordinator.ts#L32)
  - `visibilityDebounceTimer` — [`L31`](../../../../../../../raw/code/codegraphcontext/website/src/lib/kuzu-coordinator.ts#L31)
- uses (calls/refs, reference-scoped): [`getSupabaseClient`](supabase-client.ts.md#getSupabaseClient), [`QueryExecutionCallback`](kuzu-coordinator.ts.md#QueryExecutionCallback), [`ToolCallCallback`](kuzu-coordinator.ts.md#ToolCallCallback), [`ToolsListCallback`](kuzu-coordinator.ts.md#ToolsListCallback), [`VISIBILITY_RECONNECT_DEBOUNCE_MS`](kuzu-coordinator.ts.md#VISIBILITY_RECONNECT_DEBOUNCE_MS), [`isChannelJoined`](kuzu-coordinator.ts.md#isChannelJoined)
- used by: [`Explore`](../pages/Explore.tsx.md#Explore), [`Explore.tsx`](../pages/Explore.tsx.md#scip-typescript-npm-vite_react_shadcn_ts-0.0.0-src-pages-Explore.tsx)

### `QueryExecutionCallback`
- def: [`website/src/lib/kuzu-coordinator.ts:5`](../../../../../../../raw/code/codegraphcontext/website/src/lib/kuzu-coordinator.ts#L5)
- signature: `type QueryExecutionCallback`
- used by: [`<constructor>`](kuzu-coordinator.ts.md#KuzuCoordinator.-constructor), [`executeQueryCallback`](kuzu-coordinator.ts.md#KuzuCoordinator.executeQueryCallback)

### `ToolCallCallback`
- def: [`website/src/lib/kuzu-coordinator.ts:13`](../../../../../../../raw/code/codegraphcontext/website/src/lib/kuzu-coordinator.ts#L13)
- signature: `type ToolCallCallback`
- used by: [`<constructor>`](kuzu-coordinator.ts.md#KuzuCoordinator.-constructor), [`executeToolCallback`](kuzu-coordinator.ts.md#KuzuCoordinator.executeToolCallback)

### `ToolsListCallback`
- def: [`website/src/lib/kuzu-coordinator.ts:11`](../../../../../../../raw/code/codegraphcontext/website/src/lib/kuzu-coordinator.ts#L11)
- signature: `type ToolsListCallback`
- used by: [`<constructor>`](kuzu-coordinator.ts.md#KuzuCoordinator.-constructor), [`getToolsCallback`](kuzu-coordinator.ts.md#KuzuCoordinator.getToolsCallback)

## Functions
- `isChannelJoined(channel: any)` — [`L17`](../../../../../../../raw/code/codegraphcontext/website/src/lib/kuzu-coordinator.ts#L17)

## Module values
- `VISIBILITY_RECONNECT_DEBOUNCE_MS` — [`L15`](../../../../../../../raw/code/codegraphcontext/website/src/lib/kuzu-coordinator.ts#L15)

