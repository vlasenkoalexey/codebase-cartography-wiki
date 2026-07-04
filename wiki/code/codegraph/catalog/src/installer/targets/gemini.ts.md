---
title: 'Module: src/installer/targets/gemini.ts'
type: catalog
provenance: extracted
module: src/installer/targets/gemini.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/installer/targets/`gemini.ts`/
symbols:
  writeMcpEntry: writeMcpEntry().
  removeInstructionsEntry: removeInstructionsEntry().
  GeminiTarget.uninstall: GeminiTarget#uninstall().
  GeminiTarget.detect: GeminiTarget#detect().
  GeminiTarget.install: GeminiTarget#install().
  settingsJsonPath: settingsJsonPath().
  instructionsPath: instructionsPath().
  GeminiTarget.printConfig: GeminiTarget#printConfig().
  GeminiTarget.describePaths: GeminiTarget#describePaths().
  configDir: configDir().
  GeminiTarget: GeminiTarget#
  GeminiTarget.supportsLocation: GeminiTarget#supportsLocation().
  geminiTarget: geminiTarget.
  GeminiTarget.id: GeminiTarget#id.
  GeminiTarget.displayName: GeminiTarget#displayName.
  GeminiTarget.docsUrl: GeminiTarget#docsUrl.
---
# Module: [`src/installer/targets/gemini.ts`](../../../../../../../raw/code/codegraph/src/installer/targets/gemini.ts)

## Classes
### `GeminiTarget`  ·  implements/extends AgentTarget
- def: [`src/installer/targets/gemini.ts:65`](../../../../../../../raw/code/codegraph/src/installer/targets/gemini.ts#L65)
- signature: `class GeminiTarget`
- members:
  - `describePaths(method)` — [`L126`](../../../../../../../raw/code/codegraph/src/installer/targets/gemini.ts#L126) — Filesystem paths this target would write to at this location.
  - `detect(method)` — [`L74`](../../../../../../../raw/code/codegraph/src/installer/targets/gemini.ts#L74) — documented in [installer-targets-shared.ts](../../../../concepts/installer-targets-shared.ts.md)
  - `install(method)` — [`L84`](../../../../../../../raw/code/codegraph/src/installer/targets/gemini.ts#L84) — documented in [installer-targets-shared.ts](../../../../concepts/installer-targets-shared.ts.md)
  - `printConfig(method)` — [`L120`](../../../../../../../raw/code/codegraph/src/installer/targets/gemini.ts#L120) — Print the MCP-server snippet a user would paste manually for this — documented in [installer-targets-shared.ts](../../../../concepts/installer-targets-shared.ts.md)
  - `supportsLocation(method)` — [`L70`](../../../../../../../raw/code/codegraph/src/installer/targets/gemini.ts#L70) — Whether this target supports the given install location.
  - `uninstall(method)` — [`L96`](../../../../../../../raw/code/codegraph/src/installer/targets/gemini.ts#L96) — Inverse of install. Removes only what install would have written; — documented in [installer-targets-shared.ts](../../../../concepts/installer-targets-shared.ts.md)
  - `displayName` — [`L67`](../../../../../../../raw/code/codegraph/src/installer/targets/gemini.ts#L67) — Human-readable name shown in clack prompts and log lines.
  - `docsUrl` — [`L68`](../../../../../../../raw/code/codegraph/src/installer/targets/gemini.ts#L68) — Optional URL for "where do I learn more about this agent."
  - `id` — [`L66`](../../../../../../../raw/code/codegraph/src/installer/targets/gemini.ts#L66) — Stable id; matches the `TargetId` union.
- uses (calls/refs, reference-scoped): [`Location`](types.ts.md#Location), [`action`](types.ts.md#WriteResult.files.Array.typeLiteral0.action), [`WriteResult`](types.ts.md#WriteResult), [`files`](types.ts.md#WriteResult.files), [`path`](types.ts.md#WriteResult.files.Array.typeLiteral0.path), [`AgentTarget`](types.ts.md#AgentTarget), [`readJsonFile`](shared.ts.md#readJsonFile), [`writeMcpEntry`](gemini.ts.md#writeMcpEntry), [`removeInstructionsEntry`](gemini.ts.md#removeInstructionsEntry), [`writeJsonFile`](shared.ts.md#writeJsonFile), [`upsertInstructionsEntry`](shared.ts.md#upsertInstructionsEntry), [`getMcpServerConfig`](shared.ts.md#getMcpServerConfig), [`DetectionResult`](types.ts.md#DetectionResult), [`InstallOptions`](types.ts.md#InstallOptions), [`installed`](types.ts.md#DetectionResult.installed), [`alreadyConfigured`](types.ts.md#DetectionResult.alreadyConfigured), [`settingsJsonPath`](gemini.ts.md#settingsJsonPath), [`configPath`](types.ts.md#DetectionResult.configPath), [`instructionsPath`](gemini.ts.md#instructionsPath), [`configDir`](gemini.ts.md#configDir)
- used by: [`AgentTarget`](types.ts.md#AgentTarget), [`gemini.ts`](gemini.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-installer-targets-gemini.ts), [`id`](types.ts.md#AgentTarget.id), [`install`](types.ts.md#AgentTarget.install), [`detect`](types.ts.md#AgentTarget.detect), [`supportsLocation`](types.ts.md#AgentTarget.supportsLocation), [`uninstall`](types.ts.md#AgentTarget.uninstall), [`displayName`](types.ts.md#AgentTarget.displayName), [`printConfig`](types.ts.md#AgentTarget.printConfig), [`describePaths`](types.ts.md#AgentTarget.describePaths), [`docsUrl`](types.ts.md#AgentTarget.docsUrl)

## Functions
- `configDir(loc: Location)` — [`L48`](../../../../../../../raw/code/codegraph/src/installer/targets/gemini.ts#L48)
- `instructionsPath(loc: Location)` — [`L56`](../../../../../../../raw/code/codegraph/src/installer/targets/gemini.ts#L56)
- `removeInstructionsEntry(loc: Location)` — [`L156`](../../../../../../../raw/code/codegraph/src/installer/targets/gemini.ts#L156) — Strip the marker-delimited CodeGraph block from GEMINI.md if a prior — documented in [installer-targets-types.ts](../../../../concepts/installer-targets-types.ts.md)
- `settingsJsonPath(loc: Location)` — [`L53`](../../../../../../../raw/code/codegraph/src/installer/targets/gemini.ts#L53)
- `writeMcpEntry(loc: Location)` — [`L131`](../../../../../../../raw/code/codegraph/src/installer/targets/gemini.ts#L131) — documented in [installer-targets-shared.ts](../../../../concepts/installer-targets-shared.ts.md)

## Module values
- `geminiTarget` — [`L162`](../../../../../../../raw/code/codegraph/src/installer/targets/gemini.ts#L162)

