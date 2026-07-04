---
title: 'Module: src/installer/targets/hermes.ts'
type: catalog
provenance: extracted
module: src/installer/targets/hermes.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/installer/targets/`hermes.ts`/
symbols:
  HermesTarget.uninstall: HermesTarget#uninstall().
  writeHermesConfig: writeHermesConfig().
  upsertCodeGraphMcpServer: upsertCodeGraphMcpServer().
  HermesTarget.detect: HermesTarget#detect().
  removeCodeGraphMcpServer: removeCodeGraphMcpServer().
  upsertCodeGraphToolset: upsertCodeGraphToolset().
  removeCodeGraphToolset: removeCodeGraphToolset().
  LineRange.typeLiteral3.end: LineRange#typeLiteral3:end.
  HermesTarget.install: HermesTarget#install().
  childRange: childRange().
  listChildBlock: listChildBlock().
  LineRange.typeLiteral3.start: LineRange#typeLiteral3:start.
  joinLines: joinLines().
  hasCodeGraphMcpServer: hasCodeGraphMcpServer().
  HermesTarget.printConfig: HermesTarget#printConfig().
  configPath: configPath().
  topLevelRange: topLevelRange().
  LineRange: LineRange#
  HermesTarget.describePaths: HermesTarget#describePaths().
  splitLines: splitLines().
  renderCodeGraphMcpBlock: renderCodeGraphMcpBlock().
  HermesTarget: HermesTarget#
  readText: readText().
  HermesTarget.supportsLocation: HermesTarget#supportsLocation().
  hermesHome: hermesHome().
  ensureTrailingNewline: ensureTrailingNewline().
  escapeRegExp: escapeRegExp().
  renderCodeGraphMcpChild: renderCodeGraphMcpChild().
  hermesTarget: hermesTarget.
  arrayEqual: arrayEqual().
  HermesTarget.id: HermesTarget#id.
  HermesTarget.displayName: HermesTarget#displayName.
  HermesTarget.docsUrl: HermesTarget#docsUrl.
---
# Module: [`src/installer/targets/hermes.ts`](../../../../../../../raw/code/codegraph/src/installer/targets/hermes.ts)

## Classes
### `HermesTarget`  ·  implements/extends AgentTarget
- def: [`src/installer/targets/hermes.ts:31`](../../../../../../../raw/code/codegraph/src/installer/targets/hermes.ts#L31)
- signature: `class HermesTarget`
- members:
  - `describePaths(method)` — [`L100`](../../../../../../../raw/code/codegraph/src/installer/targets/hermes.ts#L100) — Filesystem paths this target would write to at this location.
  - `detect(method)` — [`L40`](../../../../../../../raw/code/codegraph/src/installer/targets/hermes.ts#L40) — documented in [installer-targets-types.ts](../../../../concepts/installer-targets-types.ts.md)
  - `install(method)` — [`L54`](../../../../../../../raw/code/codegraph/src/installer/targets/hermes.ts#L54)
  - `printConfig(method)` — [`L83`](../../../../../../../raw/code/codegraph/src/installer/targets/hermes.ts#L83) — Print the MCP-server snippet a user would paste manually for this
  - `supportsLocation(method)` — [`L36`](../../../../../../../raw/code/codegraph/src/installer/targets/hermes.ts#L36) — Whether this target supports the given install location.
  - `uninstall(method)` — [`L67`](../../../../../../../raw/code/codegraph/src/installer/targets/hermes.ts#L67) — Inverse of install. Removes only what install would have written; — documented in [installer-targets-types.ts](../../../../concepts/installer-targets-types.ts.md)
  - `displayName` — [`L33`](../../../../../../../raw/code/codegraph/src/installer/targets/hermes.ts#L33) — Human-readable name shown in clack prompts and log lines.
  - `docsUrl` — [`L34`](../../../../../../../raw/code/codegraph/src/installer/targets/hermes.ts#L34) — Optional URL for "where do I learn more about this agent."
  - `id` — [`L32`](../../../../../../../raw/code/codegraph/src/installer/targets/hermes.ts#L32) — Stable id; matches the `TargetId` union.
- uses (calls/refs, reference-scoped): [`Location`](types.ts.md#Location), [`action`](types.ts.md#WriteResult.files.Array.typeLiteral0.action), [`WriteResult`](types.ts.md#WriteResult), [`files`](types.ts.md#WriteResult.files), [`path`](types.ts.md#WriteResult.files.Array.typeLiteral0.path), [`AgentTarget`](types.ts.md#AgentTarget), [`writeHermesConfig`](hermes.ts.md#writeHermesConfig), [`DetectionResult`](types.ts.md#DetectionResult), [`InstallOptions`](types.ts.md#InstallOptions), [`atomicWriteFileSync`](shared.ts.md#atomicWriteFileSync), [`removeCodeGraphMcpServer`](hermes.ts.md#removeCodeGraphMcpServer), [`removeCodeGraphToolset`](hermes.ts.md#removeCodeGraphToolset), [`installed`](types.ts.md#DetectionResult.installed), [`alreadyConfigured`](types.ts.md#DetectionResult.alreadyConfigured), [`notes`](types.ts.md#WriteResult.notes), [`hasCodeGraphMcpServer`](hermes.ts.md#hasCodeGraphMcpServer), [`configPath`](types.ts.md#DetectionResult.configPath), [`configPath`](hermes.ts.md#configPath), [`renderCodeGraphMcpBlock`](hermes.ts.md#renderCodeGraphMcpBlock), [`readText`](hermes.ts.md#readText), [`ensureTrailingNewline`](hermes.ts.md#ensureTrailingNewline), [`hermesHome`](hermes.ts.md#hermesHome)
- used by: [`AgentTarget`](types.ts.md#AgentTarget), [`id`](types.ts.md#AgentTarget.id), [`install`](types.ts.md#AgentTarget.install), [`detect`](types.ts.md#AgentTarget.detect), [`supportsLocation`](types.ts.md#AgentTarget.supportsLocation), [`uninstall`](types.ts.md#AgentTarget.uninstall), [`displayName`](types.ts.md#AgentTarget.displayName), [`hermes.ts`](hermes.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-installer-targets-hermes.ts), [`printConfig`](types.ts.md#AgentTarget.printConfig), [`describePaths`](types.ts.md#AgentTarget.describePaths), [`docsUrl`](types.ts.md#AgentTarget.docsUrl)

### `LineRange`
- def: [`src/installer/targets/hermes.ts:29`](../../../../../../../raw/code/codegraph/src/installer/targets/hermes.ts#L29)
- signature: `type LineRange`
- members:
  - `end` — [`L29`](../../../../../../../raw/code/codegraph/src/installer/targets/hermes.ts#L29)
  - `start` — [`L29`](../../../../../../../raw/code/codegraph/src/installer/targets/hermes.ts#L29)
- used by: [`upsertCodeGraphMcpServer`](hermes.ts.md#upsertCodeGraphMcpServer), [`removeCodeGraphMcpServer`](hermes.ts.md#removeCodeGraphMcpServer), [`removeCodeGraphToolset`](hermes.ts.md#removeCodeGraphToolset), [`upsertCodeGraphToolset`](hermes.ts.md#upsertCodeGraphToolset), [`childRange`](hermes.ts.md#childRange), [`listChildBlock`](hermes.ts.md#listChildBlock), [`topLevelRange`](hermes.ts.md#topLevelRange)

## Functions
- `arrayEqual(a: string[], b: string[])` — [`L352`](../../../../../../../raw/code/codegraph/src/installer/targets/hermes.ts#L352)
- `childRange(lines: string[], parent: LineRange, child: string)` — [`L165`](../../../../../../../raw/code/codegraph/src/installer/targets/hermes.ts#L165)
- `configPath()` — [`L111`](../../../../../../../raw/code/codegraph/src/installer/targets/hermes.ts#L111)
- `ensureTrailingNewline(text: string)` — [`L137`](../../../../../../../raw/code/codegraph/src/installer/targets/hermes.ts#L137)
- `escapeRegExp(value: string)` — [`L248`](../../../../../../../raw/code/codegraph/src/installer/targets/hermes.ts#L248)
- `hasCodeGraphMcpServer(content: string)` — [`L269`](../../../../../../../raw/code/codegraph/src/installer/targets/hermes.ts#L269)
- `hermesHome()` — [`L105`](../../../../../../../raw/code/codegraph/src/installer/targets/hermes.ts#L105)
- `joinLines(lines: string[])` — [`L145`](../../../../../../../raw/code/codegraph/src/installer/targets/hermes.ts#L145)
- `listChildBlock(lines: string[], parent: LineRange, child: string)` — [`L207`](../../../../../../../raw/code/codegraph/src/installer/targets/hermes.ts#L207) — Block-range for a 2-space-indented child whose value is a YAML block list.
- `readText(file: string)` — [`L115`](../../../../../../../raw/code/codegraph/src/installer/targets/hermes.ts#L115)
- `removeCodeGraphMcpServer(content: string)` — [`L299`](../../../../../../../raw/code/codegraph/src/installer/targets/hermes.ts#L299)
- `removeCodeGraphToolset(content: string)` — [`L334`](../../../../../../../raw/code/codegraph/src/installer/targets/hermes.ts#L334)
- `renderCodeGraphMcpBlock()` — [`L265`](../../../../../../../raw/code/codegraph/src/installer/targets/hermes.ts#L265)
- `renderCodeGraphMcpChild()` — [`L252`](../../../../../../../raw/code/codegraph/src/installer/targets/hermes.ts#L252)
- `splitLines(content: string)` — [`L141`](../../../../../../../raw/code/codegraph/src/installer/targets/hermes.ts#L141)
- `topLevelRange(lines: string[], key: string)` — [`L150`](../../../../../../../raw/code/codegraph/src/installer/targets/hermes.ts#L150)
- `upsertCodeGraphMcpServer(content: string)` — [`L275`](../../../../../../../raw/code/codegraph/src/installer/targets/hermes.ts#L275)
- `upsertCodeGraphToolset(content: string)` — [`L308`](../../../../../../../raw/code/codegraph/src/installer/targets/hermes.ts#L308)
- `writeHermesConfig()` — [`L123`](../../../../../../../raw/code/codegraph/src/installer/targets/hermes.ts#L123) — documented in [installer-targets-types.ts](../../../../concepts/installer-targets-types.ts.md)

## Module values
- `hermesTarget` — [`L356`](../../../../../../../raw/code/codegraph/src/installer/targets/hermes.ts#L356)

