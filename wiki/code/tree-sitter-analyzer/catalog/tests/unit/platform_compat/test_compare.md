---
title: 'Module: tests/unit/platform_compat/test_compare.py'
type: catalog
provenance: extracted
module: tests/unit/platform_compat/test_compare.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.platform_compat.test_compare`/
symbols:
  _profile: _profile().
  TestProfileComparison.test_has_differences_true: TestProfileComparison#test_has_differences_true().
  _behavior: _behavior().
  TestGenerateDiffReport.test_with_differences: TestGenerateDiffReport#test_with_differences().
  TestCompareProfilesMissing.test_construct_in_a_missing_in_b: TestCompareProfilesMissing#test_construct_in_a_missing_in_b().
  TestCompareProfilesMissing.test_construct_in_b_missing_in_a: TestCompareProfilesMissing#test_construct_in_b_missing_in_a().
  TestBehaviorDifference.test_fields: TestBehaviorDifference#test_fields().
  TestBehaviorDifference.test_diff_types: TestBehaviorDifference#test_diff_types().
  TestProfileComparison.test_has_differences_false_when_empty: TestProfileComparison#test_has_differences_false_when_empty().
  TestCompareProfilesMismatch.test_error_mismatch: TestCompareProfilesMismatch#test_error_mismatch().
  TestCompareProfilesMismatch.test_count_mismatch: TestCompareProfilesMismatch#test_count_mismatch().
  TestCompareProfilesMismatch.test_attribute_mismatch: TestCompareProfilesMismatch#test_attribute_mismatch().
  TestCompareProfilesIdentical.test_identical_profiles_no_differences: TestCompareProfilesIdentical#test_identical_profiles_no_differences().
  TestCompareProfilesIdentical.test_identical_platform_keys_in_result: TestCompareProfilesIdentical#test_identical_platform_keys_in_result().
  TestCompareProfilesMismatch.test_no_diff_when_same_attributes: TestCompareProfilesMismatch#test_no_diff_when_same_attributes().
  TestGenerateDiffReport.test_multiple_differences: TestGenerateDiffReport#test_multiple_differences().
  TestGenerateDiffReport.test_no_differences: TestGenerateDiffReport#test_no_differences().
  TestBehaviorDifference: TestBehaviorDifference#
  TestProfileComparison: TestProfileComparison#
  TestCompareProfilesIdentical: TestCompareProfilesIdentical#
  TestCompareProfilesMissing: TestCompareProfilesMissing#
  TestCompareProfilesMismatch: TestCompareProfilesMismatch#
  TestGenerateDiffReport: TestGenerateDiffReport#
---
# Module: [`tests/unit/platform_compat/test_compare.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/platform_compat/test_compare.py)

## Classes
### `TestBehaviorDifference`
- def: [`tests/unit/platform_compat/test_compare.py:43`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/platform_compat/test_compare.py#L43)
- signature: `class TestBehaviorDifference:`
- members:
  - `test_diff_types(self)` — [`L55`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/platform_compat/test_compare.py#L55)
  - `test_fields(self)` — [`L44`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/platform_compat/test_compare.py#L44)
- uses (calls/refs, reference-scoped): [`diff_type`](../../../tree_sitter_analyzer/platform_compat/compare.md#BehaviorDifference.diff_type), [`BehaviorDifference`](../../../tree_sitter_analyzer/platform_compat/compare.md#BehaviorDifference), [`construct_id`](../../../tree_sitter_analyzer/platform_compat/compare.md#BehaviorDifference.construct_id), [`platform_b_value`](../../../tree_sitter_analyzer/platform_compat/compare.md#BehaviorDifference.platform_b_value), [`details`](../../../tree_sitter_analyzer/platform_compat/compare.md#BehaviorDifference.details), [`platform_a_value`](../../../tree_sitter_analyzer/platform_compat/compare.md#BehaviorDifference.platform_a_value)

### `TestCompareProfilesIdentical`
- def: [`tests/unit/platform_compat/test_compare.py:92`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/platform_compat/test_compare.py#L92)
- signature: `class TestCompareProfilesIdentical:`
- members:
  - `test_identical_platform_keys_in_result(self)` — [`L100`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/platform_compat/test_compare.py#L100)
  - `test_identical_profiles_no_differences(self)` — [`L93`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/platform_compat/test_compare.py#L93)
- uses (calls/refs, reference-scoped): [`compare_profiles`](../../../tree_sitter_analyzer/platform_compat/compare.md#compare_profiles), [`has_differences`](../../../tree_sitter_analyzer/platform_compat/compare.md#ProfileComparison.has_differences), [`platform_a`](../../../tree_sitter_analyzer/platform_compat/compare.md#ProfileComparison.platform_a), [`platform_b`](../../../tree_sitter_analyzer/platform_compat/compare.md#ProfileComparison.platform_b)  (2 test-only)

### `TestCompareProfilesMismatch`
- def: [`tests/unit/platform_compat/test_compare.py:132`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/platform_compat/test_compare.py#L132)
- signature: `class TestCompareProfilesMismatch:`
- members:
  - `test_attribute_mismatch(self)` — [`L145`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/platform_compat/test_compare.py#L145)
  - `test_count_mismatch(self)` — [`L139`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/platform_compat/test_compare.py#L139)
  - `test_error_mismatch(self)` — [`L133`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/platform_compat/test_compare.py#L133)
  - `test_no_diff_when_same_attributes(self)` — [`L151`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/platform_compat/test_compare.py#L151)
- uses (calls/refs, reference-scoped): [`compare_profiles`](../../../tree_sitter_analyzer/platform_compat/compare.md#compare_profiles), [`diff_type`](../../../tree_sitter_analyzer/platform_compat/compare.md#BehaviorDifference.diff_type), [`differences`](../../../tree_sitter_analyzer/platform_compat/compare.md#ProfileComparison.differences), [`has_differences`](../../../tree_sitter_analyzer/platform_compat/compare.md#ProfileComparison.has_differences)  (2 test-only)

### `TestCompareProfilesMissing`
- def: [`tests/unit/platform_compat/test_compare.py:108`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/platform_compat/test_compare.py#L108)
- signature: `class TestCompareProfilesMissing:`
- members:
  - `test_construct_in_a_missing_in_b(self)` — [`L109`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/platform_compat/test_compare.py#L109)
  - `test_construct_in_b_missing_in_a(self)` — [`L120`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/platform_compat/test_compare.py#L120)
- uses (calls/refs, reference-scoped): [`compare_profiles`](../../../tree_sitter_analyzer/platform_compat/compare.md#compare_profiles), [`diff_type`](../../../tree_sitter_analyzer/platform_compat/compare.md#BehaviorDifference.diff_type), [`differences`](../../../tree_sitter_analyzer/platform_compat/compare.md#ProfileComparison.differences), [`has_differences`](../../../tree_sitter_analyzer/platform_compat/compare.md#ProfileComparison.has_differences), [`platform_b_value`](../../../tree_sitter_analyzer/platform_compat/compare.md#BehaviorDifference.platform_b_value), [`platform_a_value`](../../../tree_sitter_analyzer/platform_compat/compare.md#BehaviorDifference.platform_a_value)  (2 test-only)

### `TestGenerateDiffReport`
- def: [`tests/unit/platform_compat/test_compare.py:157`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/platform_compat/test_compare.py#L157)
- signature: `class TestGenerateDiffReport:`
- members:
  - `test_multiple_differences(self)` — [`L179`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/platform_compat/test_compare.py#L179)
  - `test_no_differences(self)` — [`L158`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/platform_compat/test_compare.py#L158)
  - `test_with_differences(self)` — [`L165`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/platform_compat/test_compare.py#L165)
- uses (calls/refs, reference-scoped): [`generate_diff_report`](../../../tree_sitter_analyzer/platform_compat/compare.md#generate_diff_report), [`diff_type`](../../../tree_sitter_analyzer/platform_compat/compare.md#BehaviorDifference.diff_type), [`BehaviorDifference`](../../../tree_sitter_analyzer/platform_compat/compare.md#BehaviorDifference), [`construct_id`](../../../tree_sitter_analyzer/platform_compat/compare.md#BehaviorDifference.construct_id), [`platform_b_value`](../../../tree_sitter_analyzer/platform_compat/compare.md#BehaviorDifference.platform_b_value), [`ProfileComparison`](../../../tree_sitter_analyzer/platform_compat/compare.md#ProfileComparison), [`details`](../../../tree_sitter_analyzer/platform_compat/compare.md#BehaviorDifference.details), [`platform_a_value`](../../../tree_sitter_analyzer/platform_compat/compare.md#BehaviorDifference.platform_a_value)

### `TestProfileComparison`
- def: [`tests/unit/platform_compat/test_compare.py:67`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/platform_compat/test_compare.py#L67)
- signature: `class TestProfileComparison:`
- members:
  - `test_has_differences_false_when_empty(self)` — [`L68`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/platform_compat/test_compare.py#L68)
  - `test_has_differences_true(self)` — [`L76`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/platform_compat/test_compare.py#L76)
- uses (calls/refs, reference-scoped): [`diff_type`](../../../tree_sitter_analyzer/platform_compat/compare.md#BehaviorDifference.diff_type), [`differences`](../../../tree_sitter_analyzer/platform_compat/compare.md#ProfileComparison.differences), [`has_differences`](../../../tree_sitter_analyzer/platform_compat/compare.md#ProfileComparison.has_differences), [`BehaviorDifference`](../../../tree_sitter_analyzer/platform_compat/compare.md#BehaviorDifference), [`construct_id`](../../../tree_sitter_analyzer/platform_compat/compare.md#BehaviorDifference.construct_id), [`platform_b_value`](../../../tree_sitter_analyzer/platform_compat/compare.md#BehaviorDifference.platform_b_value), [`ProfileComparison`](../../../tree_sitter_analyzer/platform_compat/compare.md#ProfileComparison), [`details`](../../../tree_sitter_analyzer/platform_compat/compare.md#BehaviorDifference.details), [`platform_a_value`](../../../tree_sitter_analyzer/platform_compat/compare.md#BehaviorDifference.platform_a_value), [`platform_a`](../../../tree_sitter_analyzer/platform_compat/compare.md#ProfileComparison.platform_a), [`platform_b`](../../../tree_sitter_analyzer/platform_compat/compare.md#ProfileComparison.platform_b)

## Functions
- `_behavior(construct_id: str = "sel_all", node_type: str = "select_statement", element_count: int = 1, attributes: list[str] | None = None, has_error: bool = False)` — [`L15`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/platform_compat/test_compare.py#L15)
- `_profile(platform_key: str = "linux-3.12", behaviors: dict[str, ParsingBehavior] | None = None)` — [`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/platform_compat/test_compare.py#L31)

