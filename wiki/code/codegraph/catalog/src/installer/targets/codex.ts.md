---
title: 'Module: src/installer/targets/codex.ts'
type: catalog
provenance: extracted
module: src/installer/targets/codex.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/installer/targets/`codex.ts`/
symbols:
  CodexTarget.uninstall: CodexTarget#uninstall().
  writeMcpEntry: writeMcpEntry().
  removeInstructionsEntry: removeInstructionsEntry().
  CodexTarget.detect: CodexTarget#detect().
  CodexTarget.install: CodexTarget#install().
  buildCodegraphBlock: buildCodegraphBlock().
  tomlConfigPath: tomlConfigPath().
  CodexTarget.printConfig: CodexTarget#printConfig().
  CodexTarget.describePaths: CodexTarget#describePaths().
  instructionsPath: instructionsPath().
  TOML_HEADER: TOML_HEADER.
  CodexTarget: CodexTarget#
  configDir: configDir().
  CodexTarget.supportsLocation: CodexTarget#supportsLocation().
  codexTarget: codexTarget.
  CodexTarget.id: CodexTarget#id.
  CodexTarget.displayName: CodexTarget#displayName.
  CodexTarget.docsUrl: CodexTarget#docsUrl.
---
# Module: [`src/installer/targets/codex.ts`](../../../../../../../raw/code/codegraph/src/installer/targets/codex.ts)

## Classes
### `CodexTarget`  ·  implements/extends AgentTarget
- def: [`src/installer/targets/codex.ts:51`](../../../../../../../raw/code/codegraph/src/installer/targets/codex.ts#L51)
- signature: `class CodexTarget`
- members:
  - `describePaths(method)` — [`L130`](../../../../../../../raw/code/codegraph/src/installer/targets/codex.ts#L130) — Filesystem paths this target would write to at this location.
  - `detect(method)` — [`L60`](../../../../../../../raw/code/codegraph/src/installer/targets/codex.ts#L60) — documented in [installer-targets-types.ts](../../../../concepts/installer-targets-types.ts.md)
  - `install(method)` — [`L76`](../../../../../../../raw/code/codegraph/src/installer/targets/codex.ts#L76) — documented in [installer-targets-shared.ts](../../../../concepts/installer-targets-shared.ts.md)
  - `printConfig(method)` — [`L122`](../../../../../../../raw/code/codegraph/src/installer/targets/codex.ts#L122) — Print the MCP-server snippet a user would paste manually for this
  - `supportsLocation(method)` — [`L56`](../../../../../../../raw/code/codegraph/src/installer/targets/codex.ts#L56) — Whether this target supports the given install location.
  - `uninstall(method)` — [`L95`](../../../../../../../raw/code/codegraph/src/installer/targets/codex.ts#L95) — Inverse of install. Removes only what install would have written; — documented in [installer-targets-types.ts](../../../../concepts/installer-targets-types.ts.md)
  - `displayName` — [`L53`](../../../../../../../raw/code/codegraph/src/installer/targets/codex.ts#L53) — Human-readable name shown in clack prompts and log lines.
  - `docsUrl` — [`L54`](../../../../../../../raw/code/codegraph/src/installer/targets/codex.ts#L54) — Optional URL for "where do I learn more about this agent."
  - `id` — [`L52`](../../../../../../../raw/code/codegraph/src/installer/targets/codex.ts#L52) — Stable id; matches the `TargetId` union.
- uses (calls/refs, reference-scoped): [`Location`](types.ts.md#Location), [`action`](types.ts.md#WriteResult.files.Array.typeLiteral0.action), [`WriteResult`](types.ts.md#WriteResult), [`files`](types.ts.md#WriteResult.files), [`path`](types.ts.md#WriteResult.files.Array.typeLiteral0.path), [`AgentTarget`](types.ts.md#AgentTarget), [`writeMcpEntry`](codex.ts.md#writeMcpEntry), [`upsertInstructionsEntry`](shared.ts.md#upsertInstructionsEntry), [`removeInstructionsEntry`](codex.ts.md#removeInstructionsEntry), [`DetectionResult`](types.ts.md#DetectionResult), [`InstallOptions`](types.ts.md#InstallOptions), [`atomicWriteFileSync`](shared.ts.md#atomicWriteFileSync), [`buildCodegraphBlock`](codex.ts.md#buildCodegraphBlock), [`installed`](types.ts.md#DetectionResult.installed), [`alreadyConfigured`](types.ts.md#DetectionResult.alreadyConfigured), [`removeTomlTable`](toml.ts.md#removeTomlTable), [`notes`](types.ts.md#WriteResult.notes), [`configPath`](types.ts.md#DetectionResult.configPath), [`tomlConfigPath`](codex.ts.md#tomlConfigPath), [`instructionsPath`](codex.ts.md#instructionsPath), [`TOML_HEADER`](codex.ts.md#TOML_HEADER), [`action`](toml.ts.md#removeTomlTable.typeLiteral55.action), [`configDir`](codex.ts.md#configDir), [`content`](toml.ts.md#removeTomlTable.typeLiteral55.content)
- used by: [`AgentTarget`](types.ts.md#AgentTarget), [`codex.ts`](codex.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-installer-targets-codex.ts), [`id`](types.ts.md#AgentTarget.id), [`install`](types.ts.md#AgentTarget.install), [`detect`](types.ts.md#AgentTarget.detect), [`supportsLocation`](types.ts.md#AgentTarget.supportsLocation), [`uninstall`](types.ts.md#AgentTarget.uninstall), [`displayName`](types.ts.md#AgentTarget.displayName), [`printConfig`](types.ts.md#AgentTarget.printConfig), [`describePaths`](types.ts.md#AgentTarget.describePaths), [`docsUrl`](types.ts.md#AgentTarget.docsUrl)

## Functions
- `buildCodegraphBlock()` — [`L136`](../../../../../../../raw/code/codegraph/src/installer/targets/codex.ts#L136) — documented in [installer-targets-shared.ts](../../../../concepts/installer-targets-shared.ts.md)
- `configDir()` — [`L41`](../../../../../../../raw/code/codegraph/src/installer/targets/codex.ts#L41)
- `instructionsPath()` — [`L47`](../../../../../../../raw/code/codegraph/src/installer/targets/codex.ts#L47)
- `removeInstructionsEntry()` — [`L169`](../../../../../../../raw/code/codegraph/src/installer/targets/codex.ts#L169) — Strip the marker-delimited CodeGraph block from `~/.codex/AGENTS.md` — documented in [installer-targets-types.ts](../../../../concepts/installer-targets-types.ts.md)
- `tomlConfigPath()` — [`L44`](../../../../../../../raw/code/codegraph/src/installer/targets/codex.ts#L44)
- `writeMcpEntry()` — [`L144`](../../../../../../../raw/code/codegraph/src/installer/targets/codex.ts#L144) — documented in [installer-targets-types.ts](../../../../concepts/installer-targets-types.ts.md)

## Module values
- `TOML_HEADER` — [`L39`](../../../../../../../raw/code/codegraph/src/installer/targets/codex.ts#L39)
- `codexTarget` — [`L175`](../../../../../../../raw/code/codegraph/src/installer/targets/codex.ts#L175)

