---
title: 'Module: tests/golden/corpus_typescript.ts'
type: catalog
provenance: extracted
module: tests/golden/corpus_typescript.ts
status: fresh
symbol_base: scip-typescript npm . . tests/golden/`corpus_typescript.ts`/
symbols:
  Person.-constructor: Person#`<constructor>`().
  name-personName-age-personAge-.typeLiteral77.age: '`{ name: personName, age: personAge
    }`.typeLiteral77:age.'
  x-...rest-.typeLiteral86.z: '`{ x, ...rest }`.typeLiteral86:z.'
  MyDog.-constructor: MyDog#`<constructor>`().
  constObject: constObject.
  counter: counter.
  Dog: Dog#
  Person: Person#
  Counter: Counter#
  Person.getSpecies: Person#getSpecies().
  Person.fetchProfile: Person#fetchProfile().
  Shape.describe: Shape#describe().
  DecoratedClass: DecoratedClass#
  complexAsyncOperation: complexAsyncOperation().
  PersonName: PersonName#
  Animal: Animal#
  Shape: Shape#
  Shape.area: Shape#area().
  Shape.perimeter: Shape#perimeter().
  DecoratedClass.name: DecoratedClass#name.
  Person.name: Person#name.
  Person._age: Person#_age.
  Person.email: Person#email.
  Box.value: Box#value.
  ReadonlyPoint: ReadonlyPoint#
  Animal.name: Animal#name.
  Animal.age: Animal#age.
  Animal.makeSound: Animal#makeSound().
  Dog.breed: Dog#breed.
  Dog.fetch: Dog#fetch().
  DogWithOwner: DogWithOwner#
  Person.greet: Person#greet().
  Person.-get-age: Person#`<get>age`().
  Person.-set-age: Person#`<set>age`().
  Person.validateEmail: Person#validateEmail().
  Person.sendNotification: Person#sendNotification().
  Box.-constructor: Box#`<constructor>`().
  Box.getValue: Box#getValue().
  Box.setValue: Box#setValue().
  Circle: Circle#
  MyDog: MyDog#
  MyDog.fetch: MyDog#fetch().
  DecoratedClass.greet: DecoratedClass#greet().
  strValue: strValue.
  strValue2: strValue2.
  PartialPerson: PartialPerson#
  RequiredPerson: RequiredPerson#
  PickedPerson: PickedPerson#
  OmittedPerson: OmittedPerson#
  definitelyNotNull: definitelyNotNull.
  getLength: getLength().
  PersonKeys: PersonKeys#
  Point: Point#
  fetchData: fetchData().
  Person.id: Person#id.
  MyDog.name: MyDog#name.
  someValue: someValue.
  name-personName-age-personAge-.typeLiteral77.name: '`{ name: personName, age: personAge
    }`.typeLiteral77:name.'
  x-...rest-.typeLiteral86.x: '`{ x, ...rest }`.typeLiteral86:x.'
  Counter.count: Counter#count.
  Point.typeLiteral0.x: Point#typeLiteral0:x.
  Point.typeLiteral0.y: Point#typeLiteral0:y.
  Result: Result#
  Person.species: Person#species.
  MyDog.age: MyDog#age.
  MyDog.breed: MyDog#breed.
  sealed: sealed().
  log: log().
  required: required().
  maybeNull: maybeNull.
  getLength.T-typeLiteral70.length: getLength().[T]typeLiteral70:length.
  x-...rest-.typeLiteral86.y: '`{ x, ...rest }`.typeLiteral86:y.'
  Counter.increment: Counter#increment().
  StringOrNumber: StringOrNumber#
  Predicate: Predicate#
  Container: Container#
  Container.value: Container#value.
  Container.getValue: Container#getValue().
  Container.setValue: Container#setValue().
  Dictionary: Dictionary#
  Callable: Callable#
  Direction: Direction#
  Direction.North: Direction#North.
  Direction.South: Direction#South.
  Direction.East: Direction#East.
  Direction.West: Direction#West.
  Color: Color#
  Color.Red: Color#Red.
  Color.Green: Color#Green.
  Color.Blue: Color#Blue.
  HttpStatus: HttpStatus#
  HttpStatus.OK: HttpStatus#OK.
  HttpStatus.NotFound: HttpStatus#NotFound.
  HttpStatus.ServerError: HttpStatus#ServerError.
  add: add().
  greet: greet().
  sum: sum().
  identity: identity().
  pair: pair().
  numberGenerator: numberGenerator().
  asyncNumberGenerator: asyncNumberGenerator().
  process: process().
  multiply: multiply.
  wrapInArray: wrapInArray.
  asyncFetch: asyncFetch.
  getFullName: getFullName.
  Box: Box#
  Circle.-constructor: Circle#`<constructor>`().
  Circle.area: Circle#area().
  Circle.perimeter: Circle#perimeter().
  MyDog.makeSound: MyDog#makeSound().
  exportedConst: exportedConst.
  exportedLet: exportedLet.
  exportedFunction: exportedFunction().
  ExportedClass: ExportedClass#
  ExportedClass.value: ExportedClass#value.
  ExportedType: ExportedType#
  ExportedType.typeLiteral61.field: ExportedType#typeLiteral61:field.
  ExportedInterface: ExportedInterface#
  ExportedInterface.method: ExportedInterface#method().
  DefaultExport: DefaultExport#
  DefaultExport.-constructor: DefaultExport#`<constructor>`().
  helper: Utilities/helper().
  HelperClass: Utilities/HelperClass#
  HelperClass.value: Utilities/HelperClass#value.
  nestedHelper: Utilities/Nested/nestedHelper().
  Window: global/Window#
  Window.customProperty: global/Window#customProperty.
  isString: isString().
  IsString: IsString#
  Optional: Optional#
  Greeting: Greeting#
  Direction2D: Direction2D#
  constNumber: constNumber.
  constString: constString.
  constArray: constArray.
  constTuple: constTuple.
  letNumber: letNumber.
  letString: letString.
  letUnion: letUnion.
  varNumber: varNumber.
  inferred: inferred.
  asConstObject: asConstObject.
  asConstArray: asConstArray.
  config: config.
  merge: merge().
---
# Module: [`tests/golden/corpus_typescript.ts`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts)

## Classes
### `Animal`
- def: [`tests/golden/corpus_typescript.ts:35`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L35)
- doc: Interface declaration
- signature: `interface Animal`
- members:
  - `makeSound(method)` — [`L38`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L38)
  - `age` — [`L37`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L37)
  - `name` — [`L36`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L36)
- uses (calls/refs, reference-scoped): (4 test-only callers)
- used by: (1 test-only callers)

### `Box`
- def: [`tests/golden/corpus_typescript.ts:287`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L287)
- doc: Class with generics
- signature: `class Box`
- members:
  - `<constructor>(value: T)` — [`L290`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L290) — Class with generics
  - `getValue(method)` — [`L294`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L294)
  - `setValue(method)` — [`L298`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L298)
  - `value` — [`L288`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L288)

### `Callable`
- def: [`tests/golden/corpus_typescript.ts:60`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L60)
- doc: Interface with call signature
- signature: `interface Callable`

### `Circle`  ·  implements/extends Shape
- def: [`tests/golden/corpus_typescript.ts:318`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L318)
- doc: Class extending abstract class
- signature: `class Circle`
- members:
  - `<constructor>(radius: number)` — [`L319`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L319) — Class extending abstract class
  - `area(method)` — [`L323`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L323)
  - `perimeter(method)` — [`L327`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L327)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (3 test-only callers)

### `Color`
- def: [`tests/golden/corpus_typescript.ts:99`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L99)
- doc: String enum
- signature: `enum Color`
- members:
  - `Blue` — [`L102`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L102)
  - `Green` — [`L101`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L101)
  - `Red` — [`L100`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L100)

### `Container`
- def: [`tests/golden/corpus_typescript.ts:44`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L44)
- doc: Interface with generics
- signature: `interface Container`
- members:
  - `getValue(method)` — [`L46`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L46)
  - `setValue(method)` — [`L47`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L47)
  - `value` — [`L45`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L45)

### `Counter`
- def: [`tests/golden/corpus_typescript.ts:605`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L605)
- signature: `interface Counter`
- members:
  - `increment(method)` — [`L607`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L607)
  - `count` — [`L606`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L606)
- used by: (1 test-only callers)

### `DecoratedClass`
- def: [`tests/golden/corpus_typescript.ts:390`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L390)
- doc: Decorated class
- signature: `class DecoratedClass`
- members:
  - `greet(method)` — [`L395`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L395)
  - `name` — [`L392`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L392)
- uses (calls/refs, reference-scoped): (3 test-only callers)

### `DefaultExport`
- def: [`tests/golden/corpus_typescript.ts:439`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L439)
- signature: `class DefaultExport`
- members:
  - `<constructor>()` — [`L440`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L440)

### `Dictionary`
- def: [`tests/golden/corpus_typescript.ts:53`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L53)
- doc: Interface with index signature
- signature: `interface Dictionary`

### `Direction`
- def: [`tests/golden/corpus_typescript.ts:89`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L89)
- doc: Regular enum
- signature: `enum Direction`
- members:
  - `East` — [`L92`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L92)
  - `North` — [`L90`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L90)
  - `South` — [`L91`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L91)
  - `West` — [`L93`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L93)

### `Direction2D`
- def: [`tests/golden/corpus_typescript.ts:511`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L511)
- signature: `type Direction2D`

### `Dog`
- def: [`tests/golden/corpus_typescript.ts:67`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L67)
- doc: Interface extension
- signature: `interface Dog`
- members:
  - `fetch(method)` — [`L69`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L69)
  - `breed` — [`L68`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L68)
- uses (calls/refs, reference-scoped): (4 test-only callers)
- used by: (2 test-only callers)

### `DogWithOwner`
- def: [`tests/golden/corpus_typescript.ts:75`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L75)
- doc: Intersection type
- signature: `type DogWithOwner`
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `ExportedClass`
- def: [`tests/golden/corpus_typescript.ts:424`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L424)
- signature: `class ExportedClass`
- members:
  - `value` — [`L425`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L425)

### `ExportedInterface`
- def: [`tests/golden/corpus_typescript.ts:430`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L430)
- signature: `interface ExportedInterface`
- members:
  - `method(method)` — [`L431`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L431)

### `ExportedType`
- def: [`tests/golden/corpus_typescript.ts:429`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L429)
- signature: `type ExportedType`
- members:
  - `field` — [`L429`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L429)

### `Greeting`
- def: [`tests/golden/corpus_typescript.ts:510`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L510)
- doc: Template literal type
- signature: `type Greeting`

### `HelperClass`
- def: [`tests/golden/corpus_typescript.ts:452`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L452)
- signature: `class HelperClass`
- members:
  - `value` — [`L453`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L453)

### `HttpStatus`
- def: [`tests/golden/corpus_typescript.ts:108`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L108)
- doc: Const enum
- signature: `enum HttpStatus`
- members:
  - `NotFound` — [`L110`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L110)
  - `OK` — [`L109`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L109)
  - `ServerError` — [`L111`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L111)

### `IsString`
- def: [`tests/golden/corpus_typescript.ts:498`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L498)
- doc: Conditional type
- signature: `type IsString`

### `MyDog`  ·  implements/extends Animal, Dog
- def: [`tests/golden/corpus_typescript.ts:335`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L335)
- doc: Class implementing interface
- signature: `class MyDog`
- members:
  - `<constructor>(name: string, age: number, breed: string)` — [`L340`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L340) — Class implementing interface
  - `fetch(method)` — [`L350`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L350)
  - `makeSound(method)` — [`L346`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L346)
  - `age` — [`L337`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L337)
  - `breed` — [`L338`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L338)
  - `name` — [`L336`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L336)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (7 test-only callers)

### `OmittedPerson`
- def: [`tests/golden/corpus_typescript.ts:519`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L519)
- signature: `type OmittedPerson`
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `Optional`
- def: [`tests/golden/corpus_typescript.ts:503`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L503)
- doc: Mapped type
- signature: `type Optional`

### `PartialPerson`
- def: [`tests/golden/corpus_typescript.ts:516`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L516)
- doc: Utility types usage
- signature: `type PartialPerson`
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `Person`
- def: [`tests/golden/corpus_typescript.ts:223`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L223)
- doc: Class with all member types
- signature: `class Person`
- members:
  - `<constructor>(name: string, age: number, email: string)` — [`L240`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L240) — Class with all member types
  - `<get>age` — [`L253`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L253)
  - `<set>age` — [`L258`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L258)
  - `fetchProfile(method)` — [`L269`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L269)
  - `getSpecies(method)` — [`L264`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L264)
  - `greet(method)` — [`L248`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L248)
  - `sendNotification(method)` — [`L279`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L279)
  - `validateEmail(method)` — [`L274`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L274)
  - `email` — [`L231`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L231)
  - `id` — [`L234`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L234)
  - `name` — [`L225`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L225)
  - `species` — [`L237`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L237)
- protocol/private: `_age`[`L228`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L228)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (6 test-only callers)

### `PersonKeys`
- def: [`tests/golden/corpus_typescript.ts:622`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L622)
- signature: `type PersonKeys`
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `PersonName`
- def: [`tests/golden/corpus_typescript.ts:621`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L621)
- signature: `type PersonName`
- uses (calls/refs, reference-scoped): (2 test-only callers)

### `PickedPerson`
- def: [`tests/golden/corpus_typescript.ts:518`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L518)
- signature: `type PickedPerson`
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `Point`
- def: [`tests/golden/corpus_typescript.ts:28`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L28)
- signature: `type Point`
- members:
  - `x` — [`L28`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L28)
  - `y` — [`L28`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L28)
- used by: (2 test-only callers)

### `Predicate`
- def: [`tests/golden/corpus_typescript.ts:29`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L29)
- signature: `type Predicate`

### `ReadonlyPoint`
- def: [`tests/golden/corpus_typescript.ts:30`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L30)
- signature: `type ReadonlyPoint`
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `RequiredPerson`
- def: [`tests/golden/corpus_typescript.ts:517`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L517)
- signature: `type RequiredPerson`
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `Result`
- def: [`tests/golden/corpus_typescript.ts:80`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L80)
- doc: Union type
- signature: `type Result`
- used by: (1 test-only callers)

### `Shape`
- def: [`tests/golden/corpus_typescript.ts:306`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L306)
- doc: Abstract class
- signature: `class Shape`
- members:
  - `area(method)` — [`L307`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L307)
  - `describe(method)` — [`L310`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L310)
  - `perimeter(method)` — [`L308`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L308)
- uses (calls/refs, reference-scoped): (3 test-only callers)
- used by: (1 test-only callers)

### `StringOrNumber`
- def: [`tests/golden/corpus_typescript.ts:27`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L27)
- doc: Type alias declaration
- signature: `type StringOrNumber`

### `Window`
- def: [`tests/golden/corpus_typescript.ts:468`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L468)
- doc: The **`Window`** interface represents a window containing a DOM document; the `document` property points to the DOM document loaded in that window.
- signature: `interface Window`
- members:
  - `customProperty` — [`L469`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L469)

## Functions
- `add(a: number, b: number)` — [`L121`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L121) — Regular function with type annotations
- `asyncNumberGenerator(max: number)` — [`L173`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L173) — Async generator function
- `complexAsyncOperation()` — [`L579`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L579)
- `exportedFunction(x: number)` — [`L420`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L420)
- `fetchData(url: string)` — [`L156`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L156) — Async function
- `getLength(value: T)` — [`L564`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L564) — Generic with constraint
- `greet(name: string, greeting?: string, punctuation?: string)` — [`L128`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L128) — Function with optional and default parameters
- `helper()` — [`L448`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L448)
- `identity(value: T)` — [`L142`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L142) — Generic function
- `isString(value: unknown)` — [`L480`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L480) — Type guard function
- `log(target: any, propertyKey: string, descriptor: PropertyDescriptor)` — [`L370`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L370) — Method decorator
- `merge(obj1: T, obj2: U)` — [`L571`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L571) — Multiple generic constraints
- `nestedHelper()` — [`L457`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L457)
- `numberGenerator(max: number)` — [`L164`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L164) — Generator function
- `pair(first: T, second: U)` — [`L149`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L149) — Function with multiple generic parameters
- `process(value: string)` — [`L182`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L182) — Function overloads
- `required(target: any, propertyKey: string)` — [`L382`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L382) — Property decorator
- `sealed(constructor: Function)` — [`L362`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L362) — Class decorator
- `sum(...numbers: number[])` — [`L135`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L135) — Function with rest parameters

## Module values
- `age` — [`L593`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L593)
- `asConstArray` — [`L545`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L545)
- `asConstObject` — [`L544`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L544)
- `asyncFetch` — [`L205`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L205) — Async arrow function
- `config` — [`L548`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L548)
- `constArray` — [`L528`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L528)
- `constNumber` — [`L526`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L526)
- `constObject` — [`L530`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L530)
- `constString` — [`L527`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L527)
- `constTuple` — [`L529`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L529)
- `counter` — [`L610`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L610)
- `definitelyNotNull` — [`L555`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L555)
- `exportedConst` — [`L417`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L417)
- `exportedLet` — [`L418`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L418)
- `getFullName` — [`L212`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L212) — Arrow function with destructured parameters
- `inferred` — [`L541`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L541)
- `length` — [`L564`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L564)
- `letNumber` — [`L533`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L533)
- `letString` — [`L534`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L534)
- `letUnion` — [`L535`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L535)
- `maybeNull` — [`L554`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L554)
- `multiply` — [`L195`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L195) — Arrow function with type annotation
- `name` — [`L593`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L593)
- `someValue` — [`L487`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L487) — Type assertion
- `strValue` — [`L488`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L488)
- `strValue2` — [`L489`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L489)
- `varNumber` — [`L538`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L538)
- `wrapInArray` — [`L200`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L200) — Arrow function with generic type
- `x` — [`L599`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L599)
- `y` — [`L599`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L599)
- `z` — [`L599`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_typescript.ts#L599)

