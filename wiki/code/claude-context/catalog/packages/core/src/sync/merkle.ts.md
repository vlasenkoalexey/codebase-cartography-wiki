---
title: 'Module: packages/core/src/sync/merkle.ts'
type: catalog
provenance: extracted
module: packages/core/src/sync/merkle.ts
status: fresh
symbol_base: scip-typescript npm @zilliz/claude-context-core 0.1.15 src/sync/`merkle.ts`/MerkleDAG
symbols:
  MerkleDAG.addNode: '#addNode().'
  MerkleDAG.compare: '#compare().'
  MerkleDAG.nodes: '#nodes.'
  MerkleDAG.deserialize: '#deserialize().'
  MerkleDAG: '#'
  MerkleDAG.-constructor: '#`<constructor>`().'
  MerkleDAG.getRootNodes: '#getRootNodes().'
  MerkleDAG.getLeafNodes: '#getLeafNodes().'
  MerkleDAG.getAllNodes: '#getAllNodes().'
  MerkleDAGNode: Node#
  MerkleDAG.serialize: '#serialize().'
  MerkleDAG.rootIds: '#rootIds.'
  MerkleDAG.getNode: '#getNode().'
  MerkleDAGNode.id: Node#id.
  MerkleDAGNode.children: Node#children.
  MerkleDAGNode.parents: Node#parents.
  MerkleDAG.compare.typeLiteral23.added: '#compare().typeLiteral23:added.'
  MerkleDAG.compare.typeLiteral23.removed: '#compare().typeLiteral23:removed.'
  MerkleDAGNode.hash: Node#hash.
  MerkleDAGNode.data: Node#data.
  MerkleDAG.hash: '#hash().'
---
# Module: [`packages/core/src/sync/merkle.ts`](../../../../../../../../raw/code/claude-context/packages/core/src/sync/merkle.ts)

## Classes
### `MerkleDAG`
- def: [`packages/core/src/sync/merkle.ts:11`](../../../../../../../../raw/code/claude-context/packages/core/src/sync/merkle.ts#L11) — documented in [packages-core-src-sync-merkle.ts](../../../../../concepts/packages-core-src-sync-merkle.ts.md)
- signature: `class MerkleDAG`
- members:
  - `<constructor>()` — [`L15`](../../../../../../../../raw/code/claude-context/packages/core/src/sync/merkle.ts#L15)
  - `addNode(method)` — [`L24`](../../../../../../../../raw/code/claude-context/packages/core/src/sync/merkle.ts#L24) — documented in [packages-core-src-context.ts](../../../../../concepts/packages-core-src-context.ts.md)
  - `compare(method)` — [`L81`](../../../../../../../../raw/code/claude-context/packages/core/src/sync/merkle.ts#L81) — documented in [packages-core-src-sync-merkle.ts](../../../../../concepts/packages-core-src-sync-merkle.ts.md)
  - `deserialize(method)` — [`L74`](../../../../../../../../raw/code/claude-context/packages/core/src/sync/merkle.ts#L74) — documented in [packages-core-src-sync-merkle.ts](../../../../../concepts/packages-core-src-sync-merkle.ts.md)
  - `getAllNodes(method)` — [`L55`](../../../../../../../../raw/code/claude-context/packages/core/src/sync/merkle.ts#L55) — documented in [packages-core-src-sync-merkle.ts](../../../../../concepts/packages-core-src-sync-merkle.ts.md)
  - `getLeafNodes(method)` — [`L63`](../../../../../../../../raw/code/claude-context/packages/core/src/sync/merkle.ts#L63) — documented in [packages-core-src-sync-merkle.ts](../../../../../concepts/packages-core-src-sync-merkle.ts.md)
  - `getNode(method)` — [`L51`](../../../../../../../../raw/code/claude-context/packages/core/src/sync/merkle.ts#L51) — documented in [packages-core-src-sync-merkle.ts](../../../../../concepts/packages-core-src-sync-merkle.ts.md)
  - `getRootNodes(method)` — [`L59`](../../../../../../../../raw/code/claude-context/packages/core/src/sync/merkle.ts#L59) — documented in [packages-core-src-sync-merkle.ts](../../../../../concepts/packages-core-src-sync-merkle.ts.md)
  - `hash(method)` — [`L20`](../../../../../../../../raw/code/claude-context/packages/core/src/sync/merkle.ts#L20) — documented in [packages-core-src-sync-merkle.ts](../../../../../concepts/packages-core-src-sync-merkle.ts.md)
  - `serialize(method)` — [`L67`](../../../../../../../../raw/code/claude-context/packages/core/src/sync/merkle.ts#L67) — documented in [packages-core-src-sync-merkle.ts](../../../../../concepts/packages-core-src-sync-merkle.ts.md)
  - `added` — [`L81`](../../../../../../../../raw/code/claude-context/packages/core/src/sync/merkle.ts#L81) — documented in [packages-core-src-sync-merkle.ts](../../../../../concepts/packages-core-src-sync-merkle.ts.md)
  - `nodes` — [`L12`](../../../../../../../../raw/code/claude-context/packages/core/src/sync/merkle.ts#L12) — documented in [packages-core-src-sync-merkle.ts](../../../../../concepts/packages-core-src-sync-merkle.ts.md)
  - `removed` — [`L81`](../../../../../../../../raw/code/claude-context/packages/core/src/sync/merkle.ts#L81) — documented in [packages-core-src-sync-merkle.ts](../../../../../concepts/packages-core-src-sync-merkle.ts.md)
  - `rootIds` — [`L13`](../../../../../../../../raw/code/claude-context/packages/core/src/sync/merkle.ts#L13) — documented in [packages-core-src-sync-merkle.ts](../../../../../concepts/packages-core-src-sync-merkle.ts.md)
- uses (calls/refs, reference-scoped): [`MerkleDAGNode`](merkle.ts.md#MerkleDAGNode), [`children`](merkle.ts.md#MerkleDAGNode.children), [`id`](merkle.ts.md#MerkleDAGNode.id), [`parents`](merkle.ts.md#MerkleDAGNode.parents), [`data`](merkle.ts.md#MerkleDAGNode.data), [`hash`](merkle.ts.md#MerkleDAGNode.hash)
- used by: [`checkForChanges`](synchronizer.ts.md#FileSynchronizer.checkForChanges), [`<constructor>`](synchronizer.ts.md#FileSynchronizer.-constructor), [`loadSnapshot`](synchronizer.ts.md#FileSynchronizer.loadSnapshot), [`synchronizer.ts`](synchronizer.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-sync-synchronizer.ts), [`saveSnapshot`](synchronizer.ts.md#FileSynchronizer.saveSnapshot), [`buildMerkleDAG`](synchronizer.ts.md#FileSynchronizer.buildMerkleDAG), [`merkleDAG`](synchronizer.ts.md#FileSynchronizer.merkleDAG)

### `MerkleDAGNode`
- def: [`packages/core/src/sync/merkle.ts:3`](../../../../../../../../raw/code/claude-context/packages/core/src/sync/merkle.ts#L3) — documented in [packages-core-src-sync-merkle.ts](../../../../../concepts/packages-core-src-sync-merkle.ts.md)
- signature: `interface MerkleDAGNode`
- members:
  - `children` — [`L8`](../../../../../../../../raw/code/claude-context/packages/core/src/sync/merkle.ts#L8) — documented in [packages-core-src-sync-merkle.ts](../../../../../concepts/packages-core-src-sync-merkle.ts.md)
  - `data` — [`L6`](../../../../../../../../raw/code/claude-context/packages/core/src/sync/merkle.ts#L6) — documented in [packages-core-src-sync-merkle.ts](../../../../../concepts/packages-core-src-sync-merkle.ts.md)
  - `hash` — [`L5`](../../../../../../../../raw/code/claude-context/packages/core/src/sync/merkle.ts#L5) — documented in [packages-core-src-sync-merkle.ts](../../../../../concepts/packages-core-src-sync-merkle.ts.md)
  - `id` — [`L4`](../../../../../../../../raw/code/claude-context/packages/core/src/sync/merkle.ts#L4) — documented in [packages-core-src-sync-merkle.ts](../../../../../concepts/packages-core-src-sync-merkle.ts.md)
  - `parents` — [`L7`](../../../../../../../../raw/code/claude-context/packages/core/src/sync/merkle.ts#L7) — documented in [packages-core-src-sync-merkle.ts](../../../../../concepts/packages-core-src-sync-merkle.ts.md)
- used by: [`addNode`](merkle.ts.md#MerkleDAG.addNode), [`compare`](merkle.ts.md#MerkleDAG.compare), [`nodes`](merkle.ts.md#MerkleDAG.nodes), [`getLeafNodes`](merkle.ts.md#MerkleDAG.getLeafNodes), [`getRootNodes`](merkle.ts.md#MerkleDAG.getRootNodes), [`getAllNodes`](merkle.ts.md#MerkleDAG.getAllNodes), [`getNode`](merkle.ts.md#MerkleDAG.getNode)

