---
title: 'Module: tests/test_file_slice.py'
type: catalog
provenance: extracted
module: tests/test_file_slice.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_file_slice`/
symbols:
  test_expand_oversized_markdown_is_sliced_with_full_coverage: test_expand_oversized_markdown_is_sliced_with_full_coverage().
  test_unit_path_resolves_slice_and_path: test_unit_path_resolves_slice_and_path().
  test_read_files_keys_every_slice_to_parent_path: test_read_files_keys_every_slice_to_parent_path().
  test_bisect_slice_splits_at_newline: test_bisect_slice_splits_at_newline().
  test_pack_chunks_handles_slices: test_pack_chunks_handles_slices().
  _write: _write().
  test_expand_does_not_slice_code_even_when_oversized: test_expand_does_not_slice_code_even_when_oversized().
  test_estimate_tokens_for_slice_scales_with_range: test_estimate_tokens_for_slice_scales_with_range().
  test_bisect_slice_returns_none_for_tiny: test_bisect_slice_returns_none_for_tiny().
  test_expand_small_file_stays_whole: test_expand_small_file_stays_whole().
  test_partition_keeps_slices_as_text: test_partition_keeps_slices_as_text().
  test_slice_boundaries_small_text_is_one_range: test_slice_boundaries_small_text_is_one_range().
  test_slice_boundaries_full_coverage_and_bounds: test_slice_boundaries_full_coverage_and_bounds().
  test_slice_boundaries_single_huge_line_still_progresses: test_slice_boundaries_single_huge_line_still_progresses().
  test_slice_boundaries_prefers_heading_boundary: test_slice_boundaries_prefers_heading_boundary().
  test_expand_unreadable_file_passes_through: test_expand_unreadable_file_passes_through().
---
# Module: [`tests/test_file_slice.py`](../../../../../raw/code/graphify/tests/test_file_slice.py)

## Functions
- `_write(p: Path, text: str)` — [`L61`](../../../../../raw/code/graphify/tests/test_file_slice.py#L61)
- `test_bisect_slice_returns_none_for_tiny(tmp_path)` — [`L163`](../../../../../raw/code/graphify/tests/test_file_slice.py#L163) — documented in [graphify-file_slice](../../concepts/graphify-file_slice.md)
- `test_bisect_slice_splits_at_newline(tmp_path)` — [`L152`](../../../../../raw/code/graphify/tests/test_file_slice.py#L152) — documented in [graphify-file_slice](../../concepts/graphify-file_slice.md)
- `test_estimate_tokens_for_slice_scales_with_range(tmp_path)` — [`L124`](../../../../../raw/code/graphify/tests/test_file_slice.py#L124) — documented in [graphify-file_slice](../../concepts/graphify-file_slice.md)
- `test_expand_does_not_slice_code_even_when_oversized(tmp_path)` — [`L87`](../../../../../raw/code/graphify/tests/test_file_slice.py#L87) — documented in [graphify-file_slice](../../concepts/graphify-file_slice.md)
- `test_expand_oversized_markdown_is_sliced_with_full_coverage(tmp_path)` — [`L72`](../../../../../raw/code/graphify/tests/test_file_slice.py#L72) — documented in [graphify-file_slice](../../concepts/graphify-file_slice.md)
- `test_expand_small_file_stays_whole(tmp_path)` — [`L66`](../../../../../raw/code/graphify/tests/test_file_slice.py#L66) — documented in [graphify-file_slice](../../concepts/graphify-file_slice.md)
- `test_expand_unreadable_file_passes_through(tmp_path)` — [`L94`](../../../../../raw/code/graphify/tests/test_file_slice.py#L94) — documented in [graphify-file_slice](../../concepts/graphify-file_slice.md)
- `test_pack_chunks_handles_slices(tmp_path)` — [`L140`](../../../../../raw/code/graphify/tests/test_file_slice.py#L140) — documented in [graphify-file_slice](../../concepts/graphify-file_slice.md)
- `test_partition_keeps_slices_as_text(tmp_path)` — [`L131`](../../../../../raw/code/graphify/tests/test_file_slice.py#L131) — documented in [graphify-file_slice](../../concepts/graphify-file_slice.md)
- `test_read_files_keys_every_slice_to_parent_path(tmp_path)` — [`L102`](../../../../../raw/code/graphify/tests/test_file_slice.py#L102) — documented in [graphify-file_slice](../../concepts/graphify-file_slice.md)
- `test_slice_boundaries_full_coverage_and_bounds(max_chars)` — [`L27`](../../../../../raw/code/graphify/tests/test_file_slice.py#L27)
- `test_slice_boundaries_prefers_heading_boundary()` — [`L49`](../../../../../raw/code/graphify/tests/test_file_slice.py#L49)
- `test_slice_boundaries_single_huge_line_still_progresses()` — [`L41`](../../../../../raw/code/graphify/tests/test_file_slice.py#L41)
- `test_slice_boundaries_small_text_is_one_range()` — [`L21`](../../../../../raw/code/graphify/tests/test_file_slice.py#L21)
- `test_unit_path_resolves_slice_and_path(tmp_path)` — [`L117`](../../../../../raw/code/graphify/tests/test_file_slice.py#L117) — documented in [graphify-file_slice](../../concepts/graphify-file_slice.md)

