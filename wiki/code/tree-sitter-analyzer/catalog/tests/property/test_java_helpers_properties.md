---
title: 'Module: tests/property/test_java_helpers_properties.py'
type: catalog
provenance: extracted
module: tests/property/test_java_helpers_properties.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.property.test_java_helpers_properties`/
symbols:
  TestDetermineVisibilityProperties._NOISE: TestDetermineVisibilityProperties#_NOISE.
  interface_list: interface_list().
  generic_type: generic_type().
  java_type: java_type().
  TestSplitRespectingGenericsProperties.test_roundtrip_element_count: TestSplitRespectingGenericsProperties#test_roundtrip_element_count().
  TestSplitRespectingGenericsProperties.test_no_empty_elements: TestSplitRespectingGenericsProperties#test_no_empty_elements().
  TestSplitRespectingGenericsProperties.test_each_element_starts_with_capital: TestSplitRespectingGenericsProperties#test_each_element_starts_with_capital().
  TestSplitRespectingGenericsProperties.test_no_depth0_comma_inside_element: TestSplitRespectingGenericsProperties#test_no_depth0_comma_inside_element().
  TestDetermineVisibilityProperties.test_private_wins_over_noise: TestDetermineVisibilityProperties#test_private_wins_over_noise().
  TestDetermineVisibilityProperties.test_protected_wins_over_noise: TestDetermineVisibilityProperties#test_protected_wins_over_noise().
  TestDetermineVisibilityProperties.test_no_visibility_modifier_returns_package: TestDetermineVisibilityProperties#test_no_visibility_modifier_returns_package().
  TestDetermineVisibilityProperties.test_return_value_is_one_of_four_options: TestDetermineVisibilityProperties#test_return_value_is_one_of_four_options().
  simple_type: simple_type().
  TestSplitRespectingGenericsProperties.test_simple_types_no_generics: TestSplitRespectingGenericsProperties#test_simple_types_no_generics().
  TestSplitRespectingGenericsProperties.test_single_generic_with_k_args: TestSplitRespectingGenericsProperties#test_single_generic_with_k_args().
  TestDetermineVisibilityProperties.test_public_wins_over_noise: TestDetermineVisibilityProperties#test_public_wins_over_noise().
  _SIMPLE_IDENT: _SIMPLE_IDENT.
  _TYPE_ARG: _TYPE_ARG.
  TestSplitRespectingGenericsProperties: TestSplitRespectingGenericsProperties#
  TestDetermineVisibilityProperties: TestDetermineVisibilityProperties#
---
# Module: [`tests/property/test_java_helpers_properties.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_java_helpers_properties.py)

## Classes
### `TestDetermineVisibilityProperties`
- def: [`tests/property/test_java_helpers_properties.py:153`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_java_helpers_properties.py#L153)
- doc: Property-based tests for Java determine_visibility.
- signature: `class TestDetermineVisibilityProperties:`
- members:
  - `test_no_visibility_modifier_returns_package(self, noise)` — [`L181`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_java_helpers_properties.py#L181) — No visibility keyword → package-private.
  - `test_private_wins_over_noise(self, noise)` — [`L167`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_java_helpers_properties.py#L167) — 'private' in modifiers always returns 'private' regardless of other modifiers.
  - `test_protected_wins_over_noise(self, noise)` — [`L174`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_java_helpers_properties.py#L174) — 'protected' in modifiers always returns 'protected' regardless of other modifiers.
  - `test_public_wins_over_noise(self, noise)` — [`L160`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_java_helpers_properties.py#L160) — 'public' in modifiers always returns 'public' regardless of other modifiers.
  - `test_return_value_is_one_of_four_options(self, modifiers)` — [`L187`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_java_helpers_properties.py#L187) — Return value is always one of the four Java visibility levels.
- protocol/private: `_NOISE`[`L156`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_java_helpers_properties.py#L156)
- uses (calls/refs, reference-scoped): [`determine_visibility`](../../tree_sitter_analyzer/languages/java_helpers.md#determine_visibility)

### `TestSplitRespectingGenericsProperties`
- def: [`tests/property/test_java_helpers_properties.py:72`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_java_helpers_properties.py#L72)
- doc: Property-based tests for _split_respecting_generics.
- signature: `class TestSplitRespectingGenericsProperties:`
- members:
  - `test_each_element_starts_with_capital(self, data)` — [`L96`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_java_helpers_properties.py#L96) — Every result element should start with a capital letter (Java type convention).
  - `test_no_depth0_comma_inside_element(self, data)` — [`L107`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_java_helpers_properties.py#L107) — No result element should contain a depth-0 comma (unbalanced generic brackets).
  - `test_no_empty_elements(self, data)` — [`L87`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_java_helpers_properties.py#L87) — No result element should be empty or whitespace-only.
  - `test_roundtrip_element_count(self, data)` — [`L77`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_java_helpers_properties.py#L77) — Split must return exactly as many elements as were joined.
  - `test_simple_types_no_generics(self, n)` — [`L126`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_java_helpers_properties.py#L126) — For n simple types joined by ', ', result should have exactly n elements.
  - `test_single_generic_with_k_args(self, k)` — [`L137`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_java_helpers_properties.py#L137) — Map<A, B, C> with k type args must come back as one element.
- uses (calls/refs, reference-scoped): [`_split_respecting_generics`](../../tree_sitter_analyzer/languages/_java_element_helpers.md#_split_respecting_generics)  (1 test-only)

## Functions
- `generic_type(draw)` — [`L45`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_java_helpers_properties.py#L45) — Generate a generic Java type like 'Map<K, V>' or 'List<String>'.
- `interface_list(draw)` — [`L60`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_java_helpers_properties.py#L60) — A comma-joined list of 1-5 Java types.
- `java_type(draw)` — [`L54`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_java_helpers_properties.py#L54) — Either a simple or a generic Java type.
- `simple_type(draw)` — [`L39`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_java_helpers_properties.py#L39) — Generate a simple Java type name without generics.

## Module values
- `_SIMPLE_IDENT` — [`L21`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_java_helpers_properties.py#L21)
- `_TYPE_ARG` — [`L31`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_java_helpers_properties.py#L31)

