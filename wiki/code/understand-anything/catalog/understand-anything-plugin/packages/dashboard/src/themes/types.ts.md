---
title: 'Module: understand-anything-plugin/packages/dashboard/src/themes/types.ts'
type: catalog
provenance: extracted
module: understand-anything-plugin/packages/dashboard/src/themes/types.ts
status: fresh
symbol_base: scip-typescript npm @understand-anything/dashboard 0.1.0 src/themes/`types.ts`/
symbols:
  AccentSwatch.id: AccentSwatch#id.
  AccentSwatch.accent: AccentSwatch#accent.
  AccentSwatch.name: AccentSwatch#name.
  AccentSwatch.accentDim: AccentSwatch#accentDim.
  AccentSwatch.accentBright: AccentSwatch#accentBright.
  ThemeConfig: ThemeConfig#
  ThemePreset.accentSwatches: ThemePreset#accentSwatches.
  ThemePreset.id: ThemePreset#id.
  HeadingFont: HeadingFont#
  ThemePreset.isDark: ThemePreset#isDark.
  ThemePreset.colors: ThemePreset#colors.
  ThemePreset.defaultAccentId: ThemePreset#defaultAccentId.
  ThemePreset: ThemePreset#
  ThemeConfig.presetId: ThemeConfig#presetId.
  PresetId: PresetId#
  AccentSwatch: AccentSwatch#
  ThemePreset.name: ThemePreset#name.
  ThemeConfig.headingFont: ThemeConfig#headingFont.
  ThemeConfig.accentId: ThemeConfig#accentId.
  DEFAULT_THEME_CONFIG: DEFAULT_THEME_CONFIG.
---
# Module: [`understand-anything-plugin/packages/dashboard/src/themes/types.ts`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/themes/types.ts)

## Classes
### `AccentSwatch`
- def: [`understand-anything-plugin/packages/dashboard/src/themes/types.ts:8`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/themes/types.ts#L8)
- signature: `interface AccentSwatch`
- members:
  - `accent` — [`L11`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/themes/types.ts#L11) — documented in [understand-anything-plugin-packages-dashboard-src-themes-types.ts](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-themes-types.ts.md)
  - `accentBright` — [`L13`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/themes/types.ts#L13)
  - `accentDim` — [`L12`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/themes/types.ts#L12) — documented in [understand-anything-plugin-packages-dashboard-src-themes-types.ts](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-themes-types.ts.md)
  - `id` — [`L9`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/themes/types.ts#L9) — documented in [understand-anything-plugin-packages-dashboard-src-themes-types.ts](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-themes-types.ts.md)
  - `name` — [`L10`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/themes/types.ts#L10) — documented in [understand-anything-plugin-packages-dashboard-src-themes-types.ts](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-themes-types.ts.md)
- used by: [`ThemePicker`](../components/ThemePicker.tsx.md#ThemePicker), [`index.ts`](index.ts.md#scip-typescript-npm-understand-anything-dashboard-0.1.0-src-themes-index.ts), [`applyTheme`](theme-engine.ts.md#applyTheme), [`DARK_ACCENT_SWATCHES`](presets.ts.md#DARK_ACCENT_SWATCHES), [`LIGHT_ACCENT_SWATCHES`](presets.ts.md#LIGHT_ACCENT_SWATCHES), [`getAccent`](presets.ts.md#getAccent), [`accentSwatches`](types.ts.md#ThemePreset.accentSwatches), [`presets.ts`](presets.ts.md#scip-typescript-npm-understand-anything-dashboard-0.1.0-src-themes-presets.ts)

### `HeadingFont`
- def: [`understand-anything-plugin/packages/dashboard/src/themes/types.ts:25`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/themes/types.ts#L25)
- signature: `type HeadingFont`
- used by: [`ThemePicker`](../components/ThemePicker.tsx.md#ThemePicker), [`index.ts`](index.ts.md#scip-typescript-npm-understand-anything-dashboard-0.1.0-src-themes-index.ts), [`ThemeProvider`](ThemeContext.tsx.md#ThemeProvider), [`ThemeContext.tsx`](ThemeContext.tsx.md#scip-typescript-npm-understand-anything-dashboard-0.1.0-src-themes-ThemeContext.tsx), [`ThemePicker.tsx`](../components/ThemePicker.tsx.md#scip-typescript-npm-understand-anything-dashboard-0.1.0-src-components-ThemePicker.tsx), [`headingFont`](types.ts.md#ThemeConfig.headingFont), [`setHeadingFont`](ThemeContext.tsx.md#ThemeContextValue.setHeadingFont)

### `PresetId`
- def: [`understand-anything-plugin/packages/dashboard/src/themes/types.ts:1`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/themes/types.ts#L1)
- signature: `type PresetId`
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-understand-anything-dashboard-0.1.0-src-themes-index.ts), [`ThemeProvider`](ThemeContext.tsx.md#ThemeProvider), [`ThemeContext.tsx`](ThemeContext.tsx.md#scip-typescript-npm-understand-anything-dashboard-0.1.0-src-themes-ThemeContext.tsx), [`id`](types.ts.md#ThemePreset.id), [`presetId`](types.ts.md#ThemeConfig.presetId), [`setPreset`](ThemeContext.tsx.md#ThemeContextValue.setPreset)

### `ThemeConfig`
- def: [`understand-anything-plugin/packages/dashboard/src/themes/types.ts:27`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/themes/types.ts#L27)
- signature: `interface ThemeConfig`
- members:
  - `accentId` — [`L29`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/themes/types.ts#L29)
  - `headingFont` — [`L30`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/themes/types.ts#L30)
  - `presetId` — [`L28`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/themes/types.ts#L28)
- uses (calls/refs, reference-scoped): [`HeadingFont`](types.ts.md#HeadingFont), [`PresetId`](types.ts.md#PresetId)
- used by: [`App.tsx`](../App.tsx.md#scip-typescript-npm-understand-anything-dashboard-0.1.0-src-App.tsx), [`ThemePicker`](../components/ThemePicker.tsx.md#ThemePicker), [`index.ts`](index.ts.md#scip-typescript-npm-understand-anything-dashboard-0.1.0-src-themes-index.ts), [`ThemeProvider`](ThemeContext.tsx.md#ThemeProvider), [`applyTheme`](theme-engine.ts.md#applyTheme), [`Dashboard`](../App.tsx.md#Dashboard), [`ThemeContext.tsx`](ThemeContext.tsx.md#scip-typescript-npm-understand-anything-dashboard-0.1.0-src-themes-ThemeContext.tsx), [`theme-engine.ts`](theme-engine.ts.md#scip-typescript-npm-understand-anything-dashboard-0.1.0-src-themes-theme-engine.ts), [`types.ts`](types.ts.md#scip-typescript-npm-understand-anything-dashboard-0.1.0-src-themes-types.ts), [`resolveInitialTheme`](ThemeContext.tsx.md#resolveInitialTheme), [`loadFromLocalStorage`](ThemeContext.tsx.md#loadFromLocalStorage), [`saveToLocalStorage`](ThemeContext.tsx.md#saveToLocalStorage), [`metaTheme`](ThemeContext.tsx.md#ThemeProviderProps.metaTheme), [`config`](ThemeContext.tsx.md#ThemeContextValue.config)

### `ThemePreset`
- def: [`understand-anything-plugin/packages/dashboard/src/themes/types.ts:16`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/themes/types.ts#L16)
- signature: `interface ThemePreset`
- members:
  - `accentSwatches` — [`L21`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/themes/types.ts#L21)
  - `colors` — [`L20`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/themes/types.ts#L20)
  - `defaultAccentId` — [`L22`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/themes/types.ts#L22)
  - `id` — [`L17`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/themes/types.ts#L17)
  - `isDark` — [`L19`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/themes/types.ts#L19)
  - `name` — [`L18`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/themes/types.ts#L18)
- uses (calls/refs, reference-scoped): [`AccentSwatch`](types.ts.md#AccentSwatch), [`PresetId`](types.ts.md#PresetId)
- used by: [`ThemePicker`](../components/ThemePicker.tsx.md#ThemePicker), [`index.ts`](index.ts.md#scip-typescript-npm-understand-anything-dashboard-0.1.0-src-themes-index.ts), [`ThemeProvider`](ThemeContext.tsx.md#ThemeProvider), [`applyTheme`](theme-engine.ts.md#applyTheme), [`PRESETS`](presets.ts.md#PRESETS), [`GraphViewInner`](../components/GraphView.tsx.md#GraphViewInner), [`ThemeContext.tsx`](ThemeContext.tsx.md#scip-typescript-npm-understand-anything-dashboard-0.1.0-src-themes-ThemeContext.tsx), [`getAccent`](presets.ts.md#getAccent), [`getPreset`](presets.ts.md#getPreset), [`presets.ts`](presets.ts.md#scip-typescript-npm-understand-anything-dashboard-0.1.0-src-themes-presets.ts), [`preset`](ThemeContext.tsx.md#ThemeContextValue.preset)

## Module values
- `DEFAULT_THEME_CONFIG` — [`L33`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/themes/types.ts#L33)

