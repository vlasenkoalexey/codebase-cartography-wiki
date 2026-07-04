---
title: 'Module: tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts'
type: catalog
provenance: extracted
module: tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts
status: fresh
symbol_base: scip-typescript npm sample_project_typescript 1.0.0 src/`classes-inheritance.ts`/
symbols:
  Animal.name: Animal#name.
  Person.-constructor: Person#`<constructor>`().
  Animal: Animal#
  Person.introduce: Person#introduce().
  Person: Person#
  EnhancedUser: EnhancedUser.
  Animal.makeSound: Animal#makeSound().
  Animal.move: Animal#move().
  Duck: Duck#
  Container.add: Container#add().
  Employee.-constructor: Employee#`<constructor>`().
  Person.getSpecies: Person#getSpecies().
  Person.updateAge: Person#updateAge().
  Employee.introduce: Employee#introduce().
  Employee.work: Employee#work().
  Dog.makeSound: Dog#makeSound().
  Container.items: Container#items.
  Database: Database#
  Database.getInstance: Database#getInstance().
  TimestampedUser: TimestampedUser.
  Employee: Employee#
  Database.instance: Database#instance.
  Person.name: Person#name.
  Person.age: Person#age.
  Employee.celebrateBirthday: Employee#celebrateBirthday().
  Animal.-constructor: Animal#`<constructor>`().
  Cat.move: Cat#move().
  NumberContainer.average: NumberContainer#average().
  Database.connections: Database#connections.
  MathUtils.calculateCircleArea: MathUtils#calculateCircleArea().
  ActivatableUser: ActivatableUser.
  classExamples: classExamples.
  Dog.-constructor: Dog#`<constructor>`().
  Container: Container#
  Container.getAll: Container#getAll().
  Timestamped: Timestamped().
  Activatable: Activatable().
  Animal.sleep: Animal#sleep().
  Dog: Dog#
  Dog.move: Dog#move().
  Cat.-constructor: Cat#`<constructor>`().
  Flyable: Flyable#
  Swimmable: Swimmable#
  NumberContainer: NumberContainer#
  NumberContainer.sum: NumberContainer#sum().
  Person._id: Person#_id.
  Employee.salary: Employee#salary.
  Employee.department: Employee#department.
  BaseUser: BaseUser#
  Person.-get-id: Person#`<get>id`().
  Person.-set-id: Person#`<set>id`().
  Person.greet: Person#greet().
  Employee.-get-monthlySalary: Employee#`<get>monthlySalary`().
  Employee.-set-monthlySalary: Employee#`<set>monthlySalary`().
  Dog.fetch: Dog#fetch().
  Cat: Cat#
  Cat.makeSound: Cat#makeSound().
  Cat.climb: Cat#climb().
  Flyable.fly: Flyable#fly().
  Flyable.land: Flyable#land().
  Swimmable.swim: Swimmable#swim().
  Swimmable.surface: Swimmable#surface().
  Duck.makeSound: Duck#makeSound().
  Duck.move: Duck#move().
  Duck.fly: Duck#fly().
  Duck.land: Duck#land().
  Duck.swim: Duck#swim().
  Duck.surface: Duck#surface().
  Container.remove: Container#remove().
  Container.size: Container#size().
  Container.clear: Container#clear().
  Database.connect: Database#connect().
  Database.disconnect: Database#disconnect().
  Dog.breed: Dog#breed.
  Cat.indoor: Cat#indoor.
  Constructor: Constructor#
  Person.birthDate: Person#birthDate.
  Person.species: Person#species.
  Person.validateAge: Person#validateAge().
  Animal.age: Animal#age.
  Duck.-constructor: Duck#`<constructor>`().
  MathUtils: MathUtils#
  MathUtils.PI: MathUtils#PI.
  MathUtils.calculateDistance: MathUtils#calculateDistance().
  MathUtils.clamp: MathUtils#clamp().
  BaseUser.-constructor: BaseUser#`<constructor>`().
---
# Module: [`tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts)

## Classes
### `Animal`
- def: [`tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts:119`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L119)
- signature: `class Animal`
- members:
  - `<constructor>(name: string, age: number)` — [`L123`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L123)
  - `makeSound(method)` — [`L134`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L134)
  - `move(method)` — [`L137`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L137)
  - `sleep(method)` — [`L129`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L129)
  - `age` — [`L121`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L121)
  - `name` — [`L120`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L120)
- uses (calls/refs, reference-scoped): (9 test-only callers)
- used by: (16 test-only callers)

### `BaseUser`
- def: [`tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts:351`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L351)
- signature: `class BaseUser`
- members:
  - `<constructor>(name: string)` — [`L352`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L352)
- used by: (3 test-only callers)

### `Cat`  ·  implements/extends Animal
- def: [`tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts:165`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L165)
- signature: `class Cat`
- members:
  - `<constructor>(name: string, age: number, indoor?: boolean)` — [`L168`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L168)
  - `climb(method)` — [`L182`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L182)
  - `makeSound(method)` — [`L173`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L173)
  - `move(method)` — [`L177`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L177)
  - `indoor` — [`L166`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L166)
- uses (calls/refs, reference-scoped): (2 test-only callers)
- used by: (4 test-only callers)

### `Constructor`
- def: [`tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts:323`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L323)
- signature: `type Constructor`
- used by: (2 test-only callers)

### `Container`
- def: [`tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts:231`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L231)
- signature: `class Container`
- members:
  - `add(method)` — [`L234`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L234)
  - `clear(method)` — [`L255`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L255)
  - `getAll(method)` — [`L247`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L247)
  - `remove(method)` — [`L238`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L238)
  - `size(method)` — [`L251`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L251)
  - `items` — [`L232`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L232)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (4 test-only callers)

### `Database`
- def: [`tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts:273`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L273)
- signature: `class Database`
- members:
  - `connect(method)` — [`L288`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L288)
  - `disconnect(method)` — [`L293`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L293)
  - `getInstance(method)` — [`L281`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L281)
  - `connections` — [`L275`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L275)
  - `instance` — [`L274`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L274)
- used by: (1 test-only callers)

### `Dog`  ·  implements/extends Animal
- def: [`tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts:141`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L141)
- signature: `class Dog`
- members:
  - `<constructor>(name: string, age: number, breed: string)` — [`L144`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L144)
  - `fetch(method)` — [`L160`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L160)
  - `makeSound(method)` — [`L150`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L150)
  - `move(method)` — [`L155`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L155)
  - `breed` — [`L142`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L142)
- uses (calls/refs, reference-scoped): (2 test-only callers)
- used by: (6 test-only callers)

### `Duck`  ·  implements/extends Animal, Flyable, Swimmable
- def: [`tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts:198`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L198)
- signature: `class Duck`
- members:
  - `<constructor>(name: string, age: number)` — [`L199`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L199)
  - `fly(method)` — [`L212`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L212)
  - `land(method)` — [`L216`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L216)
  - `makeSound(method)` — [`L203`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L203)
  - `move(method)` — [`L207`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L207)
  - `surface(method)` — [`L225`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L225)
  - `swim(method)` — [`L221`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L221)
- uses (calls/refs, reference-scoped): (4 test-only callers)
- used by: (10 test-only callers)

### `Employee`  ·  implements/extends Person
- def: [`tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts:77`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L77)
- signature: `class Employee`
- members:
  - `<constructor>(name: string, age: number, id: number, department: string, salary: number)` — [`L81`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L81)
  - `<get>monthlySalary` — [`L104`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L104)
  - `<set>monthlySalary` — [`L109`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L109)
  - `celebrateBirthday(method)` — [`L98`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L98)
  - `introduce(method)` — [`L88`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L88)
  - `work(method)` — [`L93`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L93)
  - `department` — [`L79`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L79)
  - `salary` — [`L78`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L78)
- uses (calls/refs, reference-scoped): (5 test-only callers)
- used by: (6 test-only callers)

### `Flyable`
- def: [`tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts:188`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L188)
- signature: `interface Flyable`
- members:
  - `fly(method)` — [`L189`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L189)
  - `land(method)` — [`L190`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L190)
- uses (calls/refs, reference-scoped): (3 test-only callers)
- used by: (1 test-only callers)

### `MathUtils`
- def: [`tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts:303`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L303)
- signature: `class MathUtils`
- members:
  - `calculateCircleArea(method)` — [`L309`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L309)
  - `calculateDistance(method)` — [`L313`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L313)
  - `clamp(method)` — [`L317`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L317)
  - `PI` — [`L307`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L307)

### `NumberContainer`  ·  implements/extends Container
- def: [`tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts:261`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L261)
- signature: `class NumberContainer`
- members:
  - `average(method)` — [`L266`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L266)
  - `sum(method)` — [`L262`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L262)
- uses (calls/refs, reference-scoped): (2 test-only callers)
- used by: (2 test-only callers)

### `Person`
- def: [`tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts:8`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L8)
- doc: Classes and Inheritance
- signature: `class Person`
- members:
  - `<constructor>(name: string, age: number, id: number)` — [`L29`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L29) — Classes and Inheritance
  - `<get>id` — [`L54`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L54)
  - `<set>id` — [`L59`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L59)
  - `getSpecies(method)` — [`L25`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L25)
  - `greet(method)` — [`L66`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L66)
  - `introduce(method)` — [`L37`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L37)
  - `updateAge(method)` — [`L47`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L47)
  - `validateAge(method)` — [`L42`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L42)
  - `age` — [`L16`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L16)
  - `birthDate` — [`L19`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L19)
  - `name` — [`L10`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L10)
  - `species` — [`L22`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L22)
- protocol/private: `_id`[`L13`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L13)
- uses (calls/refs, reference-scoped): (2 test-only callers)
- used by: (8 test-only callers)

### `Swimmable`
- def: [`tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts:193`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L193)
- signature: `interface Swimmable`
- members:
  - `surface(method)` — [`L195`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L195)
  - `swim(method)` — [`L194`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L194)
- uses (calls/refs, reference-scoped): (3 test-only callers)
- used by: (1 test-only callers)

## Functions
- `Activatable(Base: TBase)` — [`L336`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L336)
- `Timestamped(Base: TBase)` — [`L326`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L326)

## Module values
- `ActivatableUser` — [`L357`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L357)
- `EnhancedUser` — [`L358`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L358)
- `TimestampedUser` — [`L356`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L356)
- `classExamples` — [`L361`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/classes-inheritance.ts#L361)

