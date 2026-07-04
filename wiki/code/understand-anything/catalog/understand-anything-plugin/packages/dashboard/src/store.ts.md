---
title: 'Module: understand-anything-plugin/packages/dashboard/src/store.ts'
type: catalog
provenance: extracted
module: understand-anything-plugin/packages/dashboard/src/store.ts
status: fresh
symbol_base: scip-typescript npm @understand-anything/dashboard 0.1.0 src/`store.ts`/
symbols:
  useDashboardStore: useDashboardStore.
  DEFAULT_FILTERS: DEFAULT_FILTERS.
  layerResetIfChanged: layerResetIfChanged().
  EdgeCategory: EdgeCategory#
  navigateTourToLayer: navigateTourToLayer().
  NodeType: NodeType#
  Complexity: Complexity#
  ALL_NODE_TYPES: ALL_NODE_TYPES.
  ALL_COMPLEXITIES: ALL_COMPLEXITIES.
  ALL_EDGE_CATEGORIES: ALL_EDGE_CATEGORIES.
  FilterState: FilterState#
  buildGraphIndexes: buildGraphIndexes().
  FilterState.nodeTypes: FilterState#nodeTypes.
  FilterState.complexities: FilterState#complexities.
  FilterState.edgeCategories: FilterState#edgeCategories.
  EDGE_CATEGORY_MAP: EDGE_CATEGORY_MAP.
  FilterState.layerIds: FilterState#layerIds.
  Persona: Persona#
  NodeCategory: NodeCategory#
  DashboardStore: DashboardStore#
  getSortedTour: getSortedTour().
  DashboardStore.navigationLevel: DashboardStore#navigationLevel.
  MAX_HISTORY: MAX_HISTORY.
  DOMAIN_EDGE_TYPES: DOMAIN_EDGE_TYPES.
  DashboardStore.persona: DashboardStore#persona.
  DashboardStore.filters: DashboardStore#filters.
  DashboardStore.nodeTypeFilters: DashboardStore#nodeTypeFilters.
  DashboardStore.toggleNodeTypeFilter: DashboardStore#toggleNodeTypeFilter.
  DashboardStore.detailLevel: DashboardStore#detailLevel.
  DashboardStore.setDetailLevel: DashboardStore#setDetailLevel.
  DashboardStore.setPersona: DashboardStore#setPersona.
  DashboardStore.setFilters: DashboardStore#setFilters.
  DashboardStore.viewMode: DashboardStore#viewMode.
  DashboardStore.setViewMode: DashboardStore#setViewMode.
  ViewMode: ViewMode#
  DetailLevel: DetailLevel#
  buildGraphIndexes.typeLiteral8.nodesById: buildGraphIndexes().typeLiteral8:nodesById.
  buildGraphIndexes.typeLiteral8.nodeIdToLayerId: buildGraphIndexes().typeLiteral8:nodeIdToLayerId.
  buildGraphIndexes.typeLiteral8.nodeIdToLayerIds: buildGraphIndexes().typeLiteral8:nodeIdToLayerIds.
  DashboardStore.activeLayerId: DashboardStore#activeLayerId.
  NavigationLevel: NavigationLevel#
  DashboardStore.expandedContainers: DashboardStore#expandedContainers.
  DashboardStore.pendingFocusContainer: DashboardStore#pendingFocusContainer.
  DashboardStore.containerLayoutCache: DashboardStore#containerLayoutCache.
  DashboardStore.containerSizeMemory: DashboardStore#containerSizeMemory.
  DashboardStore.graph: DashboardStore#graph.
  DashboardStore.nodesById: DashboardStore#nodesById.
  DashboardStore.nodeIdToLayerId: DashboardStore#nodeIdToLayerId.
  DashboardStore.nodeIdToLayerIds: DashboardStore#nodeIdToLayerIds.
  DashboardStore.selectedNodeId: DashboardStore#selectedNodeId.
  DashboardStore.searchQuery: DashboardStore#searchQuery.
  DashboardStore.searchResults: DashboardStore#searchResults.
  DashboardStore.searchEngine: DashboardStore#searchEngine.
  DashboardStore.searchMode: DashboardStore#searchMode.
  DashboardStore.setSearchMode: DashboardStore#setSearchMode.
  DashboardStore.codeViewerOpen: DashboardStore#codeViewerOpen.
  DashboardStore.codeViewerNodeId: DashboardStore#codeViewerNodeId.
  DashboardStore.codeViewerExpanded: DashboardStore#codeViewerExpanded.
  DashboardStore.tourActive: DashboardStore#tourActive.
  DashboardStore.currentTourStep: DashboardStore#currentTourStep.
  DashboardStore.tourHighlightedNodeIds: DashboardStore#tourHighlightedNodeIds.
  DashboardStore.diffMode: DashboardStore#diffMode.
  DashboardStore.changedNodeIds: DashboardStore#changedNodeIds.
  DashboardStore.affectedNodeIds: DashboardStore#affectedNodeIds.
  DashboardStore.focusNodeId: DashboardStore#focusNodeId.
  DashboardStore.nodeHistory: DashboardStore#nodeHistory.
  DashboardStore.filterPanelOpen: DashboardStore#filterPanelOpen.
  DashboardStore.exportMenuOpen: DashboardStore#exportMenuOpen.
  DashboardStore.pathFinderOpen: DashboardStore#pathFinderOpen.
  DashboardStore.reactFlowInstance: DashboardStore#reactFlowInstance.
  DashboardStore.showFunctionsInClassView: DashboardStore#showFunctionsInClassView.
  DashboardStore.toggleShowFunctionsInClassView: DashboardStore#toggleShowFunctionsInClassView.
  DashboardStore.setGraph: DashboardStore#setGraph.
  DashboardStore.selectNode: DashboardStore#selectNode.
  DashboardStore.navigateToNode: DashboardStore#navigateToNode.
  DashboardStore.navigateToNodeInLayer: DashboardStore#navigateToNodeInLayer.
  DashboardStore.navigateToHistoryIndex: DashboardStore#navigateToHistoryIndex.
  DashboardStore.goBackNode: DashboardStore#goBackNode.
  DashboardStore.drillIntoLayer: DashboardStore#drillIntoLayer.
  DashboardStore.navigateToOverview: DashboardStore#navigateToOverview.
  DashboardStore.setFocusNode: DashboardStore#setFocusNode.
  DashboardStore.setSearchQuery: DashboardStore#setSearchQuery.
  DashboardStore.openCodeViewer: DashboardStore#openCodeViewer.
  DashboardStore.closeCodeViewer: DashboardStore#closeCodeViewer.
  DashboardStore.expandCodeViewer: DashboardStore#expandCodeViewer.
  DashboardStore.collapseCodeViewer: DashboardStore#collapseCodeViewer.
  DashboardStore.setDiffOverlay: DashboardStore#setDiffOverlay.
  DashboardStore.toggleDiffMode: DashboardStore#toggleDiffMode.
  DashboardStore.clearDiffOverlay: DashboardStore#clearDiffOverlay.
  DashboardStore.toggleFilterPanel: DashboardStore#toggleFilterPanel.
  DashboardStore.toggleExportMenu: DashboardStore#toggleExportMenu.
  DashboardStore.togglePathFinder: DashboardStore#togglePathFinder.
  DashboardStore.setReactFlowInstance: DashboardStore#setReactFlowInstance.
  DashboardStore.resetFilters: DashboardStore#resetFilters.
  DashboardStore.hasActiveFilters: DashboardStore#hasActiveFilters.
  DashboardStore.startTour: DashboardStore#startTour.
  DashboardStore.stopTour: DashboardStore#stopTour.
  DashboardStore.setTourStep: DashboardStore#setTourStep.
  DashboardStore.nextTourStep: DashboardStore#nextTourStep.
  DashboardStore.prevTourStep: DashboardStore#prevTourStep.
  DashboardStore.isKnowledgeGraph: DashboardStore#isKnowledgeGraph.
  DashboardStore.domainGraph: DashboardStore#domainGraph.
  DashboardStore.activeDomainId: DashboardStore#activeDomainId.
  DashboardStore.setDomainGraph: DashboardStore#setDomainGraph.
  DashboardStore.setIsKnowledgeGraph: DashboardStore#setIsKnowledgeGraph.
  DashboardStore.navigateToDomain: DashboardStore#navigateToDomain.
  DashboardStore.clearActiveDomain: DashboardStore#clearActiveDomain.
  DashboardStore.toggleContainer: DashboardStore#toggleContainer.
  DashboardStore.expandContainer: DashboardStore#expandContainer.
  DashboardStore.collapseContainer: DashboardStore#collapseContainer.
  DashboardStore.collapseAllContainers: DashboardStore#collapseAllContainers.
  DashboardStore.setPendingFocusContainer: DashboardStore#setPendingFocusContainer.
  DashboardStore.tourFitPending: DashboardStore#tourFitPending.
  DashboardStore.setTourFitPending: DashboardStore#setTourFitPending.
  DashboardStore.containerLayoutCache.Map.typeLiteral83.childPositions: DashboardStore#containerLayoutCache.Map:typeLiteral83:childPositions.
  DashboardStore.containerLayoutCache.Map.typeLiteral83.childPositions.Map.typeLiteral84.x: DashboardStore#containerLayoutCache.Map:typeLiteral83:childPositions.Map:typeLiteral84:x.
  DashboardStore.containerLayoutCache.Map.typeLiteral83.childPositions.Map.typeLiteral84.y: DashboardStore#containerLayoutCache.Map:typeLiteral83:childPositions.Map:typeLiteral84:y.
  DashboardStore.containerLayoutCache.Map.typeLiteral83.actualSize: DashboardStore#containerLayoutCache.Map:typeLiteral83:actualSize.
  DashboardStore.containerLayoutCache.Map.typeLiteral83.actualSize.typeLiteral85.width: DashboardStore#containerLayoutCache.Map:typeLiteral83:actualSize.typeLiteral85:width.
  DashboardStore.containerLayoutCache.Map.typeLiteral83.actualSize.typeLiteral85.height: DashboardStore#containerLayoutCache.Map:typeLiteral83:actualSize.typeLiteral85:height.
  DashboardStore.setContainerLayout: DashboardStore#setContainerLayout.
  DashboardStore.clearContainerLayouts: DashboardStore#clearContainerLayouts.
  DashboardStore.containerSizeMemory.Map.typeLiteral97.width: DashboardStore#containerSizeMemory.Map:typeLiteral97:width.
  DashboardStore.containerSizeMemory.Map.typeLiteral97.height: DashboardStore#containerSizeMemory.Map:typeLiteral97:height.
  DashboardStore.stage1Tick: DashboardStore#stage1Tick.
  DashboardStore.bumpStage1Tick: DashboardStore#bumpStage1Tick.
  DashboardStore.layoutIssues: DashboardStore#layoutIssues.
  DashboardStore.appendLayoutIssues: DashboardStore#appendLayoutIssues.
  DashboardStore.clearLayoutIssues: DashboardStore#clearLayoutIssues.
---
# Module: [`understand-anything-plugin/packages/dashboard/src/store.ts`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts)

## Classes
### `Complexity`
- def: [`understand-anything-plugin/packages/dashboard/src/store.ts:15`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L15) — documented in [understand-anything-plugin-packages-dashboard-src-store.ts](../../../../../concepts/understand-anything-plugin-packages-dashboard-src-store.ts.md)
- signature: `type Complexity`
- used by: [`store.ts`](store.ts.md#scip-typescript-npm-understand-anything-dashboard-0.1.0-src-store.ts), [`defaultFilters`](utils/__tests__/filters.test.ts.md#defaultFilters), [`filters.test.ts`](utils/__tests__/filters.test.ts.md#scip-typescript-npm-understand-anything-dashboard-0.1.0-src-utils-__tests__-filters.test.ts), [`DEFAULT_FILTERS`](store.ts.md#DEFAULT_FILTERS), [`FilterPanel.tsx`](components/FilterPanel.tsx.md#scip-typescript-npm-understand-anything-dashboard-0.1.0-src-components-FilterPanel.tsx), [`FilterPanel`](components/FilterPanel.tsx.md#FilterPanel), [`filterNodes`](utils/filters.ts.md#filterNodes), [`node`](utils/__tests__/filters.test.ts.md#node), [`filters.ts`](utils/filters.ts.md#scip-typescript-npm-understand-anything-dashboard-0.1.0-src-utils-filters.ts), [`ALL_COMPLEXITIES`](store.ts.md#ALL_COMPLEXITIES), [`complexities`](store.ts.md#FilterState.complexities)

### `DashboardStore`
- def: [`understand-anything-plugin/packages/dashboard/src/store.ts:100`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L100)
- signature: `interface DashboardStore`
- members:
  - `activeDomainId` — [`L195`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L195)
  - `activeLayerId` — [`L117`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L117)
  - `actualSize` — [`L220`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L220)
  - `affectedNodeIds` — [`L131`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L131)
  - `appendLayoutIssues` — [`L238`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L238)
  - `bumpStage1Tick` — [`L233`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L233)
  - `changedNodeIds` — [`L130`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L130)
  - `childPositions` — [`L219`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L219)
  - `clearActiveDomain` — [`L201`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L201)
  - `clearContainerLayouts` — [`L228`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L228)
  - `clearDiffOverlay` — [`L175`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L175)
  - `clearLayoutIssues` — [`L239`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L239)
  - `closeCodeViewer` — [`L169`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L169)
  - `codeViewerExpanded` — [`L121`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L121)
  - `codeViewerNodeId` — [`L120`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L120)
  - `codeViewerOpen` — [`L119`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L119)
  - `collapseAllContainers` — [`L208`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L208)
  - `collapseCodeViewer` — [`L171`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L171)
  - `collapseContainer` — [`L207`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L207)
  - `containerLayoutCache` — [`L216`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L216)
  - `containerSizeMemory` — [`L230`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L230)
  - `currentTourStep` — [`L124`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L124)
  - `detailLevel` — [`L152`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L152)
  - `diffMode` — [`L129`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L129)
  - `domainGraph` — [`L194`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L194)
  - `drillIntoLayer` — [`L163`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L163)
  - `expandCodeViewer` — [`L170`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L170)
  - `expandContainer` — [`L206`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L206)
  - `expandedContainers` — [`L204`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L204)
  - `exportMenuOpen` — [`L142`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L142)
  - `filterPanelOpen` — [`L141`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L141)
  - `filters` — [`L140`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L140)
  - `focusNodeId` — [`L134`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L134)
  - `goBackNode` — [`L162`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L162)
  - `graph` — [`L101`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L101)
  - `hasActiveFilters` — [`L183`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L183)
  - `height` — [`L220`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L220)
  - `height` — [`L230`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L230)
  - `isKnowledgeGraph` — [`L193`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L193)
  - `layoutIssues` — [`L237`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L237)
  - `navigateToDomain` — [`L200`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L200)
  - `navigateToHistoryIndex` — [`L161`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L161)
  - `navigateToNode` — [`L159`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L159)
  - `navigateToNodeInLayer` — [`L160`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L160)
  - `navigateToOverview` — [`L164`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L164)
  - `navigationLevel` — [`L116`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L116)
  - `nextTourStep` — [`L188`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L188)
  - `nodeHistory` — [`L137`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L137)
  - `nodeIdToLayerId` — [`L105`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L105) — id → layer id (first-matching-layer wins), rebuilt by setGraph. Empty before any graph loads.
  - `nodeIdToLayerIds` — [`L107`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L107) — id → set of every layer the node belongs to, rebuilt by setGraph. Empty before any graph loads.
  - `nodeTypeFilters` — [`L147`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L147)
  - `nodesById` — [`L103`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L103) — id → node lookup, rebuilt by setGraph. Empty before any graph loads.
  - `openCodeViewer` — [`L168`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L168)
  - `pathFinderOpen` — [`L143`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L143)
  - `pendingFocusContainer` — [`L210`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L210) — Container the user just manually expanded; viewport should lock onto it. Cleared by GraphView once the lock is applied.
  - `persona` — [`L127`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L127)
  - `prevTourStep` — [`L189`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L189)
  - `reactFlowInstance` — [`L144`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L144)
  - `resetFilters` — [`L182`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L182)
  - `searchEngine` — [`L111`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L111)
  - `searchMode` — [`L112`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L112)
  - `searchQuery` — [`L109`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L109)
  - `searchResults` — [`L110`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L110)
  - `selectNode` — [`L158`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L158)
  - `selectedNodeId` — [`L108`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L108)
  - `setContainerLayout` — [`L223`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L223)
  - `setDetailLevel` — [`L153`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L153)
  - `setDiffOverlay` — [`L173`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L173)
  - `setDomainGraph` — [`L197`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L197)
  - `setFilters` — [`L181`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L181)
  - `setFocusNode` — [`L165`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L165)
  - `setGraph` — [`L157`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L157)
  - `setIsKnowledgeGraph` — [`L199`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L199)
  - `setPendingFocusContainer` — [`L211`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L211)
  - `setPersona` — [`L167`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L167)
  - `setReactFlowInstance` — [`L180`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L180)
  - `setSearchMode` — [`L113`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L113)
  - `setSearchQuery` — [`L166`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L166)
  - `setTourFitPending` — [`L214`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L214)
  - `setTourStep` — [`L187`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L187)
  - `setViewMode` — [`L198`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L198)
  - `showFunctionsInClassView` — [`L154`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L154)
  - `stage1Tick` — [`L232`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L232)
  - `startTour` — [`L185`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L185)
  - `stopTour` — [`L186`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L186)
  - `toggleContainer` — [`L205`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L205)
  - `toggleDiffMode` — [`L174`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L174)
  - `toggleExportMenu` — [`L178`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L178)
  - `toggleFilterPanel` — [`L177`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L177)
  - `toggleNodeTypeFilter` — [`L148`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L148)
  - `togglePathFinder` — [`L179`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L179)
  - `toggleShowFunctionsInClassView` — [`L155`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L155)
  - `tourActive` — [`L123`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L123)
  - `tourFitPending` — [`L213`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L213) — True while TourFitView is waiting for highlighted nodes to materialise (Stage 2 layout in progress). Drives the "Computing layout…" overlay.
  - `tourHighlightedNodeIds` — [`L125`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L125)
  - `viewMode` — [`L192`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L192)
  - `width` — [`L220`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L220)
  - `width` — [`L230`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L230)
  - `x` — [`L219`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L219)
  - `y` — [`L219`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L219)
- uses (calls/refs, reference-scoped): [`FilterState`](store.ts.md#FilterState), [`NodeCategory`](store.ts.md#NodeCategory), [`Persona`](store.ts.md#Persona), [`DetailLevel`](store.ts.md#DetailLevel), [`ViewMode`](store.ts.md#ViewMode), [`NavigationLevel`](store.ts.md#NavigationLevel)
- used by: [`store.ts`](store.ts.md#scip-typescript-npm-understand-anything-dashboard-0.1.0-src-store.ts), [`layerResetIfChanged`](store.ts.md#layerResetIfChanged), [`navigateTourToLayer`](store.ts.md#navigateTourToLayer)

### `DetailLevel`
- def: [`understand-anything-plugin/packages/dashboard/src/store.ts:18`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L18)
- signature: `type DetailLevel`
- used by: [`detailLevel`](store.ts.md#DashboardStore.detailLevel), [`setDetailLevel`](store.ts.md#DashboardStore.setDetailLevel)

### `EdgeCategory`
- def: [`understand-anything-plugin/packages/dashboard/src/store.ts:16`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L16) — documented in [understand-anything-plugin-packages-dashboard-src-store.ts](../../../../../concepts/understand-anything-plugin-packages-dashboard-src-store.ts.md)
- signature: `type EdgeCategory`
- used by: [`store.ts`](store.ts.md#scip-typescript-npm-understand-anything-dashboard-0.1.0-src-store.ts), [`defaultFilters`](utils/__tests__/filters.test.ts.md#defaultFilters), [`filters.test.ts`](utils/__tests__/filters.test.ts.md#scip-typescript-npm-understand-anything-dashboard-0.1.0-src-utils-__tests__-filters.test.ts), [`DEFAULT_FILTERS`](store.ts.md#DEFAULT_FILTERS), [`FilterPanel.tsx`](components/FilterPanel.tsx.md#scip-typescript-npm-understand-anything-dashboard-0.1.0-src-components-FilterPanel.tsx), [`FilterPanel`](components/FilterPanel.tsx.md#FilterPanel), [`filters.ts`](utils/filters.ts.md#scip-typescript-npm-understand-anything-dashboard-0.1.0-src-utils-filters.ts), [`ALL_EDGE_CATEGORIES`](store.ts.md#ALL_EDGE_CATEGORIES), [`edgeCategories`](store.ts.md#FilterState.edgeCategories), [`getEdgeCategory`](utils/filters.ts.md#getEdgeCategory), [`EDGE_CATEGORY_MAP`](store.ts.md#EDGE_CATEGORY_MAP)

### `FilterState`
- def: [`understand-anything-plugin/packages/dashboard/src/store.ts:20`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L20) — documented in [understand-anything-plugin-packages-dashboard-src-store.ts](../../../../../concepts/understand-anything-plugin-packages-dashboard-src-store.ts.md)
- signature: `interface FilterState`
- members:
  - `complexities` — [`L22`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L22)
  - `edgeCategories` — [`L24`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L24)
  - `layerIds` — [`L23`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L23)
  - `nodeTypes` — [`L21`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L21)
- uses (calls/refs, reference-scoped): [`EdgeCategory`](store.ts.md#EdgeCategory), [`Complexity`](store.ts.md#Complexity), [`NodeType`](store.ts.md#NodeType)
- used by: [`store.ts`](store.ts.md#scip-typescript-npm-understand-anything-dashboard-0.1.0-src-store.ts), [`defaultFilters`](utils/__tests__/filters.test.ts.md#defaultFilters), [`filters.test.ts`](utils/__tests__/filters.test.ts.md#scip-typescript-npm-understand-anything-dashboard-0.1.0-src-utils-__tests__-filters.test.ts), [`DEFAULT_FILTERS`](store.ts.md#DEFAULT_FILTERS), [`filterNodes`](utils/filters.ts.md#filterNodes), [`filters.ts`](utils/filters.ts.md#scip-typescript-npm-understand-anything-dashboard-0.1.0-src-utils-filters.ts), [`filterEdges`](utils/filters.ts.md#filterEdges), [`filters`](store.ts.md#DashboardStore.filters), [`setFilters`](store.ts.md#DashboardStore.setFilters)

### `NavigationLevel`
- def: [`understand-anything-plugin/packages/dashboard/src/store.ts:13`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L13)
- signature: `type NavigationLevel`
- used by: [`navigationLevel`](store.ts.md#DashboardStore.navigationLevel)

### `NodeCategory`
- def: [`understand-anything-plugin/packages/dashboard/src/store.ts:52`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L52)
- doc: Categories used for node type filter toggles. Single source of truth for NodeCategory.
- signature: `type NodeCategory`
- used by: [`nodeTypes`](components/GraphView.tsx.md#nodeTypes), [`NODE_TYPE_TO_CATEGORY`](components/GraphView.tsx.md#NODE_TYPE_TO_CATEGORY), [`nodeTypeFilters`](store.ts.md#DashboardStore.nodeTypeFilters), [`toggleNodeTypeFilter`](store.ts.md#DashboardStore.toggleNodeTypeFilter)

### `NodeType`
- def: [`understand-anything-plugin/packages/dashboard/src/store.ts:14`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L14) — documented in [understand-anything-plugin-packages-dashboard-src-store.ts](../../../../../concepts/understand-anything-plugin-packages-dashboard-src-store.ts.md)
- signature: `type NodeType`
- used by: [`store.ts`](store.ts.md#scip-typescript-npm-understand-anything-dashboard-0.1.0-src-store.ts), [`defaultFilters`](utils/__tests__/filters.test.ts.md#defaultFilters), [`filters.test.ts`](utils/__tests__/filters.test.ts.md#scip-typescript-npm-understand-anything-dashboard-0.1.0-src-utils-__tests__-filters.test.ts), [`DEFAULT_FILTERS`](store.ts.md#DEFAULT_FILTERS), [`FilterPanel.tsx`](components/FilterPanel.tsx.md#scip-typescript-npm-understand-anything-dashboard-0.1.0-src-components-FilterPanel.tsx), [`FilterPanel`](components/FilterPanel.tsx.md#FilterPanel), [`filterNodes`](utils/filters.ts.md#filterNodes), [`node`](utils/__tests__/filters.test.ts.md#node), [`filters.ts`](utils/filters.ts.md#scip-typescript-npm-understand-anything-dashboard-0.1.0-src-utils-filters.ts), [`ALL_NODE_TYPES`](store.ts.md#ALL_NODE_TYPES), [`nodeTypes`](store.ts.md#FilterState.nodeTypes)

### `Persona`
- def: [`understand-anything-plugin/packages/dashboard/src/store.ts:12`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L12)
- signature: `type Persona`
- used by: [`PersonaSelector.tsx`](components/PersonaSelector.tsx.md#scip-typescript-npm-understand-anything-dashboard-0.1.0-src-components-PersonaSelector.tsx), [`PersonaSelector`](components/PersonaSelector.tsx.md#PersonaSelector), [`persona`](store.ts.md#DashboardStore.persona), [`setPersona`](store.ts.md#DashboardStore.setPersona)

### `ViewMode`
- def: [`understand-anything-plugin/packages/dashboard/src/store.ts:17`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L17)
- signature: `type ViewMode`
- used by: [`setViewMode`](store.ts.md#DashboardStore.setViewMode), [`viewMode`](store.ts.md#DashboardStore.viewMode)

## Functions
- `buildGraphIndexes(graph: KnowledgeGraph)` — [`L74`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L74) — Build the (id → node) and (id → layerId) lookup maps that the rest of
- `getSortedTour(graph: KnowledgeGraph)` — [`L242`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L242)
- `layerResetIfChanged(layerNav: Partial<DashboardStore>, prevLayerId: string | null)` — [`L272`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L272) — Container ids derive from per-layer state — folder names in folder-strategy — documented in [understand-anything-plugin-packages-dashboard-src-store.ts](../../../../../concepts/understand-anything-plugin-packages-dashboard-src-store.ts.md)
- `navigateTourToLayer(nodeIdToLayerId: Map<string, string>, nodeIds: string[])` — [`L248`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L248) — Navigate tour step to the correct layer for the first highlighted node.

## Module values
- `ALL_COMPLEXITIES` — [`L28`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L28) — documented in [understand-anything-plugin-packages-dashboard-src-store.ts](../../../../../concepts/understand-anything-plugin-packages-dashboard-src-store.ts.md)
- `ALL_EDGE_CATEGORIES` — [`L29`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L29) — documented in [understand-anything-plugin-packages-dashboard-src-store.ts](../../../../../concepts/understand-anything-plugin-packages-dashboard-src-store.ts.md)
- `ALL_NODE_TYPES` — [`L27`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L27) — documented in [understand-anything-plugin-packages-dashboard-src-store.ts](../../../../../concepts/understand-anything-plugin-packages-dashboard-src-store.ts.md)
- `DEFAULT_FILTERS` — [`L44`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L44) — documented in [understand-anything-plugin-packages-dashboard-src-store.ts](../../../../../concepts/understand-anything-plugin-packages-dashboard-src-store.ts.md)
- `DOMAIN_EDGE_TYPES` — [`L42`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L42)
- `EDGE_CATEGORY_MAP` — [`L31`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L31)
- `MAX_HISTORY` — [`L98`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L98) — Maximum number of entries in the sidebar navigation history.
- `nodeIdToLayerId` — [`L76`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L76)
- `nodeIdToLayerIds` — [`L77`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L77)
- `nodesById` — [`L75`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L75)
- `useDashboardStore` — [`L289`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/store.ts#L289) — documented in [understand-anything-plugin-packages-dashboard-src-components-FileExplorer.tsx](../../../../../concepts/understand-anything-plugin-packages-dashboard-src-components-FileExplorer.tsx.md)

