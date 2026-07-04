---
title: 'Module: src/mcp/query-worker.ts'
type: catalog
provenance: extracted
module: src/mcp/query-worker.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/mcp/`query-worker.ts`/
symbols:
  errorResult: errorResult().
  loadToolHandler: loadToolHandler.
  loadCodeGraph: loadCodeGraph.
  CallMessage.id: CallMessage#id.
  CallMessage: CallMessage#
  CallMessage.toolName: CallMessage#toolName.
  WorkerInit: WorkerInit#
  WorkerInit.root: WorkerInit#root.
  CallMessage.type: CallMessage#type.
  CallMessage.args: CallMessage#args.
---
# Module: [`src/mcp/query-worker.ts`](../../../../../../raw/code/codegraph/src/mcp/query-worker.ts)

## Classes
### `CallMessage`
- def: [`src/mcp/query-worker.ts:31`](../../../../../../raw/code/codegraph/src/mcp/query-worker.ts#L31)
- signature: `interface CallMessage`
- members:
  - `args` — [`L35`](../../../../../../raw/code/codegraph/src/mcp/query-worker.ts#L35)
  - `id` — [`L33`](../../../../../../raw/code/codegraph/src/mcp/query-worker.ts#L33)
  - `toolName` — [`L34`](../../../../../../raw/code/codegraph/src/mcp/query-worker.ts#L34)
  - `type` — [`L32`](../../../../../../raw/code/codegraph/src/mcp/query-worker.ts#L32)
- used by: [`query-worker.ts`](query-worker.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-mcp-query-worker.ts)

### `WorkerInit`
- def: [`src/mcp/query-worker.ts:27`](../../../../../../raw/code/codegraph/src/mcp/query-worker.ts#L27)
- signature: `interface WorkerInit`
- members:
  - `root` — [`L28`](../../../../../../raw/code/codegraph/src/mcp/query-worker.ts#L28)
- used by: [`query-worker.ts`](query-worker.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-mcp-query-worker.ts)

## Functions
- `errorResult(text: string)` — [`L101`](../../../../../../raw/code/codegraph/src/mcp/query-worker.ts#L101)

## Module values
- `loadCodeGraph` — [`L40`](../../../../../../raw/code/codegraph/src/mcp/query-worker.ts#L40)
- `loadToolHandler` — [`L42`](../../../../../../raw/code/codegraph/src/mcp/query-worker.ts#L42)

