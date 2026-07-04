---
title: 'Module: understand-anything-plugin/packages/core/src/persistence/index.ts'
type: catalog
provenance: extracted
module: understand-anything-plugin/packages/core/src/persistence/index.ts
status: fresh
symbol_base: scip-typescript npm @understand-anything/core 0.1.0 src/persistence/`index.ts`/
symbols:
  loadGraph: loadGraph().
  loadDomainGraph: loadDomainGraph().
  saveGraph: saveGraph().
  loadConfig: loadConfig().
  saveDomainGraph: saveDomainGraph().
  loadFingerprints: loadFingerprints().
  saveMeta: saveMeta().
  loadMeta: loadMeta().
  saveFingerprints: saveFingerprints().
  saveConfig: saveConfig().
  sanitiseFilePaths: sanitiseFilePaths().
  DEFAULT_CONFIG: DEFAULT_CONFIG.
  ensureDir: ensureDir().
  UA_DIR: UA_DIR.
  GRAPH_FILE: GRAPH_FILE.
  META_FILE: META_FILE.
  FINGERPRINT_FILE: FINGERPRINT_FILE.
  CONFIG_FILE: CONFIG_FILE.
  DOMAIN_GRAPH_FILE: DOMAIN_GRAPH_FILE.
  loadGraph.options-typeLiteral29.validate: loadGraph().(options)typeLiteral29:validate.
  loadDomainGraph.options-typeLiteral63.validate: loadDomainGraph().(options)typeLiteral63:validate.
---
# Module: [`understand-anything-plugin/packages/core/src/persistence/index.ts`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/persistence/index.ts)

## Functions
- `ensureDir(projectRoot: string)` — [`L13`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/persistence/index.ts#L13) — documented in [understand-anything-plugin-packages-core-src-persistence-index.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-persistence-index.ts.md)
- `loadConfig(projectRoot: string)` — [`L140`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/persistence/index.ts#L140) — documented in [understand-anything-plugin-packages-core-src-persistence-index.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-persistence-index.ts.md)
- `loadDomainGraph(projectRoot: string, options?: { validate?: boolean | undefined; } | undefined)` — [`L162`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/persistence/index.ts#L162) — documented in [understand-anything-plugin-packages-core-src-persistence-index.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-persistence-index.ts.md)
- `loadFingerprints(projectRoot: string)` — [`L123`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/persistence/index.ts#L123)
- `loadGraph(projectRoot: string, options?: { validate?: boolean | undefined; } | undefined)` — [`L85`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/persistence/index.ts#L85) — documented in [understand-anything-plugin-packages-core-src-persistence-index.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-persistence-index.ts.md)
- `loadMeta(projectRoot: string)` — [`L112`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/persistence/index.ts#L112)
- `sanitiseFilePaths(graph: KnowledgeGraph, projectRoot: string)` — [`L38`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/persistence/index.ts#L38) — Sanitise every node's filePath before writing to disk. — documented in [understand-anything-plugin-packages-core-src-persistence-index.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-persistence-index.ts.md)
- `saveConfig(projectRoot: string, config: ProjectConfig)` — [`L135`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/persistence/index.ts#L135)
- `saveDomainGraph(projectRoot: string, graph: KnowledgeGraph)` — [`L152`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/persistence/index.ts#L152)
- `saveFingerprints(projectRoot: string, store: FingerprintStore)` — [`L118`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/persistence/index.ts#L118)
- `saveGraph(projectRoot: string, graph: KnowledgeGraph)` — [`L69`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/persistence/index.ts#L69) — documented in [understand-anything-plugin-packages-core-src-persistence-index.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-persistence-index.ts.md)
- `saveMeta(projectRoot: string, meta: AnalysisMeta)` — [`L107`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/persistence/index.ts#L107)

## Module values
- `CONFIG_FILE` — [`L11`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/persistence/index.ts#L11) — documented in [understand-anything-plugin-packages-core-src-persistence-index.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-persistence-index.ts.md)
- `DEFAULT_CONFIG` — [`L133`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/persistence/index.ts#L133) — documented in [understand-anything-plugin-packages-core-src-persistence-index.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-persistence-index.ts.md)
- `DOMAIN_GRAPH_FILE` — [`L150`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/persistence/index.ts#L150) — documented in [understand-anything-plugin-packages-core-src-persistence-index.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-persistence-index.ts.md)
- `FINGERPRINT_FILE` — [`L10`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/persistence/index.ts#L10)
- `GRAPH_FILE` — [`L8`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/persistence/index.ts#L8) — documented in [understand-anything-plugin-packages-core-src-persistence-index.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-persistence-index.ts.md)
- `META_FILE` — [`L9`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/persistence/index.ts#L9)
- `UA_DIR` — [`L7`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/persistence/index.ts#L7) — documented in [understand-anything-plugin-packages-core-src-persistence-index.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-persistence-index.ts.md)
- `validate` — [`L87`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/persistence/index.ts#L87) — documented in [understand-anything-plugin-packages-core-src-persistence-index.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-persistence-index.ts.md)
- `validate` — [`L164`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/persistence/index.ts#L164) — documented in [understand-anything-plugin-packages-core-src-persistence-index.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-persistence-index.ts.md)

