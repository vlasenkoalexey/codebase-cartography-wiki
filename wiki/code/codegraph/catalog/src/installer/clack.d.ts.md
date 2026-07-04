---
title: 'Module: src/installer/clack.d.ts'
type: catalog
provenance: extracted
module: src/installer/clack.d.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/installer/`clack.d.ts`/`'@clack/prompts'`/
symbols:
  log: log.
  log.typeLiteral32.info: log.typeLiteral32:info().
  outro: outro().
  isCancel: isCancel().
  log.typeLiteral32.success: log.typeLiteral32:success().
  intro: intro().
  cancel: cancel().
  log.typeLiteral32.warn: log.typeLiteral32:warn().
  confirm: confirm().
  confirm.opts-typeLiteral27.message: confirm().(opts)typeLiteral27:message.
  confirm.opts-typeLiteral27.initialValue: confirm().(opts)typeLiteral27:initialValue.
  select: select().
  log.typeLiteral32.error: log.typeLiteral32:error().
  select.opts-typeLiteral45.message: select().(opts)typeLiteral45:message.
  select.opts-typeLiteral45.options: select().(opts)typeLiteral45:options.
  select.opts-typeLiteral45.initialValue: select().(opts)typeLiteral45:initialValue.
  spinner.typeLiteral31.stop: spinner().typeLiteral31:stop().
  note: note().
  multiselect: multiselect().
  multiselect.opts-typeLiteral190.message: multiselect().(opts)typeLiteral190:message.
  multiselect.opts-typeLiteral190.options: multiselect().(opts)typeLiteral190:options.
  multiselect.opts-typeLiteral190.initialValues: multiselect().(opts)typeLiteral190:initialValues.
  multiselect.opts-typeLiteral190.required: multiselect().(opts)typeLiteral190:required.
  spinner: spinner().
  spinner.typeLiteral31.start: spinner().typeLiteral31:start().
  confirm.opts-typeLiteral27.active: confirm().(opts)typeLiteral27:active.
  confirm.opts-typeLiteral27.inactive: confirm().(opts)typeLiteral27:inactive.
  spinner.typeLiteral31.message: spinner().typeLiteral31:message().
  log.typeLiteral32.message: log.typeLiteral32:message().
  log.typeLiteral32.step: log.typeLiteral32:step().
---
# Module: [`src/installer/clack.d.ts`](../../../../../../raw/code/codegraph/src/installer/clack.d.ts)

## Functions
- `cancel(message?: string | undefined)` — [`L11`](../../../../../../raw/code/codegraph/src/installer/clack.d.ts#L11)
- `confirm(opts: { message: string; active?: string | undefined; inactive?: string | undefined; initialValue?: boolean | undefined; })` — [`L14`](../../../../../../raw/code/codegraph/src/installer/clack.d.ts#L14)
- `error(method)` — [`L48`](../../../../../../raw/code/codegraph/src/installer/clack.d.ts#L48)
- `info(method)` — [`L44`](../../../../../../raw/code/codegraph/src/installer/clack.d.ts#L44)
- `intro(title?: string | undefined)` — [`L9`](../../../../../../raw/code/codegraph/src/installer/clack.d.ts#L9)
- `isCancel(value: unknown)` — [`L12`](../../../../../../raw/code/codegraph/src/installer/clack.d.ts#L12)
- `message(method)` — [`L37`](../../../../../../raw/code/codegraph/src/installer/clack.d.ts#L37)
- `message(method)` — [`L43`](../../../../../../raw/code/codegraph/src/installer/clack.d.ts#L43)
- `multiselect(opts: { message: string; options: { value: Value; label: string; hint?: string | undefined; }[]; initialValues?: Value[] | undefined; required?: boolean | undefined; })` — [`L27`](../../../../../../raw/code/codegraph/src/installer/clack.d.ts#L27)
- `note(message: string, title?: string | undefined)` — [`L40`](../../../../../../raw/code/codegraph/src/installer/clack.d.ts#L40)
- `outro(message?: string | undefined)` — [`L10`](../../../../../../raw/code/codegraph/src/installer/clack.d.ts#L10)
- `select(opts: { message: string; options: { value: Value; label: string; hint?: string | undefined; }[]; initialValue?: Value | undefined; })` — [`L21`](../../../../../../raw/code/codegraph/src/installer/clack.d.ts#L21)
- `spinner()` — [`L34`](../../../../../../raw/code/codegraph/src/installer/clack.d.ts#L34)
- `start(method)` — [`L35`](../../../../../../raw/code/codegraph/src/installer/clack.d.ts#L35)
- `step(method)` — [`L46`](../../../../../../raw/code/codegraph/src/installer/clack.d.ts#L46)
- `stop(method)` — [`L36`](../../../../../../raw/code/codegraph/src/installer/clack.d.ts#L36)
- `success(method)` — [`L45`](../../../../../../raw/code/codegraph/src/installer/clack.d.ts#L45)
- `warn(method)` — [`L47`](../../../../../../raw/code/codegraph/src/installer/clack.d.ts#L47)

## Module values
- `active` — [`L16`](../../../../../../raw/code/codegraph/src/installer/clack.d.ts#L16)
- `inactive` — [`L17`](../../../../../../raw/code/codegraph/src/installer/clack.d.ts#L17)
- `initialValue` — [`L18`](../../../../../../raw/code/codegraph/src/installer/clack.d.ts#L18)
- `initialValue` — [`L24`](../../../../../../raw/code/codegraph/src/installer/clack.d.ts#L24)
- `initialValues` — [`L30`](../../../../../../raw/code/codegraph/src/installer/clack.d.ts#L30)
- `log` — [`L42`](../../../../../../raw/code/codegraph/src/installer/clack.d.ts#L42)
- `message` — [`L15`](../../../../../../raw/code/codegraph/src/installer/clack.d.ts#L15)
- `message` — [`L22`](../../../../../../raw/code/codegraph/src/installer/clack.d.ts#L22)
- `message` — [`L28`](../../../../../../raw/code/codegraph/src/installer/clack.d.ts#L28)
- `options` — [`L23`](../../../../../../raw/code/codegraph/src/installer/clack.d.ts#L23)
- `options` — [`L29`](../../../../../../raw/code/codegraph/src/installer/clack.d.ts#L29)
- `required` — [`L31`](../../../../../../raw/code/codegraph/src/installer/clack.d.ts#L31)

