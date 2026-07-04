---
title: 'Module: tests/fixtures/sample_projects/sample_project/advanced_classes.py'
type: catalog
provenance: extracted
module: tests/fixtures/sample_projects/sample_project/advanced_classes.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `tests.fixtures.sample_projects.sample_project.advanced_classes`/
symbols:
  C: C#
  A: A#
  B: B#
  AbstractThing: AbstractThing#
  AbstractThing.do: AbstractThing#do().
  ConcreteThing: ConcreteThing#
  WithMeta: WithMeta#
  WithMeta2: WithMeta2#
  WithMeta2.__str__: WithMeta2#__str__().
  WithMeta2.change_value: WithMeta2#change_value().
  Meta: Meta#
  WithMeta2.value: WithMeta2#value.
  A.foo: A#foo().
  B.foo: B#foo().
  C.bar: C#bar().
  ConcreteThing.do: ConcreteThing#do().
  Meta.__new__: Meta#__new__().
  WithMeta2.__init__: WithMeta2#__init__().
---
# Module: [`tests/fixtures/sample_projects/sample_project/advanced_classes.py`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/advanced_classes.py)

## Classes
### `A`
- def: [`tests/fixtures/sample_projects/sample_project/advanced_classes.py:3`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/advanced_classes.py#L3)
- signature: `class A:`
- members:
  - `foo(self)` — [`L4`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/advanced_classes.py#L4)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `AbstractThing`  ·  implements/extends ABC
- def: [`tests/fixtures/sample_projects/sample_project/advanced_classes.py:12`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/advanced_classes.py#L12)
- signature: `class AbstractThing(ABC):`
- members:
  - `do(self)` — [`L14`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/advanced_classes.py#L14)
- uses (calls/refs, reference-scoped): (2 test-only callers)
- used by: (1 test-only callers)

### `B`
- def: [`tests/fixtures/sample_projects/sample_project/advanced_classes.py:6`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/advanced_classes.py#L6)
- signature: `class B:`
- members:
  - `foo(self)` — [`L7`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/advanced_classes.py#L7)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `C`  ·  implements/extends A, B
- def: [`tests/fixtures/sample_projects/sample_project/advanced_classes.py:9`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/advanced_classes.py#L9)
- signature: `class C(A, B):`
- members:
  - `bar(self)` — [`L10`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/advanced_classes.py#L10)
- uses (calls/refs, reference-scoped): (2 test-only callers)
- used by: (2 test-only callers)

### `ConcreteThing`  ·  implements/extends AbstractThing
- def: [`tests/fixtures/sample_projects/sample_project/advanced_classes.py:16`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/advanced_classes.py#L16)
- signature: `class ConcreteThing(AbstractThing):`
- members:
  - `do(self)` — [`L17`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/advanced_classes.py#L17)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (2 test-only callers)

### `Meta`  ·  implements/extends type
- def: [`tests/fixtures/sample_projects/sample_project/advanced_classes.py:19`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/advanced_classes.py#L19)
- signature: `class Meta(type):`
- protocol/private: `__new__`[`L20`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/advanced_classes.py#L20)
- used by: (2 test-only callers)

### `WithMeta`
- def: [`tests/fixtures/sample_projects/sample_project/advanced_classes.py:24`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/advanced_classes.py#L24)
- signature: `class WithMeta(metaclass=Meta):`
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `WithMeta2`
- def: [`tests/fixtures/sample_projects/sample_project/advanced_classes.py:27`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/advanced_classes.py#L27)
- signature: `class WithMeta2(metaclass=Meta):`
- members:
  - `change_value(self, new_value)` — [`L34`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/advanced_classes.py#L34)
  - `value` — [`L29`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/advanced_classes.py#L29)
- protocol/private: `__init__`[`L28`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/advanced_classes.py#L28), `__str__`[`L31`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/advanced_classes.py#L31)
- uses (calls/refs, reference-scoped): (1 test-only callers)

