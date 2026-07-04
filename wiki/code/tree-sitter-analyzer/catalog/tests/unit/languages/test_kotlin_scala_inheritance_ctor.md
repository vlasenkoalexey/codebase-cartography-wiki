---
title: 'Module: tests/unit/languages/test_kotlin_scala_inheritance_ctor.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_kotlin_scala_inheritance_ctor.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_kotlin_scala_inheritance_ctor`/
symbols:
  TestScalaQualifiedGenericInheritance.test_generic_and_qualified_parents: TestScalaQualifiedGenericInheritance#test_generic_and_qualified_parents().
  TestKotlinInheritance.classes: TestKotlinInheritance#classes().
  TestScalaInheritance.classes: TestScalaInheritance#classes().
  TestKotlinPrimaryConstructors.functions: TestKotlinPrimaryConstructors#functions().
  _StubNode: _StubNode#
  TestKotlinPrimaryCtorFallbacks.test_orphan_node_returns_anonymous: TestKotlinPrimaryCtorFallbacks#test_orphan_node_returns_anonymous().
  TestKotlinPrimaryCtorFallbacks.test_parent_without_identifier_returns_anonymous: TestKotlinPrimaryCtorFallbacks#test_parent_without_identifier_returns_anonymous().
  TestKotlinPrimaryCtorFallbacks.test_extractor_swallows_node_errors: TestKotlinPrimaryCtorFallbacks#test_extractor_swallows_node_errors().
  TestKotlinPrimaryCtorFallbacks.test_extractor_swallows_node_errors._Exploding: TestKotlinPrimaryCtorFallbacks#test_extractor_swallows_node_errors()._Exploding#
  _kotlin_parser: _kotlin_parser().
  KOTLIN_INHERITANCE_SRC: KOTLIN_INHERITANCE_SRC.
  SCALA_INHERITANCE_SRC: SCALA_INHERITANCE_SRC.
  KOTLIN_PRIMARY_CTOR_SRC: KOTLIN_PRIMARY_CTOR_SRC.
  TestScalaQualifiedGenericInheritance.CODE: TestScalaQualifiedGenericInheritance#CODE.
  _scala_parser: _scala_parser().
  TestKotlinInheritance: TestKotlinInheritance#
  TestKotlinInheritance.test_success_extends_result: TestKotlinInheritance#test_success_extends_result().
  TestKotlinInheritance.test_success_no_interfaces: TestKotlinInheritance#test_success_no_interfaces().
  TestKotlinInheritance.test_user_manager_no_superclass: TestKotlinInheritance#test_user_manager_no_superclass().
  TestKotlinInheritance.test_user_manager_interfaces: TestKotlinInheritance#test_user_manager_interfaces().
  TestKotlinInheritance.test_plain_class_no_delegation: TestKotlinInheritance#test_plain_class_no_delegation().
  TestKotlinInheritance.test_class_count_unchanged: TestKotlinInheritance#test_class_count_unchanged().
  TestScalaInheritance: TestScalaInheritance#
  TestScalaInheritance.test_circle_superclass: TestScalaInheritance#test_circle_superclass().
  TestScalaInheritance.test_circle_interfaces: TestScalaInheritance#test_circle_interfaces().
  TestScalaInheritance.test_rectangle_superclass: TestScalaInheritance#test_rectangle_superclass().
  TestScalaInheritance.test_rectangle_interfaces: TestScalaInheritance#test_rectangle_interfaces().
  TestScalaInheritance.test_shape_no_extends: TestScalaInheritance#test_shape_no_extends().
  TestScalaInheritance.test_standalone_no_extends: TestScalaInheritance#test_standalone_no_extends().
  TestScalaInheritance.test_class_count_unchanged: TestScalaInheritance#test_class_count_unchanged().
  TestKotlinPrimaryConstructors: TestKotlinPrimaryConstructors#
  TestKotlinPrimaryConstructors.test_point_ctor_emitted: TestKotlinPrimaryConstructors#test_point_ctor_emitted().
  TestKotlinPrimaryConstructors.test_point_ctor_is_constructor_true: TestKotlinPrimaryConstructors#test_point_ctor_is_constructor_true().
  TestKotlinPrimaryConstructors.test_point_ctor_parameters: TestKotlinPrimaryConstructors#test_point_ctor_parameters().
  TestKotlinPrimaryConstructors.test_named_ctor_emitted: TestKotlinPrimaryConstructors#test_named_ctor_emitted().
  TestKotlinPrimaryConstructors.test_named_ctor_params: TestKotlinPrimaryConstructors#test_named_ctor_params().
  TestKotlinPrimaryConstructors.test_noargs_class_no_ctor: TestKotlinPrimaryConstructors#test_noargs_class_no_ctor().
  TestKotlinPrimaryConstructors.test_regular_methods_still_present: TestKotlinPrimaryConstructors#test_regular_methods_still_present().
  TestKotlinPrimaryConstructors.test_total_function_count: TestKotlinPrimaryConstructors#test_total_function_count().
  TestKotlinPrimaryConstructors.test_ctor_language_kotlin: TestKotlinPrimaryConstructors#test_ctor_language_kotlin().
  TestScalaQualifiedGenericInheritance: TestScalaQualifiedGenericInheritance#
  _StubNode.__init__: _StubNode#__init__().
  _StubNode.parent: _StubNode#parent.
  _StubNode.children: _StubNode#children.
  TestKotlinPrimaryCtorFallbacks: TestKotlinPrimaryCtorFallbacks#
  TestKotlinPrimaryCtorFallbacks.test_extractor_swallows_node_errors._Exploding.start_point: TestKotlinPrimaryCtorFallbacks#test_extractor_swallows_node_errors()._Exploding#start_point().
---
# Module: [`tests/unit/languages/test_kotlin_scala_inheritance_ctor.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_scala_inheritance_ctor.py)

## Classes
### `TestKotlinInheritance`
- def: [`tests/unit/languages/test_kotlin_scala_inheritance_ctor.py:71`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_scala_inheritance_ctor.py#L71)
- doc: delegation_specifiers → superclass / interfaces populated.
- signature: `class TestKotlinInheritance:`
- members:
  - `classes(self)` — [`L75`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_scala_inheritance_ctor.py#L75)
  - `test_class_count_unchanged(self, classes: dict)` — [`L107`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_scala_inheritance_ctor.py#L107) — No extra classes emitted by reading delegation_specifiers.
  - `test_plain_class_no_delegation(self, classes: dict)` — [`L101`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_scala_inheritance_ctor.py#L101) — Result has no delegation_specifiers — fields stay default.
  - `test_success_extends_result(self, classes: dict)` — [`L81`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_scala_inheritance_ctor.py#L81) — constructor_invocation child → superclass.
  - `test_success_no_interfaces(self, classes: dict)` — [`L86`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_scala_inheritance_ctor.py#L86)
  - `test_user_manager_interfaces(self, classes: dict)` — [`L96`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_scala_inheritance_ctor.py#L96) — Two user_type delegation_specifiers → interfaces list.
  - `test_user_manager_no_superclass(self, classes: dict)` — [`L90`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_scala_inheritance_ctor.py#L90) — When only user_type children present (no constructor_invocation) all
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`KotlinElementExtractor`](../../../tree_sitter_analyzer/languages/kotlin_plugin.md#KotlinElementExtractor), [`extract_classes`](../../../tree_sitter_analyzer/languages/kotlin_plugin.md#KotlinElementExtractor.extract_classes)  (2 test-only)

### `TestKotlinPrimaryConstructors`
- def: [`tests/unit/languages/test_kotlin_scala_inheritance_ctor.py:198`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_scala_inheritance_ctor.py#L198)
- doc: primary_constructor nodes emitted as Function(is_constructor=True).
- signature: `class TestKotlinPrimaryConstructors:`
- members:
  - `functions(self)` — [`L202`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_scala_inheritance_ctor.py#L202)
  - `test_ctor_language_kotlin(self, functions: list)` — [`L244`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_scala_inheritance_ctor.py#L244)
  - `test_named_ctor_emitted(self, functions: list)` — [`L221`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_scala_inheritance_ctor.py#L221)
  - `test_named_ctor_params(self, functions: list)` — [`L225`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_scala_inheritance_ctor.py#L225)
  - `test_noargs_class_no_ctor(self, functions: list)` — [`L229`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_scala_inheritance_ctor.py#L229) — class NoArgs {} has no primary_constructor node — not emitted.
  - `test_point_ctor_emitted(self, functions: list)` — [`L208`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_scala_inheritance_ctor.py#L208)
  - `test_point_ctor_is_constructor_true(self, functions: list)` — [`L212`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_scala_inheritance_ctor.py#L212)
  - `test_point_ctor_parameters(self, functions: list)` — [`L216`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_scala_inheritance_ctor.py#L216) — Primary constructor parameters extracted.
  - `test_regular_methods_still_present(self, functions: list)` — [`L234`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_scala_inheritance_ctor.py#L234) — greet and doWork still extracted.
  - `test_total_function_count(self, functions: list)` — [`L240`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_scala_inheritance_ctor.py#L240) — Point ctor + Named ctor + greet + doWork = 4.
- uses (calls/refs, reference-scoped): [`KotlinElementExtractor`](../../../tree_sitter_analyzer/languages/kotlin_plugin.md#KotlinElementExtractor), [`extract_functions`](../../../tree_sitter_analyzer/languages/kotlin_plugin.md#KotlinElementExtractor.extract_functions)  (2 test-only)

### `TestKotlinPrimaryCtorFallbacks`
- def: [`tests/unit/languages/test_kotlin_scala_inheritance_ctor.py:284`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_scala_inheritance_ctor.py#L284)
- doc: codecov/patch on #585: anonymous fallbacks + extractor error branch.
- signature: `class TestKotlinPrimaryCtorFallbacks:`
- members:
  - `test_extractor_swallows_node_errors(self)` — [`L306`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_scala_inheritance_ctor.py#L306)
  - `test_orphan_node_returns_anonymous(self)` — [`L287`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_scala_inheritance_ctor.py#L287)
  - `test_parent_without_identifier_returns_anonymous(self)` — [`L295`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_scala_inheritance_ctor.py#L295)
- uses (calls/refs, reference-scoped): [`extract_kotlin_primary_constructor`](../../../tree_sitter_analyzer/languages/kotlin_helpers.md#extract_kotlin_primary_constructor), [`_kotlin_primary_ctor_class_name`](../../../tree_sitter_analyzer/languages/kotlin_helpers.md#_kotlin_primary_ctor_class_name)  (2 test-only)

### `TestScalaInheritance`
- def: [`tests/unit/languages/test_kotlin_scala_inheritance_ctor.py:139`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_scala_inheritance_ctor.py#L139)
- doc: extends_clause → superclass / interfaces populated.
- signature: `class TestScalaInheritance:`
- members:
  - `classes(self)` — [`L143`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_scala_inheritance_ctor.py#L143)
  - `test_circle_interfaces(self, classes: dict)` — [`L153`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_scala_inheritance_ctor.py#L153) — type_identifier after 'with' keywords = interfaces.
  - `test_circle_superclass(self, classes: dict)` — [`L149`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_scala_inheritance_ctor.py#L149) — First type_identifier after 'extends' = superclass.
  - `test_class_count_unchanged(self, classes: dict)` — [`L172`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_scala_inheritance_ctor.py#L172) — No extra classes emitted by reading extends_clause.
  - `test_rectangle_interfaces(self, classes: dict)` — [`L160`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_scala_inheritance_ctor.py#L160)
  - `test_rectangle_superclass(self, classes: dict)` — [`L157`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_scala_inheritance_ctor.py#L157)
  - `test_shape_no_extends(self, classes: dict)` — [`L163`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_scala_inheritance_ctor.py#L163) — Abstract base class — no extends_clause.
  - `test_standalone_no_extends(self, classes: dict)` — [`L168`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_scala_inheritance_ctor.py#L168)
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`ScalaElementExtractor`](../../../tree_sitter_analyzer/languages/scala_plugin.md#ScalaElementExtractor), [`extract_classes`](../../../tree_sitter_analyzer/languages/scala_plugin.md#ScalaElementExtractor.extract_classes)  (2 test-only)

### `TestScalaQualifiedGenericInheritance`
- def: [`tests/unit/languages/test_kotlin_scala_inheritance_ctor.py:249`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_scala_inheritance_ctor.py#L249)
- doc: Codex P2 on #585: Base\[String\] (generic_type) and pkg.M
- signature: `class TestScalaQualifiedGenericInheritance:`
- members:
  - `test_generic_and_qualified_parents(self)` — [`L258`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_scala_inheritance_ctor.py#L258)
  - `CODE` — [`L253`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_scala_inheritance_ctor.py#L253)
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`ScalaElementExtractor`](../../../tree_sitter_analyzer/languages/scala_plugin.md#ScalaElementExtractor), [`interfaces`](../../../tree_sitter_analyzer/models/base.md#Class.interfaces), [`superclass`](../../../tree_sitter_analyzer/models/base.md#Class.superclass), [`extract_classes`](../../../tree_sitter_analyzer/languages/scala_plugin.md#ScalaElementExtractor.extract_classes)

### `_Exploding`  ·  implements/extends _StubNode
- def: [`tests/unit/languages/test_kotlin_scala_inheritance_ctor.py:311`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_scala_inheritance_ctor.py#L311)
- signature: `class _Exploding(_StubNode):`
- members:
  - `start_point(self)` — [`L313`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_scala_inheritance_ctor.py#L313)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (2 test-only callers)

### `_StubNode`
- def: [`tests/unit/languages/test_kotlin_scala_inheritance_ctor.py:275`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_scala_inheritance_ctor.py#L275)
- doc: Minimal stand-in for a tree-sitter node (explicit parent, no auto-chains).
- signature: `class _StubNode:`
- members:
  - `children` — [`L281`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_scala_inheritance_ctor.py#L281)
  - `parent` — [`L280`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_scala_inheritance_ctor.py#L280)
- protocol/private: `__init__`[`L278`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_scala_inheritance_ctor.py#L278)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (3 test-only callers)

## Functions
- `_kotlin_parser()` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_scala_inheritance_ctor.py#L33)
- `_scala_parser()` — [`L40`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_scala_inheritance_ctor.py#L40)

## Module values
- `KOTLIN_INHERITANCE_SRC` — [`L52`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_scala_inheritance_ctor.py#L52)
- `KOTLIN_PRIMARY_CTOR_SRC` — [`L183`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_scala_inheritance_ctor.py#L183)
- `SCALA_INHERITANCE_SRC` — [`L118`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_scala_inheritance_ctor.py#L118)

