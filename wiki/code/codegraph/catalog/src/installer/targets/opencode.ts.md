---
title: 'Module: src/installer/targets/opencode.ts'
type: catalog
provenance: extracted
module: src/installer/targets/opencode.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/installer/targets/`opencode.ts`/
symbols:
  writeMcpEntry: writeMcpEntry().
  OpencodeTarget.detect: OpencodeTarget#detect().
  cleanupLegacyWindowsState: cleanupLegacyWindowsState().
  removeInstructionsEntry: removeInstructionsEntry().
  removeMcpEntryAt: removeMcpEntryAt().
  OpencodeTarget.install: OpencodeTarget#install().
  OpencodeTarget.uninstall: OpencodeTarget#uninstall().
  configPath: configPath().
  getOpencodeServerEntry: getOpencodeServerEntry().
  instructionsPath: instructionsPath().
  OpencodeTarget.printConfig: OpencodeTarget#printConfig().
  OpencodeTarget.describePaths: OpencodeTarget#describePaths().
  configBaseDir: configBaseDir().
  legacyWindowsConfigDir: legacyWindowsConfigDir().
  parseConfig: parseConfig().
  FORMATTING: FORMATTING.
  OpencodeTarget: OpencodeTarget#
  globalConfigDir: globalConfigDir().
  readConfigText: readConfigText().
  OpencodeTarget.supportsLocation: OpencodeTarget#supportsLocation().
  opencodeTarget: opencodeTarget.
  getOpencodeServerEntry.typeLiteral30.type: getOpencodeServerEntry().typeLiteral30:type.
  getOpencodeServerEntry.typeLiteral30.command: getOpencodeServerEntry().typeLiteral30:command.
  getOpencodeServerEntry.typeLiteral30.enabled: getOpencodeServerEntry().typeLiteral30:enabled.
  OpencodeTarget.id: OpencodeTarget#id.
  OpencodeTarget.displayName: OpencodeTarget#displayName.
  OpencodeTarget.docsUrl: OpencodeTarget#docsUrl.
---
# Module: [`src/installer/targets/opencode.ts`](../../../../../../../raw/code/codegraph/src/installer/targets/opencode.ts)

## Classes
### `OpencodeTarget`  ·  implements/extends AgentTarget
- def: [`src/installer/targets/opencode.ts:128`](../../../../../../../raw/code/codegraph/src/installer/targets/opencode.ts#L128)
- signature: `class OpencodeTarget`
- members:
  - `describePaths(method)` — [`L184`](../../../../../../../raw/code/codegraph/src/installer/targets/opencode.ts#L184) — Filesystem paths this target would write to at this location.
  - `detect(method)` — [`L137`](../../../../../../../raw/code/codegraph/src/installer/targets/opencode.ts#L137) — documented in [installer-targets-types.ts](../../../../concepts/installer-targets-types.ts.md)
  - `install(method)` — [`L151`](../../../../../../../raw/code/codegraph/src/installer/targets/opencode.ts#L151) — documented in [installer-targets-shared.ts](../../../../concepts/installer-targets-shared.ts.md)
  - `printConfig(method)` — [`L175`](../../../../../../../raw/code/codegraph/src/installer/targets/opencode.ts#L175) — Print the MCP-server snippet a user would paste manually for this
  - `supportsLocation(method)` — [`L133`](../../../../../../../raw/code/codegraph/src/installer/targets/opencode.ts#L133) — Whether this target supports the given install location.
  - `uninstall(method)` — [`L167`](../../../../../../../raw/code/codegraph/src/installer/targets/opencode.ts#L167) — Inverse of install. Removes only what install would have written;
  - `displayName` — [`L130`](../../../../../../../raw/code/codegraph/src/installer/targets/opencode.ts#L130) — Human-readable name shown in clack prompts and log lines.
  - `docsUrl` — [`L131`](../../../../../../../raw/code/codegraph/src/installer/targets/opencode.ts#L131) — Optional URL for "where do I learn more about this agent."
  - `id` — [`L129`](../../../../../../../raw/code/codegraph/src/installer/targets/opencode.ts#L129) — Stable id; matches the `TargetId` union.
- uses (calls/refs, reference-scoped): [`Location`](types.ts.md#Location), [`WriteResult`](types.ts.md#WriteResult), [`files`](types.ts.md#WriteResult.files), [`AgentTarget`](types.ts.md#AgentTarget), [`writeMcpEntry`](opencode.ts.md#writeMcpEntry), [`cleanupLegacyWindowsState`](opencode.ts.md#cleanupLegacyWindowsState), [`removeInstructionsEntry`](opencode.ts.md#removeInstructionsEntry), [`upsertInstructionsEntry`](shared.ts.md#upsertInstructionsEntry), [`removeMcpEntryAt`](opencode.ts.md#removeMcpEntryAt), [`DetectionResult`](types.ts.md#DetectionResult), [`InstallOptions`](types.ts.md#InstallOptions), [`installed`](types.ts.md#DetectionResult.installed), [`alreadyConfigured`](types.ts.md#DetectionResult.alreadyConfigured), [`configPath`](opencode.ts.md#configPath), [`getOpencodeServerEntry`](opencode.ts.md#getOpencodeServerEntry), [`configPath`](types.ts.md#DetectionResult.configPath), [`instructionsPath`](opencode.ts.md#instructionsPath), [`legacyWindowsConfigDir`](opencode.ts.md#legacyWindowsConfigDir), [`parseConfig`](opencode.ts.md#parseConfig), [`globalConfigDir`](opencode.ts.md#globalConfigDir), [`readConfigText`](opencode.ts.md#readConfigText)
- used by: [`AgentTarget`](types.ts.md#AgentTarget), [`opencode.ts`](opencode.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-installer-targets-opencode.ts), [`id`](types.ts.md#AgentTarget.id), [`install`](types.ts.md#AgentTarget.install), [`detect`](types.ts.md#AgentTarget.detect), [`supportsLocation`](types.ts.md#AgentTarget.supportsLocation), [`uninstall`](types.ts.md#AgentTarget.uninstall), [`displayName`](types.ts.md#AgentTarget.displayName), [`printConfig`](types.ts.md#AgentTarget.printConfig), [`describePaths`](types.ts.md#AgentTarget.describePaths), [`docsUrl`](types.ts.md#AgentTarget.docsUrl)

## Functions
- `cleanupLegacyWindowsState()` — [`L263`](../../../../../../../raw/code/codegraph/src/installer/targets/opencode.ts#L263) — Remove whatever a pre-#535 install left in `%APPDATA%/opencode` — an MCP — documented in [installer-targets-types.ts](../../../../concepts/installer-targets-types.ts.md)
- `configBaseDir(loc: Location)` — [`L83`](../../../../../../../raw/code/codegraph/src/installer/targets/opencode.ts#L83)
- `configPath(loc: Location)` — [`L90`](../../../../../../../raw/code/codegraph/src/installer/targets/opencode.ts#L90)
- `getOpencodeServerEntry()` — [`L118`](../../../../../../../raw/code/codegraph/src/installer/targets/opencode.ts#L118)
- `globalConfigDir()` — [`L59`](../../../../../../../raw/code/codegraph/src/installer/targets/opencode.ts#L59)
- `instructionsPath(loc: Location)` — [`L99`](../../../../../../../raw/code/codegraph/src/installer/targets/opencode.ts#L99)
- `legacyWindowsConfigDir()` — [`L76`](../../../../../../../raw/code/codegraph/src/installer/targets/opencode.ts#L76) — Pre-#535 installs wrote the global entry to `%APPDATA%/opencode` — a dir
- `parseConfig(text: string)` — [`L108`](../../../../../../../raw/code/codegraph/src/installer/targets/opencode.ts#L108)
- `readConfigText(file: string)` — [`L103`](../../../../../../../raw/code/codegraph/src/installer/targets/opencode.ts#L103)
- `removeInstructionsEntry(loc: Location)` — [`L282`](../../../../../../../raw/code/codegraph/src/installer/targets/opencode.ts#L282) — Strip the marker-delimited CodeGraph block from AGENTS.md if a prior — documented in [installer-targets-types.ts](../../../../concepts/installer-targets-types.ts.md)
- `removeMcpEntryAt(file: string)` — [`L233`](../../../../../../../raw/code/codegraph/src/installer/targets/opencode.ts#L233) — Surgically drop `mcp.codegraph` from one config file. Leaves sibling — documented in [installer-targets-types.ts](../../../../concepts/installer-targets-types.ts.md)
- `writeMcpEntry(loc: Location)` — [`L189`](../../../../../../../raw/code/codegraph/src/installer/targets/opencode.ts#L189) — documented in [installer-targets-types.ts](../../../../concepts/installer-targets-types.ts.md)

## Module values
- `FORMATTING` — [`L126`](../../../../../../../raw/code/codegraph/src/installer/targets/opencode.ts#L126)
- `command` — [`L118`](../../../../../../../raw/code/codegraph/src/installer/targets/opencode.ts#L118)
- `enabled` — [`L118`](../../../../../../../raw/code/codegraph/src/installer/targets/opencode.ts#L118)
- `opencodeTarget` — [`L288`](../../../../../../../raw/code/codegraph/src/installer/targets/opencode.ts#L288)
- `type` — [`L118`](../../../../../../../raw/code/codegraph/src/installer/targets/opencode.ts#L118)

