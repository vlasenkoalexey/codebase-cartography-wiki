---
title: 'Module: tests/test_cache.py'
type: catalog
provenance: extracted
module: tests/test_cache.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_cache`/
symbols:
  test_cache_portable_across_roots: test_cache_portable_across_roots().
  test_semantic_prune_removes_orphan_entries: test_semantic_prune_removes_orphan_entries().
  test_semantic_prune_keeps_live_unchanged_entries: test_semantic_prune_keeps_live_unchanged_entries().
  test_semantic_prune_handles_deleted_file: test_semantic_prune_handles_deleted_file().
  test_cached_files: test_cached_files().
  test_save_cached_relativizes_source_file: test_save_cached_relativizes_source_file().
  test_load_cached_passes_through_legacy_absolute_source_file: test_load_cached_passes_through_legacy_absolute_source_file().
  test_legacy_unversioned_ast_entries_not_served: test_legacy_unversioned_ast_entries_not_served().
  test_semantic_cache_survives_version_bump: test_semantic_cache_survives_version_bump().
  test_save_cached_in_root_symlink_keeps_symlink_name: test_save_cached_in_root_symlink_keeps_symlink_name().
  test_semantic_prune_ignores_ast_and_tmp: test_semantic_prune_ignores_ast_and_tmp().
  test_cache_roundtrip: test_cache_roundtrip().
  test_cache_miss_on_change: test_cache_miss_on_change().
  test_clear_cache: test_clear_cache().
  test_load_cached_absolutizes_source_file: test_load_cached_absolutizes_source_file().
  test_ast_cache_invalidated_on_version_bump: test_ast_cache_invalidated_on_version_bump().
  test_ast_cache_version_bump_cleans_stale_entries: test_ast_cache_version_bump_cleans_stale_entries().
  test_file_hash_consistent: test_file_hash_consistent().
  test_file_hash_changes: test_file_hash_changes().
  test_md_frontmatter_only_change_same_hash: test_md_frontmatter_only_change_same_hash().
  test_md_body_change_different_hash: test_md_body_change_different_hash().
  test_md_no_frontmatter_hashed_normally: test_md_no_frontmatter_hashed_normally().
  test_non_md_file_hashed_fully: test_non_md_file_hashed_fully().
  test_body_content_strips_frontmatter: test_body_content_strips_frontmatter().
  test_body_content_no_frontmatter: test_body_content_no_frontmatter().
  test_body_content_hr_start_is_not_frontmatter: test_body_content_hr_start_is_not_frontmatter().
  test_body_content_dash_title_start_is_not_frontmatter: test_body_content_dash_title_start_is_not_frontmatter().
  test_body_content_dash_text_line_is_not_close_delimiter: test_body_content_dash_text_line_is_not_close_delimiter().
  test_body_content_later_proper_close_skips_dash_text_lines: test_body_content_later_proper_close_skips_dash_text_lines().
  test_body_content_well_formed_output_byte_identical: test_body_content_well_formed_output_byte_identical().
  test_md_edit_above_hr_changes_hash: test_md_edit_above_hr_changes_hash().
  tmp_file: tmp_file().
  cache_root: cache_root().
---
# Module: [`tests/test_cache.py`](../../../../../raw/code/graphify/tests/test_cache.py)

## Functions
- `cache_root(tmp_path)` — [`L15`](../../../../../raw/code/graphify/tests/test_cache.py#L15)
- `test_ast_cache_invalidated_on_version_bump(tmp_path, monkeypatch)` — [`L310`](../../../../../raw/code/graphify/tests/test_cache.py#L310) — An AST entry written by version X must not be served after upgrading
- `test_ast_cache_version_bump_cleans_stale_entries(tmp_path, monkeypatch)` — [`L328`](../../../../../raw/code/graphify/tests/test_cache.py#L328) — Upgrading removes AST entries left behind by previous versions so the
- `test_body_content_dash_text_line_is_not_close_delimiter()` — [`L146`](../../../../../raw/code/graphify/tests/test_cache.py#L146) — ``--- text`` and ``----`` lines inside opened frontmatter are not the
- `test_body_content_dash_title_start_is_not_frontmatter()` — [`L140`](../../../../../raw/code/graphify/tests/test_cache.py#L140) — ``--- title`` on the first line is prose, not an open delimiter.
- `test_body_content_hr_start_is_not_frontmatter()` — [`L133`](../../../../../raw/code/graphify/tests/test_cache.py#L133) — A document opening with a ``----`` thematic break has no frontmatter;
- `test_body_content_later_proper_close_skips_dash_text_lines()` — [`L153`](../../../../../raw/code/graphify/tests/test_cache.py#L153) — A ``--- text`` line is skipped; the next whole ``---`` line closes.
- `test_body_content_no_frontmatter()` — [`L125`](../../../../../raw/code/graphify/tests/test_cache.py#L125) — _body_content returns content unchanged when no frontmatter present.
- `test_body_content_strips_frontmatter()` — [`L119`](../../../../../raw/code/graphify/tests/test_cache.py#L119) — _body_content correctly strips YAML frontmatter.
- `test_body_content_well_formed_output_byte_identical()` — [`L159`](../../../../../raw/code/graphify/tests/test_cache.py#L159) — For well-formed frontmatter the stripped body must stay byte-identical
- `test_cache_miss_on_change(tmp_file, cache_root)` — [`L45`](../../../../../raw/code/graphify/tests/test_cache.py#L45) — After file content changes, load_cached returns None.
- `test_cache_portable_across_roots(tmp_path)` — [`L270`](../../../../../raw/code/graphify/tests/test_cache.py#L270) — End-to-end portability: a cache entry written at one root can be
- `test_cache_roundtrip(tmp_file, cache_root)` — [`L37`](../../../../../raw/code/graphify/tests/test_cache.py#L37) — Save then load returns the same result dict.
- `test_cached_files(tmp_path, cache_root)` — [`L54`](../../../../../raw/code/graphify/tests/test_cache.py#L54) — cached_files returns the set of cached hashes.
- `test_clear_cache(tmp_file, cache_root)` — [`L69`](../../../../../raw/code/graphify/tests/test_cache.py#L69) — clear_cache removes all .json files from graphify-out/cache/ (all subdirs).
- `test_file_hash_changes(tmp_path)` — [`L28`](../../../../../raw/code/graphify/tests/test_cache.py#L28) — Different file contents give different hashes.
- `test_file_hash_consistent(tmp_file)` — [`L19`](../../../../../raw/code/graphify/tests/test_cache.py#L19) — Same file gives same hash on repeated calls.
- `test_legacy_unversioned_ast_entries_not_served(tmp_path)` — [`L349`](../../../../../raw/code/graphify/tests/test_cache.py#L349) — Entries written by pre-versioning graphify (flat cache/ or unversioned
- `test_load_cached_absolutizes_source_file(tmp_path)` — [`L224`](../../../../../raw/code/graphify/tests/test_cache.py#L224) — ``load_cached`` returns the same absolute-path shape that a fresh
- `test_load_cached_passes_through_legacy_absolute_source_file(tmp_path)` — [`L245`](../../../../../raw/code/graphify/tests/test_cache.py#L245) — Cache entries written by an older graphify (with absolute source_file
- `test_md_body_change_different_hash(tmp_path)` — [`L89`](../../../../../raw/code/graphify/tests/test_cache.py#L89) — Changing the body of a .md file produces a different hash.
- `test_md_edit_above_hr_changes_hash(tmp_path)` — [`L180`](../../../../../raw/code/graphify/tests/test_cache.py#L180) — Editing content above a mid-document ``----`` break must change the
- `test_md_frontmatter_only_change_same_hash(tmp_path)` — [`L79`](../../../../../raw/code/graphify/tests/test_cache.py#L79) — Changing only frontmatter fields in a .md file does not change the hash.
- `test_md_no_frontmatter_hashed_normally(tmp_path)` — [`L99`](../../../../../raw/code/graphify/tests/test_cache.py#L99) — A .md file with no frontmatter is hashed by its full content.
- `test_non_md_file_hashed_fully(tmp_path)` — [`L109`](../../../../../raw/code/graphify/tests/test_cache.py#L109) — Non-.md files are still hashed by their full content.
- `test_save_cached_in_root_symlink_keeps_symlink_name(tmp_path)` — [`L392`](../../../../../raw/code/graphify/tests/test_cache.py#L392) — ``source_file`` for an in-root symlink must be stored under the
- `test_save_cached_relativizes_source_file(tmp_path)` — [`L197`](../../../../../raw/code/graphify/tests/test_cache.py#L197) — The on-disk cache JSON contains forward-slash relative source_file
- `test_semantic_cache_survives_version_bump(tmp_path, monkeypatch)` — [`L371`](../../../../../raw/code/graphify/tests/test_cache.py#L371) — The semantic cache is deliberately not versioned: entries are produced
- `test_semantic_prune_handles_deleted_file(tmp_path)` — [`L471`](../../../../../raw/code/graphify/tests/test_cache.py#L471) — An entry for a file that no longer exists (dropped from the live set) is
- `test_semantic_prune_ignores_ast_and_tmp(tmp_path)` — [`L490`](../../../../../raw/code/graphify/tests/test_cache.py#L490) — Prune touches only cache/semantic/*.json: AST entries and atomic-write
- `test_semantic_prune_keeps_live_unchanged_entries(tmp_path)` — [`L450`](../../../../../raw/code/graphify/tests/test_cache.py#L450) — Pruning against the FULL live set must keep every live entry — guards
- `test_semantic_prune_removes_orphan_entries(tmp_path)` — [`L425`](../../../../../raw/code/graphify/tests/test_cache.py#L425) — Changing a file's content leaves the old content-hash entry orphaned;
- `tmp_file(tmp_path)` — [`L8`](../../../../../raw/code/graphify/tests/test_cache.py#L8)

