---
title: 'Module: understand-anything-plugin/packages/core/src/plugins/discovery.ts'
type: catalog
provenance: extracted
module: understand-anything-plugin/packages/core/src/plugins/discovery.ts
status: fresh
symbol_base: scip-typescript npm @understand-anything/core 0.1.0 src/plugins/`discovery.ts`/
symbols:
  parsePluginConfig: parsePluginConfig().
  DEFAULT_PLUGIN_CONFIG: DEFAULT_PLUGIN_CONFIG.
  PluginConfig.plugins: PluginConfig#plugins.
  PluginConfig: PluginConfig#
  PluginEntry.name: PluginEntry#name.
  PluginEntry.enabled: PluginEntry#enabled.
  serializePluginConfig: serializePluginConfig().
  PluginEntry.languages: PluginEntry#languages.
  PluginEntry: PluginEntry#
  PluginEntry.options: PluginEntry#options.
---
# Module: [`understand-anything-plugin/packages/core/src/plugins/discovery.ts`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/discovery.ts)

## Classes
### `PluginConfig`
- def: [`understand-anything-plugin/packages/core/src/plugins/discovery.ts:10`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/discovery.ts#L10)
- signature: `interface PluginConfig`
- members:
  - `plugins` — [`L11`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/discovery.ts#L11)
- uses (calls/refs, reference-scoped): [`PluginEntry`](discovery.ts.md#PluginEntry)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-index.ts), [`parsePluginConfig`](discovery.ts.md#parsePluginConfig), [`DEFAULT_PLUGIN_CONFIG`](discovery.ts.md#DEFAULT_PLUGIN_CONFIG), [`plugin-discovery.test.ts`](../__tests__/plugin-discovery.test.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-__tests__-plugin-discovery.test.ts), [`serializePluginConfig`](discovery.ts.md#serializePluginConfig)

### `PluginEntry`
- def: [`understand-anything-plugin/packages/core/src/plugins/discovery.ts:3`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/discovery.ts#L3)
- signature: `interface PluginEntry`
- members:
  - `enabled` — [`L5`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/discovery.ts#L5)
  - `languages` — [`L6`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/discovery.ts#L6)
  - `name` — [`L4`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/discovery.ts#L4)
  - `options` — [`L7`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/discovery.ts#L7)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-index.ts), [`parsePluginConfig`](discovery.ts.md#parsePluginConfig), [`DEFAULT_PLUGIN_CONFIG`](discovery.ts.md#DEFAULT_PLUGIN_CONFIG), [`plugin-discovery.test.ts`](../__tests__/plugin-discovery.test.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-__tests__-plugin-discovery.test.ts), [`PluginConfig`](discovery.ts.md#PluginConfig)

## Functions
- `parsePluginConfig(jsonString: string)` — [`L30`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/discovery.ts#L30) — Parse a plugin config JSON string.
- `serializePluginConfig(config: PluginConfig)` — [`L66`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/discovery.ts#L66) — Serialize a plugin config to JSON for saving.

## Module values
- `DEFAULT_PLUGIN_CONFIG` — [`L14`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/plugins/discovery.ts#L14)

