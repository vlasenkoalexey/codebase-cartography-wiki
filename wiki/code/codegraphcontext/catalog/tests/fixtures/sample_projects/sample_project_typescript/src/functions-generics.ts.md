---
title: 'Module: tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts'
type: catalog
provenance: extracted
module: tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts
status: fresh
symbol_base: scip-typescript npm sample_project_typescript 1.0.0 src/`functions-generics.ts`/
symbols:
  Queue.enqueue: Queue#enqueue().
  functionExamples: functionExamples.
  Stack.push: Stack#push().
  deepClone: deepClone().
  createUser: createUser().
  Stack.items: Stack#items.
  logLength: logLength().
  Queue.items: Queue#items.
  PriorityQueue.items: PriorityQueue#items.
  PriorityQueue.enqueue: PriorityQueue#enqueue().
  Stack.peek: Stack#peek().
  Queue.dequeue: Queue#dequeue().
  Queue.size: Queue#size().
  memoize: memoize().
  Stack: Stack#
  Queue: Queue#
  createArray: createArray().
  createInstance: createInstance().
  pipe: pipe().
  Stack.pop: Stack#pop().
  Stack.isEmpty: Stack#isEmpty().
  Stack.size: Stack#size().
  Queue.front: Queue#front().
  Queue.isEmpty: Queue#isEmpty().
  PriorityQueue: PriorityQueue#
  PriorityQueue.dequeue: PriorityQueue#dequeue().
  PriorityQueue.peek: PriorityQueue#peek().
  PriorityQueue.isEmpty: PriorityQueue#isEmpty().
  curriedFilter: curriedFilter.
  sum: sum().
  parseValue: parseValue().
  identity: identity().
  UnaryFunction: UnaryFunction#
  greet: greet().
  createUser.typeLiteral0.name: createUser().typeLiteral0:name.
  createUser.typeLiteral0.active: createUser().typeLiteral0:active.
  createMultiplier: createMultiplier.
  merge: merge().
  Lengthwise: Lengthwise#
  Lengthwise.length: Lengthwise#length.
  Constructable: Constructable#
  Predicate: Predicate#
  Comparable: Comparable#
  Comparable.compareTo: Comparable#compareTo().
  arrayChunk: arrayChunk().
  arrayUnique: arrayUnique().
  arrayGroupBy: arrayGroupBy().
  simpleFunction: simpleFunction().
  processData: processData().
  multiply: multiply.
  isEven: isEven.
  getFirstElement: getFirstElement().
  getProperty: getProperty().
  processItem: processItem().
  sortBy: sortBy().
  BinaryFunction: BinaryFunction#
  Mapper: Mapper#
  debounce: debounce().
  throttle: throttle().
  curriedAdd: curriedAdd.
  pick: pick().
  omit: omit().
  compose: compose().
---
# Module: [`tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts)

## Classes
### `BinaryFunction`
- def: [`tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts:136`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts#L136)
- signature: `type BinaryFunction`

### `Comparable`
- def: [`tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts:241`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts#L241)
- signature: `interface Comparable`
- members:
  - `compareTo(method)` — [`L242`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts#L242)
- used by: (2 test-only callers)

### `Constructable`
- def: [`tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts:110`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts#L110)
- signature: `interface Constructable`
- used by: (1 test-only callers)

### `Lengthwise`
- def: [`tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts:89`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts#L89)
- signature: `interface Lengthwise`
- members:
  - `length` — [`L90`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts#L90)
- used by: (1 test-only callers)

### `Mapper`
- def: [`tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts:138`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts#L138)
- signature: `type Mapper`

### `Predicate`
- def: [`tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts:137`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts#L137)
- signature: `type Predicate`
- used by: (1 test-only callers)

### `PriorityQueue`
- def: [`tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts:245`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts#L245)
- signature: `class PriorityQueue`
- members:
  - `dequeue(method)` — [`L253`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts#L253)
  - `enqueue(method)` — [`L248`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts#L248)
  - `isEmpty(method)` — [`L261`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts#L261)
  - `peek(method)` — [`L257`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts#L257)
  - `items` — [`L246`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts#L246)
- uses (calls/refs, reference-scoped): (2 test-only callers)

### `Queue`
- def: [`tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts:216`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts#L216)
- signature: `class Queue`
- members:
  - `dequeue(method)` — [`L223`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts#L223)
  - `enqueue(method)` — [`L219`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts#L219)
  - `front(method)` — [`L227`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts#L227)
  - `isEmpty(method)` — [`L231`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts#L231)
  - `size(method)` — [`L235`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts#L235)
  - `items` — [`L217`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts#L217)
- used by: (3 test-only callers)

### `Stack`
- def: [`tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts:192`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts#L192)
- signature: `class Stack`
- members:
  - `isEmpty(method)` — [`L207`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts#L207)
  - `peek(method)` — [`L203`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts#L203)
  - `pop(method)` — [`L199`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts#L199)
  - `push(method)` — [`L195`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts#L195)
  - `size(method)` — [`L211`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts#L211)
  - `items` — [`L193`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts#L193)
- used by: (3 test-only callers)

### `UnaryFunction`
- def: [`tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts:135`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts#L135)
- signature: `type UnaryFunction`
- used by: (1 test-only callers)

## Functions
- `arrayChunk(array: T[], size: number)` — [`L267`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts#L267)
- `arrayGroupBy(array: T[], keyFn: (item: T) => K)` — [`L279`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts#L279)
- `arrayUnique(array: T[])` — [`L275`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts#L275)
- `compose(fn1: (arg: T) => R1, fn2: (arg: R1) => R2)` — [`L338`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts#L338)
- `createArray(length: number, defaultValue: T)` — [`L78`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts#L78)
- `createInstance(constructor: Constructable<T>, ...args: any[])` — [`L114`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts#L114)
- `createUser(name: string, active?: boolean)` — [`L18`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts#L18)
- `debounce(...args: any[])` — [`L164`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts#L164)
- `deepClone(obj: T)` — [`L313`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts#L313)
- `getFirstElement(array: T[])` — [`L68`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts#L68)
- `getProperty(obj: T, key: K)` — [`L84`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts#L84)
- `greet(name: string, greeting?: string)` — [`L13`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts#L13)
- `identity(arg: T)` — [`L64`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts#L64)
- `logLength(arg: T)` — [`L93`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts#L93)
- `memoize(...args: any[])` — [`L150`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts#L150)
- `merge(obj1: T, obj2: U)` — [`L73`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts#L73)
- `omit(obj: T, ...keys: K[])` — [`L305`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts#L305)
- `parseValue(value: string)` — [`L28`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts#L28)
- `pick(obj: T, ...keys: K[])` — [`L297`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts#L297)
- `pipe(input: T, fn1: UnaryFunction<T, R1>, fn2: UnaryFunction<R1, R2>)` — [`L141`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts#L141)
- `processData(data: string[])` — [`L42`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts#L42)
- `processItem(item: T)` — [`L99`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts#L99)
- `simpleFunction(x: number, y: number)` — [`L8`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts#L8) — Functions and Generics
- `sortBy(array: T[], key: K, ascending?: boolean)` — [`L119`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts#L119)
- `sum(...numbers: number[])` — [`L23`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts#L23)
- `throttle(...args: any[])` — [`L176`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts#L176)

## Module values
- `active` — [`L18`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts#L18)
- `createMultiplier` — [`L61`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts#L61)
- `curriedAdd` — [`L292`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts#L292)
- `curriedFilter` — [`L293`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts#L293)
- `functionExamples` — [`L352`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts#L352)
- `isEven` — [`L58`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts#L58)
- `multiply` — [`L56`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts#L56)
- `name` — [`L18`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/functions-generics.ts#L18)

