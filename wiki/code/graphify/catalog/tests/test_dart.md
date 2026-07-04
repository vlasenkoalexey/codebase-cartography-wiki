---
title: 'Module: tests/test_dart.py'
type: catalog
provenance: extracted
module: tests/test_dart.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_dart`/TestDart#
symbols:
  TestDart.temp_path: temp_path.
  TestDart.test_universal_generic_syntax_extraction: test_universal_generic_syntax_extraction().
  TestDart.test_roadmap_bug_fixes: test_roadmap_bug_fixes().
  TestDart.test_advanced_dart_features: test_advanced_dart_features().
  TestDart.test_namespace_and_spaced_generics: test_namespace_and_spaced_generics().
  TestDart.test_dart_and_flutter_specifics: test_dart_and_flutter_specifics().
  TestDart.tearDown: tearDown().
  TestDart.temp_dir: temp_dir.
  TestDart: ''
  TestDart.setUp: setUp().
---
# Module: [`tests/test_dart.py`](../../../../../raw/code/graphify/tests/test_dart.py)

## Classes
### `TestDart`  ·  implements/extends TestCase
- def: [`tests/test_dart.py:10`](../../../../../raw/code/graphify/tests/test_dart.py#L10)
- signature: `class TestDart(unittest.TestCase):`
- members:
  - `setUp(self)` — [`L11`](../../../../../raw/code/graphify/tests/test_dart.py#L11)
  - `tearDown(self)` — [`L15`](../../../../../raw/code/graphify/tests/test_dart.py#L15)
  - `test_advanced_dart_features(self)` — [`L268`](../../../../../raw/code/graphify/tests/test_dart.py#L268) — Test complex Dart 3+ syntax and precise Riverpod/Bloc mappings.
  - `test_dart_and_flutter_specifics(self)` — [`L467`](../../../../../raw/code/graphify/tests/test_dart.py#L467) — Test typedefs, mixin on, factories, constructor DI types, and universal navigation.
  - `test_namespace_and_spaced_generics(self)` — [`L426`](../../../../../raw/code/graphify/tests/test_dart.py#L426) — Test that the parser successfully handles namespaces in extends/implements, and spaces/commas in nested generic variables and methods.
  - `test_roadmap_bug_fixes(self)` — [`L565`](../../../../../raw/code/graphify/tests/test_dart.py#L565) — Test all 5 roadmap bug fixes (Bug A, B, C, D, E).
  - `test_universal_generic_syntax_extraction(self)` — [`L18`](../../../../../raw/code/graphify/tests/test_dart.py#L18) — Test that the universal parser successfully extracts generic relationships, annotations, extensions, classes, and generic calls.
  - `temp_dir` — [`L12`](../../../../../raw/code/graphify/tests/test_dart.py#L12)
  - `temp_path` — [`L13`](../../../../../raw/code/graphify/tests/test_dart.py#L13)
- uses (calls/refs, reference-scoped): [`_make_id`](../graphify/extractors/base.md#_make_id), [`extract_dart`](../graphify/extract.md#extract_dart)

