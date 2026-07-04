---
title: 'Module: tests/test_data/test_class.py'
type: catalog
provenance: extracted
module: tests/test_data/test_class.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.test_data.test_class`/
symbols:
  Animal.speak: Animal#speak().
  Point.distance_from_origin: Point#distance_from_origin().
  Animal: Animal#
  Dog: Dog#
  Dog.__init__: Dog#__init__().
  Dog.speak: Dog#speak().
  Dog.get_breed: Dog#get_breed().
  Animal.name: Animal#name.
  Animal.__init__: Animal#__init__().
  Dog.breed: Dog#breed.
  Point.x: Point#x.
  Point.y: Point#y.
  Animal._age: Animal#_age.
  Animal.__secret: Animal#__secret.
  Animal._protected_method: Animal#_protected_method().
  Animal.__private_method: Animal#__private_method().
  Point: Point#
---
# Module: [`tests/test_data/test_class.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/test_data/test_class.py)

## Classes
### `Animal`
- def: [`tests/test_data/test_class.py:6`](../../../../../../raw/code/tree-sitter-analyzer/tests/test_data/test_class.py#L6)
- doc: Base animal class
- signature: `class Animal:`
- members:
  - `__private_method(self)` — [`L21`](../../../../../../raw/code/tree-sitter-analyzer/tests/test_data/test_class.py#L21) — Private method (convention)
  - `_protected_method(self)` — [`L17`](../../../../../../raw/code/tree-sitter-analyzer/tests/test_data/test_class.py#L17) — Protected method (convention)
  - `speak(self)` — [`L14`](../../../../../../raw/code/tree-sitter-analyzer/tests/test_data/test_class.py#L14)
  - `name` — [`L10`](../../../../../../raw/code/tree-sitter-analyzer/tests/test_data/test_class.py#L10)
- protocol/private: `__init__`[`L9`](../../../../../../raw/code/tree-sitter-analyzer/tests/test_data/test_class.py#L9), `__secret`[`L12`](../../../../../../raw/code/tree-sitter-analyzer/tests/test_data/test_class.py#L12), `_age`[`L11`](../../../../../../raw/code/tree-sitter-analyzer/tests/test_data/test_class.py#L11)
- uses (calls/refs, reference-scoped): (2 test-only callers)
- used by: (3 test-only callers)

### `Dog`  ·  implements/extends Animal
- def: [`tests/test_data/test_class.py:26`](../../../../../../raw/code/tree-sitter-analyzer/tests/test_data/test_class.py#L26)
- doc: Dog class extending Animal
- signature: `class Dog(Animal):`
- members:
  - `get_breed(self)` — [`L36`](../../../../../../raw/code/tree-sitter-analyzer/tests/test_data/test_class.py#L36)
  - `speak(self)` — [`L33`](../../../../../../raw/code/tree-sitter-analyzer/tests/test_data/test_class.py#L33)
  - `breed` — [`L31`](../../../../../../raw/code/tree-sitter-analyzer/tests/test_data/test_class.py#L31)
- protocol/private: `__init__`[`L29`](../../../../../../raw/code/tree-sitter-analyzer/tests/test_data/test_class.py#L29)
- uses (calls/refs, reference-scoped): (3 test-only callers)
- used by: (2 test-only callers)

### `Point`
- def: [`tests/test_data/test_class.py:41`](../../../../../../raw/code/tree-sitter-analyzer/tests/test_data/test_class.py#L41)
- signature: `class Point:`
- members:
  - `distance_from_origin(self)` — [`L45`](../../../../../../raw/code/tree-sitter-analyzer/tests/test_data/test_class.py#L45)
  - `x` — [`L42`](../../../../../../raw/code/tree-sitter-analyzer/tests/test_data/test_class.py#L42)
  - `y` — [`L43`](../../../../../../raw/code/tree-sitter-analyzer/tests/test_data/test_class.py#L43)

