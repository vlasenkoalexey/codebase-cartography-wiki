---
title: 'Module: website/src/hooks/use-toast.ts'
type: catalog
provenance: extracted
module: website/src/hooks/use-toast.ts
status: fresh
symbol_base: scip-typescript npm vite_react_shadcn_ts 0.0.0 src/hooks/`use-toast.ts`/
symbols:
  dispatch: dispatch().
  reducer: reducer.
  useToast: useToast().
  toast: toast().
  State.toasts: State#toasts.
  addToRemoveQueue: addToRemoveQueue.
  listeners: listeners.
  memoryState: memoryState.
  State: State#
  ToasterToast: ToasterToast#
  Action: Action#
  ActionType: ActionType#
  genId: genId().
  Toast: Toast#
  count: count.
  toastTimeouts: toastTimeouts.
  TOAST_LIMIT: TOAST_LIMIT.
  TOAST_REMOVE_DELAY: TOAST_REMOVE_DELAY.
  actionTypes: actionTypes.
---
# Module: [`website/src/hooks/use-toast.ts`](../../../../../../../raw/code/codegraphcontext/website/src/hooks/use-toast.ts)

## Classes
### `Action`
- def: [`website/src/hooks/use-toast.ts:31`](../../../../../../../raw/code/codegraphcontext/website/src/hooks/use-toast.ts#L31)
- signature: `type Action`
- uses (calls/refs, reference-scoped): [`ToasterToast`](use-toast.ts.md#ToasterToast), [`ActionType`](use-toast.ts.md#ActionType)
- used by: [`dispatch`](use-toast.ts.md#dispatch), [`reducer`](use-toast.ts.md#reducer)

### `ActionType`
- def: [`website/src/hooks/use-toast.ts:29`](../../../../../../../raw/code/codegraphcontext/website/src/hooks/use-toast.ts#L29)
- signature: `type ActionType`
- uses (calls/refs, reference-scoped): [`actionTypes`](use-toast.ts.md#actionTypes)
- used by: [`Action`](use-toast.ts.md#Action)

### `State`
- def: [`website/src/hooks/use-toast.ts:49`](../../../../../../../raw/code/codegraphcontext/website/src/hooks/use-toast.ts#L49)
- signature: `interface State`
- members:
  - `toasts` — [`L50`](../../../../../../../raw/code/codegraphcontext/website/src/hooks/use-toast.ts#L50)
- uses (calls/refs, reference-scoped): [`ToasterToast`](use-toast.ts.md#ToasterToast)
- used by: [`reducer`](use-toast.ts.md#reducer), [`useToast`](use-toast.ts.md#useToast), [`listeners`](use-toast.ts.md#listeners), [`memoryState`](use-toast.ts.md#memoryState)

### `Toast`
- def: [`website/src/hooks/use-toast.ts:135`](../../../../../../../raw/code/codegraphcontext/website/src/hooks/use-toast.ts#L135)
- signature: `type Toast`
- uses (calls/refs, reference-scoped): [`ToasterToast`](use-toast.ts.md#ToasterToast)
- used by: [`toast`](use-toast.ts.md#toast)

### `ToasterToast`
- def: [`website/src/hooks/use-toast.ts:8`](../../../../../../../raw/code/codegraphcontext/website/src/hooks/use-toast.ts#L8)
- signature: `type ToasterToast`
- used by: [`toast`](use-toast.ts.md#toast), [`State`](use-toast.ts.md#State), [`Action`](use-toast.ts.md#Action), [`Toast`](use-toast.ts.md#Toast)

## Functions
- `dispatch(action: Action)` — [`L128`](../../../../../../../raw/code/codegraphcontext/website/src/hooks/use-toast.ts#L128)
- `genId()` — [`L24`](../../../../../../../raw/code/codegraphcontext/website/src/hooks/use-toast.ts#L24)
- `toast({ ...props }: Toast)` — [`L137`](../../../../../../../raw/code/codegraphcontext/website/src/hooks/use-toast.ts#L137)
- `useToast()` — [`L166`](../../../../../../../raw/code/codegraphcontext/website/src/hooks/use-toast.ts#L166)

## Module values
- `TOAST_LIMIT` — [`L5`](../../../../../../../raw/code/codegraphcontext/website/src/hooks/use-toast.ts#L5)
- `TOAST_REMOVE_DELAY` — [`L6`](../../../../../../../raw/code/codegraphcontext/website/src/hooks/use-toast.ts#L6)
- `actionTypes` — [`L15`](../../../../../../../raw/code/codegraphcontext/website/src/hooks/use-toast.ts#L15)
- `addToRemoveQueue` — [`L55`](../../../../../../../raw/code/codegraphcontext/website/src/hooks/use-toast.ts#L55)
- `count` — [`L22`](../../../../../../../raw/code/codegraphcontext/website/src/hooks/use-toast.ts#L22)
- `listeners` — [`L124`](../../../../../../../raw/code/codegraphcontext/website/src/hooks/use-toast.ts#L124)
- `memoryState` — [`L126`](../../../../../../../raw/code/codegraphcontext/website/src/hooks/use-toast.ts#L126)
- `reducer` — [`L71`](../../../../../../../raw/code/codegraphcontext/website/src/hooks/use-toast.ts#L71)
- `toastTimeouts` — [`L53`](../../../../../../../raw/code/codegraphcontext/website/src/hooks/use-toast.ts#L53)

