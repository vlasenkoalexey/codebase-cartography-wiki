---
title: 'Module: src/installer/targets/shared.ts'
type: catalog
provenance: extracted
module: src/installer/targets/shared.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/installer/targets/`shared.ts`/
symbols:
  readJsonFile: readJsonFile().
  writeJsonFile: writeJsonFile().
  upsertInstructionsEntry: upsertInstructionsEntry().
  getMcpServerConfig: getMcpServerConfig().
  jsonDeepEqual: jsonDeepEqual().
  atomicWriteFileSync: atomicWriteFileSync().
  removeMarkedSection: removeMarkedSection().
  replaceOrAppendMarkedSection: replaceOrAppendMarkedSection().
  getMcpServerConfig.typeLiteral2.args: getMcpServerConfig().typeLiteral2:args.
  getMcpServerConfig.typeLiteral2.command: getMcpServerConfig().typeLiteral2:command.
  getCodeGraphPermissions: getCodeGraphPermissions().
  getMcpServerConfig.typeLiteral2.type: getMcpServerConfig().typeLiteral2:type.
  upsertInstructionsEntry.typeLiteral69.path: upsertInstructionsEntry().typeLiteral69:path.
  upsertInstructionsEntry.typeLiteral69.action: upsertInstructionsEntry().typeLiteral69:action.
---
# Module: [`src/installer/targets/shared.ts`](../../../../../../../raw/code/codegraph/src/installer/targets/shared.ts)

## Functions
- `atomicWriteFileSync(filePath: string, content: string)` — [`L81`](../../../../../../../raw/code/codegraph/src/installer/targets/shared.ts#L81) — Write a file atomically: write to `<path>.tmp.<pid>`, then rename. — documented in [installer-targets-shared.ts](../../../../concepts/installer-targets-shared.ts.md)
- `getCodeGraphPermissions()` — [`L47`](../../../../../../../raw/code/codegraph/src/installer/targets/shared.ts#L47) — Permissions list for Claude `settings.json`. Other targets that
- `getMcpServerConfig()` — [`L24`](../../../../../../../raw/code/codegraph/src/installer/targets/shared.ts#L24) — The MCP-server config block codegraph injects. Same shape across — documented in [installer-targets-shared.ts](../../../../concepts/installer-targets-shared.ts.md)
- `jsonDeepEqual(a: unknown, b: unknown)` — [`L111`](../../../../../../../raw/code/codegraph/src/installer/targets/shared.ts#L111) — Compare two JSON values for deep equality, ignoring key order.
- `readJsonFile(filePath: string)` — [`L58`](../../../../../../../raw/code/codegraph/src/installer/targets/shared.ts#L58) — Read a JSON file, returning `{}` when missing or unparseable. — documented in [installer-targets-shared.ts](../../../../concepts/installer-targets-shared.ts.md)
- `removeMarkedSection(filePath: string, startMarker: string, endMarker: string)` — [`L205`](../../../../../../../raw/code/codegraph/src/installer/targets/shared.ts#L205) — Inverse of `replaceOrAppendMarkedSection`. Strips the marker
- `replaceOrAppendMarkedSection(filePath: string, body: string, startMarker: string, endMarker: string)` — [`L142`](../../../../../../../raw/code/codegraph/src/installer/targets/shared.ts#L142) — Replace or append a marker-delimited section in a markdown-ish file. — documented in [installer-targets-shared.ts](../../../../concepts/installer-targets-shared.ts.md)
- `upsertInstructionsEntry(file: string)` — [`L186`](../../../../../../../raw/code/codegraph/src/installer/targets/shared.ts#L186) — Upsert the CodeGraph instructions block into an agent instructions — documented in [installer-targets-shared.ts](../../../../concepts/installer-targets-shared.ts.md)
- `writeJsonFile(filePath: string, data: Record<string, any>)` — [`L100`](../../../../../../../raw/code/codegraph/src/installer/targets/shared.ts#L100) — Atomic JSON write. Trailing newline matches the convention every — documented in [installer-targets-shared.ts](../../../../concepts/installer-targets-shared.ts.md)

## Module values
- `action` — [`L186`](../../../../../../../raw/code/codegraph/src/installer/targets/shared.ts#L186) — documented in [installer-targets-shared.ts](../../../../concepts/installer-targets-shared.ts.md)
- `args` — [`L24`](../../../../../../../raw/code/codegraph/src/installer/targets/shared.ts#L24) — documented in [installer-targets-shared.ts](../../../../concepts/installer-targets-shared.ts.md)
- `command` — [`L24`](../../../../../../../raw/code/codegraph/src/installer/targets/shared.ts#L24) — documented in [installer-targets-shared.ts](../../../../concepts/installer-targets-shared.ts.md)
- `path` — [`L186`](../../../../../../../raw/code/codegraph/src/installer/targets/shared.ts#L186) — documented in [installer-targets-shared.ts](../../../../concepts/installer-targets-shared.ts.md)
- `type` — [`L24`](../../../../../../../raw/code/codegraph/src/installer/targets/shared.ts#L24) — documented in [installer-targets-shared.ts](../../../../concepts/installer-targets-shared.ts.md)

