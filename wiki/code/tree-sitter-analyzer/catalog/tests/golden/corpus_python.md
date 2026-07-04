---
title: 'Module: tests/golden/corpus_python.py'
type: catalog
provenance: extracted
module: tests/golden/corpus_python.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.golden.corpus_python`/
symbols:
  num: num.
  dog: dog.
  prop_example: prop_example.
  person: person.
  PropertyExample: PropertyExample#
  PropertyExample.value: PropertyExample#value().
  numbers: numbers.
  Animal.describe: Animal#describe().
  Person.greet: Person#greet().
  timing_decorator: timing_decorator().
  decorated_function: decorated_function().
  list_comp: list_comp.
  dict_comp: dict_comp.
  set_comp: set_comp.
  Animal: Animal#
  Dog: Dog#
  Dog.fetch: Dog#fetch().
  ComplexNesting.level2_nested: ComplexNesting#level2_nested().
  Person.__post_init__: Person#__post_init__().
  gen_expr: gen_expr.
  filtered_gen: filtered_gen.
  Animal.make_sound: Animal#make_sound().
  Dog.__init__: Dog#__init__().
  ComplexNesting.level1_method: ComplexNesting#level1_method().
  PropertyExample._value: PropertyExample#_value.
  Animal.name: Animal#name.
  Person: Person#
  Person.name: Person#name.
  Person.age: Person#age.
  timing_decorator.wrapper: timing_decorator().wrapper().
  square: square.
  generator_function: generator_function().
  Animal.__init__: Animal#__init__().
  Animal.species: Animal#species.
  Dog.make_sound: Dog#make_sound().
  ComplexNesting.level2_nested.Level3Class: ComplexNesting#level2_nested().Level3Class#
  Person.email: Person#email.
  PropertyExample.__init__: PropertyExample#__init__().
  PropertyExample.static_method: PropertyExample#static_method().
  PropertyExample.class_method: PropertyExample#class_method().
  regular_function: regular_function().
  async_function: async_function().
  function_with_defaults: function_with_defaults().
  variadic_function: variadic_function().
  add: add.
  complex_lambda: complex_lambda.
  key_function: key_function.
  filter_function: filter_function.
  fibonacci_generator: fibonacci_generator().
  async_generator: async_generator().
  Dog.breed: Dog#breed.
  NestedClassExample: NestedClassExample#
  NestedClassExample.Inner: NestedClassExample#Inner#
  NestedClassExample.Inner.inner_method: NestedClassExample#Inner#inner_method().
  NestedClassExample.outer_method: NestedClassExample#outer_method().
  ComplexNesting: ComplexNesting#
  ComplexNesting.level2_nested.Level3Class.level4_method: ComplexNesting#level2_nested().Level3Class#level4_method().
---
# Module: [`tests/golden/corpus_python.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_python.py)

## Classes
### `Animal`  ·  implements/extends ABC
- def: [`tests/golden/corpus_python.py:150`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_python.py#L150)
- doc: 抽象基类
- signature: `class Animal(ABC):`
- members:
  - `describe(self)` — [`L162`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_python.py#L162) — 普通方法
  - `make_sound(self)` — [`L158`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_python.py#L158) — 抽象方法（必须被子类实现）
  - `name` — [`L154`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_python.py#L154)
  - `species` — [`L155`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_python.py#L155)
- protocol/private: `__init__`[`L153`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_python.py#L153)
- uses (calls/refs, reference-scoped): (2 test-only callers)
- used by: (3 test-only callers)

### `ComplexNesting`
- def: [`tests/golden/corpus_python.py:200`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_python.py#L200)
- doc: 复杂嵌套结构（测试深度遍历）
- signature: `class ComplexNesting:`
- members:
  - `level1_method(self)` — [`L203`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_python.py#L203) — 第一层方法
  - `level2_nested()` — [`L206`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_python.py#L206) — 嵌套函数（第二层）
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `Dog`  ·  implements/extends Animal
- def: [`tests/golden/corpus_python.py:167`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_python.py#L167)
- doc: 继承自 Animal 的子类
- signature: `class Dog(Animal):`
- members:
  - `fetch(self, item: str)` — [`L178`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_python.py#L178) — 狗的特有方法
  - `make_sound(self)` — [`L174`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_python.py#L174) — 实现抽象方法
  - `breed` — [`L172`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_python.py#L172)
- protocol/private: `__init__`[`L170`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_python.py#L170)
- uses (calls/refs, reference-scoped): (3 test-only callers)
- used by: (3 test-only callers)

### `Inner`
- def: [`tests/golden/corpus_python.py:186`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_python.py#L186)
- doc: 内部类
- signature: `class Inner:`
- members:
  - `inner_method(self)` — [`L188`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_python.py#L188)

### `Level3Class`
- def: [`tests/golden/corpus_python.py:209`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_python.py#L209)
- doc: 嵌套类（第三层）
- signature: `class Level3Class:`
- members:
  - `level4_method(self)` — [`L212`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_python.py#L212) — 嵌套类的方法（第四层）
- used by: (1 test-only callers)

### `NestedClassExample`
- def: [`tests/golden/corpus_python.py:183`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_python.py#L183)
- doc: 嵌套类示例
- signature: `class NestedClassExample:`
- members:
  - `outer_method(self)` — [`L191`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_python.py#L191) — 外部方法

### `Person`
- def: [`tests/golden/corpus_python.py:18`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_python.py#L18)
- doc: 使用 @dataclass 装饰器的类（decorated_definition）
- signature: `class Person:`
- members:
  - `__post_init__(self)` — [`L24`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_python.py#L24) — 数据类的初始化后处理
  - `greet(self)` — [`L29`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_python.py#L29) — 问候方法
  - `age` — [`L21`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_python.py#L21)
  - `email` — [`L22`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_python.py#L22)
  - `name` — [`L20`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_python.py#L20)
- used by: (1 test-only callers)

### `PropertyExample`
- def: [`tests/golden/corpus_python.py:34`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_python.py#L34)
- doc: 属性装饰器示例（decorated_definition）
- signature: `class PropertyExample:`
- members:
  - `class_method(cls)` — [`L56`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_python.py#L56) — 类方法（decorated_definition）
  - `static_method()` — [`L51`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_python.py#L51) — 静态方法（decorated_definition）
  - `value(self)` — [`L41`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_python.py#L41) — 使用 @property 装饰器（decorated_definition）
- protocol/private: `__init__`[`L37`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_python.py#L37), `_value`[`L38`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_python.py#L38)
- used by: (1 test-only callers)

## Functions
- `async_function(url: str)` — [`L83`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_python.py#L83) — 异步函数定义
- `async_generator(n: int)` — [`L129`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_python.py#L129) — 异步生成器（yield）
- `decorated_function(x: int)` — [`L69`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_python.py#L69) — 使用自定义装饰器的函数（decorated_definition）
- `fibonacci_generator(limit: int)` — [`L121`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_python.py#L121) — 斐波那契生成器（yield）
- `function_with_defaults(x: int, y: int = 10, z: str = "default")` — [`L88`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_python.py#L88) — 带默认参数的函数
- `generator_function(n: int)` — [`L114`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_python.py#L114) — 生成器函数（yield）
- `regular_function(a: int, b: int)` — [`L78`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_python.py#L78) — 常规函数定义
- `timing_decorator(func)` — [`L61`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_python.py#L61) — 自定义装饰器
- `variadic_function(*args: int, **kwargs: str)` — [`L93`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_python.py#L93) — 可变参数函数
- `wrapper(*args, **kwargs)` — [`L63`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_python.py#L63)

## Module values
- `add` — [`L104`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_python.py#L104)
- `complex_lambda` — [`L105`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_python.py#L105)
- `dict_comp` — [`L138`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_python.py#L138)
- `dog` — [`L235`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_python.py#L235)
- `filter_function` — [`L107`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_python.py#L107)
- `filtered_gen` — [`L143`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_python.py#L143)
- `gen_expr` — [`L142`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_python.py#L142)
- `key_function` — [`L106`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_python.py#L106)
- `list_comp` — [`L137`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_python.py#L137)
- `num` — [`L240`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_python.py#L240)
- `numbers` — [`L136`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_python.py#L136)
- `person` — [`L227`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_python.py#L227)
- `prop_example` — [`L230`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_python.py#L230)
- `set_comp` — [`L139`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_python.py#L139)
- `square` — [`L103`](../../../../../../raw/code/tree-sitter-analyzer/tests/golden/corpus_python.py#L103)

