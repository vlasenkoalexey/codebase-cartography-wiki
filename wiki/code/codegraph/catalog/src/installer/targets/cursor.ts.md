---
title: 'Module: src/installer/targets/cursor.ts'
type: catalog
provenance: extracted
module: src/installer/targets/cursor.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/installer/targets/`cursor.ts`/
symbols:
  writeMcpEntry: writeMcpEntry().
  removeRulesEntry: removeRulesEntry().
  CursorTarget.uninstall: CursorTarget#uninstall().
  CursorTarget.install: CursorTarget#install().
  CursorTarget.detect: CursorTarget#detect().
  buildCursorMcpConfig: buildCursorMcpConfig().
  mcpJsonPath: mcpJsonPath().
  CursorTarget.printConfig: CursorTarget#printConfig().
  CursorTarget.describePaths: CursorTarget#describePaths().
  CursorTarget: CursorTarget#
  CursorTarget.supportsLocation: CursorTarget#supportsLocation().
  rulesPath: rulesPath().
  cursorTarget: cursorTarget.
  MDC_FRONTMATTER: MDC_FRONTMATTER.
  buildCursorMcpConfig.typeLiteral36.args: buildCursorMcpConfig().typeLiteral36:args.
  CursorTarget.id: CursorTarget#id.
  CursorTarget.displayName: CursorTarget#displayName.
  CursorTarget.docsUrl: CursorTarget#docsUrl.
  buildCursorMcpConfig.typeLiteral36.type: buildCursorMcpConfig().typeLiteral36:type.
  buildCursorMcpConfig.typeLiteral36.command: buildCursorMcpConfig().typeLiteral36:command.
---
# Module: [`src/installer/targets/cursor.ts`](../../../../../../../raw/code/codegraph/src/installer/targets/cursor.ts)

## Classes
### `CursorTarget`  ·  implements/extends AgentTarget
- def: [`src/installer/targets/cursor.ts:84`](../../../../../../../raw/code/codegraph/src/installer/targets/cursor.ts#L84)
- signature: `class CursorTarget`
- members:
  - `describePaths(method)` — [`L157`](../../../../../../../raw/code/codegraph/src/installer/targets/cursor.ts#L157) — Filesystem paths this target would write to at this location.
  - `detect(method)` — [`L96`](../../../../../../../raw/code/codegraph/src/installer/targets/cursor.ts#L96) — documented in [installer-targets-shared.ts](../../../../concepts/installer-targets-shared.ts.md)
  - `install(method)` — [`L108`](../../../../../../../raw/code/codegraph/src/installer/targets/cursor.ts#L108) — documented in [installer-targets-types.ts](../../../../concepts/installer-targets-types.ts.md)
  - `printConfig(method)` — [`L151`](../../../../../../../raw/code/codegraph/src/installer/targets/cursor.ts#L151) — Print the MCP-server snippet a user would paste manually for this
  - `supportsLocation(method)` — [`L89`](../../../../../../../raw/code/codegraph/src/installer/targets/cursor.ts#L89) — Whether this target supports the given install location.
  - `uninstall(method)` — [`L128`](../../../../../../../raw/code/codegraph/src/installer/targets/cursor.ts#L128) — Inverse of install. Removes only what install would have written; — documented in [installer-targets-shared.ts](../../../../concepts/installer-targets-shared.ts.md)
  - `displayName` — [`L86`](../../../../../../../raw/code/codegraph/src/installer/targets/cursor.ts#L86) — Human-readable name shown in clack prompts and log lines.
  - `docsUrl` — [`L87`](../../../../../../../raw/code/codegraph/src/installer/targets/cursor.ts#L87) — Optional URL for "where do I learn more about this agent."
  - `id` — [`L85`](../../../../../../../raw/code/codegraph/src/installer/targets/cursor.ts#L85) — Stable id; matches the `TargetId` union.
- uses (calls/refs, reference-scoped): [`Location`](types.ts.md#Location), [`action`](types.ts.md#WriteResult.files.Array.typeLiteral0.action), [`WriteResult`](types.ts.md#WriteResult), [`files`](types.ts.md#WriteResult.files), [`path`](types.ts.md#WriteResult.files.Array.typeLiteral0.path), [`AgentTarget`](types.ts.md#AgentTarget), [`readJsonFile`](shared.ts.md#readJsonFile), [`writeMcpEntry`](cursor.ts.md#writeMcpEntry), [`removeRulesEntry`](cursor.ts.md#removeRulesEntry), [`writeJsonFile`](shared.ts.md#writeJsonFile), [`DetectionResult`](types.ts.md#DetectionResult), [`InstallOptions`](types.ts.md#InstallOptions), [`installed`](types.ts.md#DetectionResult.installed), [`alreadyConfigured`](types.ts.md#DetectionResult.alreadyConfigured), [`buildCursorMcpConfig`](cursor.ts.md#buildCursorMcpConfig), [`notes`](types.ts.md#WriteResult.notes), [`mcpJsonPath`](cursor.ts.md#mcpJsonPath), [`configPath`](types.ts.md#DetectionResult.configPath), [`rulesPath`](cursor.ts.md#rulesPath)
- used by: [`AgentTarget`](types.ts.md#AgentTarget), [`cursor.ts`](cursor.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-installer-targets-cursor.ts), [`id`](types.ts.md#AgentTarget.id), [`install`](types.ts.md#AgentTarget.install), [`detect`](types.ts.md#AgentTarget.detect), [`supportsLocation`](types.ts.md#AgentTarget.supportsLocation), [`uninstall`](types.ts.md#AgentTarget.uninstall), [`displayName`](types.ts.md#AgentTarget.displayName), [`printConfig`](types.ts.md#AgentTarget.printConfig), [`describePaths`](types.ts.md#AgentTarget.describePaths), [`docsUrl`](types.ts.md#AgentTarget.docsUrl)

## Functions
- `buildCursorMcpConfig(loc: Location)` — [`L171`](../../../../../../../raw/code/codegraph/src/installer/targets/cursor.ts#L171) — Build the codegraph MCP-server config for Cursor at the given — documented in [installer-targets-shared.ts](../../../../concepts/installer-targets-shared.ts.md)
- `mcpJsonPath(loc: Location)` — [`L56`](../../../../../../../raw/code/codegraph/src/installer/targets/cursor.ts#L56)
- `removeRulesEntry()` — [`L208`](../../../../../../../raw/code/codegraph/src/installer/targets/cursor.ts#L208) — Remove the Cursor rules file on uninstall (and as a self-heal on — documented in [installer-targets-types.ts](../../../../concepts/installer-targets-types.ts.md)
- `rulesPath()` — [`L66`](../../../../../../../raw/code/codegraph/src/installer/targets/cursor.ts#L66) — Cursor "rules" file. Only meaningful for the project-local
- `writeMcpEntry(loc: Location)` — [`L177`](../../../../../../../raw/code/codegraph/src/installer/targets/cursor.ts#L177) — documented in [installer-targets-shared.ts](../../../../concepts/installer-targets-shared.ts.md)

## Module values
- `MDC_FRONTMATTER` — [`L76`](../../../../../../../raw/code/codegraph/src/installer/targets/cursor.ts#L76) — Cursor `.mdc` rules use YAML-ish frontmatter. `alwaysApply: true`
- `args` — [`L171`](../../../../../../../raw/code/codegraph/src/installer/targets/cursor.ts#L171)
- `command` — [`L171`](../../../../../../../raw/code/codegraph/src/installer/targets/cursor.ts#L171)
- `cursorTarget` — [`L247`](../../../../../../../raw/code/codegraph/src/installer/targets/cursor.ts#L247)
- `type` — [`L171`](../../../../../../../raw/code/codegraph/src/installer/targets/cursor.ts#L171)

