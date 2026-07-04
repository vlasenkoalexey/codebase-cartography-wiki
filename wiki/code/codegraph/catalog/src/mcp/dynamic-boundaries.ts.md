---
title: 'Module: src/mcp/dynamic-boundaries.ts'
type: catalog
provenance: extracted
module: src/mcp/dynamic-boundaries.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/mcp/`dynamic-boundaries.ts`/
symbols:
  scanDynamicDispatch: scanDynamicDispatch().
  FORMS: FORMS.
  scanPythonGetattr: scanPythonGetattr().
  FormSpec.form: FormSpec#form.
  FormSpec.re: FormSpec#re.
  FormSpec.label: FormSpec#label.
  FormSpec.langs: FormSpec#langs.
  BoundaryMatch: BoundaryMatch#
  BoundaryMatch.moreSites: BoundaryMatch#moreSites.
  FormSpec.keyFrom: FormSpec#keyFrom.
  BoundaryMatch.line: BoundaryMatch#line.
  FormSpec.keyWindow: FormSpec#keyWindow.
  singleStringLiteral: singleStringLiteral().
  commentLang: commentLang().
  matchBalancedParen: matchBalancedParen().
  BoundaryMatch.form: BoundaryMatch#form.
  BoundaryMatch.label: BoundaryMatch#label.
  BoundaryMatch.snippet: BoundaryMatch#snippet.
  BoundaryMatch.key: BoundaryMatch#key.
  MAX_MATCHES_PER_BODY: MAX_MATCHES_PER_BODY.
  JS_FAMILY: JS_FAMILY.
  MAX_BODY_CHARS: MAX_BODY_CHARS.
  GETATTR_RE: GETATTR_RE.
  countNewlines: countNewlines().
  snippetAround: snippetAround().
  BoundaryMatch.keyIsType: BoundaryMatch#keyIsType.
  FormSpec: FormSpec#
  PY: PY.
  RB: RB.
  PHP: PHP.
  JVM_CS_GO: JVM_CS_GO.
  SWIFT_OBJC: SWIFT_OBJC.
  blankStringContents: blankStringContents().
  MAX_GETATTR_ARGS: MAX_GETATTR_ARGS.
---
# Module: [`src/mcp/dynamic-boundaries.ts`](../../../../../../raw/code/codegraph/src/mcp/dynamic-boundaries.ts)

## Classes
### `BoundaryMatch`
- def: [`src/mcp/dynamic-boundaries.ts:26`](../../../../../../raw/code/codegraph/src/mcp/dynamic-boundaries.ts#L26)
- signature: `interface BoundaryMatch`
- members:
  - `form` — [`L28`](../../../../../../raw/code/codegraph/src/mcp/dynamic-boundaries.ts#L28) — Stable form id, e.g. 'computed-call' — used for per-form dedupe.
  - `key` — [`L41`](../../../../../../raw/code/codegraph/src/mcp/dynamic-boundaries.ts#L41) — Statically-visible dispatch key, when one exists: the string literal in
  - `keyIsType` — [`L43`](../../../../../../raw/code/codegraph/src/mcp/dynamic-boundaries.ts#L43) — For typed-bus matches the key is a TYPE name (candidates ~ `${key}Handler`).
  - `label` — [`L30`](../../../../../../raw/code/codegraph/src/mcp/dynamic-boundaries.ts#L30) — Human label for the dispatch form, e.g. 'computed member call'.
  - `line` — [`L34`](../../../../../../raw/code/codegraph/src/mcp/dynamic-boundaries.ts#L34) — 1-based line within the scanned body's FILE (absolute, ready to print).
  - `moreSites` — [`L45`](../../../../../../raw/code/codegraph/src/mcp/dynamic-boundaries.ts#L45) — Additional sites of the same form+key in this body beyond the reported one.
  - `snippet` — [`L32`](../../../../../../raw/code/codegraph/src/mcp/dynamic-boundaries.ts#L32) — One-line source snippet of the site (from the original, untrimmed text).
- used by: [`scanDynamicDispatch`](dynamic-boundaries.ts.md#scanDynamicDispatch), [`buildDynamicBoundaries`](tools.ts.md#ToolHandler.buildDynamicBoundaries), [`scanPythonGetattr`](dynamic-boundaries.ts.md#scanPythonGetattr)

### `FormSpec`
- def: [`src/mcp/dynamic-boundaries.ts:48`](../../../../../../raw/code/codegraph/src/mcp/dynamic-boundaries.ts#L48)
- signature: `interface FormSpec`
- members:
  - `form` — [`L49`](../../../../../../raw/code/codegraph/src/mcp/dynamic-boundaries.ts#L49)
  - `keyFrom` — [`L58`](../../../../../../raw/code/codegraph/src/mcp/dynamic-boundaries.ts#L58) — Derive the dispatch key from the ORIGINAL-source snippet around the match
  - `keyWindow` — [`L65`](../../../../../../raw/code/codegraph/src/mcp/dynamic-boundaries.ts#L65) — Extra ORIGINAL chars after the match end handed to keyFrom, capped at the
  - `label` — [`L50`](../../../../../../raw/code/codegraph/src/mcp/dynamic-boundaries.ts#L50)
  - `langs` — [`L52`](../../../../../../raw/code/codegraph/src/mcp/dynamic-boundaries.ts#L52) — Languages this form applies to; undefined = all. Node.language values.
  - `re` — [`L53`](../../../../../../raw/code/codegraph/src/mcp/dynamic-boundaries.ts#L53)
- used by: [`scanDynamicDispatch`](dynamic-boundaries.ts.md#scanDynamicDispatch), [`FORMS`](dynamic-boundaries.ts.md#FORMS)

## Functions
- `blankStringContents(text: string)` — [`L233`](../../../../../../raw/code/codegraph/src/mcp/dynamic-boundaries.ts#L233) — Blank the CONTENTS of string literals (quotes preserved, offsets preserved)
- `commentLang(language: string)` — [`L189`](../../../../../../raw/code/codegraph/src/mcp/dynamic-boundaries.ts#L189) — Map a Node.language to the comment-stripper's language set.
- `countNewlines(text: string, end: number)` — [`L384`](../../../../../../raw/code/codegraph/src/mcp/dynamic-boundaries.ts#L384)
- `matchBalancedParen(text: string, open: number)` — [`L373`](../../../../../../raw/code/codegraph/src/mcp/dynamic-boundaries.ts#L373) — Index of the `)` balancing `text[open]`, or -1 (cap: MAX_GETATTR_ARGS chars).
- `scanDynamicDispatch(body: string, language: string, fileStartLine: number)` — [`L269`](../../../../../../raw/code/codegraph/src/mcp/dynamic-boundaries.ts#L269) — Scan one symbol's body for dynamic-dispatch sites. — documented in [mcp-tools.ts](../../../concepts/mcp-tools.ts.md)
- `scanPythonGetattr(stripped: string, original: string, fileStartLine: number, out: BoundaryMatch[], seen: Map<string, BoundaryMatch>)` — [`L326`](../../../../../../raw/code/codegraph/src/mcp/dynamic-boundaries.ts#L326)
- `singleStringLiteral(text: string)` — [`L76`](../../../../../../raw/code/codegraph/src/mcp/dynamic-boundaries.ts#L76) — Exactly one quoted literal and no concatenation → that literal is the key.
- `snippetAround(text: string, index: number)` — [`L391`](../../../../../../raw/code/codegraph/src/mcp/dynamic-boundaries.ts#L391) — The full source line containing `index`, trimmed and capped for display.

## Module values
- `FORMS` — [`L81`](../../../../../../raw/code/codegraph/src/mcp/dynamic-boundaries.ts#L81)
- `GETATTR_RE` — [`L323`](../../../../../../raw/code/codegraph/src/mcp/dynamic-boundaries.ts#L323) — Python getattr dispatch — handled in code, not the FORMS table, because real
- `JS_FAMILY` — [`L68`](../../../../../../raw/code/codegraph/src/mcp/dynamic-boundaries.ts#L68)
- `JVM_CS_GO` — [`L72`](../../../../../../raw/code/codegraph/src/mcp/dynamic-boundaries.ts#L72)
- `MAX_BODY_CHARS` — [`L222`](../../../../../../raw/code/codegraph/src/mcp/dynamic-boundaries.ts#L222)
- `MAX_GETATTR_ARGS` — [`L324`](../../../../../../raw/code/codegraph/src/mcp/dynamic-boundaries.ts#L324)
- `MAX_MATCHES_PER_BODY` — [`L221`](../../../../../../raw/code/codegraph/src/mcp/dynamic-boundaries.ts#L221)
- `PHP` — [`L71`](../../../../../../raw/code/codegraph/src/mcp/dynamic-boundaries.ts#L71)
- `PY` — [`L69`](../../../../../../raw/code/codegraph/src/mcp/dynamic-boundaries.ts#L69)
- `RB` — [`L70`](../../../../../../raw/code/codegraph/src/mcp/dynamic-boundaries.ts#L70)
- `SWIFT_OBJC` — [`L73`](../../../../../../raw/code/codegraph/src/mcp/dynamic-boundaries.ts#L73)

