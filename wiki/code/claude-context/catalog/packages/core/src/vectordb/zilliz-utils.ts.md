---
title: 'Module: packages/core/src/vectordb/zilliz-utils.ts'
type: catalog
provenance: extracted
module: packages/core/src/vectordb/zilliz-utils.ts
status: fresh
symbol_base: scip-typescript npm @zilliz/claude-context-core 0.1.15 src/vectordb/`zilliz-utils.ts`/
symbols:
  ClusterManager.getAddressFromToken: ClusterManager#getAddressFromToken().
  ClusterManager.createFreeCluster: ClusterManager#createFreeCluster().
  ClusterManager.-constructor: ClusterManager#`<constructor>`().
  ClusterManager.listProjects: ClusterManager#listProjects().
  ClusterManager.describeCluster: ClusterManager#describeCluster().
  ClusterManager.listClusters: ClusterManager#listClusters().
  ClusterManager.makeRequest: ClusterManager#makeRequest().
  CreateFreeClusterWithDetailsResponse: CreateFreeClusterWithDetailsResponse#
  ClusterManager: ClusterManager#
  ClusterManager.listClusters.Promise.typeLiteral31.clusters: ClusterManager#listClusters().Promise:typeLiteral31:clusters.
  DescribeClusterResponse: DescribeClusterResponse#
  DescribeClusterResponse.status: DescribeClusterResponse#status.
  ListProjectsResponse: ListProjectsResponse#
  CreateFreeClusterApiResponse: CreateFreeClusterApiResponse#
  DescribeClusterApiResponse: DescribeClusterApiResponse#
  Project: Project#
  Cluster: Cluster#
  CreateFreeClusterResponse: CreateFreeClusterResponse#
  ClusterManager.token: ClusterManager#token.
  ListClustersResponse.data.typeLiteral0.clusters: ListClustersResponse#data.typeLiteral0:clusters.
  ZillizConfig: ZillizConfig#
  Project.projectId: Project#projectId.
  CreateFreeClusterRequest: CreateFreeClusterRequest#
  CreateFreeClusterResponse.clusterId: CreateFreeClusterResponse#clusterId.
  CreateFreeClusterApiResponse.data: CreateFreeClusterApiResponse#data.
  ClusterManager.baseUrl: ClusterManager#baseUrl.
  ZillizConfig.baseUrl: ZillizConfig#baseUrl.
  ZillizConfig.token: ZillizConfig#token.
  Project.projectName: Project#projectName.
  Cluster.clusterId: Cluster#clusterId.
  Cluster.clusterName: Cluster#clusterName.
  Cluster.connectAddress: Cluster#connectAddress.
  CreateFreeClusterRequest.clusterName: CreateFreeClusterRequest#clusterName.
  CreateFreeClusterRequest.projectId: CreateFreeClusterRequest#projectId.
  CreateFreeClusterRequest.regionId: CreateFreeClusterRequest#regionId.
  CreateFreeClusterWithDetailsResponse.clusterDetails: CreateFreeClusterWithDetailsResponse#clusterDetails.
  ListProjectsResponse.code: ListProjectsResponse#code.
  ListProjectsResponse.data: ListProjectsResponse#data.
  ListClustersResponse: ListClustersResponse#
  ListClustersResponse.code: ListClustersResponse#code.
  ListClustersResponse.data: ListClustersResponse#data.
  CreateFreeClusterApiResponse.code: CreateFreeClusterApiResponse#code.
  DescribeClusterResponse.connectAddress: DescribeClusterResponse#connectAddress.
  DescribeClusterApiResponse.code: DescribeClusterApiResponse#code.
  DescribeClusterApiResponse.data: DescribeClusterApiResponse#data.
  Project.instanceCount: Project#instanceCount.
  Project.createTime: Project#createTime.
  Cluster.description: Cluster#description.
  Cluster.regionId: Cluster#regionId.
  Cluster.plan: Cluster#plan.
  Cluster.cuType: Cluster#cuType.
  Cluster.cuSize: Cluster#cuSize.
  Cluster.status: Cluster#status.
  Cluster.privateLinkAddress: Cluster#privateLinkAddress.
  Cluster.projectId: Cluster#projectId.
  Cluster.createTime: Cluster#createTime.
  CreateFreeClusterResponse.username: CreateFreeClusterResponse#username.
  CreateFreeClusterResponse.password: CreateFreeClusterResponse#password.
  CreateFreeClusterResponse.prompt: CreateFreeClusterResponse#prompt.
  ListClustersResponse.data.typeLiteral0.count: ListClustersResponse#data.typeLiteral0:count.
  ListClustersResponse.data.typeLiteral0.currentPage: ListClustersResponse#data.typeLiteral0:currentPage.
  ListClustersResponse.data.typeLiteral0.pageSize: ListClustersResponse#data.typeLiteral0:pageSize.
  DescribeClusterResponse.clusterId: DescribeClusterResponse#clusterId.
  DescribeClusterResponse.clusterName: DescribeClusterResponse#clusterName.
  DescribeClusterResponse.projectId: DescribeClusterResponse#projectId.
  DescribeClusterResponse.description: DescribeClusterResponse#description.
  DescribeClusterResponse.regionId: DescribeClusterResponse#regionId.
  DescribeClusterResponse.cuType: DescribeClusterResponse#cuType.
  DescribeClusterResponse.plan: DescribeClusterResponse#plan.
  DescribeClusterResponse.privateLinkAddress: DescribeClusterResponse#privateLinkAddress.
  DescribeClusterResponse.createTime: DescribeClusterResponse#createTime.
  DescribeClusterResponse.cuSize: DescribeClusterResponse#cuSize.
  DescribeClusterResponse.storageSize: DescribeClusterResponse#storageSize.
  DescribeClusterResponse.snapshotNumber: DescribeClusterResponse#snapshotNumber.
  DescribeClusterResponse.createProgress: DescribeClusterResponse#createProgress.
  ErrorResponse: ErrorResponse#
  ErrorResponse.code: ErrorResponse#code.
  ErrorResponse.message: ErrorResponse#message.
  ClusterManager.listClusters.Promise.typeLiteral31.count: ClusterManager#listClusters().Promise:typeLiteral31:count.
  ClusterManager.listClusters.Promise.typeLiteral31.currentPage: ClusterManager#listClusters().Promise:typeLiteral31:currentPage.
  ClusterManager.listClusters.Promise.typeLiteral31.pageSize: ClusterManager#listClusters().Promise:typeLiteral31:pageSize.
---
# Module: [`packages/core/src/vectordb/zilliz-utils.ts`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts)

## Classes
### `Cluster`
- def: [`packages/core/src/vectordb/zilliz-utils.ts:15`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L15) — documented in [packages-core-src-vectordb-zilliz-utils.ts](../../../../../concepts/packages-core-src-vectordb-zilliz-utils.ts.md)
- signature: `interface Cluster`
- members:
  - `clusterId` — [`L16`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L16) — documented in [packages-core-src-vectordb-zilliz-utils.ts](../../../../../concepts/packages-core-src-vectordb-zilliz-utils.ts.md)
  - `clusterName` — [`L17`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L17) — documented in [packages-core-src-vectordb-zilliz-utils.ts](../../../../../concepts/packages-core-src-vectordb-zilliz-utils.ts.md)
  - `connectAddress` — [`L24`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L24) — documented in [packages-core-src-vectordb-zilliz-utils.ts](../../../../../concepts/packages-core-src-vectordb-zilliz-utils.ts.md)
  - `createTime` — [`L27`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L27)
  - `cuSize` — [`L22`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L22)
  - `cuType` — [`L21`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L21)
  - `description` — [`L18`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L18)
  - `plan` — [`L20`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L20)
  - `privateLinkAddress` — [`L25`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L25)
  - `projectId` — [`L26`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L26)
  - `regionId` — [`L19`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L19)
  - `status` — [`L23`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L23)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-vectordb-index.ts), [`getAddressFromToken`](zilliz-utils.ts.md#ClusterManager.getAddressFromToken), [`clusters`](zilliz-utils.ts.md#ClusterManager.listClusters.Promise.typeLiteral31.clusters), [`clusters`](zilliz-utils.ts.md#ListClustersResponse.data.typeLiteral0.clusters)

### `ClusterManager`
- def: [`packages/core/src/vectordb/zilliz-utils.ts:100`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L100)
- doc: Zilliz Cloud cluster manager
- signature: `class ClusterManager`
- members:
  - `<constructor>(config?: ZillizConfig | undefined)` — [`L104`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L104) — Zilliz Cloud cluster manager — documented in [packages-core-src-vectordb-zilliz-utils.ts](../../../../../concepts/packages-core-src-vectordb-zilliz-utils.ts.md)
  - `createFreeCluster(method)` — [`L224`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L224) — Create free cluster and wait for it to be ready — documented in [packages-core-src-vectordb-zilliz-utils.ts](../../../../../concepts/packages-core-src-vectordb-zilliz-utils.ts.md)
  - `describeCluster(method)` — [`L207`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L207) — Describe cluster details — documented in [packages-core-src-vectordb-zilliz-utils.ts](../../../../../concepts/packages-core-src-vectordb-zilliz-utils.ts.md)
  - `getAddressFromToken(method)` — [`L278`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L278) — Static utility method to get address from token using Zilliz Cloud API — documented in [packages-core-src-vectordb-zilliz-utils.ts](../../../../../concepts/packages-core-src-vectordb-zilliz-utils.ts.md)
  - `listClusters(method)` — [`L182`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L182) — List all clusters — documented in [packages-core-src-vectordb-zilliz-utils.ts](../../../../../concepts/packages-core-src-vectordb-zilliz-utils.ts.md)
  - `listProjects(method)` — [`L165`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L165) — List all projects — documented in [packages-core-src-vectordb-zilliz-utils.ts](../../../../../concepts/packages-core-src-vectordb-zilliz-utils.ts.md)
  - `makeRequest(method)` — [`L117`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L117) — Generic method for sending HTTP requests — documented in [packages-core-src-vectordb-zilliz-utils.ts](../../../../../concepts/packages-core-src-vectordb-zilliz-utils.ts.md)
  - `baseUrl` — [`L101`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L101) — documented in [packages-core-src-vectordb-zilliz-utils.ts](../../../../../concepts/packages-core-src-vectordb-zilliz-utils.ts.md)
  - `clusters` — [`L183`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L183) — documented in [packages-core-src-vectordb-zilliz-utils.ts](../../../../../concepts/packages-core-src-vectordb-zilliz-utils.ts.md)
  - `count` — [`L184`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L184)
  - `currentPage` — [`L185`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L185)
  - `pageSize` — [`L186`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L186)
  - `token` — [`L102`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L102) — documented in [packages-core-src-vectordb-zilliz-utils.ts](../../../../../concepts/packages-core-src-vectordb-zilliz-utils.ts.md)
- uses (calls/refs, reference-scoped): [`envManager`](../utils/env-manager.ts.md#envManager), [`get`](../utils/env-manager.ts.md#EnvManager.get), [`CreateFreeClusterWithDetailsResponse`](zilliz-utils.ts.md#CreateFreeClusterWithDetailsResponse), [`DescribeClusterResponse`](zilliz-utils.ts.md#DescribeClusterResponse), [`status`](zilliz-utils.ts.md#DescribeClusterResponse.status), [`CreateFreeClusterApiResponse`](zilliz-utils.ts.md#CreateFreeClusterApiResponse), [`DescribeClusterApiResponse`](zilliz-utils.ts.md#DescribeClusterApiResponse), [`ListProjectsResponse`](zilliz-utils.ts.md#ListProjectsResponse), [`Cluster`](zilliz-utils.ts.md#Cluster), [`Project`](zilliz-utils.ts.md#Project), [`CreateFreeClusterRequest`](zilliz-utils.ts.md#CreateFreeClusterRequest), [`ZillizConfig`](zilliz-utils.ts.md#ZillizConfig), [`clusterId`](zilliz-utils.ts.md#CreateFreeClusterResponse.clusterId), [`data`](zilliz-utils.ts.md#CreateFreeClusterApiResponse.data), [`projectId`](zilliz-utils.ts.md#Project.projectId), [`ListClustersResponse`](zilliz-utils.ts.md#ListClustersResponse), [`baseUrl`](zilliz-utils.ts.md#ZillizConfig.baseUrl), [`clusterDetails`](zilliz-utils.ts.md#CreateFreeClusterWithDetailsResponse.clusterDetails), [`clusterId`](zilliz-utils.ts.md#Cluster.clusterId), [`clusterName`](zilliz-utils.ts.md#Cluster.clusterName), [`clusterName`](zilliz-utils.ts.md#CreateFreeClusterRequest.clusterName), [`code`](zilliz-utils.ts.md#CreateFreeClusterApiResponse.code), [`code`](zilliz-utils.ts.md#DescribeClusterApiResponse.code), [`code`](zilliz-utils.ts.md#ListClustersResponse.code), [`code`](zilliz-utils.ts.md#ListProjectsResponse.code), [`connectAddress`](zilliz-utils.ts.md#Cluster.connectAddress), [`connectAddress`](zilliz-utils.ts.md#DescribeClusterResponse.connectAddress), [`data`](zilliz-utils.ts.md#DescribeClusterApiResponse.data), [`data`](zilliz-utils.ts.md#ListClustersResponse.data), [`data`](zilliz-utils.ts.md#ListProjectsResponse.data), [`projectId`](zilliz-utils.ts.md#CreateFreeClusterRequest.projectId), [`projectName`](zilliz-utils.ts.md#Project.projectName), [`regionId`](zilliz-utils.ts.md#CreateFreeClusterRequest.regionId), [`token`](zilliz-utils.ts.md#ZillizConfig.token)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-vectordb-index.ts), [`milvus-restful-vectordb.ts`](milvus-restful-vectordb.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-vectordb-milvus-restful-vectordb.ts), [`milvus-vectordb.ts`](milvus-vectordb.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-vectordb-milvus-vectordb.ts), [`resolveAddress`](milvus-restful-vectordb.ts.md#MilvusRestfulVectorDatabase.resolveAddress), [`resolveAddress`](milvus-vectordb.ts.md#MilvusVectorDatabase.resolveAddress)

### `CreateFreeClusterApiResponse`
- def: [`packages/core/src/vectordb/zilliz-utils.ts:62`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L62) — documented in [packages-core-src-vectordb-zilliz-utils.ts](../../../../../concepts/packages-core-src-vectordb-zilliz-utils.ts.md)
- signature: `interface CreateFreeClusterApiResponse`
- members:
  - `code` — [`L63`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L63)
  - `data` — [`L64`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L64)
- uses (calls/refs, reference-scoped): [`CreateFreeClusterResponse`](zilliz-utils.ts.md#CreateFreeClusterResponse)
- used by: [`createFreeCluster`](zilliz-utils.ts.md#ClusterManager.createFreeCluster)

### `CreateFreeClusterRequest`
- def: [`packages/core/src/vectordb/zilliz-utils.ts:30`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L30) — documented in [packages-core-src-vectordb-zilliz-utils.ts](../../../../../concepts/packages-core-src-vectordb-zilliz-utils.ts.md)
- signature: `interface CreateFreeClusterRequest`
- members:
  - `clusterName` — [`L31`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L31) — documented in [packages-core-src-vectordb-zilliz-utils.ts](../../../../../concepts/packages-core-src-vectordb-zilliz-utils.ts.md)
  - `projectId` — [`L32`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L32) — documented in [packages-core-src-vectordb-zilliz-utils.ts](../../../../../concepts/packages-core-src-vectordb-zilliz-utils.ts.md)
  - `regionId` — [`L33`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L33) — documented in [packages-core-src-vectordb-zilliz-utils.ts](../../../../../concepts/packages-core-src-vectordb-zilliz-utils.ts.md)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-vectordb-index.ts), [`getAddressFromToken`](zilliz-utils.ts.md#ClusterManager.getAddressFromToken), [`createFreeCluster`](zilliz-utils.ts.md#ClusterManager.createFreeCluster)

### `CreateFreeClusterResponse`
- def: [`packages/core/src/vectordb/zilliz-utils.ts:36`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L36)
- signature: `interface CreateFreeClusterResponse`
- members:
  - `clusterId` — [`L37`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L37) — documented in [packages-core-src-vectordb-zilliz-utils.ts](../../../../../concepts/packages-core-src-vectordb-zilliz-utils.ts.md)
  - `password` — [`L39`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L39)
  - `prompt` — [`L40`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L40)
  - `username` — [`L38`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L38)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-vectordb-index.ts), [`getAddressFromToken`](zilliz-utils.ts.md#ClusterManager.getAddressFromToken), [`createFreeCluster`](zilliz-utils.ts.md#ClusterManager.createFreeCluster), [`CreateFreeClusterWithDetailsResponse`](zilliz-utils.ts.md#CreateFreeClusterWithDetailsResponse), [`CreateFreeClusterApiResponse`](zilliz-utils.ts.md#CreateFreeClusterApiResponse)

### `CreateFreeClusterWithDetailsResponse`
- def: [`packages/core/src/vectordb/zilliz-utils.ts:43`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L43) — documented in [packages-core-src-vectordb-zilliz-utils.ts](../../../../../concepts/packages-core-src-vectordb-zilliz-utils.ts.md)
- signature: `interface CreateFreeClusterWithDetailsResponse`
- members:
  - `clusterDetails` — [`L44`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L44) — documented in [packages-core-src-vectordb-zilliz-utils.ts](../../../../../concepts/packages-core-src-vectordb-zilliz-utils.ts.md)
- uses (calls/refs, reference-scoped): [`DescribeClusterResponse`](zilliz-utils.ts.md#DescribeClusterResponse), [`CreateFreeClusterResponse`](zilliz-utils.ts.md#CreateFreeClusterResponse)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-vectordb-index.ts), [`getAddressFromToken`](zilliz-utils.ts.md#ClusterManager.getAddressFromToken), [`createFreeCluster`](zilliz-utils.ts.md#ClusterManager.createFreeCluster)

### `DescribeClusterApiResponse`
- def: [`packages/core/src/vectordb/zilliz-utils.ts:85`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L85) — documented in [packages-core-src-vectordb-zilliz-utils.ts](../../../../../concepts/packages-core-src-vectordb-zilliz-utils.ts.md)
- signature: `interface DescribeClusterApiResponse`
- members:
  - `code` — [`L86`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L86)
  - `data` — [`L87`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L87)
- uses (calls/refs, reference-scoped): [`DescribeClusterResponse`](zilliz-utils.ts.md#DescribeClusterResponse)
- used by: [`describeCluster`](zilliz-utils.ts.md#ClusterManager.describeCluster)

### `DescribeClusterResponse`
- def: [`packages/core/src/vectordb/zilliz-utils.ts:67`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L67) — documented in [packages-core-src-vectordb-zilliz-utils.ts](../../../../../concepts/packages-core-src-vectordb-zilliz-utils.ts.md)
- signature: `interface DescribeClusterResponse`
- members:
  - `clusterId` — [`L68`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L68)
  - `clusterName` — [`L69`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L69)
  - `connectAddress` — [`L76`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L76)
  - `createProgress` — [`L82`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L82)
  - `createTime` — [`L78`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L78)
  - `cuSize` — [`L79`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L79)
  - `cuType` — [`L73`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L73)
  - `description` — [`L71`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L71)
  - `plan` — [`L74`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L74)
  - `privateLinkAddress` — [`L77`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L77)
  - `projectId` — [`L70`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L70)
  - `regionId` — [`L72`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L72)
  - `snapshotNumber` — [`L81`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L81)
  - `status` — [`L75`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L75) — documented in [packages-core-src-vectordb-zilliz-utils.ts](../../../../../concepts/packages-core-src-vectordb-zilliz-utils.ts.md)
  - `storageSize` — [`L80`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L80)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-vectordb-index.ts), [`getAddressFromToken`](zilliz-utils.ts.md#ClusterManager.getAddressFromToken), [`createFreeCluster`](zilliz-utils.ts.md#ClusterManager.createFreeCluster), [`describeCluster`](zilliz-utils.ts.md#ClusterManager.describeCluster), [`CreateFreeClusterWithDetailsResponse`](zilliz-utils.ts.md#CreateFreeClusterWithDetailsResponse), [`DescribeClusterApiResponse`](zilliz-utils.ts.md#DescribeClusterApiResponse)

### `ErrorResponse`
- def: [`packages/core/src/vectordb/zilliz-utils.ts:90`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L90)
- signature: `interface ErrorResponse`
- members:
  - `code` — [`L91`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L91)
  - `message` — [`L92`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L92)

### `ListClustersResponse`
- def: [`packages/core/src/vectordb/zilliz-utils.ts:52`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L52) — documented in [packages-core-src-vectordb-zilliz-utils.ts](../../../../../concepts/packages-core-src-vectordb-zilliz-utils.ts.md)
- signature: `interface ListClustersResponse`
- members:
  - `clusters` — [`L58`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L58)
  - `code` — [`L53`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L53)
  - `count` — [`L55`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L55)
  - `currentPage` — [`L56`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L56)
  - `data` — [`L54`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L54)
  - `pageSize` — [`L57`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L57)
- uses (calls/refs, reference-scoped): [`Cluster`](zilliz-utils.ts.md#Cluster)
- used by: [`listClusters`](zilliz-utils.ts.md#ClusterManager.listClusters)

### `ListProjectsResponse`
- def: [`packages/core/src/vectordb/zilliz-utils.ts:47`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L47) — documented in [packages-core-src-vectordb-zilliz-utils.ts](../../../../../concepts/packages-core-src-vectordb-zilliz-utils.ts.md)
- signature: `interface ListProjectsResponse`
- members:
  - `code` — [`L48`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L48) — documented in [packages-core-src-vectordb-zilliz-utils.ts](../../../../../concepts/packages-core-src-vectordb-zilliz-utils.ts.md)
  - `data` — [`L49`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L49)
- uses (calls/refs, reference-scoped): [`Project`](zilliz-utils.ts.md#Project)
- used by: [`listProjects`](zilliz-utils.ts.md#ClusterManager.listProjects)

### `Project`
- def: [`packages/core/src/vectordb/zilliz-utils.ts:8`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L8) — documented in [packages-core-src-vectordb-zilliz-utils.ts](../../../../../concepts/packages-core-src-vectordb-zilliz-utils.ts.md)
- signature: `interface Project`
- members:
  - `createTime` — [`L12`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L12)
  - `instanceCount` — [`L11`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L11)
  - `projectId` — [`L9`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L9) — documented in [packages-core-src-vectordb-zilliz-utils.ts](../../../../../concepts/packages-core-src-vectordb-zilliz-utils.ts.md)
  - `projectName` — [`L10`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L10) — documented in [packages-core-src-vectordb-zilliz-utils.ts](../../../../../concepts/packages-core-src-vectordb-zilliz-utils.ts.md)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-vectordb-index.ts), [`getAddressFromToken`](zilliz-utils.ts.md#ClusterManager.getAddressFromToken), [`listProjects`](zilliz-utils.ts.md#ClusterManager.listProjects), [`ListProjectsResponse`](zilliz-utils.ts.md#ListProjectsResponse)

### `ZillizConfig`
- def: [`packages/core/src/vectordb/zilliz-utils.ts:3`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L3) — documented in [packages-core-src-vectordb-zilliz-utils.ts](../../../../../concepts/packages-core-src-vectordb-zilliz-utils.ts.md)
- signature: `interface ZillizConfig`
- members:
  - `baseUrl` — [`L4`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L4) — documented in [packages-core-src-vectordb-zilliz-utils.ts](../../../../../concepts/packages-core-src-vectordb-zilliz-utils.ts.md)
  - `token` — [`L5`](../../../../../../../../raw/code/claude-context/packages/core/src/vectordb/zilliz-utils.ts#L5) — documented in [packages-core-src-vectordb-zilliz-utils.ts](../../../../../concepts/packages-core-src-vectordb-zilliz-utils.ts.md)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-vectordb-index.ts), [`<constructor>`](zilliz-utils.ts.md#ClusterManager.-constructor)

