---
title: 'Module: tests/fixtures/sample_projects/sample_project_typescript/src/tough_cases.ts'
type: catalog
provenance: extracted
module: tests/fixtures/sample_projects/sample_project_typescript/src/tough_cases.ts
status: fresh
symbol_base: scip-typescript npm sample_project_typescript 1.0.0 src/`tough_cases.ts`/
symbols:
  ClassA.-constructor: ClassA#`<constructor>`().
  ClassA.execute: ClassA#execute().
  PrivacyTest.getPrivate: PrivacyTest#getPrivate().
  ClassA: ClassA#
  ClassA.ping: ClassA#ping().
  PrivacyTest.-realPrivate: PrivacyTest#`#realPrivate`.
  loadModuleDynamically: loadModuleDynamically().
  createNestedState: createNestedState().
  DataMap: DataMap#
  ReadonlyData: ReadonlyData#
  OverloadedMethod: OverloadedMethod#
  OverloadedMethod.process: OverloadedMethod#process().
  PrivacyTest: PrivacyTest#
  PrivacyTest.tsPrivate: PrivacyTest#tsPrivate.
---
# Module: [`tests/fixtures/sample_projects/sample_project_typescript/src/tough_cases.ts`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/tough_cases.ts)

## Classes
### `ClassA`
- def: [`tests/fixtures/sample_projects/sample_project_typescript/src/tough_cases.ts:7`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/tough_cases.ts#L7)
- signature: `class ClassA`
- members:
  - `<constructor>(b: ClassB)` — [`L8`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/tough_cases.ts#L8)
  - `execute(method)` — [`L10`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/tough_cases.ts#L10)
  - `ping(method)` — [`L15`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/tough_cases.ts#L15)
- uses (calls/refs, reference-scoped): (2 test-only callers)
- used by: (3 test-only callers)

### `DataMap`
- def: [`tests/fixtures/sample_projects/sample_project_typescript/src/tough_cases.ts:55`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/tough_cases.ts#L55)
- doc: Tough Case 5: Complex Mapped Types and Overloads
- signature: `interface DataMap`

### `OverloadedMethod`
- def: [`tests/fixtures/sample_projects/sample_project_typescript/src/tough_cases.ts:63`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/tough_cases.ts#L63)
- signature: `class OverloadedMethod`
- members:
  - `process(method)` — [`L64`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/tough_cases.ts#L64)

### `PrivacyTest`
- def: [`tests/fixtures/sample_projects/sample_project_typescript/src/tough_cases.ts:74`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/tough_cases.ts#L74)
- doc: Tough Case 6: Private Fields and Mixed Scopes
- signature: `class PrivacyTest`
- members:
  - `getPrivate(method)` — [`L78`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/tough_cases.ts#L78)
  - `#realPrivate` — [`L75`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/tough_cases.ts#L75)
  - `tsPrivate` — [`L76`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/tough_cases.ts#L76)

### `ReadonlyData`
- def: [`tests/fixtures/sample_projects/sample_project_typescript/src/tough_cases.ts:59`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/tough_cases.ts#L59)
- signature: `type ReadonlyData`

## Functions
- `createNestedState(initial: number)` — [`L38`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/tough_cases.ts#L38) — Tough Case 4: Shadowing and Closures
- `loadModuleDynamically(moduleName: string)` — [`L29`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/tough_cases.ts#L29) — Tough Case 3: Dynamic Imports with Variables

