---
title: 'Module: tests/unit/test_check_loose_assertions.py'
type: catalog
provenance: extracted
module: tests/unit/test_check_loose_assertions.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_check_loose_assertions`/
symbols:
  _git: _git().
  _checker: _checker.
  _violations_in_source: _violations_in_source().
  _loader: _loader.
  _make_repo: _make_repo().
  _spec: _spec.
  test_preexisting_loose_assert_not_flagged_on_unrelated_edit: test_preexisting_loose_assert_not_flagged_on_unrelated_edit().
  test_added_loose_assert_is_flagged: test_added_loose_assert_is_flagged().
  test_added_placeholder_assert_is_flagged: test_added_placeholder_assert_is_flagged().
  test_added_tautology_assert_is_flagged: test_added_tautology_assert_is_flagged().
  test_staged_placeholder_assert_is_flagged: test_staged_placeholder_assert_is_flagged().
  test_renamed_file_with_added_loose_assert_is_flagged: test_renamed_file_with_added_loose_assert_is_flagged().
  test_multiline_assert_partially_touched_is_flagged: test_multiline_assert_partially_touched_is_flagged().
  _SCRIPT_PATH: _SCRIPT_PATH.
  test_baseline_count_format_remains_plain_number: test_baseline_count_format_remains_plain_number().
  test_git_diff_output_is_decoded_as_utf8: test_git_diff_output_is_decoded_as_utf8().
  test_git_diff_output_is_decoded_as_utf8.fake_run: test_git_diff_output_is_decoded_as_utf8().fake_run().
  test_multiline_assert_gte_is_caught: test_multiline_assert_gte_is_caught().
  test_inline_assert_gte_is_caught: test_inline_assert_gte_is_caught().
  test_inline_assert_gt_zero_is_caught: test_inline_assert_gt_zero_is_caught().
  test_len_gte_is_caught: test_len_gte_is_caught().
  test_exemption_marker_on_same_line_exempts: test_exemption_marker_on_same_line_exempts().
  test_exemption_marker_on_closing_paren_of_multiline_exempts: test_exemption_marker_on_closing_paren_of_multiline_exempts().
  test_exact_equality_assert_not_flagged: test_exact_equality_assert_not_flagged().
  test_string_literal_gte_not_flagged: test_string_literal_gte_not_flagged().
  test_unpaired_result_is_not_none_placeholder_is_caught: test_unpaired_result_is_not_none_placeholder_is_caught().
  test_result_is_not_none_placeholder_paired_with_behavior_is_allowed: test_result_is_not_none_placeholder_paired_with_behavior_is_allowed().
  test_none_check_tautology_is_caught: test_none_check_tautology_is_caught().
  test_clean_file_returns_no_violations: test_clean_file_returns_no_violations().
  test_baseline_counter_counts_violations: test_baseline_counter_counts_violations().
  test_baseline_json_format_uses_repo_relative_paths: test_baseline_json_format_uses_repo_relative_paths().
  test_baseline_json_includes_placeholder_metadata: test_baseline_json_includes_placeholder_metadata().
  test_baseline_table_format_includes_total_and_top_paths: test_baseline_table_format_includes_total_and_top_paths().
  test_property_file_skipped_in_baseline: test_property_file_skipped_in_baseline().
  test_multiple_violations_in_one_file: test_multiple_violations_in_one_file().
  _PROJECT_ROOT: _PROJECT_ROOT.
  test_git_diff_output_is_decoded_as_utf8.Result: test_git_diff_output_is_decoded_as_utf8().Result#
  test_git_diff_output_is_decoded_as_utf8.Result.stdout: test_git_diff_output_is_decoded_as_utf8().Result#stdout.
---
# Module: [`tests/unit/test_check_loose_assertions.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_check_loose_assertions.py)

## Classes
### `Result`
- def: [`tests/unit/test_check_loose_assertions.py:511`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_check_loose_assertions.py#L511)
- signature: `class Result:`
- members:
  - `stdout` — [`L512`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_check_loose_assertions.py#L512)
- used by: (1 test-only callers)

## Functions
- `_git(repo: Path, *args: str)` — [`L377`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_check_loose_assertions.py#L377)
- `_make_repo(tmp_path: Path)` — [`L389`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_check_loose_assertions.py#L389)
- `_violations_in_source(source: str)` — [`L57`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_check_loose_assertions.py#L57) — Parse *source* as a synthetic test file and return violations.
- `fake_run(*args, **kwargs)` — [`L519`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_check_loose_assertions.py#L519)
- `test_added_loose_assert_is_flagged(tmp_path: Path, monkeypatch)` — [`L431`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_check_loose_assertions.py#L431)
- `test_added_placeholder_assert_is_flagged(tmp_path: Path, monkeypatch)` — [`L451`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_check_loose_assertions.py#L451)
- `test_added_tautology_assert_is_flagged(tmp_path: Path, monkeypatch)` — [`L471`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_check_loose_assertions.py#L471)
- `test_baseline_count_format_remains_plain_number(tmp_path: Path, monkeypatch, capsys)` — [`L324`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_check_loose_assertions.py#L324)
- `test_baseline_counter_counts_violations(tmp_path: Path)` — [`L225`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_check_loose_assertions.py#L225) — count_baseline should return the exact number of loose asserts.
- `test_baseline_json_format_uses_repo_relative_paths(tmp_path: Path)` — [`L248`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_check_loose_assertions.py#L248)
- `test_baseline_json_includes_placeholder_metadata(tmp_path: Path)` — [`L275`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_check_loose_assertions.py#L275)
- `test_baseline_table_format_includes_total_and_top_paths(tmp_path: Path)` — [`L302`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_check_loose_assertions.py#L302)
- `test_clean_file_returns_no_violations(tmp_path: Path)` — [`L210`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_check_loose_assertions.py#L210)
- `test_exact_equality_assert_not_flagged()` — [`L148`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_check_loose_assertions.py#L148) — assert x == N is an exact assertion — must never be flagged.
- `test_exemption_marker_on_closing_paren_of_multiline_exempts()` — [`L134`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_check_loose_assertions.py#L134) — Marker on the closing line of a multiline assert should also exempt.
- `test_exemption_marker_on_same_line_exempts()` — [`L123`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_check_loose_assertions.py#L123) — # ratchet: nondeterministic on the assert line should suppress it.
- `test_git_diff_output_is_decoded_as_utf8(monkeypatch)` — [`L508`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_check_loose_assertions.py#L508)
- `test_inline_assert_gt_zero_is_caught()` — [`L103`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_check_loose_assertions.py#L103)
- `test_inline_assert_gte_is_caught()` — [`L93`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_check_loose_assertions.py#L93)
- `test_len_gte_is_caught()` — [`L113`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_check_loose_assertions.py#L113)
- `test_multiline_assert_gte_is_caught()` — [`L79`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_check_loose_assertions.py#L79) — Multiline assert with >= should be flagged — the primary blind spot.
- `test_multiline_assert_partially_touched_is_flagged(tmp_path: Path, monkeypatch)` — [`L558`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_check_loose_assertions.py#L558) — Editing any line of an existing multiline loose assert re-flags it —
- `test_multiple_violations_in_one_file()` — [`L357`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_check_loose_assertions.py#L357)
- `test_none_check_tautology_is_caught()` — [`L196`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_check_loose_assertions.py#L196)
- `test_preexisting_loose_assert_not_flagged_on_unrelated_edit(tmp_path: Path, monkeypatch)` — [`L404`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_check_loose_assertions.py#L404) — Codex P1: touching a file must not re-flag its baseline asserts.
- `test_property_file_skipped_in_baseline(tmp_path: Path)` — [`L345`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_check_loose_assertions.py#L345) — Files matching *propert* (case-insensitive) should be skipped.
- `test_renamed_file_with_added_loose_assert_is_flagged(tmp_path: Path, monkeypatch)` — [`L533`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_check_loose_assertions.py#L533) — Codex P2: --diff-filter must include renames (new path scanned).
- `test_result_is_not_none_placeholder_paired_with_behavior_is_allowed()` — [`L183`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_check_loose_assertions.py#L183)
- `test_staged_placeholder_assert_is_flagged(tmp_path: Path, monkeypatch)` — [`L491`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_check_loose_assertions.py#L491)
- `test_string_literal_gte_not_flagged()` — [`L159`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_check_loose_assertions.py#L159) — A '>=' inside a string literal is not a loose comparison.
- `test_unpaired_result_is_not_none_placeholder_is_caught()` — [`L169`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_check_loose_assertions.py#L169)

## Module values
- `_PROJECT_ROOT` — [`L38`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_check_loose_assertions.py#L38)
- `_SCRIPT_PATH` — [`L39`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_check_loose_assertions.py#L39)
- `_checker` — [`L43`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_check_loose_assertions.py#L43)
- `_loader` — [`L44`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_check_loose_assertions.py#L44)
- `_spec` — [`L41`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_check_loose_assertions.py#L41)

