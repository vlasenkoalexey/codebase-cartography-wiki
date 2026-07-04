---
title: 'Module: tests/test_data/test_enum.ts'
type: catalog
provenance: extracted
module: tests/test_data/test_enum.ts
status: fresh
symbol_base: scip-typescript npm . . tests/test_data/`test_enum.ts`/
symbols:
  Person: Person#
  Person.greet: Person#greet().
  User: User#
  Color: Color#
  Color.Red: Color#Red.
  Color.Green: Color#Green.
  Color.Blue: Color#Blue.
  Status: Status#
  Status.Active: Status#Active.
  Status.Inactive: Status#Inactive.
  Status.Pending: Status#Pending.
  MathConstants: MathConstants#
  MathConstants.PI: MathConstants#PI.
  MathConstants.E: MathConstants#E.
  getPrecision: MathConstants/getPrecision().
  Person.name: Person#name.
  Person.age: Person#age.
  Point: Point#
  Point.typeLiteral0.x: Point#typeLiteral0:x.
  Point.typeLiteral0.y: Point#typeLiteral0:y.
  User.-constructor: User#`<constructor>`().
  User.greet: User#greet().
---
# Module: [`tests/test_data/test_enum.ts`](../../../../../../raw/code/tree-sitter-analyzer/tests/test_data/test_enum.ts)

## Classes
### `Color`
- def: [`tests/test_data/test_enum.ts:3`](../../../../../../raw/code/tree-sitter-analyzer/tests/test_data/test_enum.ts#L3)
- signature: `enum Color`
- members:
  - `Blue` — [`L6`](../../../../../../raw/code/tree-sitter-analyzer/tests/test_data/test_enum.ts#L6)
  - `Green` — [`L5`](../../../../../../raw/code/tree-sitter-analyzer/tests/test_data/test_enum.ts#L5)
  - `Red` — [`L4`](../../../../../../raw/code/tree-sitter-analyzer/tests/test_data/test_enum.ts#L4)

### `MathConstants`
- def: [`tests/test_data/test_enum.ts:16`](../../../../../../raw/code/tree-sitter-analyzer/tests/test_data/test_enum.ts#L16)
- signature: `enum MathConstants`
- members:
  - `E` — [`L18`](../../../../../../raw/code/tree-sitter-analyzer/tests/test_data/test_enum.ts#L18)
  - `PI` — [`L17`](../../../../../../raw/code/tree-sitter-analyzer/tests/test_data/test_enum.ts#L17)

### `Person`
- def: [`tests/test_data/test_enum.ts:28`](../../../../../../raw/code/tree-sitter-analyzer/tests/test_data/test_enum.ts#L28)
- signature: `interface Person`
- members:
  - `greet(method)` — [`L31`](../../../../../../raw/code/tree-sitter-analyzer/tests/test_data/test_enum.ts#L31)
  - `age` — [`L30`](../../../../../../raw/code/tree-sitter-analyzer/tests/test_data/test_enum.ts#L30)
  - `name` — [`L29`](../../../../../../raw/code/tree-sitter-analyzer/tests/test_data/test_enum.ts#L29)
- uses (calls/refs, reference-scoped): (2 test-only callers)
- used by: (1 test-only callers)

### `Point`
- def: [`tests/test_data/test_enum.ts:35`](../../../../../../raw/code/tree-sitter-analyzer/tests/test_data/test_enum.ts#L35)
- signature: `type Point`
- members:
  - `x` — [`L36`](../../../../../../raw/code/tree-sitter-analyzer/tests/test_data/test_enum.ts#L36)
  - `y` — [`L37`](../../../../../../raw/code/tree-sitter-analyzer/tests/test_data/test_enum.ts#L37)

### `Status`
- def: [`tests/test_data/test_enum.ts:9`](../../../../../../raw/code/tree-sitter-analyzer/tests/test_data/test_enum.ts#L9)
- signature: `enum Status`
- members:
  - `Active` — [`L10`](../../../../../../raw/code/tree-sitter-analyzer/tests/test_data/test_enum.ts#L10)
  - `Inactive` — [`L11`](../../../../../../raw/code/tree-sitter-analyzer/tests/test_data/test_enum.ts#L11)
  - `Pending` — [`L12`](../../../../../../raw/code/tree-sitter-analyzer/tests/test_data/test_enum.ts#L12)

### `User`  ·  implements/extends Person
- def: [`tests/test_data/test_enum.ts:41`](../../../../../../raw/code/tree-sitter-analyzer/tests/test_data/test_enum.ts#L41)
- signature: `class User`
- members:
  - `<constructor>(name: string, age: number)` — [`L42`](../../../../../../raw/code/tree-sitter-analyzer/tests/test_data/test_enum.ts#L42)
  - `greet(method)` — [`L44`](../../../../../../raw/code/tree-sitter-analyzer/tests/test_data/test_enum.ts#L44)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (2 test-only callers)

## Functions
- `getPrecision()` — [`L22`](../../../../../../raw/code/tree-sitter-analyzer/tests/test_data/test_enum.ts#L22)

