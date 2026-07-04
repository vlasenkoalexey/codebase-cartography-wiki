---
title: 'Module: understand-anything-plugin/packages/dashboard/src/App.tsx'
type: catalog
provenance: extracted
module: understand-anything-plugin/packages/dashboard/src/App.tsx
status: fresh
symbol_base: scip-typescript npm @understand-anything/dashboard 0.1.0 src/`App.tsx`/
symbols:
  DashboardContent: DashboardContent().
  Dashboard: Dashboard().
  App: App().
  dataUrl: dataUrl().
  resolveInitialToken: resolveInitialToken().
  CodeViewer: CodeViewer.
  LearnPanel: LearnPanel.
  PathFinderModal: PathFinderModal.
  KeyboardShortcutsHelp: KeyboardShortcutsHelp.
  OnboardingOverlay: OnboardingOverlay.
  shouldShowOnboarding: shouldShowOnboarding().
  DEMO_MODE: DEMO_MODE.
  SESSION_TOKEN_KEY: SESSION_TOKEN_KEY.
  Dashboard.-accessToken-.typeLiteral47.accessToken: Dashboard().(`{ accessToken }`)typeLiteral47:accessToken.
  ONBOARDING_DISMISSED_KEY: ONBOARDING_DISMISSED_KEY.
  DashboardContent.-accessToken-loadError-graphIssues-.typeLiteral161.accessToken: "DashboardContent().(`{\n\
    \  accessToken,\n  loadError,\n  graphIssues,\n}`)typeLiteral161:accessToken."
  DashboardContent.-accessToken-loadError-graphIssues-.typeLiteral161.loadError: "DashboardContent().(`{\n\
    \  accessToken,\n  loadError,\n  graphIssues,\n}`)typeLiteral161:loadError."
  DashboardContent.-accessToken-loadError-graphIssues-.typeLiteral161.graphIssues: "DashboardContent().(`{\n\
    \  accessToken,\n  loadError,\n  graphIssues,\n}`)typeLiteral161:graphIssues."
  SidebarTab: SidebarTab#
---
# Module: [`understand-anything-plugin/packages/dashboard/src/App.tsx`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/App.tsx)

## Classes
### `SidebarTab`
- def: [`understand-anything-plugin/packages/dashboard/src/App.tsx:40`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/App.tsx#L40)
- signature: `type SidebarTab`
- used by: [`DashboardContent`](App.tsx.md#DashboardContent)

## Functions
- `App()` — [`L89`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/App.tsx#L89)
- `Dashboard({ accessToken }: { accessToken: string; })` — [`L110`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/App.tsx#L110) — documented in [understand-anything-plugin-packages-dashboard-src-contexts-I18nContext.tsx](../../../../../concepts/understand-anything-plugin-packages-dashboard-src-contexts-I18nContext.tsx.md)
- `DashboardContent({ accessToken, loadError, graphIssues, }: { accessToken: string; loadError: string | null; graphIssues: GraphIssue[]; })` — [`L222`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/App.tsx#L222) — documented in [understand-anything-plugin-packages-dashboard-src-components-FileExplorer.tsx](../../../../../concepts/understand-anything-plugin-packages-dashboard-src-components-FileExplorer.tsx.md)
- `dataUrl(fileName: string, token: string | null)` — [`L50`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/App.tsx#L50) — Resolve data file URL — in demo mode, use env var URLs; otherwise use local paths with token.
- `resolveInitialToken()` — [`L72`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/App.tsx#L72) — Resolve the access token from the URL query string or sessionStorage.
- `shouldShowOnboarding()` — [`L42`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/App.tsx#L42)

## Module values
- `CodeViewer` — [`L29`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/App.tsx#L29)
- `DEMO_MODE` — [`L37`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/App.tsx#L37)
- `KeyboardShortcutsHelp` — [`L32`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/App.tsx#L32)
- `LearnPanel` — [`L30`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/App.tsx#L30)
- `ONBOARDING_DISMISSED_KEY` — [`L39`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/App.tsx#L39)
- `OnboardingOverlay` — [`L35`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/App.tsx#L35)
- `PathFinderModal` — [`L31`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/App.tsx#L31)
- `SESSION_TOKEN_KEY` — [`L38`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/App.tsx#L38)
- `accessToken` — [`L110`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/App.tsx#L110)
- `accessToken` — [`L227`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/App.tsx#L227)
- `graphIssues` — [`L229`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/App.tsx#L229)
- `loadError` — [`L228`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/App.tsx#L228)

