---
title: 'Module: src/installer/targets/toml.ts'
type: catalog
provenance: extracted
module: src/installer/targets/toml.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/installer/targets/`toml.ts`/
symbols:
  upsertTomlTable: upsertTomlTable().
  removeTomlTable: removeTomlTable().
  buildTomlTable: buildTomlTable().
  upsertTomlTable.typeLiteral18.content: upsertTomlTable().typeLiteral18:content.
  upsertTomlTable.typeLiteral18.action: upsertTomlTable().typeLiteral18:action.
  serializeTomlTableBody: serializeTomlTableBody().
  removeTomlTable.typeLiteral55.content: removeTomlTable().typeLiteral55:content.
  removeTomlTable.typeLiteral55.action: removeTomlTable().typeLiteral55:action.
  quoteString: quoteString().
  findHeaderIndex: findHeaderIndex().
  findNextTableHeader: findNextTableHeader().
---
# Module: [`src/installer/targets/toml.ts`](../../../../../../../raw/code/codegraph/src/installer/targets/toml.ts)

## Functions
- `buildTomlTable(header: string, values: Record<string, string | string[]>)` — [`L52`](../../../../../../../raw/code/codegraph/src/installer/targets/toml.ts#L52) — Build a full table block: header line + body. Suitable for direct
- `findHeaderIndex(content: string, headerLine: string)` — [`L127`](../../../../../../../raw/code/codegraph/src/installer/targets/toml.ts#L127) — Locate the byte index of a header line (`[foo.bar]`) when it
- `findNextTableHeader(content: string, from: number)` — [`L140`](../../../../../../../raw/code/codegraph/src/installer/targets/toml.ts#L140) — Find the byte index of the next top-level `[...]` table header
- `quoteString(s: string)` — [`L42`](../../../../../../../raw/code/codegraph/src/installer/targets/toml.ts#L42)
- `removeTomlTable(fileContent: string, header: string)` — [`L108`](../../../../../../../raw/code/codegraph/src/installer/targets/toml.ts#L108) — Remove a top-level dotted-key TOML table block. Returns the
- `serializeTomlTableBody(values: Record<string, string | string[]>)` — [`L27`](../../../../../../../raw/code/codegraph/src/installer/targets/toml.ts#L27) — Serialize a record into the body lines of a TOML table. Values
- `upsertTomlTable(fileContent: string, header: string, block: string)` — [`L64`](../../../../../../../raw/code/codegraph/src/installer/targets/toml.ts#L64) — Insert or replace a top-level dotted-key TOML table block in the

## Module values
- `action` — [`L68`](../../../../../../../raw/code/codegraph/src/installer/targets/toml.ts#L68)
- `action` — [`L111`](../../../../../../../raw/code/codegraph/src/installer/targets/toml.ts#L111)
- `content` — [`L68`](../../../../../../../raw/code/codegraph/src/installer/targets/toml.ts#L68)
- `content` — [`L111`](../../../../../../../raw/code/codegraph/src/installer/targets/toml.ts#L111)

