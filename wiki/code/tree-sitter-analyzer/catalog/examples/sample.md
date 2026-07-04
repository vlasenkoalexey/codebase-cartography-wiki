---
title: 'Module: examples/sample.py'
type: catalog
provenance: extracted
module: examples/sample.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `examples.sample`/
symbols:
  main: main().
  process_animals: process_animals().
  Animal: Animal#
  Person.greet: Person#greet().
  Animal.make_sound: Animal#make_sound().
  Animal.describe: Animal#describe().
  Dog: Dog#
  Cat: Cat#
  decorator_example: decorator_example().
  decorated_function: decorated_function().
  Person.__post_init__: Person#__post_init__().
  Dog.__init__: Dog#__init__().
  Dog.fetch: Dog#fetch().
  Cat.__init__: Cat#__init__().
  Person.age: Person#age.
  Animal.__init__: Animal#__init__().
  Animal.name: Animal#name.
  Animal.species: Animal#species.
  Person: Person#
  Person.name: Person#name.
  calculate_statistics: calculate_statistics().
  fibonacci_generator: fibonacci_generator().
  list_comprehension_examples: list_comprehension_examples().
  exception_handling_example: exception_handling_example().
  context_manager_example: context_manager_example().
  lambda_and_higher_order_functions: lambda_and_higher_order_functions().
  decorator_example.wrapper: decorator_example().wrapper().
  Person.email: Person#email.
  Dog.breed: Dog#breed.
  Dog.make_sound: Dog#make_sound().
  Cat.indoor: Cat#indoor.
  Cat.make_sound: Cat#make_sound().
  Cat.purr: Cat#purr().
  fetch_data: fetch_data().
---
# Module: [`examples/sample.py`](../../../../../raw/code/tree-sitter-analyzer/examples/sample.py)

## Classes
### `Animal`  ·  implements/extends ABC
- def: [`examples/sample.py:31`](../../../../../raw/code/tree-sitter-analyzer/examples/sample.py#L31)
- doc: Abstract base class for animals.
- signature: `class Animal(ABC):`
- members:
  - `describe(self)` — [`L43`](../../../../../raw/code/tree-sitter-analyzer/examples/sample.py#L43) — Describe the animal.
  - `make_sound(self)` — [`L39`](../../../../../raw/code/tree-sitter-analyzer/examples/sample.py#L39) — Make the sound characteristic of this animal.
  - `name` — [`L35`](../../../../../raw/code/tree-sitter-analyzer/examples/sample.py#L35)
  - `species` — [`L36`](../../../../../raw/code/tree-sitter-analyzer/examples/sample.py#L36)
- protocol/private: `__init__`[`L34`](../../../../../raw/code/tree-sitter-analyzer/examples/sample.py#L34)
- uses (calls/refs, reference-scoped): (4 test-only callers)
- used by: (6 test-only callers)

### `Cat`  ·  implements/extends Animal
- def: [`examples/sample.py:64`](../../../../../raw/code/tree-sitter-analyzer/examples/sample.py#L64)
- doc: A cat implementation of Animal.
- signature: `class Cat(Animal):`
- members:
  - `make_sound(self)` — [`L71`](../../../../../raw/code/tree-sitter-analyzer/examples/sample.py#L71) — Cats meow.
  - `purr()` — [`L76`](../../../../../raw/code/tree-sitter-analyzer/examples/sample.py#L76) — Cats can purr.
  - `indoor` — [`L69`](../../../../../raw/code/tree-sitter-analyzer/examples/sample.py#L69)
- protocol/private: `__init__`[`L67`](../../../../../raw/code/tree-sitter-analyzer/examples/sample.py#L67)
- uses (calls/refs, reference-scoped): (2 test-only callers)
- used by: (3 test-only callers)

### `Dog`  ·  implements/extends Animal
- def: [`examples/sample.py:48`](../../../../../raw/code/tree-sitter-analyzer/examples/sample.py#L48)
- doc: A dog implementation of Animal.
- signature: `class Dog(Animal):`
- members:
  - `fetch(self, item: str)` — [`L59`](../../../../../raw/code/tree-sitter-analyzer/examples/sample.py#L59) — Dogs can fetch items.
  - `make_sound(self)` — [`L55`](../../../../../raw/code/tree-sitter-analyzer/examples/sample.py#L55) — Dogs bark.
  - `breed` — [`L53`](../../../../../raw/code/tree-sitter-analyzer/examples/sample.py#L53)
- protocol/private: `__init__`[`L51`](../../../../../raw/code/tree-sitter-analyzer/examples/sample.py#L51)
- uses (calls/refs, reference-scoped): (3 test-only callers)
- used by: (3 test-only callers)

### `Person`
- def: [`examples/sample.py:14`](../../../../../raw/code/tree-sitter-analyzer/examples/sample.py#L14)
- doc: A simple person data class.
- signature: `class Person:`
- members:
  - `__post_init__(self)` — [`L21`](../../../../../raw/code/tree-sitter-analyzer/examples/sample.py#L21) — Validate the person data after initialization.
  - `greet(self)` — [`L26`](../../../../../raw/code/tree-sitter-analyzer/examples/sample.py#L26) — Return a greeting message.
  - `age` — [`L18`](../../../../../raw/code/tree-sitter-analyzer/examples/sample.py#L18)
  - `email` — [`L19`](../../../../../raw/code/tree-sitter-analyzer/examples/sample.py#L19)
  - `name` — [`L17`](../../../../../raw/code/tree-sitter-analyzer/examples/sample.py#L17)
- used by: (1 test-only callers)

## Functions
- `calculate_statistics(numbers: list[int | float])` — [`L106`](../../../../../raw/code/tree-sitter-analyzer/examples/sample.py#L106) — Calculate basic statistics for a list of numbers.
- `context_manager_example()` — [`L163`](../../../../../raw/code/tree-sitter-analyzer/examples/sample.py#L163) — Demonstrate context managers.
- `decorated_function(message: str)` — [`L202`](../../../../../raw/code/tree-sitter-analyzer/examples/sample.py#L202) — A function that uses the decorator.
- `decorator_example(func)` — [`L189`](../../../../../raw/code/tree-sitter-analyzer/examples/sample.py#L189) — A simple decorator example.
- `exception_handling_example()` — [`L145`](../../../../../raw/code/tree-sitter-analyzer/examples/sample.py#L145) — Demonstrate exception handling.
- `fetch_data(url: str)` — [`L81`](../../../../../raw/code/tree-sitter-analyzer/examples/sample.py#L81) — Asynchronously fetch data from a URL.
- `fibonacci_generator(n: int)` — [`L120`](../../../../../raw/code/tree-sitter-analyzer/examples/sample.py#L120) — Generate Fibonacci numbers up to n.
- `lambda_and_higher_order_functions()` — [`L171`](../../../../../raw/code/tree-sitter-analyzer/examples/sample.py#L171) — Demonstrate lambda functions and higher-order functions.
- `list_comprehension_examples()` — [`L128`](../../../../../raw/code/tree-sitter-analyzer/examples/sample.py#L128) — Demonstrate various list comprehensions.
- `main()` — [`L207`](../../../../../raw/code/tree-sitter-analyzer/examples/sample.py#L207) — Main function to demonstrate all features.
- `process_animals(animals: list[Animal])` — [`L90`](../../../../../raw/code/tree-sitter-analyzer/examples/sample.py#L90) — Process a list of animals and categorize their sounds.
- `wrapper(*args, **kwargs)` — [`L192`](../../../../../raw/code/tree-sitter-analyzer/examples/sample.py#L192)

