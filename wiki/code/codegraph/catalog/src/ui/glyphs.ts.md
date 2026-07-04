---
title: 'Module: src/ui/glyphs.ts'
type: catalog
provenance: extracted
module: src/ui/glyphs.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/ui/`glyphs.ts`/
symbols:
  UNICODE_GLYPHS: UNICODE_GLYPHS.
  ASCII_GLYPHS: ASCII_GLYPHS.
  getGlyphs: getGlyphs().
  Glyphs.dash: Glyphs#dash.
  Glyphs.rail: Glyphs#rail.
  cached: cached.
  Glyphs: Glyphs#
  Glyphs.err: Glyphs#err.
  Glyphs.info: Glyphs#info.
  Glyphs.warn: Glyphs#warn.
  Glyphs.barEmpty: Glyphs#barEmpty.
  Glyphs.ok: Glyphs#ok.
  Glyphs.spinner: Glyphs#spinner.
  Glyphs.barFilled: Glyphs#barFilled.
  Glyphs.phaseDone: Glyphs#phaseDone.
  Glyphs.treeBranch: Glyphs#treeBranch.
  Glyphs.treeLast: Glyphs#treeLast.
  Glyphs.treePipe: Glyphs#treePipe.
  _resetGlyphsCache: _resetGlyphsCache().
  Glyphs.hLine: Glyphs#hLine.
  supportsUnicode: supportsUnicode().
---
# Module: [`src/ui/glyphs.ts`](../../../../../../raw/code/codegraph/src/ui/glyphs.ts)

## Classes
### `Glyphs`
- def: [`src/ui/glyphs.ts:28`](../../../../../../raw/code/codegraph/src/ui/glyphs.ts#L28)
- signature: `interface Glyphs`
- members:
  - `barEmpty` — [`L35`](../../../../../../raw/code/codegraph/src/ui/glyphs.ts#L35)
  - `barFilled` — [`L34`](../../../../../../raw/code/codegraph/src/ui/glyphs.ts#L34)
  - `dash` — [`L38`](../../../../../../raw/code/codegraph/src/ui/glyphs.ts#L38)
  - `err` — [`L30`](../../../../../../raw/code/codegraph/src/ui/glyphs.ts#L30)
  - `hLine` — [`L39`](../../../../../../raw/code/codegraph/src/ui/glyphs.ts#L39)
  - `info` — [`L31`](../../../../../../raw/code/codegraph/src/ui/glyphs.ts#L31)
  - `ok` — [`L29`](../../../../../../raw/code/codegraph/src/ui/glyphs.ts#L29)
  - `phaseDone` — [`L37`](../../../../../../raw/code/codegraph/src/ui/glyphs.ts#L37)
  - `rail` — [`L36`](../../../../../../raw/code/codegraph/src/ui/glyphs.ts#L36)
  - `spinner` — [`L33`](../../../../../../raw/code/codegraph/src/ui/glyphs.ts#L33)
  - `treeBranch` — [`L40`](../../../../../../raw/code/codegraph/src/ui/glyphs.ts#L40)
  - `treeLast` — [`L41`](../../../../../../raw/code/codegraph/src/ui/glyphs.ts#L41)
  - `treePipe` — [`L42`](../../../../../../raw/code/codegraph/src/ui/glyphs.ts#L42)
  - `warn` — [`L32`](../../../../../../raw/code/codegraph/src/ui/glyphs.ts#L32)
- used by: [`main`](../bin/codegraph.ts.md#main), [`ASCII_GLYPHS`](glyphs.ts.md#ASCII_GLYPHS), [`UNICODE_GLYPHS`](glyphs.ts.md#UNICODE_GLYPHS), [`render`](shimmer-worker.ts.md#render), [`getGlyphs`](glyphs.ts.md#getGlyphs), [`finishPhase`](shimmer-worker.ts.md#finishPhase), [`loadCodeGraph`](../bin/codegraph.ts.md#loadCodeGraph), [`renderBar`](shimmer-worker.ts.md#renderBar), [`SPINNER_GLYPHS`](shimmer-worker.ts.md#SPINNER_GLYPHS), [`cached`](glyphs.ts.md#cached)

## Functions
- `_resetGlyphsCache()` — [`L89`](../../../../../../raw/code/codegraph/src/ui/glyphs.ts#L89) — Reset the cached glyph set. Test-only; production code should call `getGlyphs()`.
- `getGlyphs()` — [`L81`](../../../../../../raw/code/codegraph/src/ui/glyphs.ts#L81)
- `supportsUnicode()` — [`L21`](../../../../../../raw/code/codegraph/src/ui/glyphs.ts#L21) — Glyph selection for CLI output.

## Module values
- `ASCII_GLYPHS` — [`L62`](../../../../../../raw/code/codegraph/src/ui/glyphs.ts#L62)
- `UNICODE_GLYPHS` — [`L45`](../../../../../../raw/code/codegraph/src/ui/glyphs.ts#L45)
- `cached` — [`L79`](../../../../../../raw/code/codegraph/src/ui/glyphs.ts#L79)

