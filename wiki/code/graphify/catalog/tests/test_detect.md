---
title: 'Module: tests/test_detect.py'
type: catalog
provenance: extracted
module: tests/test_detect.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_detect`/
symbols:
  test_shebang_interpreter_env_unset_with_operand: test_shebang_interpreter_env_unset_with_operand().
  test_shebang_interpreter_env_chdir_with_operand: test_shebang_interpreter_env_chdir_with_operand().
  test_shebang_interpreter_env_path_with_operand: test_shebang_interpreter_env_path_with_operand().
  test_shebang_interpreter_env_dash_s_after_flag: test_shebang_interpreter_env_dash_s_after_flag().
  test_shebang_interpreter_env_clumped_u_operand: test_shebang_interpreter_env_clumped_u_operand().
  test_shebang_interpreter_env_gnu_split_string_equals: test_shebang_interpreter_env_gnu_split_string_equals().
  test_shebang_interpreter_env_gnu_split_string_separate: test_shebang_interpreter_env_gnu_split_string_separate().
  test_shebang_interpreter_env_gnu_argv0_operand: test_shebang_interpreter_env_gnu_argv0_operand().
  test_shebang_interpreter_env_compact_dash_s: test_shebang_interpreter_env_compact_dash_s().
  test_shebang_interpreter_env_compact_v_then_s: test_shebang_interpreter_env_compact_v_then_s().
  test_shebang_interpreter_env_long_unset_separate_operand: test_shebang_interpreter_env_long_unset_separate_operand().
  test_shebang_interpreter_env_long_unset_equals: test_shebang_interpreter_env_long_unset_equals().
  test_shebang_interpreter_env_long_chdir_separate_operand: test_shebang_interpreter_env_long_chdir_separate_operand().
  test_shebang_interpreter_env_long_chdir_equals: test_shebang_interpreter_env_long_chdir_equals().
  test_shebang_interpreter_env_signal_flags: test_shebang_interpreter_env_signal_flags().
  test_shebang_interpreter_env_dash_s_assignment_before_interpreter: test_shebang_interpreter_env_dash_s_assignment_before_interpreter().
  test_shebang_interpreter_env_dash_s_flag_before_interpreter: test_shebang_interpreter_env_dash_s_flag_before_interpreter().
  test_shebang_interpreter_env_long_split_assignment_before_interpreter: test_shebang_interpreter_env_long_split_assignment_before_interpreter().
  test_shebang_interpreter_env_long_split_flag_before_interpreter: test_shebang_interpreter_env_long_split_flag_before_interpreter().
  test_shebang_interpreter_env_vs_assignment_before_interpreter: test_shebang_interpreter_env_vs_assignment_before_interpreter().
  test_classify_python: test_classify_python().
  test_classify_typescript: test_classify_typescript().
  test_classify_powershell_module: test_classify_powershell_module().
  test_classify_powershell_manifest: test_classify_powershell_manifest().
  test_classify_markdown: test_classify_markdown().
  test_classify_pdf: test_classify_pdf().
  test_classify_image: test_classify_image().
  test_classify_md_paper_by_signals: test_classify_md_paper_by_signals().
  test_classify_md_doc_without_signals: test_classify_md_doc_without_signals().
  test_classify_attention_paper: test_classify_attention_paper().
  test_classify_video_extensions: test_classify_video_extensions().
  test_classify_google_workspace_shortcuts: test_classify_google_workspace_shortcuts().
  test_shebang_file_type_classifies_via_interpreter: test_shebang_file_type_classifies_via_interpreter().
  test_count_words_sample_md: test_count_words_sample_md().
  test_detect_finds_fixtures: test_detect_finds_fixtures().
  test_detect_warns_small_corpus: test_detect_warns_small_corpus().
  test_detect_skips_noise_dot_dirs: test_detect_skips_noise_dot_dirs().
  test_detect_incremental_propagates_follow_symlinks: test_detect_incremental_propagates_follow_symlinks().
  test_detect_converts_google_workspace_shortcuts_when_enabled: test_detect_converts_google_workspace_shortcuts_when_enabled().
  test_negation_cannot_rescue_file_under_excluded_dir: test_negation_cannot_rescue_file_under_excluded_dir().
  test_negation_works_when_no_ancestor_excluded: test_negation_works_when_no_ancestor_excluded().
  test_negation_ancestor_itself_reincluded: test_negation_ancestor_itself_reincluded().
  test_negation_does_not_disable_directory_pruning: test_negation_does_not_disable_directory_pruning().
  test_anchored_dir_not_matched_at_depth: test_anchored_dir_not_matched_at_depth().
  test_anchored_dir_matches_at_root: test_anchored_dir_matches_at_root().
  test_anchored_file_not_matched_at_depth: test_anchored_file_not_matched_at_depth().
  test_unanchored_dir_still_matches_at_depth: test_unanchored_dir_still_matches_at_depth().
  test_anchored_multi_segment_pattern: test_anchored_multi_segment_pattern().
  test_is_ignored_cache_matches_uncached_results: test_is_ignored_cache_matches_uncached_results().
  test_is_ignored_cache_evaluates_each_dir_once: test_is_ignored_cache_evaluates_each_dir_once().
  test_save_manifest_skips_semantic_hash_for_files_without_cache: test_save_manifest_skips_semantic_hash_for_files_without_cache().
  test_save_manifest_relativizes_keys_when_root_given: test_save_manifest_relativizes_keys_when_root_given().
  test_detect_incremental_portable_across_paths: test_detect_incremental_portable_across_paths().
  test_save_manifest_in_root_symlink_roundtrips: test_save_manifest_in_root_symlink_roundtrips().
  FIXTURES: FIXTURES.
  test_classify_pdf_in_xcassets_skipped: test_classify_pdf_in_xcassets_skipped().
  test_classify_pdf_in_xcassets_root_skipped: test_classify_pdf_in_xcassets_root_skipped().
  test_classify_unknown_returns_none: test_classify_unknown_returns_none().
  test_graphifyignore_excludes_file: test_graphifyignore_excludes_file().
  test_graphifyignore_missing_is_fine: test_graphifyignore_missing_is_fine().
  test_graphifyignore_comments_ignored: test_graphifyignore_comments_ignored().
  test_detect_follows_symlinked_directory: test_detect_follows_symlinked_directory().
  test_detect_follows_symlinked_file: test_detect_follows_symlinked_file().
  test_graphifyignore_hermetic_without_vcs: test_graphifyignore_hermetic_without_vcs().
  test_graphifyignore_discovered_from_parent_in_vcs: test_graphifyignore_discovered_from_parent_in_vcs().
  test_graphifyignore_stops_at_git_boundary: test_graphifyignore_stops_at_git_boundary().
  test_graphifyignore_at_git_root_is_included: test_graphifyignore_at_git_root_is_included().
  test_detect_handles_circular_symlinks: test_detect_handles_circular_symlinks().
  test_detect_default_does_not_auto_follow_direct_symlink_child: test_detect_default_does_not_auto_follow_direct_symlink_child().
  test_detect_default_does_not_follow_when_no_symlinks: test_detect_default_does_not_follow_when_no_symlinks().
  test_detect_explicit_false_overrides_auto_detect: test_detect_explicit_false_overrides_auto_detect().
  test_detect_skips_out_of_root_symlinked_directory_even_when_following: test_detect_skips_out_of_root_symlinked_directory_even_when_following().
  test_detect_skips_out_of_root_symlinked_file_by_default: test_detect_skips_out_of_root_symlinked_file_by_default().
  test_detect_incremental_survives_dict_valued_mtime: test_detect_incremental_survives_dict_valued_mtime().
  test_detect_skips_google_workspace_shortcuts_by_default: test_detect_skips_google_workspace_shortcuts_by_default().
  test_detect_includes_video_key: test_detect_includes_video_key().
  test_detect_finds_video_files: test_detect_finds_video_files().
  test_detect_video_not_in_words: test_detect_video_not_in_words().
  test_detect_skips_coverage_dir: test_detect_skips_coverage_dir().
  test_detect_skips_visual_tests_dir: test_detect_skips_visual_tests_dir().
  test_detect_skips_snapshots_dir: test_detect_skips_snapshots_dir().
  test_detect_skips_storybook_static_dir: test_detect_skips_storybook_static_dir().
  test_detect_allows_github_dir: test_detect_allows_github_dir().
  test_detect_skips_next_cache: test_detect_skips_next_cache().
  test_detect_skips_graphify_own_cache: test_detect_skips_graphify_own_cache().
  test_sensitive_flags_api_token_txt: test_sensitive_flags_api_token_txt().
  test_sensitive_flags_oauth_token_json: test_sensitive_flags_oauth_token_json().
  test_sensitive_flags_underscore_secret: test_sensitive_flags_underscore_secret().
  test_sensitive_does_not_flag_tokenizer_py: test_sensitive_does_not_flag_tokenizer_py().
  test_sensitive_does_not_flag_tokenize_py: test_sensitive_does_not_flag_tokenize_py().
  test_sensitive_flags_passwords_py: test_sensitive_flags_passwords_py().
  test_sensitive_flags_ssh_dir: test_sensitive_flags_ssh_dir().
  test_sensitive_flags_secrets_dir: test_sensitive_flags_secrets_dir().
  test_sensitive_flags_token_txt: test_sensitive_flags_token_txt().
  test_sensitive_flags_credentials_json: test_sensitive_flags_credentials_json().
  test_sensitive_does_not_flag_root_file_named_credentials: test_sensitive_does_not_flag_root_file_named_credentials().
  test_sensitive_secret_handler_txt: test_sensitive_secret_handler_txt().
  test_sensitive_token_config_yaml: test_sensitive_token_config_yaml().
  test_sensitive_does_not_flag_token_economics_note: test_sensitive_does_not_flag_token_economics_note().
  test_sensitive_does_not_flag_password_policy_discussion: test_sensitive_does_not_flag_password_policy_discussion().
  test_sensitive_flags_keyword_at_end_of_long_name: test_sensitive_flags_keyword_at_end_of_long_name().
  test_sensitive_flags_my_private_key_txt: test_sensitive_flags_my_private_key_txt().
  test_sensitive_flags_dotfile_token: test_sensitive_flags_dotfile_token().
  test_sensitive_flags_plural_tokens_txt: test_sensitive_flags_plural_tokens_txt().
  test_save_manifest_without_filter_unchanged_for_code: test_save_manifest_without_filter_unchanged_for_code().
  test_gitignore_fallback_when_no_graphifyignore: test_gitignore_fallback_when_no_graphifyignore().
  test_graphifyignore_and_gitignore_are_merged: test_graphifyignore_and_gitignore_are_merged().
  test_graphifyignore_negation_overrides_gitignore: test_graphifyignore_negation_overrides_gitignore().
  test_detect_skips_worktrees_dir: test_detect_skips_worktrees_dir().
  test_detect_skips_nested_worktrees_dir: test_detect_skips_nested_worktrees_dir().
  test_detect_extra_excludes_pattern: test_detect_extra_excludes_pattern().
  test_shebang_interpreter_plain: test_shebang_interpreter_plain().
  test_shebang_interpreter_env_single_arg: test_shebang_interpreter_env_single_arg().
  test_shebang_interpreter_env_dash_s: test_shebang_interpreter_env_dash_s().
  test_shebang_interpreter_env_with_flags: test_shebang_interpreter_env_with_flags().
  test_shebang_interpreter_env_with_assignment: test_shebang_interpreter_env_with_assignment().
  test_shebang_interpreter_no_shebang: test_shebang_interpreter_no_shebang().
  test_shebang_interpreter_quoted_path: test_shebang_interpreter_quoted_path().
  test_shebang_interpreter_unreadable_returns_none: test_shebang_interpreter_unreadable_returns_none().
  test_shebang_interpreter_env_missing_operand_returns_none: test_shebang_interpreter_env_missing_operand_returns_none().
  test_shebang_interpreter_env_unknown_option_returns_none: test_shebang_interpreter_env_unknown_option_returns_none().
  test_shebang_interpreter_env_nested_split_string_rejected: test_shebang_interpreter_env_nested_split_string_rejected().
  test_save_manifest_without_root_keeps_absolute_keys: test_save_manifest_without_root_keeps_absolute_keys().
  test_load_manifest_absolutizes_relative_keys: test_load_manifest_absolutizes_relative_keys().
  test_load_manifest_passes_through_legacy_absolute_keys: test_load_manifest_passes_through_legacy_absolute_keys().
  test_save_manifest_out_of_root_keeps_absolute: test_save_manifest_out_of_root_keeps_absolute().
  test_convert_office_file_hash_stable_across_nfc_nfd: test_convert_office_file_hash_stable_across_nfc_nfd().
  test_convert_office_file_does_not_rewrite_existing_sidecar: test_convert_office_file_does_not_rewrite_existing_sidecar().
  test_detect_converts_google_workspace_shortcuts_when_enabled.fake_convert: test_detect_converts_google_workspace_shortcuts_when_enabled().fake_convert().
  test_negation_does_not_disable_directory_pruning.tracking_walk: test_negation_does_not_disable_directory_pruning().tracking_walk().
  test_is_ignored_cache_evaluates_each_dir_once.CountingCache: test_is_ignored_cache_evaluates_each_dir_once().CountingCache#
  test_is_ignored_cache_evaluates_each_dir_once.CountingCache.__setitem__: test_is_ignored_cache_evaluates_each_dir_once().CountingCache#__setitem__().
---
# Module: [`tests/test_detect.py`](../../../../../raw/code/graphify/tests/test_detect.py)

## Classes
### `CountingCache`  ·  implements/extends dict
- def: [`tests/test_detect.py:775`](../../../../../raw/code/graphify/tests/test_detect.py#L775)
- signature: `class CountingCache(dict):`
- protocol/private: `__setitem__`[`L776`](../../../../../raw/code/graphify/tests/test_detect.py#L776)
- used by: (1 test-only callers)

## Functions
- `fake_convert(path, out_dir, *, xlsx_to_markdown=None)` — [`L401`](../../../../../raw/code/graphify/tests/test_detect.py#L401)
- `test_anchored_dir_matches_at_root(tmp_path)` — [`L640`](../../../../../raw/code/graphify/tests/test_detect.py#L640) — /inbox/ must still match inbox/ at the anchor root (positive case).
- `test_anchored_dir_not_matched_at_depth(tmp_path)` — [`L623`](../../../../../raw/code/graphify/tests/test_detect.py#L623) — /inbox/ must not match src/inbox/ — only inbox/ at the anchor root.
- `test_anchored_file_not_matched_at_depth(tmp_path)` — [`L657`](../../../../../raw/code/graphify/tests/test_detect.py#L657) — /build must not match src/build.
- `test_anchored_multi_segment_pattern(tmp_path)` — [`L683`](../../../../../raw/code/graphify/tests/test_detect.py#L683) — /src/inbox/ must match src/inbox/ but not x/src/inbox/.
- `test_classify_attention_paper()` — [`L91`](../../../../../raw/code/graphify/tests/test_detect.py#L91) — The real attention paper file should be classified as PAPER.
- `test_classify_google_workspace_shortcuts()` — [`L382`](../../../../../raw/code/graphify/tests/test_detect.py#L382)
- `test_classify_image()` — [`L40`](../../../../../raw/code/graphify/tests/test_detect.py#L40)
- `test_classify_markdown()` — [`L22`](../../../../../raw/code/graphify/tests/test_detect.py#L22)
- `test_classify_md_doc_without_signals(tmp_path)` — [`L84`](../../../../../raw/code/graphify/tests/test_detect.py#L84) — A plain .md file without paper signals should stay DOCUMENT.
- `test_classify_md_paper_by_signals(tmp_path)` — [`L73`](../../../../../raw/code/graphify/tests/test_detect.py#L73) — A .md file with enough paper signals should classify as PAPER.
- `test_classify_pdf()` — [`L25`](../../../../../raw/code/graphify/tests/test_detect.py#L25)
- `test_classify_pdf_in_xcassets_root_skipped()` — [`L33`](../../../../../raw/code/graphify/tests/test_detect.py#L33)
- `test_classify_pdf_in_xcassets_skipped()` — [`L28`](../../../../../raw/code/graphify/tests/test_detect.py#L28)
- `test_classify_powershell_manifest()` — [`L18`](../../../../../raw/code/graphify/tests/test_detect.py#L18)
- `test_classify_powershell_module()` — [`L14`](../../../../../raw/code/graphify/tests/test_detect.py#L14)
- `test_classify_python()` — [`L8`](../../../../../raw/code/graphify/tests/test_detect.py#L8)
- `test_classify_typescript()` — [`L11`](../../../../../raw/code/graphify/tests/test_detect.py#L11)
- `test_classify_unknown_returns_none()` — [`L37`](../../../../../raw/code/graphify/tests/test_detect.py#L37)
- `test_classify_video_extensions()` — [`L371`](../../../../../raw/code/graphify/tests/test_detect.py#L371) — Video and audio file extensions should classify as VIDEO.
- `test_convert_office_file_does_not_rewrite_existing_sidecar(tmp_path, monkeypatch)` — [`L1525`](../../../../../raw/code/graphify/tests/test_detect.py#L1525) — A second conversion of an unchanged source must not rewrite the sidecar,
- `test_convert_office_file_hash_stable_across_nfc_nfd(tmp_path, monkeypatch)` — [`L1497`](../../../../../raw/code/graphify/tests/test_detect.py#L1497) — The sidecar name must be identical whether the source path arrives in
- `test_count_words_sample_md()` — [`L45`](../../../../../raw/code/graphify/tests/test_detect.py#L45)
- `test_detect_allows_github_dir(tmp_path)` — [`L495`](../../../../../raw/code/graphify/tests/test_detect.py#L495) — Files inside .github/ (workflows etc.) are now indexed (#873).
- `test_detect_converts_google_workspace_shortcuts_when_enabled(tmp_path, monkeypatch)` — [`L397`](../../../../../raw/code/graphify/tests/test_detect.py#L397)
- `test_detect_default_does_not_auto_follow_direct_symlink_child(tmp_path)` — [`L239`](../../../../../raw/code/graphify/tests/test_detect.py#L239) — Symlink directory following is explicit opt-in.
- `test_detect_default_does_not_follow_when_no_symlinks(tmp_path)` — [`L251`](../../../../../raw/code/graphify/tests/test_detect.py#L251) — Ordinary scans still walk normal directories by default.
- `test_detect_explicit_false_overrides_auto_detect(tmp_path)` — [`L263`](../../../../../raw/code/graphify/tests/test_detect.py#L263) — An explicit follow_symlinks=False skips symlinked directories.
- `test_detect_extra_excludes_pattern(tmp_path)` — [`L1010`](../../../../../raw/code/graphify/tests/test_detect.py#L1010) — extra_excludes patterns exclude matching files from detect() (#947).
- `test_detect_finds_fixtures()` — [`L49`](../../../../../raw/code/graphify/tests/test_detect.py#L49)
- `test_detect_finds_video_files(tmp_path)` — [`L423`](../../../../../raw/code/graphify/tests/test_detect.py#L423) — detect() correctly counts video files and does not add them to word count.
- `test_detect_follows_symlinked_directory(tmp_path)` — [`L133`](../../../../../raw/code/graphify/tests/test_detect.py#L133)
- `test_detect_follows_symlinked_file(tmp_path)` — [`L147`](../../../../../raw/code/graphify/tests/test_detect.py#L147)
- `test_detect_handles_circular_symlinks(tmp_path)` — [`L229`](../../../../../raw/code/graphify/tests/test_detect.py#L229)
- `test_detect_includes_video_key(tmp_path)` — [`L416`](../../../../../raw/code/graphify/tests/test_detect.py#L416) — detect() result always includes a 'video' key even with no video files.
- `test_detect_incremental_portable_across_paths(tmp_path)` — [`L1424`](../../../../../raw/code/graphify/tests/test_detect.py#L1424) — End-to-end: a manifest written at one root must be readable from a
- `test_detect_incremental_propagates_follow_symlinks(tmp_path, monkeypatch)` — [`L303`](../../../../../raw/code/graphify/tests/test_detect.py#L303) — detect_incremental must forward follow_symlinks so symlinked sub-trees
- `test_detect_incremental_survives_dict_valued_mtime(tmp_path, monkeypatch)` — [`L334`](../../../../../raw/code/graphify/tests/test_detect.py#L334) — A schema-drifted manifest whose entry stores mtime as a nested dict
- `test_detect_skips_coverage_dir(tmp_path)` — [`L442`](../../../../../raw/code/graphify/tests/test_detect.py#L442) — coverage/ and lcov-report/ are noise dirs — HTML reports inside must be excluded (#870).
- `test_detect_skips_google_workspace_shortcuts_by_default(tmp_path)` — [`L388`](../../../../../raw/code/graphify/tests/test_detect.py#L388)
- `test_detect_skips_graphify_own_cache(tmp_path)` — [`L520`](../../../../../raw/code/graphify/tests/test_detect.py#L520) — .graphify/ (extraction cache) must never be re-indexed as source (#873).
- `test_detect_skips_nested_worktrees_dir(tmp_path)` — [`L997`](../../../../../raw/code/graphify/tests/test_detect.py#L997) — Files inside .claude/worktrees/ (nested placement) are never indexed (#1023).
- `test_detect_skips_next_cache(tmp_path)` — [`L506`](../../../../../raw/code/graphify/tests/test_detect.py#L506) — .next/ (Next.js build cache) must be excluded even after dot-dir fix (#873).
- `test_detect_skips_noise_dot_dirs()` — [`L60`](../../../../../raw/code/graphify/tests/test_detect.py#L60) — Noise dot dirs (.next, .nuxt, .graphify cache, …) are skipped (#873).
- `test_detect_skips_out_of_root_symlinked_directory_even_when_following(tmp_path)` — [`L275`](../../../../../raw/code/graphify/tests/test_detect.py#L275)
- `test_detect_skips_out_of_root_symlinked_file_by_default(tmp_path)` — [`L289`](../../../../../raw/code/graphify/tests/test_detect.py#L289)
- `test_detect_skips_snapshots_dir(tmp_path)` — [`L469`](../../../../../raw/code/graphify/tests/test_detect.py#L469) — __snapshots__/ and snapshots/ are jest/vitest artefacts — must be excluded.
- `test_detect_skips_storybook_static_dir(tmp_path)` — [`L480`](../../../../../raw/code/graphify/tests/test_detect.py#L480) — storybook-static/ is a build artefact — must be excluded.
- `test_detect_skips_visual_tests_dir(tmp_path)` — [`L456`](../../../../../raw/code/graphify/tests/test_detect.py#L456) — visual-tests/ bundles and snapshots are noise — must be excluded (#869).
- `test_detect_skips_worktrees_dir(tmp_path)` — [`L984`](../../../../../raw/code/graphify/tests/test_detect.py#L984) — Files inside .worktrees/ are never indexed (#947).
- `test_detect_video_not_in_words(tmp_path)` — [`L434`](../../../../../raw/code/graphify/tests/test_detect.py#L434) — Video files do not contribute to total_words.
- `test_detect_warns_small_corpus()` — [`L55`](../../../../../raw/code/graphify/tests/test_detect.py#L55)
- `test_gitignore_fallback_when_no_graphifyignore(tmp_path)` — [`L931`](../../../../../raw/code/graphify/tests/test_detect.py#L931) — When no .graphifyignore exists, .gitignore patterns are honored (#945).
- `test_graphifyignore_and_gitignore_are_merged(tmp_path)` — [`L948`](../../../../../raw/code/graphify/tests/test_detect.py#L948) — When both exist, their patterns are MERGED — a file excluded only by
- `test_graphifyignore_at_git_root_is_included(tmp_path)` — [`L209`](../../../../../raw/code/graphify/tests/test_detect.py#L209) — A .graphifyignore at the git repo root is included when scanning a subdir.
- `test_graphifyignore_comments_ignored(tmp_path)` — [`L123`](../../../../../raw/code/graphify/tests/test_detect.py#L123) — Comment lines in .graphifyignore are not treated as patterns.
- `test_graphifyignore_discovered_from_parent_in_vcs(tmp_path)` — [`L175`](../../../../../raw/code/graphify/tests/test_detect.py#L175) — Inside a VCS repo, parent .graphifyignore applies to subdirectory scans.
- `test_graphifyignore_excludes_file(tmp_path)` — [`L99`](../../../../../raw/code/graphify/tests/test_detect.py#L99) — Files matching .graphifyignore patterns are excluded from detect().
- `test_graphifyignore_hermetic_without_vcs(tmp_path)` — [`L157`](../../../../../raw/code/graphify/tests/test_detect.py#L157) — Without a VCS root, parent .graphifyignore does NOT apply (hermetic).
- `test_graphifyignore_missing_is_fine(tmp_path)` — [`L116`](../../../../../raw/code/graphify/tests/test_detect.py#L116) — No .graphifyignore is not an error.
- `test_graphifyignore_negation_overrides_gitignore(tmp_path)` — [`L967`](../../../../../raw/code/graphify/tests/test_detect.py#L967) — .graphifyignore is evaluated after .gitignore, so a `!` negation in it can
- `test_graphifyignore_stops_at_git_boundary(tmp_path)` — [`L193`](../../../../../raw/code/graphify/tests/test_detect.py#L193) — Upward search stops at the git repo root (.git directory).
- `test_is_ignored_cache_evaluates_each_dir_once()` — [`L749`](../../../../../raw/code/graphify/tests/test_detect.py#L749) — Siblings under the same subtree must share the cached parent result (#1235).
- `test_is_ignored_cache_matches_uncached_results(tmp_path)` — [`L704`](../../../../../raw/code/graphify/tests/test_detect.py#L704) — A shared _cache must not change _is_ignored results, including negation.
- `test_load_manifest_absolutizes_relative_keys(tmp_path)` — [`L1370`](../../../../../raw/code/graphify/tests/test_detect.py#L1370) — ``load_manifest(root=...)`` re-anchors stored relative keys so the
- `test_load_manifest_passes_through_legacy_absolute_keys(tmp_path)` — [`L1388`](../../../../../raw/code/graphify/tests/test_detect.py#L1388) — Legacy absolute-keyed manifests still load correctly when ``root``
- `test_negation_ancestor_itself_reincluded(tmp_path)` — [`L563`](../../../../../raw/code/graphify/tests/test_detect.py#L563) — If the ancestor dir itself is re-included, its children should not be blocked (#882).
- `test_negation_cannot_rescue_file_under_excluded_dir(tmp_path)` — [`L534`](../../../../../raw/code/graphify/tests/test_detect.py#L534) — A ! re-include cannot un-ignore a file whose parent dir is excluded (#882).
- `test_negation_does_not_disable_directory_pruning(tmp_path, monkeypatch)` — [`L576`](../../../../../raw/code/graphify/tests/test_detect.py#L576) — A single `!` re-include must not switch off pruning of *unrelated* ignored dirs.
- `test_negation_works_when_no_ancestor_excluded(tmp_path)` — [`L549`](../../../../../raw/code/graphify/tests/test_detect.py#L549) — A ! re-include must still un-ignore a file when no ancestor is excluded (#882).
- `test_save_manifest_in_root_symlink_roundtrips(tmp_path)` — [`L1463`](../../../../../raw/code/graphify/tests/test_detect.py#L1463) — In-root symlinks must store under the symlink's own name, not the
- `test_save_manifest_out_of_root_keeps_absolute(tmp_path)` — [`L1403`](../../../../../raw/code/graphify/tests/test_detect.py#L1403) — Files outside ``root`` (e.g. symlinked external corpora) are stored
- `test_save_manifest_relativizes_keys_when_root_given(tmp_path)` — [`L1324`](../../../../../raw/code/graphify/tests/test_detect.py#L1324) — ``save_manifest(root=...)`` writes forward-slash relative keys.
- `test_save_manifest_skips_semantic_hash_for_files_without_cache(tmp_path)` — [`L880`](../../../../../raw/code/graphify/tests/test_detect.py#L880) — Files in failed chunks have no semantic cache entry; save_manifest must
- `test_save_manifest_without_filter_unchanged_for_code(tmp_path)` — [`L915`](../../../../../raw/code/graphify/tests/test_detect.py#L915) — Code files must be stamped in the manifest regardless of semantic cache.
- `test_save_manifest_without_root_keeps_absolute_keys(tmp_path)` — [`L1352`](../../../../../raw/code/graphify/tests/test_detect.py#L1352) — Back-compat: callers that don't pass ``root`` still get the legacy
- `test_sensitive_does_not_flag_password_policy_discussion()` — [`L858`](../../../../../raw/code/graphify/tests/test_detect.py#L858)
- `test_sensitive_does_not_flag_root_file_named_credentials()` — [`L829`](../../../../../raw/code/graphify/tests/test_detect.py#L829)
- `test_sensitive_does_not_flag_token_economics_note()` — [`L855`](../../../../../raw/code/graphify/tests/test_detect.py#L855)
- `test_sensitive_does_not_flag_tokenize_py()` — [`L810`](../../../../../raw/code/graphify/tests/test_detect.py#L810)
- `test_sensitive_does_not_flag_tokenizer_py()` — [`L807`](../../../../../raw/code/graphify/tests/test_detect.py#L807)
- `test_sensitive_flags_api_token_txt()` — [`L798`](../../../../../raw/code/graphify/tests/test_detect.py#L798)
- `test_sensitive_flags_credentials_json()` — [`L826`](../../../../../raw/code/graphify/tests/test_detect.py#L826)
- `test_sensitive_flags_dotfile_token()` — [`L870`](../../../../../raw/code/graphify/tests/test_detect.py#L870)
- `test_sensitive_flags_keyword_at_end_of_long_name()` — [`L861`](../../../../../raw/code/graphify/tests/test_detect.py#L861)
- `test_sensitive_flags_my_private_key_txt()` — [`L865`](../../../../../raw/code/graphify/tests/test_detect.py#L865)
- `test_sensitive_flags_oauth_token_json()` — [`L801`](../../../../../raw/code/graphify/tests/test_detect.py#L801)
- `test_sensitive_flags_passwords_py()` — [`L813`](../../../../../raw/code/graphify/tests/test_detect.py#L813)
- `test_sensitive_flags_plural_tokens_txt()` — [`L874`](../../../../../raw/code/graphify/tests/test_detect.py#L874)
- `test_sensitive_flags_secrets_dir()` — [`L820`](../../../../../raw/code/graphify/tests/test_detect.py#L820)
- `test_sensitive_flags_ssh_dir()` — [`L817`](../../../../../raw/code/graphify/tests/test_detect.py#L817)
- `test_sensitive_flags_token_txt()` — [`L823`](../../../../../raw/code/graphify/tests/test_detect.py#L823)
- `test_sensitive_flags_underscore_secret()` — [`L804`](../../../../../raw/code/graphify/tests/test_detect.py#L804)
- `test_sensitive_secret_handler_txt()` — [`L841`](../../../../../raw/code/graphify/tests/test_detect.py#L841)
- `test_sensitive_token_config_yaml()` — [`L846`](../../../../../raw/code/graphify/tests/test_detect.py#L846)
- `test_shebang_file_type_classifies_via_interpreter(tmp_path)` — [`L1087`](../../../../../raw/code/graphify/tests/test_detect.py#L1087) — Classify file type via interpreter, including env -S form.
- `test_shebang_interpreter_env_chdir_with_operand(tmp_path)` — [`L1111`](../../../../../raw/code/graphify/tests/test_detect.py#L1111) — `env -C /tmp python3` skips both -C and its workdir operand.
- `test_shebang_interpreter_env_clumped_u_operand(tmp_path)` — [`L1138`](../../../../../raw/code/graphify/tests/test_detect.py#L1138) — Clumped `-uPYTHONPATH` form (no space between flag and operand) is one arg.
- `test_shebang_interpreter_env_compact_dash_s(tmp_path)` — [`L1182`](../../../../../raw/code/graphify/tests/test_detect.py#L1182) — Compact `-Spython3 -u` form (no space between -S and packed string).
- `test_shebang_interpreter_env_compact_v_then_s(tmp_path)` — [`L1191`](../../../../../raw/code/graphify/tests/test_detect.py#L1191) — Compact `-vSpython3` (-v plus compact -S).
- `test_shebang_interpreter_env_dash_s(tmp_path)` — [`L1045`](../../../../../raw/code/graphify/tests/test_detect.py#L1045) — `#!/usr/bin/env -S python3 -u` (-S split-args form) recovers the interpreter.
- `test_shebang_interpreter_env_dash_s_after_flag(tmp_path)` — [`L1129`](../../../../../raw/code/graphify/tests/test_detect.py#L1129) — `env -i -S "python3 -u"` handles -S after another env flag.
- `test_shebang_interpreter_env_dash_s_assignment_before_interpreter(tmp_path)` — [`L1255`](../../../../../raw/code/graphify/tests/test_detect.py#L1255) — `-S` payload may carry NAME=value assignments before the interpreter.
- `test_shebang_interpreter_env_dash_s_flag_before_interpreter(tmp_path)` — [`L1267`](../../../../../raw/code/graphify/tests/test_detect.py#L1267) — `-S` payload may carry env flags (e.g. -i) before the interpreter.
- `test_shebang_interpreter_env_gnu_argv0_operand(tmp_path)` — [`L1173`](../../../../../raw/code/graphify/tests/test_detect.py#L1173) — GNU `-a alias python3` skips both -a and its argv0 operand.
- `test_shebang_interpreter_env_gnu_split_string_equals(tmp_path)` — [`L1155`](../../../../../raw/code/graphify/tests/test_detect.py#L1155) — GNU `--split-string='python3 -u'` (with `=` operand) → python3.
- `test_shebang_interpreter_env_gnu_split_string_separate(tmp_path)` — [`L1164`](../../../../../raw/code/graphify/tests/test_detect.py#L1164) — GNU `--split-string "python3 -u"` (separate operand) → python3.
- `test_shebang_interpreter_env_long_chdir_equals(tmp_path)` — [`L1227`](../../../../../raw/code/graphify/tests/test_detect.py#L1227) — GNU `--chdir=/tmp python3` (`=` operand form).
- `test_shebang_interpreter_env_long_chdir_separate_operand(tmp_path)` — [`L1218`](../../../../../raw/code/graphify/tests/test_detect.py#L1218) — GNU `--chdir /tmp python3` (separate operand).
- `test_shebang_interpreter_env_long_split_assignment_before_interpreter(tmp_path)` — [`L1276`](../../../../../raw/code/graphify/tests/test_detect.py#L1276) — `--split-string=` payload may carry assignments before the interpreter.
- `test_shebang_interpreter_env_long_split_flag_before_interpreter(tmp_path)` — [`L1288`](../../../../../raw/code/graphify/tests/test_detect.py#L1288) — `--split-string=` payload may carry env flags before the interpreter.
- `test_shebang_interpreter_env_long_unset_equals(tmp_path)` — [`L1209`](../../../../../raw/code/graphify/tests/test_detect.py#L1209) — GNU `--unset=PYTHONPATH python3` (`=` operand form).
- `test_shebang_interpreter_env_long_unset_separate_operand(tmp_path)` — [`L1200`](../../../../../raw/code/graphify/tests/test_detect.py#L1200) — GNU `--unset PYTHONPATH python3` (separate operand).
- `test_shebang_interpreter_env_missing_operand_returns_none(tmp_path)` — [`L1147`](../../../../../raw/code/graphify/tests/test_detect.py#L1147) — `env -u` with no operand → not a valid command, return None.
- `test_shebang_interpreter_env_nested_split_string_rejected(tmp_path)` — [`L1297`](../../../../../raw/code/graphify/tests/test_detect.py#L1297) — A `-S` payload that itself starts with `-S` is rejected (allow_split=False
- `test_shebang_interpreter_env_path_with_operand(tmp_path)` — [`L1120`](../../../../../raw/code/graphify/tests/test_detect.py#L1120) — `env -P /bin python3` skips both -P and its utilpath operand.
- `test_shebang_interpreter_env_signal_flags(tmp_path)` — [`L1236`](../../../../../raw/code/graphify/tests/test_detect.py#L1236) — GNU signal-handling flags skip transparently.
- `test_shebang_interpreter_env_single_arg(tmp_path)` — [`L1037`](../../../../../raw/code/graphify/tests/test_detect.py#L1037) — `#!/usr/bin/env python3` returns the interpreter, not 'env'.
- `test_shebang_interpreter_env_unknown_option_returns_none(tmp_path)` — [`L1245`](../../../../../raw/code/graphify/tests/test_detect.py#L1245) — Unknown hyphen-prefixed env option → return None rather than guessing.
- `test_shebang_interpreter_env_unset_with_operand(tmp_path)` — [`L1102`](../../../../../raw/code/graphify/tests/test_detect.py#L1102) — `env -u VAR python3` skips both -u and its required operand.
- `test_shebang_interpreter_env_vs_assignment_before_interpreter(tmp_path)` — [`L1309`](../../../../../raw/code/graphify/tests/test_detect.py#L1309) — `-vS` packed payload also re-parses for leading assignments.
- `test_shebang_interpreter_env_with_assignment(tmp_path)` — [`L1061`](../../../../../raw/code/graphify/tests/test_detect.py#L1061) — `#!/usr/bin/env DEBUG=1 python3` skips var=value assignments.
- `test_shebang_interpreter_env_with_flags(tmp_path)` — [`L1053`](../../../../../raw/code/graphify/tests/test_detect.py#L1053) — `#!/usr/bin/env -i bash` skips env flags and resolves to the interpreter.
- `test_shebang_interpreter_no_shebang(tmp_path)` — [`L1069`](../../../../../raw/code/graphify/tests/test_detect.py#L1069) — File without shebang returns None.
- `test_shebang_interpreter_plain(tmp_path)` — [`L1029`](../../../../../raw/code/graphify/tests/test_detect.py#L1029) — Plain shebang returns the interpreter basename.
- `test_shebang_interpreter_quoted_path(tmp_path)` — [`L1077`](../../../../../raw/code/graphify/tests/test_detect.py#L1077) — Quoted interpreter path with spaces parses correctly via shlex.
- `test_shebang_interpreter_unreadable_returns_none(tmp_path)` — [`L1095`](../../../../../raw/code/graphify/tests/test_detect.py#L1095) — Unreadable / nonexistent files return None, never raise.
- `test_unanchored_dir_still_matches_at_depth(tmp_path)` — [`L669`](../../../../../raw/code/graphify/tests/test_detect.py#L669) — inbox/ (no leading /) must still match src/inbox/ anywhere in the tree.
- `tracking_walk(top, *args, **kwargs)` — [`L601`](../../../../../raw/code/graphify/tests/test_detect.py#L601)

## Module values
- `FIXTURES` — [`L6`](../../../../../raw/code/graphify/tests/test_detect.py#L6)

