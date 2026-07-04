---
title: 'Module: src/installer/targets/kiro.ts'
type: catalog
provenance: extracted
module: src/installer/targets/kiro.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/installer/targets/`kiro.ts`/
symbols:
  writeMcpEntry: writeMcpEntry().
  KiroTarget.uninstall: KiroTarget#uninstall().
  KiroTarget.detect: KiroTarget#detect().
  KiroTarget.install: KiroTarget#install().
  removeSteeringEntry: removeSteeringEntry().
  mcpJsonPath: mcpJsonPath().
  KiroTarget.printConfig: KiroTarget#printConfig().
  KiroTarget.describePaths: KiroTarget#describePaths().
  steeringPath: steeringPath().
  configDir: configDir().
  KiroTarget: KiroTarget#
  KiroTarget.supportsLocation: KiroTarget#supportsLocation().
  kiroTarget: kiroTarget.
  KiroTarget.id: KiroTarget#id.
  KiroTarget.displayName: KiroTarget#displayName.
  KiroTarget.docsUrl: KiroTarget#docsUrl.
---
# Module: [`src/installer/targets/kiro.ts`](../../../../../../../raw/code/codegraph/src/installer/targets/kiro.ts)

## Classes
### `KiroTarget`  ·  implements/extends AgentTarget
- def: [`src/installer/targets/kiro.ts:55`](../../../../../../../raw/code/codegraph/src/installer/targets/kiro.ts#L55)
- signature: `class KiroTarget`
- members:
  - `describePaths(method)` — [`L126`](../../../../../../../raw/code/codegraph/src/installer/targets/kiro.ts#L126) — Filesystem paths this target would write to at this location.
  - `detect(method)` — [`L64`](../../../../../../../raw/code/codegraph/src/installer/targets/kiro.ts#L64) — documented in [installer-targets-shared.ts](../../../../concepts/installer-targets-shared.ts.md)
  - `install(method)` — [`L74`](../../../../../../../raw/code/codegraph/src/installer/targets/kiro.ts#L74)
  - `printConfig(method)` — [`L120`](../../../../../../../raw/code/codegraph/src/installer/targets/kiro.ts#L120) — Print the MCP-server snippet a user would paste manually for this — documented in [installer-targets-shared.ts](../../../../concepts/installer-targets-shared.ts.md)
  - `supportsLocation(method)` — [`L60`](../../../../../../../raw/code/codegraph/src/installer/targets/kiro.ts#L60) — Whether this target supports the given install location.
  - `uninstall(method)` — [`L99`](../../../../../../../raw/code/codegraph/src/installer/targets/kiro.ts#L99) — Inverse of install. Removes only what install would have written; — documented in [installer-targets-shared.ts](../../../../concepts/installer-targets-shared.ts.md)
  - `displayName` — [`L57`](../../../../../../../raw/code/codegraph/src/installer/targets/kiro.ts#L57) — Human-readable name shown in clack prompts and log lines.
  - `docsUrl` — [`L58`](../../../../../../../raw/code/codegraph/src/installer/targets/kiro.ts#L58) — Optional URL for "where do I learn more about this agent."
  - `id` — [`L56`](../../../../../../../raw/code/codegraph/src/installer/targets/kiro.ts#L56) — Stable id; matches the `TargetId` union.
- uses (calls/refs, reference-scoped): [`Location`](types.ts.md#Location), [`action`](types.ts.md#WriteResult.files.Array.typeLiteral0.action), [`WriteResult`](types.ts.md#WriteResult), [`files`](types.ts.md#WriteResult.files), [`path`](types.ts.md#WriteResult.files.Array.typeLiteral0.path), [`AgentTarget`](types.ts.md#AgentTarget), [`readJsonFile`](shared.ts.md#readJsonFile), [`writeMcpEntry`](kiro.ts.md#writeMcpEntry), [`writeJsonFile`](shared.ts.md#writeJsonFile), [`getMcpServerConfig`](shared.ts.md#getMcpServerConfig), [`DetectionResult`](types.ts.md#DetectionResult), [`InstallOptions`](types.ts.md#InstallOptions), [`removeSteeringEntry`](kiro.ts.md#removeSteeringEntry), [`installed`](types.ts.md#DetectionResult.installed), [`alreadyConfigured`](types.ts.md#DetectionResult.alreadyConfigured), [`mcpJsonPath`](kiro.ts.md#mcpJsonPath), [`notes`](types.ts.md#WriteResult.notes), [`configPath`](types.ts.md#DetectionResult.configPath), [`steeringPath`](kiro.ts.md#steeringPath), [`configDir`](kiro.ts.md#configDir)
- used by: [`AgentTarget`](types.ts.md#AgentTarget), [`id`](types.ts.md#AgentTarget.id), [`kiro.ts`](kiro.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-installer-targets-kiro.ts), [`install`](types.ts.md#AgentTarget.install), [`detect`](types.ts.md#AgentTarget.detect), [`supportsLocation`](types.ts.md#AgentTarget.supportsLocation), [`uninstall`](types.ts.md#AgentTarget.uninstall), [`displayName`](types.ts.md#AgentTarget.displayName), [`printConfig`](types.ts.md#AgentTarget.printConfig), [`describePaths`](types.ts.md#AgentTarget.describePaths), [`docsUrl`](types.ts.md#AgentTarget.docsUrl)

## Functions
- `configDir(loc: Location)` — [`L43`](../../../../../../../raw/code/codegraph/src/installer/targets/kiro.ts#L43)
- `mcpJsonPath(loc: Location)` — [`L48`](../../../../../../../raw/code/codegraph/src/installer/targets/kiro.ts#L48)
- `removeSteeringEntry(loc: Location)` — [`L158`](../../../../../../../raw/code/codegraph/src/installer/targets/kiro.ts#L158) — Delete the steering file we own. If a user has hand-edited the file
- `steeringPath(loc: Location)` — [`L51`](../../../../../../../raw/code/codegraph/src/installer/targets/kiro.ts#L51)
- `writeMcpEntry(loc: Location)` — [`L131`](../../../../../../../raw/code/codegraph/src/installer/targets/kiro.ts#L131) — documented in [installer-targets-shared.ts](../../../../concepts/installer-targets-shared.ts.md)

## Module values
- `kiroTarget` — [`L165`](../../../../../../../raw/code/codegraph/src/installer/targets/kiro.ts#L165)

