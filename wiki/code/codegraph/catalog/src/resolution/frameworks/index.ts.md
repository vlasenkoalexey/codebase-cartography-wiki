---
title: 'Module: src/resolution/frameworks/index.ts'
type: catalog
provenance: extracted
module: src/resolution/frameworks/index.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/resolution/frameworks/`index.ts`/
symbols:
  FRAMEWORK_RESOLVERS: FRAMEWORK_RESOLVERS.
  detectFrameworks: detectFrameworks().
  getApplicableFrameworks: getApplicableFrameworks().
  getFrameworkResolver: getFrameworkResolver().
  registerFrameworkResolver: registerFrameworkResolver().
  getAllFrameworkResolvers: getAllFrameworkResolvers().
---
# Module: [`src/resolution/frameworks/index.ts`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/index.ts)

## Functions
- `detectFrameworks(context: ResolutionContext)` — [`L98`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/index.ts#L98) — Detect which frameworks are used in a project
- `getAllFrameworkResolvers()` — [`L84`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/index.ts#L84) — Get all framework resolvers
- `getApplicableFrameworks(detected: FrameworkResolver[], language: "typescript" | "javascript" | "tsx" | "jsx" | "python" | "go" | "rust" | "java" | "c" | "cpp" | "csharp" | "razor" | "php" | ... 26 more ... | "unknown")` — [`L112`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/index.ts#L112) — Filter a list of detected frameworks down to ones that apply to a given language.
- `getFrameworkResolver(name: string)` — [`L91`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/index.ts#L91) — Get a resolver by name
- `registerFrameworkResolver(resolver: FrameworkResolver)` — [`L124`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/index.ts#L124) — Register a custom framework resolver

## Module values
- `FRAMEWORK_RESOLVERS` — [`L36`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/index.ts#L36) — All registered framework resolvers

