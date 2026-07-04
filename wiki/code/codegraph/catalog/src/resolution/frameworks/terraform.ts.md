---
title: 'Module: src/resolution/frameworks/terraform.ts'
type: catalog
provenance: extracted
module: src/resolution/frameworks/terraform.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/resolution/frameworks/`terraform.ts`/
symbols:
  terraformResolver: terraformResolver.
  resolveScopedModuleRef: resolveScopedModuleRef().
  readNodeSpanMatch: readNodeSpanMatch().
  dirOf: dirOf().
  nearestAncestorMatch: nearestAncestorMatch().
  readModuleAttr: readModuleAttr().
  parentOf: parentOf().
  SCOPED_REF: SCOPED_REF.
  nearestAncestorMatch.T-typeLiteral43.filePath: nearestAncestorMatch().[T]typeLiteral43:filePath.
  joinDirs: joinDirs().
  normalizeRel: normalizeRel().
---
# Module: [`src/resolution/frameworks/terraform.ts`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/terraform.ts)

## Functions
- `dirOf(p: string)` — [`L238`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/terraform.ts#L238) — Directory of a stored (forward-slash, project-relative) path.
- `joinDirs(base: string, rel: string)` — [`L251`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/terraform.ts#L251) — Join a base directory with a `./`/`../` relative source path.
- `nearestAncestorMatch(candidates: T[], refDir: string)` — [`L116`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/terraform.ts#L116) — Nearest candidate walking UP the directory tree from refDir (exclusive).
- `normalizeRel(p: string)` — [`L256`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/terraform.ts#L256) — Normalize to the stored path shape: forward slashes, '.' for the root.
- `parentOf(dir: string)` — [`L244`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/terraform.ts#L244) — Parent directory, or null above the project root.
- `readModuleAttr(decl: Node, name: string, context: ResolutionContext)` — [`L220`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/terraform.ts#L220) — A direct string-literal attribute (`source = "…"`, `component = "…"`) of a
- `readNodeSpanMatch(node: Node, re: RegExp, context: ResolutionContext)` — [`L225`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/terraform.ts#L225) — First capture of `re` across the node's line span, or null.
- `resolveScopedModuleRef(ref: UnresolvedRef, moduleName: string, child: string, refDir: string, context: ResolutionContext)` — [`L129`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/terraform.ts#L129) — Resolve `module.M:<child>` by locating the `module "M"` declaration in the

## Module values
- `SCOPED_REF` — [`L42`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/terraform.ts#L42) — `module.M:file` / `module.M:var.X` / `module.M:output.X` / `module.M:remote-output.X` — extractor-emitted scoped refs.
- `filePath` — [`L116`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/terraform.ts#L116)
- `terraformResolver` — [`L44`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/terraform.ts#L44)

