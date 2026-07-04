---
title: 'Module: src/db/queries.ts'
type: catalog
provenance: extracted
module: src/db/queries.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/db/`queries.ts`/
symbols:
  rowToNode: rowToNode().
  QueryBuilder.searchNodes: QueryBuilder#searchNodes().
  QueryBuilder.stmts: QueryBuilder#stmts.
  QueryBuilder.db: QueryBuilder#db.
  QueryBuilder.insertNode: QueryBuilder#insertNode().
  QueryBuilder.updateNode: QueryBuilder#updateNode().
  QueryBuilder.getNodeById: QueryBuilder#getNodeById().
  rowToFileRecord: rowToFileRecord().
  rowToEdge: rowToEdge().
  QueryBuilder.getOutgoingEdges: QueryBuilder#getOutgoingEdges().
  QueryBuilder.getUnresolvedReferencesBatch: QueryBuilder#getUnresolvedReferencesBatch().
  QueryBuilder: QueryBuilder#
  QueryBuilder.getUnresolvedByName: QueryBuilder#getUnresolvedByName().
  QueryBuilder.getUnresolvedReferencesByFiles: QueryBuilder#getUnresolvedReferencesByFiles().
  QueryBuilder.getUnresolvedReferences: QueryBuilder#getUnresolvedReferences().
  QueryBuilder.getStats: QueryBuilder#getStats().
  QueryBuilder.getNodesByKind: QueryBuilder#getNodesByKind().
  QueryBuilder.getIncomingEdges: QueryBuilder#getIncomingEdges().
  QueryBuilder.getNodesByIds: QueryBuilder#getNodesByIds().
  QueryBuilder.searchNodesFuzzy: QueryBuilder#searchNodesFuzzy().
  QueryBuilder.findNodesByExactName: QueryBuilder#findNodesByExactName().
  QueryBuilder.upsertFile: QueryBuilder#upsertFile().
  QueryBuilder.insertUnresolvedRef: QueryBuilder#insertUnresolvedRef().
  QueryBuilder.insertEdge: QueryBuilder#insertEdge().
  QueryBuilder.searchNodesFTS: QueryBuilder#searchNodesFTS().
  QueryBuilder.searchNodesLike: QueryBuilder#searchNodesLike().
  QueryBuilder.iterateNodesByKind: QueryBuilder#iterateNodesByKind().
  QueryBuilder.findNodesByNameSubstring: QueryBuilder#findNodesByNameSubstring().
  QueryBuilder.insertEdges: QueryBuilder#insertEdges().
  QueryBuilder.getAllFiles: QueryBuilder#getAllFiles().
  QueryBuilder.insertNameSegments: QueryBuilder#insertNameSegments().
  QueryBuilder.getNodesByName: QueryBuilder#getNodesByName().
  QueryBuilder.getFileByPath: QueryBuilder#getFileByPath().
  QueryBuilder.searchAllByFilters: QueryBuilder#searchAllByFilters().
  QueryBuilder.getNodesByFile: QueryBuilder#getNodesByFile().
  QueryBuilder.getNodesByQualifiedNameExact: QueryBuilder#getNodesByQualifiedNameExact().
  QueryBuilder.getNodesByLowerName: QueryBuilder#getNodesByLowerName().
  QueryBuilder.nodeCache: QueryBuilder#nodeCache.
  QueryBuilder.deleteSpecificResolvedReferences: QueryBuilder#deleteSpecificResolvedReferences().
  QueryBuilder.deleteFile: QueryBuilder#deleteFile().
  QueryBuilder.deleteNodesByFile: QueryBuilder#deleteNodesByFile().
  QueryBuilder.findEdgesBetweenNodes: QueryBuilder#findEdgesBetweenNodes().
  QueryBuilder.getCrossFileIncomingEdgesWithTarget: QueryBuilder#getCrossFileIncomingEdgesWithTarget().
  NodeRow: NodeRow#
  QueryBuilder.getUnresolvedReferencesCount: QueryBuilder#getUnresolvedReferencesCount().
  QueryBuilder.getDominantFile: QueryBuilder#getDominantFile().
  QueryBuilder.getTopRouteFile: QueryBuilder#getTopRouteFile().
  QueryBuilder.getRoutingManifest: QueryBuilder#getRoutingManifest().
  QueryBuilder.getAllNodes: QueryBuilder#getAllNodes().
  QueryBuilder.deleteNode: QueryBuilder#deleteNode().
  QueryBuilder.getAllFilePaths: QueryBuilder#getAllFilePaths().
  QueryBuilder.getAllNodeNames: QueryBuilder#getAllNodeNames().
  QueryBuilder.getSegmentCoOccurrence.Array.typeLiteral34.matches: QueryBuilder#getSegmentCoOccurrence().Array:typeLiteral34:matches.
  QueryBuilder.deleteEdgesBySource: QueryBuilder#deleteEdgesBySource().
  QueryBuilder.deleteUnresolvedByNode: QueryBuilder#deleteUnresolvedByNode().
  QueryBuilder.cacheNode: QueryBuilder#cacheNode().
  QueryBuilder.getNodeAndEdgeCount: QueryBuilder#getNodeAndEdgeCount().
  QueryBuilder.-constructor: QueryBuilder#`<constructor>`().
  QueryBuilder.insertNodes: QueryBuilder#insertNodes().
  QueryBuilder.getExistingNodeIds: QueryBuilder#getExistingNodeIds().
  QueryBuilder.insertUnresolvedRefsBatch: QueryBuilder#insertUnresolvedRefsBatch().
  QueryBuilder.clear: QueryBuilder#clear().
  QueryBuilder.isNameSegmentVocabEmpty: QueryBuilder#isNameSegmentVocabEmpty().
  QueryBuilder.getStaleFiles: QueryBuilder#getStaleFiles().
  QueryBuilder.deleteResolvedReferences: QueryBuilder#deleteResolvedReferences().
  QueryBuilder.getLastIndexedAt: QueryBuilder#getLastIndexedAt().
  QueryBuilder.getMetadata: QueryBuilder#getMetadata().
  QueryBuilder.setMetadata: QueryBuilder#setMetadata().
  QueryBuilder.clearNameSegmentVocab: QueryBuilder#clearNameSegmentVocab().
  QueryBuilder.getDistinctNodeNames: QueryBuilder#getDistinctNodeNames().
  QueryBuilder.insertNameSegmentsBatch: QueryBuilder#insertNameSegmentsBatch().
  QueryBuilder.getSegmentNameCounts: QueryBuilder#getSegmentNameCounts().
  QueryBuilder.getNamesForSegment: QueryBuilder#getNamesForSegment().
  QueryBuilder.getDependentFilePaths: QueryBuilder#getDependentFilePaths().
  QueryBuilder.getDependencyFilePaths: QueryBuilder#getDependencyFilePaths().
  SQLITE_PARAM_CHUNK_SIZE: SQLITE_PARAM_CHUNK_SIZE.
  UnresolvedRefRow.candidates: UnresolvedRefRow#candidates.
  QueryBuilder.getAllMetadata: QueryBuilder#getAllMetadata().
  EdgeRow: EdgeRow#
  isLowValueFile: isLowValueFile().
  QueryBuilder.stmts.typeLiteral3.insertNode: QueryBuilder#stmts.typeLiteral3:insertNode.
  QueryBuilder.stmts.typeLiteral3.updateNode: QueryBuilder#stmts.typeLiteral3:updateNode.
  QueryBuilder.stmts.typeLiteral3.deleteNode: QueryBuilder#stmts.typeLiteral3:deleteNode.
  QueryBuilder.stmts.typeLiteral3.deleteNodesByFile: QueryBuilder#stmts.typeLiteral3:deleteNodesByFile.
  QueryBuilder.stmts.typeLiteral3.getNodeById: QueryBuilder#stmts.typeLiteral3:getNodeById.
  QueryBuilder.stmts.typeLiteral3.getNodesByFile: QueryBuilder#stmts.typeLiteral3:getNodesByFile.
  QueryBuilder.stmts.typeLiteral3.getNodesByKind: QueryBuilder#stmts.typeLiteral3:getNodesByKind.
  QueryBuilder.stmts.typeLiteral3.insertEdge: QueryBuilder#stmts.typeLiteral3:insertEdge.
  QueryBuilder.stmts.typeLiteral3.upsertFile: QueryBuilder#stmts.typeLiteral3:upsertFile.
  QueryBuilder.stmts.typeLiteral3.deleteEdgesBySource: QueryBuilder#stmts.typeLiteral3:deleteEdgesBySource.
  QueryBuilder.stmts.typeLiteral3.getEdgesBySource: QueryBuilder#stmts.typeLiteral3:getEdgesBySource.
  QueryBuilder.stmts.typeLiteral3.getEdgesByTarget: QueryBuilder#stmts.typeLiteral3:getEdgesByTarget.
  QueryBuilder.stmts.typeLiteral3.deleteFile: QueryBuilder#stmts.typeLiteral3:deleteFile.
  QueryBuilder.stmts.typeLiteral3.getFileByPath: QueryBuilder#stmts.typeLiteral3:getFileByPath.
  QueryBuilder.stmts.typeLiteral3.getAllFiles: QueryBuilder#stmts.typeLiteral3:getAllFiles.
  QueryBuilder.stmts.typeLiteral3.insertUnresolved: QueryBuilder#stmts.typeLiteral3:insertUnresolved.
  QueryBuilder.stmts.typeLiteral3.deleteUnresolvedByNode: QueryBuilder#stmts.typeLiteral3:deleteUnresolvedByNode.
  QueryBuilder.stmts.typeLiteral3.getUnresolvedByName: QueryBuilder#stmts.typeLiteral3:getUnresolvedByName.
  QueryBuilder.stmts.typeLiteral3.getNodesByName: QueryBuilder#stmts.typeLiteral3:getNodesByName.
  QueryBuilder.stmts.typeLiteral3.getNodesByQualifiedNameExact: QueryBuilder#stmts.typeLiteral3:getNodesByQualifiedNameExact.
  QueryBuilder.stmts.typeLiteral3.getNodesByLowerName: QueryBuilder#stmts.typeLiteral3:getNodesByLowerName.
  QueryBuilder.stmts.typeLiteral3.getUnresolvedCount: QueryBuilder#stmts.typeLiteral3:getUnresolvedCount.
  QueryBuilder.stmts.typeLiteral3.getUnresolvedBatch: QueryBuilder#stmts.typeLiteral3:getUnresolvedBatch.
  QueryBuilder.stmts.typeLiteral3.getAllFilePaths: QueryBuilder#stmts.typeLiteral3:getAllFilePaths.
  QueryBuilder.stmts.typeLiteral3.getAllNodeNames: QueryBuilder#stmts.typeLiteral3:getAllNodeNames.
  QueryBuilder.stmts.typeLiteral3.getDominantFile: QueryBuilder#stmts.typeLiteral3:getDominantFile.
  QueryBuilder.stmts.typeLiteral3.getTopRouteFile: QueryBuilder#stmts.typeLiteral3:getTopRouteFile.
  QueryBuilder.stmts.typeLiteral3.getRoutingManifest: QueryBuilder#stmts.typeLiteral3:getRoutingManifest.
  QueryBuilder.stmts.typeLiteral3.insertNameSegment: QueryBuilder#stmts.typeLiteral3:insertNameSegment.
  NodeRow.id: NodeRow#id.
  UnresolvedRefRow: UnresolvedRefRow#
  QueryBuilder.segmentedNames: QueryBuilder#segmentedNames.
  QueryBuilder.clearUnresolvedReferences: QueryBuilder#clearUnresolvedReferences().
  QueryBuilder.searchAllByFilters.options-typeLiteral308.kinds: QueryBuilder#searchAllByFilters().(options)typeLiteral308:kinds.
  QueryBuilder.searchAllByFilters.options-typeLiteral308.languages: QueryBuilder#searchAllByFilters().(options)typeLiteral308:languages.
  QueryBuilder.searchNodesFuzzy.options-typeLiteral309.kinds: QueryBuilder#searchNodesFuzzy().(options)typeLiteral309:kinds.
  QueryBuilder.searchNodesFuzzy.options-typeLiteral309.languages: QueryBuilder#searchNodesFuzzy().(options)typeLiteral309:languages.
  UnresolvedRefRow.from_node_id: UnresolvedRefRow#from_node_id.
  UnresolvedRefRow.reference_name: UnresolvedRefRow#reference_name.
  UnresolvedRefRow.reference_kind: UnresolvedRefRow#reference_kind.
  UnresolvedRefRow.line: UnresolvedRefRow#line.
  UnresolvedRefRow.col: UnresolvedRefRow#col.
  UnresolvedRefRow.file_path: UnresolvedRefRow#file_path.
  UnresolvedRefRow.language: UnresolvedRefRow#language.
  QueryBuilder.getNodeAndEdgeCount.typeLiteral895.nodes: QueryBuilder#getNodeAndEdgeCount().typeLiteral895:nodes.
  QueryBuilder.setProjectNameTokens: QueryBuilder#setProjectNameTokens().
  QueryBuilder.getProjectNameTokens: QueryBuilder#getProjectNameTokens().
  FileRow: FileRow#
  QueryBuilder.projectNameTokens: QueryBuilder#projectNameTokens.
  QueryBuilder.stmts.typeLiteral3.deleteEdgesByTarget: QueryBuilder#stmts.typeLiteral3:deleteEdgesByTarget.
  QueryBuilder.stmts.typeLiteral3.insertFile: QueryBuilder#stmts.typeLiteral3:insertFile.
  QueryBuilder.stmts.typeLiteral3.updateFile: QueryBuilder#stmts.typeLiteral3:updateFile.
  QueryBuilder.clearCache: QueryBuilder#clearCache().
  NodeRow.decorators: NodeRow#decorators.
  NodeRow.type_parameters: NodeRow#type_parameters.
  EdgeRow.metadata: EdgeRow#metadata.
  FileRow.errors: FileRow#errors.
  QueryBuilder.isSegmentableKind: QueryBuilder#isSegmentableKind().
  QueryBuilder.getSegmentCoOccurrence.variants-Array.typeLiteral33.segment: QueryBuilder#getSegmentCoOccurrence().(variants)Array:typeLiteral33:segment.
  QueryBuilder.getSegmentCoOccurrence.Array.typeLiteral34.name: QueryBuilder#getSegmentCoOccurrence().Array:typeLiteral34:name.
  QueryBuilder.searchAllByFilters.options-typeLiteral308.limit: QueryBuilder#searchAllByFilters().(options)typeLiteral308:limit.
  QueryBuilder.searchNodesFuzzy.options-typeLiteral309.limit: QueryBuilder#searchNodesFuzzy().(options)typeLiteral309:limit.
  QueryBuilder.getNodeAndEdgeCount.typeLiteral895.edges: QueryBuilder#getNodeAndEdgeCount().typeLiteral895:edges.
  NodeRow.kind: NodeRow#kind.
  NodeRow.name: NodeRow#name.
  NodeRow.qualified_name: NodeRow#qualified_name.
  NodeRow.file_path: NodeRow#file_path.
  NodeRow.language: NodeRow#language.
  NodeRow.start_line: NodeRow#start_line.
  NodeRow.end_line: NodeRow#end_line.
  NodeRow.start_column: NodeRow#start_column.
  NodeRow.end_column: NodeRow#end_column.
  NodeRow.docstring: NodeRow#docstring.
  NodeRow.signature: NodeRow#signature.
  NodeRow.visibility: NodeRow#visibility.
  NodeRow.is_exported: NodeRow#is_exported.
  NodeRow.is_async: NodeRow#is_async.
  NodeRow.is_static: NodeRow#is_static.
  NodeRow.is_abstract: NodeRow#is_abstract.
  NodeRow.return_type: NodeRow#return_type.
  NodeRow.updated_at: NodeRow#updated_at.
  EdgeRow.source: EdgeRow#source.
  EdgeRow.target: EdgeRow#target.
  EdgeRow.kind: EdgeRow#kind.
  EdgeRow.line: EdgeRow#line.
  EdgeRow.col: EdgeRow#col.
  EdgeRow.provenance: EdgeRow#provenance.
  FileRow.path: FileRow#path.
  FileRow.content_hash: FileRow#content_hash.
  FileRow.language: FileRow#language.
  FileRow.size: FileRow#size.
  FileRow.modified_at: FileRow#modified_at.
  FileRow.indexed_at: FileRow#indexed_at.
  FileRow.node_count: FileRow#node_count.
  QueryBuilder.maxCacheSize: QueryBuilder#maxCacheSize.
  QueryBuilder.MAX_SEGMENTED_NAMES: QueryBuilder#MAX_SEGMENTED_NAMES.
  QueryBuilder.getSegmentCoOccurrence: QueryBuilder#getSegmentCoOccurrence().
  QueryBuilder.getSegmentCoOccurrence.variants-Array.typeLiteral33.word: QueryBuilder#getSegmentCoOccurrence().(variants)Array:typeLiteral33:word.
  QueryBuilder.deleteSpecificResolvedReferences.refs-Array.typeLiteral882.fromNodeId: QueryBuilder#deleteSpecificResolvedReferences().(refs)Array:typeLiteral882:fromNodeId.
  QueryBuilder.deleteSpecificResolvedReferences.refs-Array.typeLiteral882.referenceName: QueryBuilder#deleteSpecificResolvedReferences().(refs)Array:typeLiteral882:referenceName.
  QueryBuilder.deleteSpecificResolvedReferences.refs-Array.typeLiteral882.referenceKind: QueryBuilder#deleteSpecificResolvedReferences().(refs)Array:typeLiteral882:referenceKind.
  EdgeRow.id: EdgeRow#id.
  UnresolvedRefRow.id: UnresolvedRefRow#id.
---
# Module: [`src/db/queries.ts`](../../../../../../raw/code/codegraph/src/db/queries.ts)

## Classes
### `EdgeRow`
- def: [`src/db/queries.ts:80`](../../../../../../raw/code/codegraph/src/db/queries.ts#L80)
- signature: `interface EdgeRow`
- members:
  - `col` — [`L87`](../../../../../../raw/code/codegraph/src/db/queries.ts#L87)
  - `id` — [`L81`](../../../../../../raw/code/codegraph/src/db/queries.ts#L81)
  - `kind` — [`L84`](../../../../../../raw/code/codegraph/src/db/queries.ts#L84)
  - `line` — [`L86`](../../../../../../raw/code/codegraph/src/db/queries.ts#L86)
  - `metadata` — [`L85`](../../../../../../raw/code/codegraph/src/db/queries.ts#L85)
  - `provenance` — [`L88`](../../../../../../raw/code/codegraph/src/db/queries.ts#L88)
  - `source` — [`L82`](../../../../../../raw/code/codegraph/src/db/queries.ts#L82)
  - `target` — [`L83`](../../../../../../raw/code/codegraph/src/db/queries.ts#L83)
- used by: [`rowToEdge`](queries.ts.md#rowToEdge), [`getOutgoingEdges`](queries.ts.md#QueryBuilder.getOutgoingEdges), [`getIncomingEdges`](queries.ts.md#QueryBuilder.getIncomingEdges), [`findEdgesBetweenNodes`](queries.ts.md#QueryBuilder.findEdgesBetweenNodes), [`getCrossFileIncomingEdgesWithTarget`](queries.ts.md#QueryBuilder.getCrossFileIncomingEdgesWithTarget)

### `FileRow`
- def: [`src/db/queries.ts:91`](../../../../../../raw/code/codegraph/src/db/queries.ts#L91)
- signature: `interface FileRow`
- members:
  - `content_hash` — [`L93`](../../../../../../raw/code/codegraph/src/db/queries.ts#L93)
  - `errors` — [`L99`](../../../../../../raw/code/codegraph/src/db/queries.ts#L99)
  - `indexed_at` — [`L97`](../../../../../../raw/code/codegraph/src/db/queries.ts#L97)
  - `language` — [`L94`](../../../../../../raw/code/codegraph/src/db/queries.ts#L94)
  - `modified_at` — [`L96`](../../../../../../raw/code/codegraph/src/db/queries.ts#L96)
  - `node_count` — [`L98`](../../../../../../raw/code/codegraph/src/db/queries.ts#L98)
  - `path` — [`L92`](../../../../../../raw/code/codegraph/src/db/queries.ts#L92)
  - `size` — [`L95`](../../../../../../raw/code/codegraph/src/db/queries.ts#L95)
- used by: [`rowToFileRecord`](queries.ts.md#rowToFileRecord), [`getAllFiles`](queries.ts.md#QueryBuilder.getAllFiles), [`getFileByPath`](queries.ts.md#QueryBuilder.getFileByPath)

### `NodeRow`
- def: [`src/db/queries.ts:56`](../../../../../../raw/code/codegraph/src/db/queries.ts#L56)
- doc: Database row types (snake_case from SQLite)
- signature: `interface NodeRow`
- members:
  - `decorators` — [`L74`](../../../../../../raw/code/codegraph/src/db/queries.ts#L74)
  - `docstring` — [`L67`](../../../../../../raw/code/codegraph/src/db/queries.ts#L67)
  - `end_column` — [`L66`](../../../../../../raw/code/codegraph/src/db/queries.ts#L66)
  - `end_line` — [`L64`](../../../../../../raw/code/codegraph/src/db/queries.ts#L64)
  - `file_path` — [`L61`](../../../../../../raw/code/codegraph/src/db/queries.ts#L61)
  - `id` — [`L57`](../../../../../../raw/code/codegraph/src/db/queries.ts#L57)
  - `is_abstract` — [`L73`](../../../../../../raw/code/codegraph/src/db/queries.ts#L73)
  - `is_async` — [`L71`](../../../../../../raw/code/codegraph/src/db/queries.ts#L71)
  - `is_exported` — [`L70`](../../../../../../raw/code/codegraph/src/db/queries.ts#L70)
  - `is_static` — [`L72`](../../../../../../raw/code/codegraph/src/db/queries.ts#L72)
  - `kind` — [`L58`](../../../../../../raw/code/codegraph/src/db/queries.ts#L58)
  - `language` — [`L62`](../../../../../../raw/code/codegraph/src/db/queries.ts#L62)
  - `name` — [`L59`](../../../../../../raw/code/codegraph/src/db/queries.ts#L59)
  - `qualified_name` — [`L60`](../../../../../../raw/code/codegraph/src/db/queries.ts#L60)
  - `return_type` — [`L76`](../../../../../../raw/code/codegraph/src/db/queries.ts#L76)
  - `signature` — [`L68`](../../../../../../raw/code/codegraph/src/db/queries.ts#L68)
  - `start_column` — [`L65`](../../../../../../raw/code/codegraph/src/db/queries.ts#L65)
  - `start_line` — [`L63`](../../../../../../raw/code/codegraph/src/db/queries.ts#L63)
  - `type_parameters` — [`L75`](../../../../../../raw/code/codegraph/src/db/queries.ts#L75)
  - `updated_at` — [`L77`](../../../../../../raw/code/codegraph/src/db/queries.ts#L77)
  - `visibility` — [`L69`](../../../../../../raw/code/codegraph/src/db/queries.ts#L69)
- used by: [`rowToNode`](queries.ts.md#rowToNode), [`searchNodes`](queries.ts.md#QueryBuilder.searchNodes), [`getNodeById`](queries.ts.md#QueryBuilder.getNodeById), [`getNodesByKind`](queries.ts.md#QueryBuilder.getNodesByKind), [`getNodesByIds`](queries.ts.md#QueryBuilder.getNodesByIds), [`findNodesByExactName`](queries.ts.md#QueryBuilder.findNodesByExactName), [`searchNodesFuzzy`](queries.ts.md#QueryBuilder.searchNodesFuzzy), [`searchNodesFTS`](queries.ts.md#QueryBuilder.searchNodesFTS), [`searchNodesLike`](queries.ts.md#QueryBuilder.searchNodesLike), [`iterateNodesByKind`](queries.ts.md#QueryBuilder.iterateNodesByKind), [`findNodesByNameSubstring`](queries.ts.md#QueryBuilder.findNodesByNameSubstring), [`getNodesByName`](queries.ts.md#QueryBuilder.getNodesByName), [`searchAllByFilters`](queries.ts.md#QueryBuilder.searchAllByFilters), [`getNodesByFile`](queries.ts.md#QueryBuilder.getNodesByFile), [`getNodesByQualifiedNameExact`](queries.ts.md#QueryBuilder.getNodesByQualifiedNameExact), [`getNodesByLowerName`](queries.ts.md#QueryBuilder.getNodesByLowerName), [`getAllNodes`](queries.ts.md#QueryBuilder.getAllNodes)

### `QueryBuilder`
- def: [`src/db/queries.ts:177`](../../../../../../raw/code/codegraph/src/db/queries.ts#L177) — documented in [index.ts](../../../concepts/index.ts.md)
- doc: Query builder for the knowledge graph database
- signature: `class QueryBuilder`
- members:
  - `<constructor>(db: SqliteDatabase)` — [`L233`](../../../../../../raw/code/codegraph/src/db/queries.ts#L233) — Query builder for the knowledge graph database
  - `cacheNode(method)` — [`L664`](../../../../../../raw/code/codegraph/src/db/queries.ts#L664) — Add a node to the cache, evicting oldest if needed
  - `clear(method)` — [`L2016`](../../../../../../raw/code/codegraph/src/db/queries.ts#L2016) — Clear all data from the database
  - `clearCache(method)` — [`L678`](../../../../../../raw/code/codegraph/src/db/queries.ts#L678) — Clear the node cache
  - `clearNameSegmentVocab(method)` — [`L473`](../../../../../../raw/code/codegraph/src/db/queries.ts#L473) — Wipe the segment vocabulary. A full index calls this at its start; the
  - `clearUnresolvedReferences(method)` — [`L1877`](../../../../../../raw/code/codegraph/src/db/queries.ts#L1877) — Delete all unresolved references (after resolution)
  - `deleteEdgesBySource(method)` — [`L1455`](../../../../../../raw/code/codegraph/src/db/queries.ts#L1455) — Delete all edges from a source node
  - `deleteFile(method)` — [`L1638`](../../../../../../raw/code/codegraph/src/db/queries.ts#L1638) — Delete a file record and its nodes
  - `deleteNode(method)` — [`L441`](../../../../../../raw/code/codegraph/src/db/queries.ts#L441) — Delete a node by ID
  - `deleteNodesByFile(method)` — [`L453`](../../../../../../raw/code/codegraph/src/db/queries.ts#L453) — Delete all nodes for a file
  - `deleteResolvedReferences(method)` — [`L1884`](../../../../../../raw/code/codegraph/src/db/queries.ts#L1884) — Delete resolved references by their IDs
  - `deleteSpecificResolvedReferences(method)` — [`L1902`](../../../../../../raw/code/codegraph/src/db/queries.ts#L1902) — Delete specific resolved references by (fromNodeId, referenceName, referenceKind) tuples.
  - `deleteUnresolvedByNode(method)` — [`L1735`](../../../../../../raw/code/codegraph/src/db/queries.ts#L1735) — Delete unresolved references from a node
  - `findEdgesBetweenNodes(method)` — [`L1512`](../../../../../../raw/code/codegraph/src/db/queries.ts#L1512) — Find all edges where both source and target are in the given node set.
  - `findNodesByExactName(method)` — [`L1276`](../../../../../../raw/code/codegraph/src/db/queries.ts#L1276) — Find nodes by exact name match — documented in [db-queries.ts](../../../concepts/db-queries.ts.md)
  - `findNodesByNameSubstring(method)` — [`L1364`](../../../../../../raw/code/codegraph/src/db/queries.ts#L1364) — Find nodes whose name contains a substring (LIKE-based). — documented in [db-queries.ts](../../../concepts/db-queries.ts.md)
  - `getAllFilePaths(method)` — [`L1822`](../../../../../../raw/code/codegraph/src/db/queries.ts#L1822) — Get all tracked file paths (lightweight — no full FileRecord objects)
  - `getAllFiles(method)` — [`L1662`](../../../../../../raw/code/codegraph/src/db/queries.ts#L1662) — Get all tracked files — documented in [db-queries.ts](../../../concepts/db-queries.ts.md)
  - `getAllMetadata(method)` — [`L2004`](../../../../../../raw/code/codegraph/src/db/queries.ts#L2004) — Get all metadata as a key-value record
  - `getAllNodeNames(method)` — [`L1833`](../../../../../../raw/code/codegraph/src/db/queries.ts#L1833) — Get all distinct node names (lightweight — just name strings for pre-filtering)
  - `getAllNodes(method)` — [`L877`](../../../../../../raw/code/codegraph/src/db/queries.ts#L877) — Get all nodes in the database — documented in [db-sqlite-adapter.ts](../../../concepts/db-sqlite-adapter.ts.md)
  - `getCrossFileIncomingEdgesWithTarget(method)` — [`L1584`](../../../../../../raw/code/codegraph/src/db/queries.ts#L1584) — Cross-file edges whose TARGET is a node in `filePath` and whose SOURCE is a
  - `getDependencyFilePaths(method)` — [`L1562`](../../../../../../raw/code/codegraph/src/db/queries.ts#L1562) — Distinct file paths that `filePath` DEPENDS ON — the inverse of
  - `getDependentFilePaths(method)` — [`L1544`](../../../../../../raw/code/codegraph/src/db/queries.ts#L1544) — Distinct file paths that DEPEND ON `filePath`: every file containing a
  - `getDistinctNodeNames(method)` — [`L488`](../../../../../../raw/code/codegraph/src/db/queries.ts#L488) — One page of distinct segmentable node names, for batched vocab rebuilds
  - `getDominantFile(method)` — [`L713`](../../../../../../raw/code/codegraph/src/db/queries.ts#L713) — Find the file that holds the densest concentration of the project's
  - `getExistingNodeIds(method)` — [`L642`](../../../../../../raw/code/codegraph/src/db/queries.ts#L642)
  - `getFileByPath(method)` — [`L1651`](../../../../../../raw/code/codegraph/src/db/queries.ts#L1651) — Get a file record by path — documented in [db-queries.ts](../../../concepts/db-queries.ts.md)
  - `getIncomingEdges(method)` — [`L1494`](../../../../../../raw/code/codegraph/src/db/queries.ts#L1494) — Get incoming edges to a node — documented in [db-queries.ts](../../../concepts/db-queries.ts.md)
  - `getLastIndexedAt(method)` — [`L1674`](../../../../../../raw/code/codegraph/src/db/queries.ts#L1674) — Most recent index timestamp (ms since epoch) across all tracked files, or
  - `getMetadata(method)` — [`L1987`](../../../../../../raw/code/codegraph/src/db/queries.ts#L1987) — Get a metadata value by key
  - `getNamesForSegment(method)` — [`L557`](../../../../../../raw/code/codegraph/src/db/queries.ts#L557) — Names containing the given segment (rare-single-word tier).
  - `getNodeAndEdgeCount(method)` — [`L1926`](../../../../../../raw/code/codegraph/src/db/queries.ts#L1926) — Lightweight (nodes, edges) count snapshot. Used around an index/sync
  - `getNodeById(method)` — [`L567`](../../../../../../raw/code/codegraph/src/db/queries.ts#L567) — Get a node by ID — documented in [db-queries.ts](../../../concepts/db-queries.ts.md)
  - `getNodesByFile(method)` — [`L685`](../../../../../../raw/code/codegraph/src/db/queries.ts#L685) — Get all nodes in a file — documented in [db-queries.ts](../../../concepts/db-queries.ts.md)
  - `getNodesByIds(method)` — [`L605`](../../../../../../raw/code/codegraph/src/db/queries.ts#L605) — Batch lookup: fetch many nodes by ID in a single SQL round-trip. — documented in [db-queries.ts](../../../concepts/db-queries.ts.md)
  - `getNodesByKind(method)` — [`L850`](../../../../../../raw/code/codegraph/src/db/queries.ts#L850) — Get all nodes of a specific kind — documented in [db-queries.ts](../../../concepts/db-queries.ts.md)
  - `getNodesByLowerName(method)` — [`L909`](../../../../../../raw/code/codegraph/src/db/queries.ts#L909) — Get nodes by lowercase name match (uses idx_nodes_lower_name expression index) — documented in [db-queries.ts](../../../concepts/db-queries.ts.md)
  - `getNodesByName(method)` — [`L885`](../../../../../../raw/code/codegraph/src/db/queries.ts#L885) — Get nodes by exact name match (uses idx_nodes_name index) — documented in [db-queries.ts](../../../concepts/db-queries.ts.md)
  - `getNodesByQualifiedNameExact(method)` — [`L896`](../../../../../../raw/code/codegraph/src/db/queries.ts#L896) — Get nodes by exact qualified name match (uses idx_nodes_qualified_name index) — documented in [db-queries.ts](../../../concepts/db-queries.ts.md)
  - `getOutgoingEdges(method)` — [`L1465`](../../../../../../raw/code/codegraph/src/db/queries.ts#L1465) — Get outgoing edges from a node — documented in [db-queries.ts](../../../concepts/db-queries.ts.md)
  - `getProjectNameTokens(method)` — [`L244`](../../../../../../raw/code/codegraph/src/db/queries.ts#L244) — The normalized project-name tokens (#720); empty if none were derived.
  - `getRoutingManifest(method)` — [`L787`](../../../../../../raw/code/codegraph/src/db/queries.ts#L787) — Build a URL → handler manifest from the index. Each route node's
  - `getSegmentCoOccurrence(method)` — [`L515`](../../../../../../raw/code/codegraph/src/db/queries.ts#L515) — Names whose segments cover at least `minWords` distinct PROMPT WORDS —
  - `getSegmentNameCounts(method)` — [`L544`](../../../../../../raw/code/codegraph/src/db/queries.ts#L544) — How many distinct names each segment appears in — the rarity signal that
  - `getStaleFiles(method)` — [`L1684`](../../../../../../raw/code/codegraph/src/db/queries.ts#L1684) — Get files that need re-indexing (hash changed)
  - `getStats(method)` — [`L1935`](../../../../../../raw/code/codegraph/src/db/queries.ts#L1935) — Get graph statistics — documented in [db-queries.ts](../../../concepts/db-queries.ts.md)
  - `getTopRouteFile(method)` — [`L755`](../../../../../../raw/code/codegraph/src/db/queries.ts#L755) — Find the file that holds the densest concentration of the project's
  - `getUnresolvedByName(method)` — [`L1747`](../../../../../../raw/code/codegraph/src/db/queries.ts#L1747) — Get unresolved references by name (for resolution) — documented in [db-queries.ts](../../../concepts/db-queries.ts.md)
  - `getUnresolvedReferences(method)` — [`L1769`](../../../../../../raw/code/codegraph/src/db/queries.ts#L1769) — Get all unresolved references — documented in [db-queries.ts](../../../concepts/db-queries.ts.md)
  - `getUnresolvedReferencesBatch(method)` — [`L1800`](../../../../../../raw/code/codegraph/src/db/queries.ts#L1800) — Get a batch of unresolved references using LIMIT/OFFSET pagination. — documented in [db-queries.ts](../../../concepts/db-queries.ts.md)
  - `getUnresolvedReferencesByFiles(method)` — [`L1845`](../../../../../../raw/code/codegraph/src/db/queries.ts#L1845) — Get unresolved references scoped to specific file paths. — documented in [db-queries.ts](../../../concepts/db-queries.ts.md)
  - `getUnresolvedReferencesCount(method)` — [`L1786`](../../../../../../raw/code/codegraph/src/db/queries.ts#L1786) — Get the count of unresolved references without loading them into memory
  - `insertEdge(method)` — [`L1410`](../../../../../../raw/code/codegraph/src/db/queries.ts#L1410) — Insert a new edge — documented in [db-queries.ts](../../../concepts/db-queries.ts.md)
  - `insertEdges(method)` — [`L1432`](../../../../../../raw/code/codegraph/src/db/queries.ts#L1432) — Insert multiple edges in a transaction — documented in [db-queries.ts](../../../concepts/db-queries.ts.md)
  - `insertNameSegments(method)` — [`L338`](../../../../../../raw/code/codegraph/src/db/queries.ts#L338) — Write `name`'s segments into name_segment_vocab (idempotent). — documented in [db-queries.ts](../../../concepts/db-queries.ts.md)
  - `insertNameSegmentsBatch(method)` — [`L496`](../../../../../../raw/code/codegraph/src/db/queries.ts#L496) — Insert segments for a batch of names in one transaction (vocab heal path).
  - `insertNode(method)` — [`L255`](../../../../../../raw/code/codegraph/src/db/queries.ts#L255) — Insert a new node — documented in [db-queries.ts](../../../concepts/db-queries.ts.md)
  - `insertNodes(method)` — [`L355`](../../../../../../raw/code/codegraph/src/db/queries.ts#L355) — Insert multiple nodes in a transaction
  - `insertUnresolvedRef(method)` — [`L1699`](../../../../../../raw/code/codegraph/src/db/queries.ts#L1699) — Insert an unresolved reference — documented in [db-queries.ts](../../../concepts/db-queries.ts.md)
  - `insertUnresolvedRefsBatch(method)` — [`L1722`](../../../../../../raw/code/codegraph/src/db/queries.ts#L1722) — Insert multiple unresolved references in a transaction
  - `isNameSegmentVocabEmpty(method)` — [`L480`](../../../../../../raw/code/codegraph/src/db/queries.ts#L480) — True when the vocab has no rows — an index built before the table existed.
  - `isSegmentableKind(method)` — [`L333`](../../../../../../raw/code/codegraph/src/db/queries.ts#L333) — Which node kinds contribute their name to the segment vocabulary — the
  - `iterateNodesByKind(method)` — [`L865`](../../../../../../raw/code/codegraph/src/db/queries.ts#L865) — Stream every node of a kind one at a time (lazy) instead of materializing — documented in [db-queries.ts](../../../concepts/db-queries.ts.md)
  - `searchAllByFilters(method)` — [`L1052`](../../../../../../raw/code/codegraph/src/db/queries.ts#L1052) — Match-everything path used when the user supplied only field — documented in [db-queries.ts](../../../concepts/db-queries.ts.md)
  - `searchNodes(method)` — [`L927`](../../../../../../raw/code/codegraph/src/db/queries.ts#L927) — Search nodes by name using FTS with fallback to LIKE for better matching — documented in [db-queries.ts](../../../concepts/db-queries.ts.md)
  - `searchNodesFTS(method)` — [`L1141`](../../../../../../raw/code/codegraph/src/db/queries.ts#L1141) — FTS5 search with prefix matching — documented in [db-queries.ts](../../../concepts/db-queries.ts.md)
  - `searchNodesFuzzy(method)` — [`L1082`](../../../../../../raw/code/codegraph/src/db/queries.ts#L1082) — Fuzzy fallback: when zero FTS/LIKE hits, try an edit-distance — documented in [db-queries.ts](../../../concepts/db-queries.ts.md)
  - `searchNodesLike(method)` — [`L1210`](../../../../../../raw/code/codegraph/src/db/queries.ts#L1210) — LIKE-based substring search for cases where FTS doesn't match — documented in [db-queries.ts](../../../concepts/db-queries.ts.md)
  - `setMetadata(method)` — [`L1995`](../../../../../../raw/code/codegraph/src/db/queries.ts#L1995) — Set a metadata key-value pair (upsert)
  - `setProjectNameTokens(method)` — [`L239`](../../../../../../raw/code/codegraph/src/db/queries.ts#L239) — Set the normalized project-name tokens used to down-weight non-discriminative
  - `updateNode(method)` — [`L366`](../../../../../../raw/code/codegraph/src/db/queries.ts#L366) — Update an existing node — documented in [db-queries.ts](../../../concepts/db-queries.ts.md)
  - `upsertFile(method)` — [`L1607`](../../../../../../raw/code/codegraph/src/db/queries.ts#L1607) — Insert or update a file record — documented in [db-queries.ts](../../../concepts/db-queries.ts.md)
  - `MAX_SEGMENTED_NAMES` — [`L231`](../../../../../../raw/code/codegraph/src/db/queries.ts#L231)
  - `db` — [`L178`](../../../../../../raw/code/codegraph/src/db/queries.ts#L178) — documented in [db-queries.ts](../../../concepts/db-queries.ts.md)
  - `deleteEdgesBySource` — [`L201`](../../../../../../raw/code/codegraph/src/db/queries.ts#L201)
  - `deleteEdgesByTarget` — [`L202`](../../../../../../raw/code/codegraph/src/db/queries.ts#L202)
  - `deleteFile` — [`L207`](../../../../../../raw/code/codegraph/src/db/queries.ts#L207)
  - `deleteNode` — [`L194`](../../../../../../raw/code/codegraph/src/db/queries.ts#L194)
  - `deleteNodesByFile` — [`L195`](../../../../../../raw/code/codegraph/src/db/queries.ts#L195)
  - `deleteUnresolvedByNode` — [`L211`](../../../../../../raw/code/codegraph/src/db/queries.ts#L211)
  - `edges` — [`L1926`](../../../../../../raw/code/codegraph/src/db/queries.ts#L1926)
  - `fromNodeId` — [`L1902`](../../../../../../raw/code/codegraph/src/db/queries.ts#L1902)
  - `getAllFilePaths` — [`L218`](../../../../../../raw/code/codegraph/src/db/queries.ts#L218)
  - `getAllFiles` — [`L209`](../../../../../../raw/code/codegraph/src/db/queries.ts#L209)
  - `getAllNodeNames` — [`L219`](../../../../../../raw/code/codegraph/src/db/queries.ts#L219)
  - `getDominantFile` — [`L220`](../../../../../../raw/code/codegraph/src/db/queries.ts#L220)
  - `getEdgesBySource` — [`L203`](../../../../../../raw/code/codegraph/src/db/queries.ts#L203)
  - `getEdgesByTarget` — [`L204`](../../../../../../raw/code/codegraph/src/db/queries.ts#L204)
  - `getFileByPath` — [`L208`](../../../../../../raw/code/codegraph/src/db/queries.ts#L208)
  - `getNodeById` — [`L196`](../../../../../../raw/code/codegraph/src/db/queries.ts#L196)
  - `getNodesByFile` — [`L197`](../../../../../../raw/code/codegraph/src/db/queries.ts#L197)
  - `getNodesByKind` — [`L198`](../../../../../../raw/code/codegraph/src/db/queries.ts#L198)
  - `getNodesByLowerName` — [`L215`](../../../../../../raw/code/codegraph/src/db/queries.ts#L215)
  - `getNodesByName` — [`L213`](../../../../../../raw/code/codegraph/src/db/queries.ts#L213)
  - `getNodesByQualifiedNameExact` — [`L214`](../../../../../../raw/code/codegraph/src/db/queries.ts#L214)
  - `getRoutingManifest` — [`L222`](../../../../../../raw/code/codegraph/src/db/queries.ts#L222)
  - `getTopRouteFile` — [`L221`](../../../../../../raw/code/codegraph/src/db/queries.ts#L221)
  - `getUnresolvedBatch` — [`L217`](../../../../../../raw/code/codegraph/src/db/queries.ts#L217)
  - `getUnresolvedByName` — [`L212`](../../../../../../raw/code/codegraph/src/db/queries.ts#L212)
  - `getUnresolvedCount` — [`L216`](../../../../../../raw/code/codegraph/src/db/queries.ts#L216)
  - `insertEdge` — [`L199`](../../../../../../raw/code/codegraph/src/db/queries.ts#L199)
  - `insertFile` — [`L205`](../../../../../../raw/code/codegraph/src/db/queries.ts#L205)
  - `insertNameSegment` — [`L223`](../../../../../../raw/code/codegraph/src/db/queries.ts#L223)
  - `insertNode` — [`L192`](../../../../../../raw/code/codegraph/src/db/queries.ts#L192)
  - `insertUnresolved` — [`L210`](../../../../../../raw/code/codegraph/src/db/queries.ts#L210)
  - `kinds` — [`L1053`](../../../../../../raw/code/codegraph/src/db/queries.ts#L1053)
  - `kinds` — [`L1084`](../../../../../../raw/code/codegraph/src/db/queries.ts#L1084)
  - `languages` — [`L1054`](../../../../../../raw/code/codegraph/src/db/queries.ts#L1054)
  - `languages` — [`L1084`](../../../../../../raw/code/codegraph/src/db/queries.ts#L1084)
  - `limit` — [`L1055`](../../../../../../raw/code/codegraph/src/db/queries.ts#L1055)
  - `limit` — [`L1084`](../../../../../../raw/code/codegraph/src/db/queries.ts#L1084)
  - `matches` — [`L519`](../../../../../../raw/code/codegraph/src/db/queries.ts#L519)
  - `maxCacheSize` — [`L188`](../../../../../../raw/code/codegraph/src/db/queries.ts#L188)
  - `name` — [`L519`](../../../../../../raw/code/codegraph/src/db/queries.ts#L519)
  - `nodeCache` — [`L187`](../../../../../../raw/code/codegraph/src/db/queries.ts#L187)
  - `nodes` — [`L1926`](../../../../../../raw/code/codegraph/src/db/queries.ts#L1926)
  - `projectNameTokens` — [`L184`](../../../../../../raw/code/codegraph/src/db/queries.ts#L184)
  - `referenceKind` — [`L1902`](../../../../../../raw/code/codegraph/src/db/queries.ts#L1902)
  - `referenceName` — [`L1902`](../../../../../../raw/code/codegraph/src/db/queries.ts#L1902)
  - `segment` — [`L516`](../../../../../../raw/code/codegraph/src/db/queries.ts#L516)
  - `segmentedNames` — [`L230`](../../../../../../raw/code/codegraph/src/db/queries.ts#L230)
  - `stmts` — [`L191`](../../../../../../raw/code/codegraph/src/db/queries.ts#L191) — documented in [db-queries.ts](../../../concepts/db-queries.ts.md)
  - `updateFile` — [`L206`](../../../../../../raw/code/codegraph/src/db/queries.ts#L206)
  - `updateNode` — [`L193`](../../../../../../raw/code/codegraph/src/db/queries.ts#L193)
  - `upsertFile` — [`L200`](../../../../../../raw/code/codegraph/src/db/queries.ts#L200)
  - `word` — [`L516`](../../../../../../raw/code/codegraph/src/db/queries.ts#L516)
- uses (calls/refs, reference-scoped): [`id`](../types.ts.md#Node.id), [`Node`](../types.ts.md#Node), [`kind`](../types.ts.md#Node.kind), [`filePath`](../types.ts.md#Node.filePath), [`name`](../types.ts.md#Node.name), [`startLine`](../types.ts.md#Node.startLine), [`Edge`](../types.ts.md#Edge), [`language`](../types.ts.md#Node.language), [`rowToNode`](queries.ts.md#rowToNode), [`target`](../types.ts.md#Edge.target), [`qualifiedName`](../types.ts.md#Node.qualifiedName), [`source`](../types.ts.md#Edge.source), [`kind`](../types.ts.md#Edge.kind), [`endLine`](../types.ts.md#Node.endLine), [`fromNodeId`](../types.ts.md#UnresolvedReference.fromNodeId), [`line`](../types.ts.md#UnresolvedReference.line), [`node`](../types.ts.md#SearchResult.node), [`referenceName`](../types.ts.md#UnresolvedReference.referenceName), [`referenceKind`](../types.ts.md#UnresolvedReference.referenceKind), [`column`](../types.ts.md#UnresolvedReference.column), [`Language`](../types.ts.md#Language), [`prepare`](sqlite-adapter.ts.md#SqliteDatabase.prepare), [`endColumn`](../types.ts.md#Node.endColumn), [`startColumn`](../types.ts.md#Node.startColumn), [`updatedAt`](../types.ts.md#Node.updatedAt), [`line`](../types.ts.md#Edge.line), [`score`](../types.ts.md#SearchResult.score), [`rowToFileRecord`](queries.ts.md#rowToFileRecord), [`rowToEdge`](queries.ts.md#rowToEdge), [`NodeKind`](../types.ts.md#NodeKind), [`signature`](../types.ts.md#Node.signature), [`all`](sqlite-adapter.ts.md#SqliteStatement.all), [`metadata`](../types.ts.md#Edge.metadata), [`provenance`](../types.ts.md#Edge.provenance), [`SqliteStatement`](sqlite-adapter.ts.md#SqliteStatement), [`path`](../types.ts.md#FileRecord.path), [`UnresolvedReference`](../types.ts.md#UnresolvedReference), [`parseQuery`](../search/query-parser.ts.md#parseQuery), [`SearchResult`](../types.ts.md#SearchResult), [`isExported`](../types.ts.md#Node.isExported)  (+67 more)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-index.ts), [`createContext`](../resolution/index.ts.md#ReferenceResolver.createContext), [`index.ts`](../resolution/index.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-resolution-index.ts), [`cFnPointerDispatchEdges`](../resolution/c-fnptr-synthesizer.ts.md#cFnPointerDispatchEdges), [`findRelevantContext`](../context/index.ts.md#ContextBuilder.findRelevantContext), [`synthesizeCallbackEdges`](../resolution/callback-synthesizer.ts.md#synthesizeCallbackEdges), [`storeExtractionResult`](../extraction/index.ts.md#ExtractionOrchestrator.storeExtractionResult), [`index.ts`](../extraction/index.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-extraction-index.ts), [`indexAll`](../index.ts.md#CodeGraph.indexAll), [`sync`](../index.ts.md#CodeGraph.sync), [`index.ts`](../context/index.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-context-index.ts), [`resolveOne`](../resolution/index.ts.md#ReferenceResolver.resolveOne), [`resolveDeferredThisMemberRefs`](../resolution/index.ts.md#ReferenceResolver.resolveDeferredThisMemberRefs), [`erlangBehaviourDispatchEdges`](../resolution/callback-synthesizer.ts.md#erlangBehaviourDispatchEdges), [`traverseBFS`](../graph/traversal.ts.md#GraphTraverser.traverseBFS), [`fieldChannelEdges`](../resolution/callback-synthesizer.ts.md#fieldChannelEdges), [`ginMiddlewareChainEdges`](../resolution/callback-synthesizer.ts.md#ginMiddlewareChainEdges), [`reduxThunkEdges`](../resolution/callback-synthesizer.ts.md#reduxThunkEdges), [`sync`](../extraction/index.ts.md#ExtractionOrchestrator.sync), [`flutterBuildEdges`](../resolution/callback-synthesizer.ts.md#flutterBuildEdges), [`getContext`](../graph/queries.ts.md#GraphQueryManager.getContext), [`reactRenderEdges`](../resolution/callback-synthesizer.ts.md#reactRenderEdges), [`resolveAndPersistBatched`](../resolution/index.ts.md#ReferenceResolver.resolveAndPersistBatched), [`closureCollectionEdges`](../resolution/callback-synthesizer.ts.md#closureCollectionEdges), [`getSegmentMatches`](../index.ts.md#CodeGraph.getSegmentMatches), [`goGrpcStubImplEdges`](../resolution/callback-synthesizer.ts.md#goGrpcStubImplEdges), [`interfaceOverrideEdges`](../resolution/callback-synthesizer.ts.md#interfaceOverrideEdges), [`kotlinExpectActualEdges`](../resolution/callback-synthesizer.ts.md#kotlinExpectActualEdges), [`callback-synthesizer.ts`](../resolution/callback-synthesizer.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-resolution-callback-synthesizer.ts), [`cppOverrideEdges`](../resolution/callback-synthesizer.ts.md#cppOverrideEdges), [`goImplementsEdges`](../resolution/callback-synthesizer.ts.md#goImplementsEdges), [`queries`](../index.ts.md#CodeGraph.queries), [`rtkQueryEdges`](../resolution/callback-synthesizer.ts.md#rtkQueryEdges), [`open`](../index.ts.md#CodeGraph.open), [`getChangedFiles`](../extraction/index.ts.md#ExtractionOrchestrator.getChangedFiles), [`goCrossFileMethodContainsEdges`](../resolution/callback-synthesizer.ts.md#goCrossFileMethodContainsEdges), [`<constructor>`](../resolution/index.ts.md#ReferenceResolver.-constructor), [`resolveThisMemberFnRef`](../resolution/index.ts.md#ReferenceResolver.resolveThisMemberFnRef), [`rnCrossPlatformEdges`](../resolution/callback-synthesizer.ts.md#rnCrossPlatformEdges), [`dfsRecursive`](../graph/traversal.ts.md#GraphTraverser.dfsRecursive)  (+78 more)

### `UnresolvedRefRow`
- def: [`src/db/queries.ts:102`](../../../../../../raw/code/codegraph/src/db/queries.ts#L102)
- signature: `interface UnresolvedRefRow`
- members:
  - `candidates` — [`L109`](../../../../../../raw/code/codegraph/src/db/queries.ts#L109)
  - `col` — [`L108`](../../../../../../raw/code/codegraph/src/db/queries.ts#L108)
  - `file_path` — [`L110`](../../../../../../raw/code/codegraph/src/db/queries.ts#L110)
  - `from_node_id` — [`L104`](../../../../../../raw/code/codegraph/src/db/queries.ts#L104)
  - `id` — [`L103`](../../../../../../raw/code/codegraph/src/db/queries.ts#L103)
  - `language` — [`L111`](../../../../../../raw/code/codegraph/src/db/queries.ts#L111)
  - `line` — [`L107`](../../../../../../raw/code/codegraph/src/db/queries.ts#L107)
  - `reference_kind` — [`L106`](../../../../../../raw/code/codegraph/src/db/queries.ts#L106)
  - `reference_name` — [`L105`](../../../../../../raw/code/codegraph/src/db/queries.ts#L105)
- used by: [`getUnresolvedReferencesBatch`](queries.ts.md#QueryBuilder.getUnresolvedReferencesBatch), [`getUnresolvedByName`](queries.ts.md#QueryBuilder.getUnresolvedByName), [`getUnresolvedReferencesByFiles`](queries.ts.md#QueryBuilder.getUnresolvedReferencesByFiles), [`getUnresolvedReferences`](queries.ts.md#QueryBuilder.getUnresolvedReferences)

## Functions
- `isLowValueFile(filePath: string)` — [`L33`](../../../../../../raw/code/codegraph/src/db/queries.ts#L33) — Path-only heuristic for files that should not be candidates for
- `rowToEdge(row: EdgeRow)` — [`L146`](../../../../../../raw/code/codegraph/src/db/queries.ts#L146) — Convert database row to Edge object
- `rowToFileRecord(row: FileRow)` — [`L161`](../../../../../../raw/code/codegraph/src/db/queries.ts#L161) — Convert database row to FileRecord object
- `rowToNode(row: NodeRow)` — [`L117`](../../../../../../raw/code/codegraph/src/db/queries.ts#L117) — Convert database row to Node object — documented in [db-queries.ts](../../../concepts/db-queries.ts.md)

## Module values
- `SQLITE_PARAM_CHUNK_SIZE` — [`L51`](../../../../../../raw/code/codegraph/src/db/queries.ts#L51)

