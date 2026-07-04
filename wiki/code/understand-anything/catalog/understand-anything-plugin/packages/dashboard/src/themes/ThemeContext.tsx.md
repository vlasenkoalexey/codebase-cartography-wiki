---
title: 'Module: understand-anything-plugin/packages/dashboard/src/themes/ThemeContext.tsx'
type: catalog
provenance: extracted
module: understand-anything-plugin/packages/dashboard/src/themes/ThemeContext.tsx
status: fresh
symbol_base: scip-typescript npm @understand-anything/dashboard 0.1.0 src/themes/`ThemeContext.tsx`/
symbols:
  ThemeProvider: ThemeProvider().
  useTheme: useTheme().
  resolveInitialTheme: resolveInitialTheme().
  loadFromLocalStorage: loadFromLocalStorage().
  saveToLocalStorage: saveToLocalStorage().
  ThemeContext: ThemeContext.
  ThemeContextValue.preset: ThemeContextValue#preset.
  ThemeProviderProps.metaTheme: ThemeProviderProps#metaTheme.
  ThemeContextValue.config: ThemeContextValue#config.
  ThemeContextValue.setPreset: ThemeContextValue#setPreset.
  ThemeContextValue.setHeadingFont: ThemeContextValue#setHeadingFont.
  STORAGE_KEY: STORAGE_KEY.
  ThemeContextValue: ThemeContextValue#
  ThemeContextValue.setAccent: ThemeContextValue#setAccent.
  ThemeProviderProps: ThemeProviderProps#
  ThemeProviderProps.children: ThemeProviderProps#children.
---
# Module: [`understand-anything-plugin/packages/dashboard/src/themes/ThemeContext.tsx`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/themes/ThemeContext.tsx)

## Classes
### `ThemeContextValue`
- def: [`understand-anything-plugin/packages/dashboard/src/themes/ThemeContext.tsx:17`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/themes/ThemeContext.tsx#L17)
- signature: `interface ThemeContextValue`
- members:
  - `config` — [`L18`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/themes/ThemeContext.tsx#L18)
  - `preset` — [`L19`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/themes/ThemeContext.tsx#L19)
  - `setAccent` — [`L21`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/themes/ThemeContext.tsx#L21)
  - `setHeadingFont` — [`L22`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/themes/ThemeContext.tsx#L22)
  - `setPreset` — [`L20`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/themes/ThemeContext.tsx#L20)
- uses (calls/refs, reference-scoped): [`ThemeConfig`](types.ts.md#ThemeConfig), [`HeadingFont`](types.ts.md#HeadingFont), [`ThemePreset`](types.ts.md#ThemePreset), [`PresetId`](types.ts.md#PresetId)
- used by: [`ThemePicker`](../components/ThemePicker.tsx.md#ThemePicker), [`GraphViewInner`](../components/GraphView.tsx.md#GraphViewInner), [`useTheme`](ThemeContext.tsx.md#useTheme), [`ThemeContext`](ThemeContext.tsx.md#ThemeContext)

### `ThemeProviderProps`
- def: [`understand-anything-plugin/packages/dashboard/src/themes/ThemeContext.tsx:53`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/themes/ThemeContext.tsx#L53)
- signature: `interface ThemeProviderProps`
- members:
  - `children` — [`L55`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/themes/ThemeContext.tsx#L55)
  - `metaTheme` — [`L54`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/themes/ThemeContext.tsx#L54)
- uses (calls/refs, reference-scoped): [`ThemeConfig`](types.ts.md#ThemeConfig)
- used by: [`ThemeProvider`](ThemeContext.tsx.md#ThemeProvider), [`Dashboard`](../App.tsx.md#Dashboard)

## Functions
- `ThemeProvider({ metaTheme, children }: ThemeProviderProps)` — [`L58`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/themes/ThemeContext.tsx#L58)
- `loadFromLocalStorage()` — [`L27`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/themes/ThemeContext.tsx#L27)
- `resolveInitialTheme(metaTheme?: ThemeConfig | null | undefined)` — [`L49`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/themes/ThemeContext.tsx#L49)
- `saveToLocalStorage(config: ThemeConfig)` — [`L41`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/themes/ThemeContext.tsx#L41)
- `useTheme()` — [`L102`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/themes/ThemeContext.tsx#L102)

## Module values
- `STORAGE_KEY` — [`L15`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/themes/ThemeContext.tsx#L15)
- `ThemeContext` — [`L25`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/themes/ThemeContext.tsx#L25)

