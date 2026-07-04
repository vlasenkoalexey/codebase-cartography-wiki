---
title: 'Module: src/installer/config-writer.ts'
type: catalog
provenance: extracted
module: src/installer/config-writer.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/installer/`config-writer.ts`/
symbols:
  writeMcpConfig: writeMcpConfig().
  writePermissions: writePermissions().
  hasMcpConfig: hasMcpConfig().
  hasPermissions: hasPermissions().
  InstallLocation: InstallLocation#
---
# Module: [`src/installer/config-writer.ts`](../../../../../../raw/code/codegraph/src/installer/config-writer.ts)

## Classes
### `InstallLocation`
- def: [`src/installer/config-writer.ts:22`](../../../../../../raw/code/codegraph/src/installer/config-writer.ts#L22)
- signature: `type InstallLocation`
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-installer-index.ts), [`hasMcpConfig`](config-writer.ts.md#hasMcpConfig), [`hasPermissions`](config-writer.ts.md#hasPermissions), [`writeMcpConfig`](config-writer.ts.md#writeMcpConfig), [`writePermissions`](config-writer.ts.md#writePermissions)

## Functions
- `hasMcpConfig(location: InstallLocation)` — [`L42`](../../../../../../raw/code/codegraph/src/installer/config-writer.ts#L42) — documented in [installer-targets-shared.ts](../../../concepts/installer-targets-shared.ts.md)
- `hasPermissions(location: InstallLocation)` — [`L52`](../../../../../../raw/code/codegraph/src/installer/config-writer.ts#L52) — documented in [installer-targets-shared.ts](../../../concepts/installer-targets-shared.ts.md)
- `writeMcpConfig(location: InstallLocation)` — [`L34`](../../../../../../raw/code/codegraph/src/installer/config-writer.ts#L34) — Each shim calls ONLY the named per-file helper — writeMcpConfig
- `writePermissions(location: InstallLocation)` — [`L38`](../../../../../../raw/code/codegraph/src/installer/config-writer.ts#L38)

