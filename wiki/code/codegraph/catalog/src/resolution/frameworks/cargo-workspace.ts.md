---
title: 'Module: src/resolution/frameworks/cargo-workspace.ts'
type: catalog
provenance: extracted
module: src/resolution/frameworks/cargo-workspace.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/resolution/frameworks/`cargo-workspace.ts`/
symbols:
  getCargoWorkspaceCrateMap: getCargoWorkspaceCrateMap().
  expandGlobMember: expandGlobMember().
  expandMembers: expandMembers().
  parseWorkspaceMembers: parseWorkspaceMembers().
  getArrayValue: getArrayValue().
  parsePackageName: parsePackageName().
  GLOB_CHARS: GLOB_CHARS.
  getSection: getSection().
  SKIP_DIRS: SKIP_DIRS.
  MAX_GLOB_WALK_DEPTH: MAX_GLOB_WALK_DEPTH.
  extractQuotedValues: extractQuotedValues().
  escapeRegExp: escapeRegExp().
  addCrateAlias: addCrateAlias().
  cleanPath: cleanPath().
---
# Module: [`src/resolution/frameworks/cargo-workspace.ts`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/cargo-workspace.ts)

## Functions
- `addCrateAlias(map: Map<string, string>, crateName: string, memberPath: string)` — [`L157`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/cargo-workspace.ts#L157)
- `cleanPath(memberPath: string)` — [`L165`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/cargo-workspace.ts#L165)
- `escapeRegExp(value: string)` — [`L81`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/cargo-workspace.ts#L81)
- `expandGlobMember(member: string, context: ResolutionContext)` — [`L169`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/cargo-workspace.ts#L169)
- `expandMembers(members: string[], context: ResolutionContext)` — [`L200`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/cargo-workspace.ts#L200)
- `extractQuotedValues(valueList: string)` — [`L42`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/cargo-workspace.ts#L42)
- `getArrayValue(section: string, key: string)` — [`L85`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/cargo-workspace.ts#L85)
- `getCargoWorkspaceCrateMap(context: ResolutionContext)` — [`L224`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/cargo-workspace.ts#L224) — Build a map from crate-name aliases to workspace member directory paths.
- `getSection(content: string, sectionName: string)` — [`L17`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/cargo-workspace.ts#L17)
- `parsePackageName(cargoToml: string)` — [`L150`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/cargo-workspace.ts#L150)
- `parseWorkspaceMembers(cargoToml: string)` — [`L142`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/cargo-workspace.ts#L142)

## Module values
- `GLOB_CHARS` — [`L13`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/cargo-workspace.ts#L13)
- `MAX_GLOB_WALK_DEPTH` — [`L15`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/cargo-workspace.ts#L15)
- `SKIP_DIRS` — [`L14`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/cargo-workspace.ts#L14)

