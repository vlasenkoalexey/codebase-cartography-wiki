---
title: 'Module: tests/unit/test_rename_symbol_pure.py'
type: catalog
provenance: extracted
module: tests/unit/test_rename_symbol_pure.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_rename_symbol_pure`/
symbols:
  TestRenameResultToDict.test_to_dict_includes_sites: TestRenameResultToDict#test_to_dict_includes_sites().
  TestDeduplicateSites._make_site: TestDeduplicateSites#_make_site().
  TestGroupSitesByFile._make_site: TestGroupSitesByFile#_make_site().
  TestRenameSymbol.test_dry_run_no_sites_returns_empty_result: TestRenameSymbol#test_dry_run_no_sites_returns_empty_result().
  TestRenameSiteToDict.test_to_dict_returns_all_fields: TestRenameSiteToDict#test_to_dict_returns_all_fields().
  TestDeduplicateSites.test_preserves_order_first_wins: TestDeduplicateSites#test_preserves_order_first_wins().
  TestApplyRenameToFile.test_simple_rename: TestApplyRenameToFile#test_simple_rename().
  TestApplyRenameToFile.test_missing_file_returns_false: TestApplyRenameToFile#test_missing_file_returns_false().
  TestApplyRenameToFile.test_word_boundary_respected: TestApplyRenameToFile#test_word_boundary_respected().
  TestApplyRenameToFile.test_line_zero_site_scans_for_name: TestApplyRenameToFile#test_line_zero_site_scans_for_name().
  TestApplyRenameToFile.test_site_with_negative_column_triggers_fallback: TestApplyRenameToFile#test_site_with_negative_column_triggers_fallback().
  TestApplyRenameToFile.test_out_of_range_line_skipped: TestApplyRenameToFile#test_out_of_range_line_skipped().
  TestApplyRenameToFile.test_col_beyond_line_length_not_renamed: TestApplyRenameToFile#test_col_beyond_line_length_not_renamed().
  TestApplyRenameToFile.test_candidate_mismatch_not_renamed: TestApplyRenameToFile#test_candidate_mismatch_not_renamed().
  TestApplyRenameToFile.test_write_failure_returns_false: TestApplyRenameToFile#test_write_failure_returns_false().
  TestRenameResultToDict.test_to_dict_empty_sites: TestRenameResultToDict#test_to_dict_empty_sites().
  TestCollectRenameSitesFromResolver.test_definition_collected: TestCollectRenameSitesFromResolver#test_definition_collected().
  TestCollectRenameSitesFromResolver.test_reference_line_zero_added_with_zero_coords: TestCollectRenameSitesFromResolver#test_reference_line_zero_added_with_zero_coords().
  TestRenameSymbol.test_dry_run_with_sites_does_not_write: TestRenameSymbol#test_dry_run_with_sites_does_not_write().
  TestCollectRenameSitesFromResolver._make_resolve: TestCollectRenameSitesFromResolver#_make_resolve().
  TestCollectRenameSitesFromResolver.test_reference_collected: TestCollectRenameSitesFromResolver#test_reference_collected().
  TestRenameSymbol.test_live_rename_writes_file: TestRenameSymbol#test_live_rename_writes_file().
  TestRenameSymbol.test_live_rename_rollback_on_write_error: TestRenameSymbol#test_live_rename_rollback_on_write_error().
  TestCollectRenameSitesFromResolver.test_missing_file_skipped: TestCollectRenameSitesFromResolver#test_missing_file_skipped().
  TestCollectRenameSitesFromResolver.test_definition_ioerror_skipped: TestCollectRenameSitesFromResolver#test_definition_ioerror_skipped().
  TestCollectRenameSitesFromResolver.test_reference_ioerror_skipped: TestCollectRenameSitesFromResolver#test_reference_ioerror_skipped().
  TestCollectRenameSitesFromResolver.test_definition_line_out_of_range: TestCollectRenameSitesFromResolver#test_definition_line_out_of_range().
  TestCollectRenameSitesFromResolver.test_reference_line_out_of_range: TestCollectRenameSitesFromResolver#test_reference_line_out_of_range().
  TestCollectRenameSitesFromResolver.test_missing_reference_file_skipped: TestCollectRenameSitesFromResolver#test_missing_reference_file_skipped().
  TestDeduplicateSites.test_no_duplicates: TestDeduplicateSites#test_no_duplicates().
  TestDeduplicateSites.test_exact_duplicate_removed: TestDeduplicateSites#test_exact_duplicate_removed().
  TestDeduplicateSites.test_different_file_not_deduped: TestDeduplicateSites#test_different_file_not_deduped().
  TestGroupSitesByFile.test_single_file: TestGroupSitesByFile#test_single_file().
  TestGroupSitesByFile.test_multiple_files: TestGroupSitesByFile#test_multiple_files().
  TestCollectRenameSitesFromResolver._make_ref: TestCollectRenameSitesFromResolver#_make_ref().
  TestCollectRenameSitesFromResolver.test_empty_resolve_result: TestCollectRenameSitesFromResolver#test_empty_resolve_result().
  TestCollectRenameSitesFromResolver._make_defn: TestCollectRenameSitesFromResolver#_make_defn().
  _make_mock_cache: _make_mock_cache().
  _make_mock_resolver: _make_mock_resolver().
  TestIsWordBoundary.test_position_before_text: TestIsWordBoundary#test_position_before_text().
  TestIsWordBoundary.test_position_after_text: TestIsWordBoundary#test_position_after_text().
  TestIsWordBoundary.test_space_is_boundary: TestIsWordBoundary#test_space_is_boundary().
  TestIsWordBoundary.test_dot_is_boundary: TestIsWordBoundary#test_dot_is_boundary().
  TestIsWordBoundary.test_underscore_is_not_boundary: TestIsWordBoundary#test_underscore_is_not_boundary().
  TestIsWordBoundary.test_alpha_is_not_boundary: TestIsWordBoundary#test_alpha_is_not_boundary().
  TestIsWordBoundary.test_digit_is_not_boundary: TestIsWordBoundary#test_digit_is_not_boundary().
  TestScanLineForName.test_single_match: TestScanLineForName#test_single_match().
  TestScanLineForName.test_no_match: TestScanLineForName#test_no_match().
  TestScanLineForName.test_prefix_not_matched: TestScanLineForName#test_prefix_not_matched().
  TestScanLineForName.test_suffix_not_matched: TestScanLineForName#test_suffix_not_matched().
  TestScanLineForName.test_multiple_occurrences: TestScanLineForName#test_multiple_occurrences().
  TestScanLineForName.test_dot_access_counts_as_boundary: TestScanLineForName#test_dot_access_counts_as_boundary().
  TestScanLineForName.test_empty_line: TestScanLineForName#test_empty_line().
  TestFindIdentifierAtOrNear.test_exact_column: TestFindIdentifierAtOrNear#test_exact_column().
  TestFindIdentifierAtOrNear.test_near_column: TestFindIdentifierAtOrNear#test_near_column().
  TestFindIdentifierAtOrNear.test_not_found: TestFindIdentifierAtOrNear#test_not_found().
  TestFindIdentifierAtOrNear.test_prefix_not_matched: TestFindIdentifierAtOrNear#test_prefix_not_matched().
  TestDeduplicateSites.test_empty_input: TestDeduplicateSites#test_empty_input().
  TestGroupSitesByFile.test_empty: TestGroupSitesByFile#test_empty().
  TestApplyRenameToFile.test_no_sites_leaves_file_unchanged: TestApplyRenameToFile#test_no_sites_leaves_file_unchanged().
  TestRenameSiteToDict: TestRenameSiteToDict#
  TestRenameResultToDict: TestRenameResultToDict#
  TestIsWordBoundary: TestIsWordBoundary#
  TestScanLineForName: TestScanLineForName#
  TestFindIdentifierAtOrNear: TestFindIdentifierAtOrNear#
  TestDeduplicateSites: TestDeduplicateSites#
  TestGroupSitesByFile: TestGroupSitesByFile#
  TestApplyRenameToFile: TestApplyRenameToFile#
  TestCollectRenameSitesFromResolver: TestCollectRenameSitesFromResolver#
  TestRenameSymbol: TestRenameSymbol#
---
# Module: [`tests/unit/test_rename_symbol_pure.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rename_symbol_pure.py)

## Classes
### `TestApplyRenameToFile`
- def: [`tests/unit/test_rename_symbol_pure.py:232`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rename_symbol_pure.py#L232)
- signature: `class TestApplyRenameToFile:`
- members:
  - `test_candidate_mismatch_not_renamed(self, tmp_path)` — [`L320`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rename_symbol_pure.py#L320) — When text at given column doesn't match old_name, nothing is renamed.
  - `test_col_beyond_line_length_not_renamed(self, tmp_path)` — [`L310`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rename_symbol_pure.py#L310) — A column beyond the line length does not raise, just skips.
  - `test_line_zero_site_scans_for_name(self, tmp_path)` — [`L275`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rename_symbol_pure.py#L275) — A site with line=0 should fall back to scanning the first line.
  - `test_missing_file_returns_false(self, tmp_path)` — [`L248`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rename_symbol_pure.py#L248)
  - `test_no_sites_leaves_file_unchanged(self, tmp_path)` — [`L254`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rename_symbol_pure.py#L254)
  - `test_out_of_range_line_skipped(self, tmp_path)` — [`L298`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rename_symbol_pure.py#L298) — A site pointing to a line beyond file length is silently skipped.
  - `test_simple_rename(self, tmp_path)` — [`L233`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rename_symbol_pure.py#L233)
  - `test_site_with_negative_column_triggers_fallback(self, tmp_path)` — [`L287`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rename_symbol_pure.py#L287) — A site with column<0 on a real line triggers _scan_line_for_name fallback.
  - `test_word_boundary_respected(self, tmp_path)` — [`L261`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rename_symbol_pure.py#L261)
  - `test_write_failure_returns_false(self, tmp_path)` — [`L334`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rename_symbol_pure.py#L334) — OSError on write returns False.
- uses (calls/refs, reference-scoped): [`RenameSite`](../../tree_sitter_analyzer/rename_symbol.md#RenameSite), [`_apply_rename_to_file`](../../tree_sitter_analyzer/rename_symbol.md#_apply_rename_to_file), [`column`](../../tree_sitter_analyzer/rename_symbol.md#RenameSite.column), [`line`](../../tree_sitter_analyzer/rename_symbol.md#RenameSite.line), [`file`](../../tree_sitter_analyzer/rename_symbol.md#RenameSite.file), [`site_type`](../../tree_sitter_analyzer/rename_symbol.md#RenameSite.site_type), [`old_text`](../../tree_sitter_analyzer/rename_symbol.md#RenameSite.old_text)

### `TestCollectRenameSitesFromResolver`
- def: [`tests/unit/test_rename_symbol_pure.py:351`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rename_symbol_pure.py#L351)
- signature: `class TestCollectRenameSitesFromResolver:`
- members:
  - `test_definition_collected(self, tmp_path)` — [`L368`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rename_symbol_pure.py#L368)
  - `test_definition_ioerror_skipped(self, tmp_path)` — [`L402`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rename_symbol_pure.py#L402) — OSError when reading definition file is silently skipped.
  - `test_definition_line_out_of_range(self, tmp_path)` — [`L422`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rename_symbol_pure.py#L422) — Definition line beyond file length adds no sites.
  - `test_empty_resolve_result(self, tmp_path)` — [`L363`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rename_symbol_pure.py#L363)
  - `test_missing_file_skipped(self, tmp_path)` — [`L385`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rename_symbol_pure.py#L385)
  - `test_missing_reference_file_skipped(self, tmp_path)` — [`L440`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rename_symbol_pure.py#L440) — Non-existent reference file is silently skipped.
  - `test_reference_collected(self, tmp_path)` — [`L377`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rename_symbol_pure.py#L377)
  - `test_reference_ioerror_skipped(self, tmp_path)` — [`L412`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rename_symbol_pure.py#L412) — OSError when reading reference file is silently skipped.
  - `test_reference_line_out_of_range(self, tmp_path)` — [`L431`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rename_symbol_pure.py#L431) — Reference line beyond file length adds no sites.
  - `test_reference_line_zero_added_with_zero_coords(self, tmp_path)` — [`L391`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rename_symbol_pure.py#L391) — References with line=0 are added with line=0, col=0.
- protocol/private: `_make_defn`[`L357`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rename_symbol_pure.py#L357), `_make_ref`[`L360`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rename_symbol_pure.py#L360), `_make_resolve`[`L352`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rename_symbol_pure.py#L352)
- uses (calls/refs, reference-scoped): [`column`](../../tree_sitter_analyzer/rename_symbol.md#RenameSite.column), [`line`](../../tree_sitter_analyzer/rename_symbol.md#RenameSite.line), [`site_type`](../../tree_sitter_analyzer/rename_symbol.md#RenameSite.site_type), [`old_text`](../../tree_sitter_analyzer/rename_symbol.md#RenameSite.old_text), [`_collect_rename_sites_from_resolver`](../../tree_sitter_analyzer/rename_symbol.md#_collect_rename_sites_from_resolver)

### `TestDeduplicateSites`
- def: [`tests/unit/test_rename_symbol_pure.py:162`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rename_symbol_pure.py#L162)
- signature: `class TestDeduplicateSites:`
- members:
  - `test_different_file_not_deduped(self)` — [`L178`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rename_symbol_pure.py#L178)
  - `test_empty_input(self)` — [`L194`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rename_symbol_pure.py#L194)
  - `test_exact_duplicate_removed(self)` — [`L172`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rename_symbol_pure.py#L172)
  - `test_no_duplicates(self)` — [`L168`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rename_symbol_pure.py#L168)
  - `test_preserves_order_first_wins(self)` — [`L184`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rename_symbol_pure.py#L184)
- protocol/private: `_make_site`[`L163`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rename_symbol_pure.py#L163)
- uses (calls/refs, reference-scoped): [`RenameSite`](../../tree_sitter_analyzer/rename_symbol.md#RenameSite), [`column`](../../tree_sitter_analyzer/rename_symbol.md#RenameSite.column), [`line`](../../tree_sitter_analyzer/rename_symbol.md#RenameSite.line), [`file`](../../tree_sitter_analyzer/rename_symbol.md#RenameSite.file), [`site_type`](../../tree_sitter_analyzer/rename_symbol.md#RenameSite.site_type), [`old_text`](../../tree_sitter_analyzer/rename_symbol.md#RenameSite.old_text), [`_deduplicate_sites`](../../tree_sitter_analyzer/rename_symbol.md#_deduplicate_sites)

### `TestFindIdentifierAtOrNear`
- def: [`tests/unit/test_rename_symbol_pure.py:136`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rename_symbol_pure.py#L136)
- signature: `class TestFindIdentifierAtOrNear:`
- members:
  - `test_exact_column(self)` — [`L137`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rename_symbol_pure.py#L137)
  - `test_near_column(self)` — [`L142`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rename_symbol_pure.py#L142)
  - `test_not_found(self)` — [`L147`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rename_symbol_pure.py#L147)
  - `test_prefix_not_matched(self)` — [`L151`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rename_symbol_pure.py#L151)
- uses (calls/refs, reference-scoped): [`_find_identifier_at_or_near`](../../tree_sitter_analyzer/rename_symbol.md#_find_identifier_at_or_near)

### `TestGroupSitesByFile`
- def: [`tests/unit/test_rename_symbol_pure.py:203`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rename_symbol_pure.py#L203)
- signature: `class TestGroupSitesByFile:`
- members:
  - `test_empty(self)` — [`L223`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rename_symbol_pure.py#L223)
  - `test_multiple_files(self)` — [`L213`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rename_symbol_pure.py#L213)
  - `test_single_file(self)` — [`L207`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rename_symbol_pure.py#L207)
- protocol/private: `_make_site`[`L204`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rename_symbol_pure.py#L204)
- uses (calls/refs, reference-scoped): [`RenameSite`](../../tree_sitter_analyzer/rename_symbol.md#RenameSite), [`column`](../../tree_sitter_analyzer/rename_symbol.md#RenameSite.column), [`line`](../../tree_sitter_analyzer/rename_symbol.md#RenameSite.line), [`file`](../../tree_sitter_analyzer/rename_symbol.md#RenameSite.file), [`site_type`](../../tree_sitter_analyzer/rename_symbol.md#RenameSite.site_type), [`old_text`](../../tree_sitter_analyzer/rename_symbol.md#RenameSite.old_text), [`_group_sites_by_file`](../../tree_sitter_analyzer/rename_symbol.md#_group_sites_by_file)

### `TestIsWordBoundary`
- def: [`tests/unit/test_rename_symbol_pure.py:75`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rename_symbol_pure.py#L75)
- signature: `class TestIsWordBoundary:`
- members:
  - `test_alpha_is_not_boundary(self)` — [`L91`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rename_symbol_pure.py#L91)
  - `test_digit_is_not_boundary(self)` — [`L94`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rename_symbol_pure.py#L94)
  - `test_dot_is_boundary(self)` — [`L85`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rename_symbol_pure.py#L85)
  - `test_position_after_text(self)` — [`L79`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rename_symbol_pure.py#L79)
  - `test_position_before_text(self)` — [`L76`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rename_symbol_pure.py#L76)
  - `test_space_is_boundary(self)` — [`L82`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rename_symbol_pure.py#L82)
  - `test_underscore_is_not_boundary(self)` — [`L88`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rename_symbol_pure.py#L88)
- uses (calls/refs, reference-scoped): [`_is_word_boundary`](../../tree_sitter_analyzer/rename_symbol.md#_is_word_boundary)

### `TestRenameResultToDict`
- def: [`tests/unit/test_rename_symbol_pure.py:48`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rename_symbol_pure.py#L48)
- signature: `class TestRenameResultToDict:`
- members:
  - `test_to_dict_empty_sites(self)` — [`L61`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rename_symbol_pure.py#L61)
  - `test_to_dict_includes_sites(self)` — [`L49`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rename_symbol_pure.py#L49)
- uses (calls/refs, reference-scoped): [`RenameSite`](../../tree_sitter_analyzer/rename_symbol.md#RenameSite), [`column`](../../tree_sitter_analyzer/rename_symbol.md#RenameSite.column), [`line`](../../tree_sitter_analyzer/rename_symbol.md#RenameSite.line), [`file`](../../tree_sitter_analyzer/rename_symbol.md#RenameSite.file), [`site_type`](../../tree_sitter_analyzer/rename_symbol.md#RenameSite.site_type), [`to_dict`](../../tree_sitter_analyzer/rename_symbol.md#RenameResult.to_dict), [`old_text`](../../tree_sitter_analyzer/rename_symbol.md#RenameSite.old_text), [`sites`](../../tree_sitter_analyzer/rename_symbol.md#RenameResult.sites), [`RenameResult`](../../tree_sitter_analyzer/rename_symbol.md#RenameResult), [`dry_run`](../../tree_sitter_analyzer/rename_symbol.md#RenameResult.dry_run), [`new_name`](../../tree_sitter_analyzer/rename_symbol.md#RenameResult.new_name), [`symbol`](../../tree_sitter_analyzer/rename_symbol.md#RenameResult.symbol)

### `TestRenameSiteToDict`
- def: [`tests/unit/test_rename_symbol_pure.py:30`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rename_symbol_pure.py#L30)
- signature: `class TestRenameSiteToDict:`
- members:
  - `test_to_dict_returns_all_fields(self)` — [`L31`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rename_symbol_pure.py#L31)
- uses (calls/refs, reference-scoped): [`RenameSite`](../../tree_sitter_analyzer/rename_symbol.md#RenameSite), [`column`](../../tree_sitter_analyzer/rename_symbol.md#RenameSite.column), [`line`](../../tree_sitter_analyzer/rename_symbol.md#RenameSite.line), [`file`](../../tree_sitter_analyzer/rename_symbol.md#RenameSite.file), [`site_type`](../../tree_sitter_analyzer/rename_symbol.md#RenameSite.site_type), [`old_text`](../../tree_sitter_analyzer/rename_symbol.md#RenameSite.old_text), [`to_dict`](../../tree_sitter_analyzer/rename_symbol.md#RenameSite.to_dict)

### `TestRenameSymbol`
- def: [`tests/unit/test_rename_symbol_pure.py:468`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rename_symbol_pure.py#L468)
- signature: `class TestRenameSymbol:`
- members:
  - `test_dry_run_no_sites_returns_empty_result(self, tmp_path)` — [`L469`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rename_symbol_pure.py#L469)
  - `test_dry_run_with_sites_does_not_write(self, tmp_path)` — [`L482`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rename_symbol_pure.py#L482)
  - `test_live_rename_rollback_on_write_error(self, tmp_path)` — [`L510`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rename_symbol_pure.py#L510)
  - `test_live_rename_writes_file(self, tmp_path)` — [`L497`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rename_symbol_pure.py#L497)
- uses (calls/refs, reference-scoped): [`rename_symbol`](../../tree_sitter_analyzer/rename_symbol.md#rename_symbol), [`sites`](../../tree_sitter_analyzer/rename_symbol.md#RenameResult.sites), [`files_changed`](../../tree_sitter_analyzer/rename_symbol.md#RenameResult.files_changed), [`dry_run`](../../tree_sitter_analyzer/rename_symbol.md#RenameResult.dry_run), [`new_name`](../../tree_sitter_analyzer/rename_symbol.md#RenameResult.new_name), [`symbol`](../../tree_sitter_analyzer/rename_symbol.md#RenameResult.symbol), [`errors`](../../tree_sitter_analyzer/rename_symbol.md#RenameResult.errors)  (2 test-only)

### `TestScanLineForName`
- def: [`tests/unit/test_rename_symbol_pure.py:103`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rename_symbol_pure.py#L103)
- signature: `class TestScanLineForName:`
- members:
  - `test_dot_access_counts_as_boundary(self)` — [`L122`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rename_symbol_pure.py#L122)
  - `test_empty_line(self)` — [`L127`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rename_symbol_pure.py#L127)
  - `test_multiple_occurrences(self)` — [`L118`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rename_symbol_pure.py#L118)
  - `test_no_match(self)` — [`L108`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rename_symbol_pure.py#L108)
  - `test_prefix_not_matched(self)` — [`L111`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rename_symbol_pure.py#L111)
  - `test_single_match(self)` — [`L104`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rename_symbol_pure.py#L104)
  - `test_suffix_not_matched(self)` — [`L115`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rename_symbol_pure.py#L115)
- uses (calls/refs, reference-scoped): [`_scan_line_for_name`](../../tree_sitter_analyzer/rename_symbol.md#_scan_line_for_name)

## Functions
- `_make_mock_cache(project_root: str)` — [`L453`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rename_symbol_pure.py#L453)
- `_make_mock_resolver(definitions=(), references=())` — [`L459`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_rename_symbol_pure.py#L459)

