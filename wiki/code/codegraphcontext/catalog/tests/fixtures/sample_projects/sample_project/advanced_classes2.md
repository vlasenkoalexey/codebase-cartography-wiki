---
title: 'Module: tests/fixtures/sample_projects/sample_project/advanced_classes2.py'
type: catalog
provenance: extracted
module: tests/fixtures/sample_projects/sample_project/advanced_classes2.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `tests.fixtures.sample_projects.sample_project.advanced_classes2`/
symbols:
  Combined: Combined#
  Color.is_primary: Color#is_primary().
  flag: flag.
  Base: Base#
  Point.magnitude: Point#magnitude().
  Mid: Mid#
  Combined.both: Combined#both().
  handle: handle().
  res: res.
  dist: dist.
  msg: msg.
  p: p.
  Mixin1: Mixin1#
  Mixin2: Mixin2#
  c: c.
  Color: Color#
  Final: Final#
  Point: Point#
  Color.RED: Color#RED.
  Mixin1.m1: Mixin1#m1().
  Mixin2.m2: Mixin2#m2().
  Point.x: Point#x.
  Point.y: Point#y.
  Color.BLUE: Color#BLUE.
---
# Module: [`tests/fixtures/sample_projects/sample_project/advanced_classes2.py`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/advanced_classes2.py)

## Classes
### `Base`
- def: [`tests/fixtures/sample_projects/sample_project/advanced_classes2.py:4`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/advanced_classes2.py#L4)
- signature: `class Base:`
- uses (calls/refs, reference-scoped): (2 test-only callers)
- used by: (2 test-only callers)

### `Color`  ·  implements/extends Enum
- def: [`tests/fixtures/sample_projects/sample_project/advanced_classes2.py:28`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/advanced_classes2.py#L28)
- signature: `class Color(Enum):`
- members:
  - `is_primary(self)` — [`L31`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/advanced_classes2.py#L31)
  - `BLUE` — [`L30`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/advanced_classes2.py#L30)
  - `RED` — [`L29`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/advanced_classes2.py#L29)
- used by: (1 test-only callers)

### `Combined`  ·  implements/extends Base, Mixin1, Mixin2
- def: [`tests/fixtures/sample_projects/sample_project/advanced_classes2.py:13`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/advanced_classes2.py#L13)
- signature: `class Combined(Mixin1, Mixin2, Base):`
- members:
  - `both(self)` — [`L14`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/advanced_classes2.py#L14)
- uses (calls/refs, reference-scoped): (5 test-only callers)
- used by: (5 test-only callers)

### `Final`  ·  implements/extends Mid
- def: [`tests/fixtures/sample_projects/sample_project/advanced_classes2.py:6`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/advanced_classes2.py#L6)
- signature: `class Final(Mid):`
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `Mid`  ·  implements/extends Base
- def: [`tests/fixtures/sample_projects/sample_project/advanced_classes2.py:5`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/advanced_classes2.py#L5)
- signature: `class Mid(Base):`
- uses (calls/refs, reference-scoped): (2 test-only callers)
- used by: (2 test-only callers)

### `Mixin1`
- def: [`tests/fixtures/sample_projects/sample_project/advanced_classes2.py:8`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/advanced_classes2.py#L8)
- signature: `class Mixin1:`
- members:
  - `m1(self)` — [`L9`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/advanced_classes2.py#L9)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (2 test-only callers)

### `Mixin2`
- def: [`tests/fixtures/sample_projects/sample_project/advanced_classes2.py:10`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/advanced_classes2.py#L10)
- signature: `class Mixin2:`
- members:
  - `m2(self)` — [`L11`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/advanced_classes2.py#L11)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (2 test-only callers)

### `Point`
- def: [`tests/fixtures/sample_projects/sample_project/advanced_classes2.py:20`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/advanced_classes2.py#L20)
- signature: `class Point:`
- members:
  - `magnitude(self)` — [`L23`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/advanced_classes2.py#L23)
  - `x` — [`L21`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/advanced_classes2.py#L21)
  - `y` — [`L22`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/advanced_classes2.py#L22)
- used by: (3 test-only callers)

## Functions
- `handle(val)` — [`L35`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/advanced_classes2.py#L35)

## Module values
- `c` — [`L16`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/advanced_classes2.py#L16)
- `dist` — [`L26`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/advanced_classes2.py#L26)
- `flag` — [`L33`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/advanced_classes2.py#L33)
- `msg` — [`L41`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/advanced_classes2.py#L41)
- `p` — [`L25`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/advanced_classes2.py#L25)
- `res` — [`L17`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/advanced_classes2.py#L17)

