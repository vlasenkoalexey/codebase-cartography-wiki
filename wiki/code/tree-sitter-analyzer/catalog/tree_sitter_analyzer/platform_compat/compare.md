---
title: 'Module: tree_sitter_analyzer/platform_compat/compare.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/platform_compat/compare.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.platform_compat.compare`/
symbols:
  compare_profiles: compare_profiles().
  generate_diff_report: generate_diff_report().
  BehaviorDifference.diff_type: BehaviorDifference#diff_type.
  ProfileComparison.differences: ProfileComparison#differences.
  load_profile_from_file: load_profile_from_file().
  ProfileComparison.has_differences: ProfileComparison#has_differences().
  BehaviorDifference: BehaviorDifference#
  BehaviorDifference.construct_id: BehaviorDifference#construct_id.
  _missing_diff: _missing_diff().
  _diff_common_behavior: _diff_common_behavior().
  report: report.
  BehaviorDifference.platform_b_value: BehaviorDifference#platform_b_value.
  BehaviorDifference.details: BehaviorDifference#details.
  BehaviorDifference.platform_a_value: BehaviorDifference#platform_a_value.
  ProfileComparison: ProfileComparison#
  path_b: path_b.
  comparison: comparison.
  ProfileComparison.platform_a: ProfileComparison#platform_a.
  ProfileComparison.platform_b: ProfileComparison#platform_b.
  parser: parser.
  profile_a: profile_a.
  profile_b: profile_b.
  args: args.
  path_a: path_a.
  e: e.
---
# Module: [`tree_sitter_analyzer/platform_compat/compare.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/compare.py)

## Classes
### `BehaviorDifference`
- def: [`tree_sitter_analyzer/platform_compat/compare.py:15`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/compare.py#L15)
- doc: Represents a difference in behavior for a specific construct.
- signature: `class BehaviorDifference:`
- members:
  - `construct_id` — [`L18`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/compare.py#L18)
  - `details` — [`L22`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/compare.py#L22)
  - `diff_type` — [`L19`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/compare.py#L19)
  - `platform_a_value` — [`L23`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/compare.py#L23)
  - `platform_b_value` — [`L24`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/compare.py#L24)
- used by: [`compare_profiles`](compare.md#compare_profiles), [`generate_diff_report`](compare.md#generate_diff_report), [`differences`](compare.md#ProfileComparison.differences), [`_missing_diff`](compare.md#_missing_diff), [`_diff_common_behavior`](compare.md#_diff_common_behavior)  (21 test-only)

### `ProfileComparison`
- def: [`tree_sitter_analyzer/platform_compat/compare.py:28`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/compare.py#L28)
- doc: Result of comparing two profiles.
- signature: `class ProfileComparison:`
- members:
  - `has_differences(self)` — [`L36`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/compare.py#L36)
  - `differences` — [`L33`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/compare.py#L33)
  - `platform_a` — [`L31`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/compare.py#L31)
  - `platform_b` — [`L32`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/compare.py#L32)
- uses (calls/refs, reference-scoped): [`BehaviorDifference`](compare.md#BehaviorDifference)
- used by: [`compare_profiles`](compare.md#compare_profiles), [`generate_diff_report`](compare.md#generate_diff_report), [`report`](compare.md#report)  (26 test-only)

## Functions
- `_diff_common_behavior(key: str, beh_a: Any, beh_b: Any, differences: list[BehaviorDifference])` — [`L64`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/compare.py#L64) — Append error / count / attribute differences for a single shared construct.
- `_missing_diff(key: str, missing_platform: str, side: str)` — [`L40`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/compare.py#L40) — Build a ``diff_type="missing"`` ``BehaviorDifference``.
- `compare_profiles(profile_a: BehaviorProfile, profile_b: BehaviorProfile)` — [`L113`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/compare.py#L113) — Compares two behavior profiles and identifies differences.
- `generate_diff_report(comparison: ProfileComparison)` — [`L151`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/compare.py#L151) — Generates a human-readable report of the differences.
- `load_profile_from_file(path: Path)` — [`L214`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/compare.py#L214)

## Module values
- `args` — [`L196`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/compare.py#L196)
- `comparison` — [`L240`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/compare.py#L240)
- `e` — [`L247`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/compare.py#L247)
- `parser` — [`L187`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/compare.py#L187)
- `path_a` — [`L199`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/compare.py#L199)
- `path_b` — [`L200`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/compare.py#L200)
- `profile_a` — [`L237`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/compare.py#L237)
- `profile_b` — [`L238`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/compare.py#L238)
- `report` — [`L241`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/compare.py#L241)

