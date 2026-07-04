---
title: 'Module: src/commands.ts'
type: catalog
provenance: extracted
module: src/commands.ts
status: fresh
symbol_base: scip-typescript npm openwiki 0.0.1 src/`commands.ts`/
symbols:
  helpContent: helpContent.
  getHelpText: getHelpText().
  parseCommand: parseCommand().
  CliCommand: CliCommand#
  HelpRow.typeLiteral0.label: HelpRow#typeLiteral0:label.
  formatRows: formatRows().
  HelpRow.typeLiteral0.description: HelpRow#typeLiteral0:description.
  HelpRow: HelpRow#
  isDevelopmentMode: isDevelopmentMode().
  HelpContent.typeLiteral1.commands: HelpContent#typeLiteral1:commands.
  HelpContent.typeLiteral1.options: HelpContent#typeLiteral1:options.
  HelpContent.typeLiteral1.developmentOptions: HelpContent#typeLiteral1:developmentOptions.
  HelpContent.typeLiteral1.description: HelpContent#typeLiteral1:description.
  HelpContent.typeLiteral1.usage: HelpContent#typeLiteral1:usage.
  HelpContent.typeLiteral1.examples: HelpContent#typeLiteral1:examples.
  HelpContent.typeLiteral1.developmentExamples: HelpContent#typeLiteral1:developmentExamples.
  HelpContent.typeLiteral1.title: HelpContent#typeLiteral1:title.
  HelpContent: HelpContent#
---
# Module: [`src/commands.ts`](../../../../../raw/code/openwiki/src/commands.ts)

## Classes
### `CliCommand`
- def: [`src/commands.ts:20`](../../../../../raw/code/openwiki/src/commands.ts#L20) — documented in [openwiki-agent-types.ts](../../concepts/openwiki-agent-types.ts.md)
- signature: `type CliCommand`
- uses (calls/refs, reference-scoped): [`OpenWikiCommand`](agent/types.ts.md#OpenWikiCommand)
- used by: [`cli.tsx`](cli.tsx.md#scip-typescript-npm-openwiki-0.0.1-src-cli.tsx), [`runPrintCommand`](cli.tsx.md#runPrintCommand), [`parseCommand`](commands.ts.md#parseCommand), [`resolveStartupCommand`](cli.tsx.md#resolveStartupCommand), [`shouldPrintStartupError`](cli.tsx.md#shouldPrintStartupError), [`AppProps`](cli.tsx.md#AppProps), [`shouldAutoExitStartupRun`](cli.tsx.md#shouldAutoExitStartupRun)

### `HelpContent`
- def: [`src/commands.ts:9`](../../../../../raw/code/openwiki/src/commands.ts#L9) — documented in [openwiki-commands.ts](../../concepts/openwiki-commands.ts.md)
- signature: `type HelpContent`
- members:
  - `commands` — [`L13`](../../../../../raw/code/openwiki/src/commands.ts#L13) — documented in [openwiki-commands.ts](../../concepts/openwiki-commands.ts.md)
  - `description` — [`L11`](../../../../../raw/code/openwiki/src/commands.ts#L11)
  - `developmentExamples` — [`L17`](../../../../../raw/code/openwiki/src/commands.ts#L17)
  - `developmentOptions` — [`L15`](../../../../../raw/code/openwiki/src/commands.ts#L15)
  - `examples` — [`L16`](../../../../../raw/code/openwiki/src/commands.ts#L16) — documented in [openwiki-commands.ts](../../concepts/openwiki-commands.ts.md)
  - `options` — [`L14`](../../../../../raw/code/openwiki/src/commands.ts#L14) — documented in [openwiki-commands.ts](../../concepts/openwiki-commands.ts.md)
  - `title` — [`L10`](../../../../../raw/code/openwiki/src/commands.ts#L10)
  - `usage` — [`L12`](../../../../../raw/code/openwiki/src/commands.ts#L12) — documented in [openwiki-commands.ts](../../concepts/openwiki-commands.ts.md)
- uses (calls/refs, reference-scoped): [`HelpRow`](commands.ts.md#HelpRow)
- used by: [`helpContent`](commands.ts.md#helpContent), [`HelpView`](cli.tsx.md#HelpView), [`getHelpText`](commands.ts.md#getHelpText)

### `HelpRow`
- def: [`src/commands.ts:4`](../../../../../raw/code/openwiki/src/commands.ts#L4) — documented in [openwiki-commands.ts](../../concepts/openwiki-commands.ts.md)
- signature: `type HelpRow`
- members:
  - `description` — [`L6`](../../../../../raw/code/openwiki/src/commands.ts#L6)
  - `label` — [`L5`](../../../../../raw/code/openwiki/src/commands.ts#L5)
- used by: [`cli.tsx`](cli.tsx.md#scip-typescript-npm-openwiki-0.0.1-src-cli.tsx), [`helpContent`](commands.ts.md#helpContent), [`Rows`](cli.tsx.md#Rows), [`formatRows`](commands.ts.md#formatRows), [`commands`](commands.ts.md#HelpContent.typeLiteral1.commands), [`developmentOptions`](commands.ts.md#HelpContent.typeLiteral1.developmentOptions), [`options`](commands.ts.md#HelpContent.typeLiteral1.options), [`RowsProps`](cli.tsx.md#RowsProps)

## Functions
- `formatRows(rows: HelpRow[])` — [`L262`](../../../../../raw/code/openwiki/src/commands.ts#L262) — documented in [openwiki-commands.ts](../../concepts/openwiki-commands.ts.md)
- `getHelpText()` — [`L224`](../../../../../raw/code/openwiki/src/commands.ts#L224) — documented in [openwiki-commands.ts](../../concepts/openwiki-commands.ts.md)
- `isDevelopmentMode()` — [`L166`](../../../../../raw/code/openwiki/src/commands.ts#L166) — documented in [openwiki-commands.ts](../../concepts/openwiki-commands.ts.md)
- `parseCommand(argv: string[])` — [`L38`](../../../../../raw/code/openwiki/src/commands.ts#L38) — documented in [openwiki-agent-types.ts](../../concepts/openwiki-agent-types.ts.md)

## Module values
- `helpContent` — [`L172`](../../../../../raw/code/openwiki/src/commands.ts#L172) — documented in [openwiki-commands.ts](../../concepts/openwiki-commands.ts.md)

