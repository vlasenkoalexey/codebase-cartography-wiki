---
title: 'Module: src/resolution/frameworks/drupal.ts'
type: catalog
provenance: extracted
module: src/resolution/frameworks/drupal.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/resolution/frameworks/`drupal.ts`/
symbols:
  extractDrupalRoutes: extractDrupalRoutes().
  extractDrupalHooks: extractDrupalHooks().
  isDrupalHookFile: isDrupalHookFile().
  extractDrupalRoutes.typeLiteral9.nodes: extractDrupalRoutes().typeLiteral9:nodes.
  extractDrupalHooks.typeLiteral85.nodes: extractDrupalHooks().typeLiteral85:nodes.
  drupalResolver: drupalResolver.
  lastSegment: lastSegment().
  moduleNameFromPath: moduleNameFromPath().
  extractDrupalRoutes.typeLiteral9.references: extractDrupalRoutes().typeLiteral9:references.
  HOOK_FILE_EXTENSIONS: HOOK_FILE_EXTENSIONS.
  extractDrupalHooks.typeLiteral85.references: extractDrupalHooks().typeLiteral85:references.
---
# Module: [`src/resolution/frameworks/drupal.ts`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/drupal.ts)

## Functions
- `extractDrupalHooks(filePath: string, content: string)` — [`L226`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/drupal.ts#L226) — Extract hook implementation references from a Drupal PHP file.
- `extractDrupalRoutes(filePath: string, content: string)` — [`L97`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/drupal.ts#L97) — Extract route nodes and handler references from a Drupal `*.routing.yml` file.
- `isDrupalHookFile(filePath: string)` — [`L207`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/drupal.ts#L207)
- `lastSegment(fqcn: string)` — [`L62`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/drupal.ts#L62) — Parse the last PHP namespace segment from a FQCN like `\Drupal\mymodule\Controller\Foo`.
- `moduleNameFromPath(filePath: string)` — [`L73`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/drupal.ts#L73) — Derive the Drupal module name from a file path.

## Module values
- `HOOK_FILE_EXTENSIONS` — [`L205`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/drupal.ts#L205)
- `drupalResolver` — [`L296`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/drupal.ts#L296)
- `nodes` — [`L100`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/drupal.ts#L100)
- `nodes` — [`L229`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/drupal.ts#L229)
- `references` — [`L100`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/drupal.ts#L100)
- `references` — [`L229`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/drupal.ts#L229)

