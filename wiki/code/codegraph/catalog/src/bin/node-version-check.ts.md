---
title: 'Module: src/bin/node-version-check.ts'
type: catalog
provenance: extracted
module: src/bin/node-version-check.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/bin/`node-version-check.ts`/
symbols:
  buildNodeTooOldBanner: buildNodeTooOldBanner().
  MIN_NODE_MAJOR: MIN_NODE_MAJOR.
  buildNode25BlockBanner: buildNode25BlockBanner().
---
# Module: [`src/bin/node-version-check.ts`](../../../../../../raw/code/codegraph/src/bin/node-version-check.ts)

## Functions
- `buildNode25BlockBanner(nodeVersion: string)` — [`L20`](../../../../../../raw/code/codegraph/src/bin/node-version-check.ts#L20) — Build the bordered banner shown when CodeGraph detects an
- `buildNodeTooOldBanner(nodeVersion: string)` — [`L58`](../../../../../../raw/code/codegraph/src/bin/node-version-check.ts#L58) — Build the bordered banner shown when CodeGraph detects a Node.js major below

## Module values
- `MIN_NODE_MAJOR` — [`L48`](../../../../../../raw/code/codegraph/src/bin/node-version-check.ts#L48) — Lowest supported Node.js major version. Matches the `engines` floor in

