---
title: 'Module: src/installer/targets/claude.ts'
type: catalog
provenance: extracted
module: src/installer/targets/claude.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/installer/targets/`claude.ts`/
symbols:
  ClaudeCodeTarget.install: ClaudeCodeTarget#install().
  ClaudeCodeTarget.uninstall: ClaudeCodeTarget#uninstall().
  writeMcpEntry: writeMcpEntry().
  writePermissionsEntry: writePermissionsEntry().
  writePromptHookEntry: writePromptHookEntry().
  removeInstructionsEntry: removeInstructionsEntry().
  removeHookCommandsMatching: removeHookCommandsMatching().
  ClaudeCodeTarget.detect: ClaudeCodeTarget#detect().
  cleanupLegacyLocalMcp: cleanupLegacyLocalMcp().
  cleanupLegacyHooks: cleanupLegacyHooks().
  removePromptHookEntry: removePromptHookEntry().
  settingsJsonPath: settingsJsonPath().
  ClaudeCodeTarget.describePaths: ClaudeCodeTarget#describePaths().
  instructionsPath: instructionsPath().
  mcpJsonPath: mcpJsonPath().
  ClaudeCodeTarget.printConfig: ClaudeCodeTarget#printConfig().
  configDir: configDir().
  isPromptHookCommand: isPromptHookCommand().
  ClaudeCodeTarget: ClaudeCodeTarget#
  claudeTarget: claudeTarget.
  ClaudeCodeTarget.supportsLocation: ClaudeCodeTarget#supportsLocation().
  PROMPT_HOOK_COMMAND: PROMPT_HOOK_COMMAND.
  legacyLocalMcpPath: legacyLocalMcpPath().
  isLegacyCodegraphHookCommand: isLegacyCodegraphHookCommand().
  ClaudeCodeTarget.id: ClaudeCodeTarget#id.
  ClaudeCodeTarget.displayName: ClaudeCodeTarget#displayName.
  ClaudeCodeTarget.docsUrl: ClaudeCodeTarget#docsUrl.
---
# Module: [`src/installer/targets/claude.ts`](../../../../../../../raw/code/codegraph/src/installer/targets/claude.ts)

## Classes
### `ClaudeCodeTarget`  ·  implements/extends AgentTarget
- def: [`src/installer/targets/claude.ts:74`](../../../../../../../raw/code/codegraph/src/installer/targets/claude.ts#L74)
- signature: `class ClaudeCodeTarget`
- members:
  - `describePaths(method)` — [`L218`](../../../../../../../raw/code/codegraph/src/installer/targets/claude.ts#L218) — Filesystem paths this target would write to at this location.
  - `detect(method)` — [`L83`](../../../../../../../raw/code/codegraph/src/installer/targets/claude.ts#L83) — documented in [installer-targets-shared.ts](../../../../concepts/installer-targets-shared.ts.md)
  - `install(method)` — [`L96`](../../../../../../../raw/code/codegraph/src/installer/targets/claude.ts#L96) — documented in [installer-targets-shared.ts](../../../../concepts/installer-targets-shared.ts.md)
  - `printConfig(method)` — [`L212`](../../../../../../../raw/code/codegraph/src/installer/targets/claude.ts#L212) — Print the MCP-server snippet a user would paste manually for this — documented in [installer-targets-shared.ts](../../../../concepts/installer-targets-shared.ts.md)
  - `supportsLocation(method)` — [`L79`](../../../../../../../raw/code/codegraph/src/installer/targets/claude.ts#L79) — Whether this target supports the given install location.
  - `uninstall(method)` — [`L146`](../../../../../../../raw/code/codegraph/src/installer/targets/claude.ts#L146) — Inverse of install. Removes only what install would have written; — documented in [installer-targets-shared.ts](../../../../concepts/installer-targets-shared.ts.md)
  - `displayName` — [`L76`](../../../../../../../raw/code/codegraph/src/installer/targets/claude.ts#L76) — Human-readable name shown in clack prompts and log lines.
  - `docsUrl` — [`L77`](../../../../../../../raw/code/codegraph/src/installer/targets/claude.ts#L77) — Optional URL for "where do I learn more about this agent."
  - `id` — [`L75`](../../../../../../../raw/code/codegraph/src/installer/targets/claude.ts#L75) — Stable id; matches the `TargetId` union.
- uses (calls/refs, reference-scoped): [`Location`](types.ts.md#Location), [`action`](types.ts.md#WriteResult.files.Array.typeLiteral0.action), [`WriteResult`](types.ts.md#WriteResult), [`files`](types.ts.md#WriteResult.files), [`path`](types.ts.md#WriteResult.files.Array.typeLiteral0.path), [`AgentTarget`](types.ts.md#AgentTarget), [`readJsonFile`](shared.ts.md#readJsonFile), [`writeMcpEntry`](claude.ts.md#writeMcpEntry), [`writePermissionsEntry`](claude.ts.md#writePermissionsEntry), [`writePromptHookEntry`](claude.ts.md#writePromptHookEntry), [`removeInstructionsEntry`](claude.ts.md#removeInstructionsEntry), [`writeJsonFile`](shared.ts.md#writeJsonFile), [`upsertInstructionsEntry`](shared.ts.md#upsertInstructionsEntry), [`getMcpServerConfig`](shared.ts.md#getMcpServerConfig), [`DetectionResult`](types.ts.md#DetectionResult), [`InstallOptions`](types.ts.md#InstallOptions), [`cleanupLegacyHooks`](claude.ts.md#cleanupLegacyHooks), [`cleanupLegacyLocalMcp`](claude.ts.md#cleanupLegacyLocalMcp), [`removePromptHookEntry`](claude.ts.md#removePromptHookEntry), [`installed`](types.ts.md#DetectionResult.installed), [`alreadyConfigured`](types.ts.md#DetectionResult.alreadyConfigured), [`settingsJsonPath`](claude.ts.md#settingsJsonPath), [`configPath`](types.ts.md#DetectionResult.configPath), [`instructionsPath`](claude.ts.md#instructionsPath), [`mcpJsonPath`](claude.ts.md#mcpJsonPath), [`configDir`](claude.ts.md#configDir), [`promptHook`](types.ts.md#InstallOptions.promptHook), [`autoAllow`](types.ts.md#InstallOptions.autoAllow)
- used by: [`AgentTarget`](types.ts.md#AgentTarget), [`claude.ts`](claude.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-installer-targets-claude.ts), [`id`](types.ts.md#AgentTarget.id), [`install`](types.ts.md#AgentTarget.install), [`detect`](types.ts.md#AgentTarget.detect), [`supportsLocation`](types.ts.md#AgentTarget.supportsLocation), [`uninstall`](types.ts.md#AgentTarget.uninstall), [`displayName`](types.ts.md#AgentTarget.displayName), [`printConfig`](types.ts.md#AgentTarget.printConfig), [`describePaths`](types.ts.md#AgentTarget.describePaths), [`docsUrl`](types.ts.md#AgentTarget.docsUrl)

## Functions
- `cleanupLegacyHooks(loc: Location)` — [`L373`](../../../../../../../raw/code/codegraph/src/installer/targets/claude.ts#L373) — Remove stale codegraph auto-sync hooks (`mark-dirty` / `sync-if-dirty`) that a
- `cleanupLegacyLocalMcp()` — [`L262`](../../../../../../../raw/code/codegraph/src/installer/targets/claude.ts#L262) — Strip the codegraph entry from a legacy project-local — documented in [installer-targets-shared.ts](../../../../concepts/installer-targets-shared.ts.md)
- `configDir(loc: Location)` — [`L44`](../../../../../../../raw/code/codegraph/src/installer/targets/claude.ts#L44)
- `instructionsPath(loc: Location)` — [`L70`](../../../../../../../raw/code/codegraph/src/installer/targets/claude.ts#L70)
- `isLegacyCodegraphHookCommand(command: unknown)` — [`L289`](../../../../../../../raw/code/codegraph/src/installer/targets/claude.ts#L289) — True when a Claude Code hook `command` is one of the auto-sync hooks
- `isPromptHookCommand(command: unknown)` — [`L303`](../../../../../../../raw/code/codegraph/src/installer/targets/claude.ts#L303)
- `legacyLocalMcpPath()` — [`L64`](../../../../../../../raw/code/codegraph/src/installer/targets/claude.ts#L64) — Where pre-#207 installers wrote the local MCP entry. Claude Code
- `mcpJsonPath(loc: Location)` — [`L49`](../../../../../../../raw/code/codegraph/src/installer/targets/claude.ts#L49)
- `removeHookCommandsMatching(loc: Location, match: (command: unknown) => boolean)` — [`L322`](../../../../../../../raw/code/codegraph/src/installer/targets/claude.ts#L322) — Remove stale codegraph auto-sync hooks from Claude `settings.json`. — documented in [installer-targets-shared.ts](../../../../concepts/installer-targets-shared.ts.md)
- `removeInstructionsEntry(loc: Location)` — [`L448`](../../../../../../../raw/code/codegraph/src/installer/targets/claude.ts#L448) — Strip the marker-delimited CodeGraph block from CLAUDE.md if a prior — documented in [installer-targets-types.ts](../../../../concepts/installer-targets-types.ts.md)
- `removePromptHookEntry(loc: Location)` — [`L382`](../../../../../../../raw/code/codegraph/src/installer/targets/claude.ts#L382) — Remove the front-load `UserPromptSubmit` hook this installer writes (see
- `settingsJsonPath(loc: Location)` — [`L67`](../../../../../../../raw/code/codegraph/src/installer/targets/claude.ts#L67)
- `writeMcpEntry(loc: Location)` — [`L230`](../../../../../../../raw/code/codegraph/src/installer/targets/claude.ts#L230) — Per-file write helpers, exported so the legacy `config-writer.ts` — documented in [installer-targets-shared.ts](../../../../concepts/installer-targets-shared.ts.md)
- `writePermissionsEntry(loc: Location)` — [`L386`](../../../../../../../raw/code/codegraph/src/installer/targets/claude.ts#L386) — documented in [installer-targets-shared.ts](../../../../concepts/installer-targets-shared.ts.md)
- `writePromptHookEntry(loc: Location)` — [`L417`](../../../../../../../raw/code/codegraph/src/installer/targets/claude.ts#L417) — Write the front-load `UserPromptSubmit` hook into Claude `settings.json` — — documented in [installer-targets-shared.ts](../../../../concepts/installer-targets-shared.ts.md)

## Module values
- `PROMPT_HOOK_COMMAND` — [`L302`](../../../../../../../raw/code/codegraph/src/installer/targets/claude.ts#L302) — The front-load prompt-hook command the installer writes into Claude's
- `claudeTarget` — [`L454`](../../../../../../../raw/code/codegraph/src/installer/targets/claude.ts#L454)

