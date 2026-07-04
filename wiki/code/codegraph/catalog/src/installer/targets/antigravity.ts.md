---
title: 'Module: src/installer/targets/antigravity.ts'
type: catalog
provenance: extracted
module: src/installer/targets/antigravity.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/installer/targets/`antigravity.ts`/
symbols:
  writeMcpEntry: writeMcpEntry().
  AntigravityTarget.detect: AntigravityTarget#detect().
  AntigravityTarget.uninstall: AntigravityTarget#uninstall().
  cleanupLegacyEntry: cleanupLegacyEntry().
  AntigravityTarget.install: AntigravityTarget#install().
  removeCodegraphFromFile: removeCodegraphFromFile().
  preferredMcpConfigPath: preferredMcpConfigPath().
  buildAntigravityEntry: buildAntigravityEntry().
  unifiedMcpConfigPath: unifiedMcpConfigPath().
  AntigravityTarget.printConfig: AntigravityTarget#printConfig().
  legacyMcpConfigPath: legacyMcpConfigPath().
  AntigravityTarget.describePaths: AntigravityTarget#describePaths().
  migratedMarkerPath: migratedMarkerPath().
  AntigravityTarget: AntigravityTarget#
  unifiedConfigDir: unifiedConfigDir().
  AntigravityTarget.supportsLocation: AntigravityTarget#supportsLocation().
  legacyConfigDir: legacyConfigDir().
  antigravityTarget: antigravityTarget.
  resolveCodegraphCommand: resolveCodegraphCommand().
  buildAntigravityEntry.typeLiteral7.command: buildAntigravityEntry().typeLiteral7:command.
  buildAntigravityEntry.typeLiteral7.args: buildAntigravityEntry().typeLiteral7:args.
  AntigravityTarget.id: AntigravityTarget#id.
  AntigravityTarget.displayName: AntigravityTarget#displayName.
  AntigravityTarget.docsUrl: AntigravityTarget#docsUrl.
---
# Module: [`src/installer/targets/antigravity.ts`](../../../../../../../raw/code/codegraph/src/installer/targets/antigravity.ts)

## Classes
### `AntigravityTarget`  ·  implements/extends AgentTarget
- def: [`src/installer/targets/antigravity.ts:149`](../../../../../../../raw/code/codegraph/src/installer/targets/antigravity.ts#L149)
- signature: `class AntigravityTarget`
- members:
  - `describePaths(method)` — [`L228`](../../../../../../../raw/code/codegraph/src/installer/targets/antigravity.ts#L228) — Filesystem paths this target would write to at this location.
  - `detect(method)` — [`L158`](../../../../../../../raw/code/codegraph/src/installer/targets/antigravity.ts#L158) — documented in [installer-targets-shared.ts](../../../../concepts/installer-targets-shared.ts.md)
  - `install(method)` — [`L175`](../../../../../../../raw/code/codegraph/src/installer/targets/antigravity.ts#L175)
  - `printConfig(method)` — [`L219`](../../../../../../../raw/code/codegraph/src/installer/targets/antigravity.ts#L219) — Print the MCP-server snippet a user would paste manually for this
  - `supportsLocation(method)` — [`L154`](../../../../../../../raw/code/codegraph/src/installer/targets/antigravity.ts#L154) — Whether this target supports the given install location.
  - `uninstall(method)` — [`L195`](../../../../../../../raw/code/codegraph/src/installer/targets/antigravity.ts#L195) — Inverse of install. Removes only what install would have written; — documented in [installer-targets-types.ts](../../../../concepts/installer-targets-types.ts.md)
  - `displayName` — [`L151`](../../../../../../../raw/code/codegraph/src/installer/targets/antigravity.ts#L151) — Human-readable name shown in clack prompts and log lines.
  - `docsUrl` — [`L152`](../../../../../../../raw/code/codegraph/src/installer/targets/antigravity.ts#L152) — Optional URL for "where do I learn more about this agent."
  - `id` — [`L150`](../../../../../../../raw/code/codegraph/src/installer/targets/antigravity.ts#L150) — Stable id; matches the `TargetId` union.
- uses (calls/refs, reference-scoped): [`Location`](types.ts.md#Location), [`action`](types.ts.md#WriteResult.files.Array.typeLiteral0.action), [`WriteResult`](types.ts.md#WriteResult), [`files`](types.ts.md#WriteResult.files), [`AgentTarget`](types.ts.md#AgentTarget), [`readJsonFile`](shared.ts.md#readJsonFile), [`writeMcpEntry`](antigravity.ts.md#writeMcpEntry), [`cleanupLegacyEntry`](antigravity.ts.md#cleanupLegacyEntry), [`DetectionResult`](types.ts.md#DetectionResult), [`InstallOptions`](types.ts.md#InstallOptions), [`removeCodegraphFromFile`](antigravity.ts.md#removeCodegraphFromFile), [`installed`](types.ts.md#DetectionResult.installed), [`preferredMcpConfigPath`](antigravity.ts.md#preferredMcpConfigPath), [`alreadyConfigured`](types.ts.md#DetectionResult.alreadyConfigured), [`buildAntigravityEntry`](antigravity.ts.md#buildAntigravityEntry), [`notes`](types.ts.md#WriteResult.notes), [`unifiedMcpConfigPath`](antigravity.ts.md#unifiedMcpConfigPath), [`configPath`](types.ts.md#DetectionResult.configPath), [`legacyMcpConfigPath`](antigravity.ts.md#legacyMcpConfigPath), [`unifiedConfigDir`](antigravity.ts.md#unifiedConfigDir), [`legacyConfigDir`](antigravity.ts.md#legacyConfigDir)
- used by: [`AgentTarget`](types.ts.md#AgentTarget), [`id`](types.ts.md#AgentTarget.id), [`antigravity.ts`](antigravity.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-installer-targets-antigravity.ts), [`install`](types.ts.md#AgentTarget.install), [`detect`](types.ts.md#AgentTarget.detect), [`supportsLocation`](types.ts.md#AgentTarget.supportsLocation), [`uninstall`](types.ts.md#AgentTarget.uninstall), [`displayName`](types.ts.md#AgentTarget.displayName), [`printConfig`](types.ts.md#AgentTarget.printConfig), [`describePaths`](types.ts.md#AgentTarget.describePaths), [`docsUrl`](types.ts.md#AgentTarget.docsUrl)

## Functions
- `buildAntigravityEntry()` — [`L142`](../../../../../../../raw/code/codegraph/src/installer/targets/antigravity.ts#L142) — Build the codegraph MCP-server entry for Antigravity. Distinct from
- `cleanupLegacyEntry()` — [`L261`](../../../../../../../raw/code/codegraph/src/installer/targets/antigravity.ts#L261) — Strip the codegraph entry from the legacy `~/.gemini/antigravity/mcp_config.json` — documented in [installer-targets-shared.ts](../../../../concepts/installer-targets-shared.ts.md)
- `legacyConfigDir()` — [`L79`](../../../../../../../raw/code/codegraph/src/installer/targets/antigravity.ts#L79)
- `legacyMcpConfigPath()` — [`L82`](../../../../../../../raw/code/codegraph/src/installer/targets/antigravity.ts#L82)
- `migratedMarkerPath()` — [`L85`](../../../../../../../raw/code/codegraph/src/installer/targets/antigravity.ts#L85)
- `preferredMcpConfigPath()` — [`L99`](../../../../../../../raw/code/codegraph/src/installer/targets/antigravity.ts#L99) — Pick the right MCP config path to write to.
- `removeCodegraphFromFile(file: string)` — [`L275`](../../../../../../../raw/code/codegraph/src/installer/targets/antigravity.ts#L275) — documented in [installer-targets-shared.ts](../../../../concepts/installer-targets-shared.ts.md)
- `resolveCodegraphCommand()` — [`L120`](../../../../../../../raw/code/codegraph/src/installer/targets/antigravity.ts#L120) — Resolve the on-disk path of the `codegraph` binary so a Mac GUI app
- `unifiedConfigDir()` — [`L73`](../../../../../../../raw/code/codegraph/src/installer/targets/antigravity.ts#L73)
- `unifiedMcpConfigPath()` — [`L76`](../../../../../../../raw/code/codegraph/src/installer/targets/antigravity.ts#L76)
- `writeMcpEntry()` — [`L234`](../../../../../../../raw/code/codegraph/src/installer/targets/antigravity.ts#L234) — documented in [installer-targets-shared.ts](../../../../concepts/installer-targets-shared.ts.md)

## Module values
- `antigravityTarget` — [`L289`](../../../../../../../raw/code/codegraph/src/installer/targets/antigravity.ts#L289)
- `args` — [`L142`](../../../../../../../raw/code/codegraph/src/installer/targets/antigravity.ts#L142)
- `command` — [`L142`](../../../../../../../raw/code/codegraph/src/installer/targets/antigravity.ts#L142)

