---
title: 'Module: tests/fixtures/sample_projects/sample_project/complex_classes.py'
type: catalog
provenance: extracted
module: tests/fixtures/sample_projects/sample_project/complex_classes.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `tests.fixtures.sample_projects.sample_project.complex_classes`/
symbols:
  Base: Base#
  Base.greet: Base#greet().
  Child.greet: Child#greet().
  decorator: decorator().
  Child: Child#
  Child.class_method: Child#class_method().
  decorated_function: decorated_function().
  decorator.wrapper: decorator().wrapper().
  Child.static_method: Child#static_method().
---
# Module: [`tests/fixtures/sample_projects/sample_project/complex_classes.py`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/complex_classes.py)

## Classes
### `Base`
- def: [`tests/fixtures/sample_projects/sample_project/complex_classes.py:1`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/complex_classes.py#L1)
- signature: `class Base:`
- members:
  - `greet(self)` — [`L2`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/complex_classes.py#L2)
- uses (calls/refs, reference-scoped): (2 test-only callers)
- used by: (2 test-only callers)

### `Child`  ·  implements/extends Base
- def: [`tests/fixtures/sample_projects/sample_project/complex_classes.py:5`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/complex_classes.py#L5)
- signature: `class Child(Base):`
- members:
  - `class_method(cls, y)` — [`L14`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/complex_classes.py#L14)
  - `greet(self)` — [`L6`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/complex_classes.py#L6)
  - `static_method(x)` — [`L10`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/complex_classes.py#L10)
- uses (calls/refs, reference-scoped): (2 test-only callers)
- used by: (2 test-only callers)

## Functions
- `decorated_function(x)` — [`L23`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/complex_classes.py#L23)
- `decorator(func)` — [`L17`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/complex_classes.py#L17)
- `wrapper(*args, **kwargs)` — [`L18`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/complex_classes.py#L18)

