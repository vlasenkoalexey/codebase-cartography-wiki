---
title: 'Module: tests/fixtures/sample_projects/sample_project/class_instantiation.py'
type: catalog
provenance: extracted
module: tests/fixtures/sample_projects/sample_project/class_instantiation.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `tests.fixtures.sample_projects.sample_project.class_instantiation`/
symbols:
  f: f.
  obj2: obj2.
  msg1: msg1.
  msg2: msg2.
  A: A#
  A.greet: A#greet().
  B: B#
  B.greet: B#greet().
  obj: obj.
  val: val.
  Fluent: Fluent#
  Fluent.step1: Fluent#step1().
  Fluent.step2: Fluent#step2().
  Fluent.step3: Fluent#step3().
---
# Module: [`tests/fixtures/sample_projects/sample_project/class_instantiation.py`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/class_instantiation.py)

## Classes
### `A`
- def: [`tests/fixtures/sample_projects/sample_project/class_instantiation.py:1`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/class_instantiation.py#L1)
- signature: `class A:`
- members:
  - `greet(self)` — [`L2`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/class_instantiation.py#L2)
- uses (calls/refs, reference-scoped): (2 test-only callers)
- used by: (4 test-only callers)

### `B`  ·  implements/extends A
- def: [`tests/fixtures/sample_projects/sample_project/class_instantiation.py:4`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/class_instantiation.py#L4)
- signature: `class B(A):`
- members:
  - `greet(self)` — [`L5`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/class_instantiation.py#L5)
- uses (calls/refs, reference-scoped): (2 test-only callers)
- used by: (4 test-only callers)

### `Fluent`
- def: [`tests/fixtures/sample_projects/sample_project/class_instantiation.py:12`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/class_instantiation.py#L12)
- signature: `class Fluent:`
- members:
  - `step1(self)` — [`L13`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/class_instantiation.py#L13)
  - `step2(self)` — [`L14`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/class_instantiation.py#L14)
  - `step3(self)` — [`L15`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/class_instantiation.py#L15)
- used by: (1 test-only callers)

## Module values
- `f` — [`L17`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/class_instantiation.py#L17)
- `msg1` — [`L8`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/class_instantiation.py#L8)
- `msg2` — [`L10`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/class_instantiation.py#L10)
- `obj` — [`L7`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/class_instantiation.py#L7)
- `obj2` — [`L9`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/class_instantiation.py#L9)
- `val` — [`L20`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/class_instantiation.py#L20)

