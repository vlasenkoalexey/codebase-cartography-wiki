---
title: 'Module: tests/unit/security/test_fixture_detector.py'
type: catalog
provenance: extracted
module: tests/unit/security/test_fixture_detector.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.security.test_fixture_detector`/
symbols:
  _make_project: _make_project().
  TestAllowlist.test_allowlist_hit_returns_confidence_1: TestAllowlist#test_allowlist_hit_returns_confidence_1().
  TestVerdictMapping.test_threshold_mapping: TestVerdictMapping#test_threshold_mapping().
  TestTier2Scan.test_sample_python_constant_idiom: TestTier2Scan#test_sample_python_constant_idiom().
  TestDisableEnvVar.test_disable_short_circuits_detection: TestDisableEnvVar#test_disable_short_circuits_detection().
  TestTier2Scan.test_bare_repo_relative_literal_is_caution: TestTier2Scan#test_bare_repo_relative_literal_is_caution().
  TestRealRepoRegression.test_real_repo_finds_java_plugin: TestRealRepoRegression#test_real_repo_finds_java_plugin().
  TestCache.test_readable_cache_uses_targeted_scan: TestCache#test_readable_cache_uses_targeted_scan().
  TestListFixtures.test_list_includes_allowlist_and_scanned: TestListFixtures#test_list_includes_allowlist_and_scanned().
  TestAllowlist.test_no_claude_md_returns_negative: TestAllowlist#test_no_claude_md_returns_negative().
  TestCache.test_targeted_scan_detects_exact_repo_relative_literal: TestCache#test_targeted_scan_detects_exact_repo_relative_literal().
  TestAllowlist.test_path_outside_project_returns_negative: TestAllowlist#test_path_outside_project_returns_negative().
  TestTier2Scan.test_plugin_manifest_exclusion: TestTier2Scan#test_plugin_manifest_exclusion().
  TestTier2Scan.test_no_signal_returns_negative: TestTier2Scan#test_no_signal_returns_negative().
  TestCache.test_cache_corrupt_falls_through_to_scan: TestCache#test_cache_corrupt_falls_through_to_scan().
  TestCache.test_hidden_test_dirs_do_not_count_as_fixture_signals: TestCache#test_hidden_test_dirs_do_not_count_as_fixture_signals().
  TestCache.test_targeted_scan_skips_unreadable_test_files: TestCache#test_targeted_scan_skips_unreadable_test_files().
  TestCache.test_basename_seen_in_tests_handles_unreadable_file: TestCache#test_basename_seen_in_tests_handles_unreadable_file().
  TestCache.test_scan_tests_skips_unreadable_and_syntax_broken_tests: TestCache#test_scan_tests_skips_unreadable_and_syntax_broken_tests().
  TestCache.test_cache_written_on_first_scan: TestCache#test_cache_written_on_first_scan().
  TestCache.test_targeted_scan_returns_none_without_tests_dir: TestCache#test_targeted_scan_returns_none_without_tests_dir().
  TestCache.test_targeted_scan_skips_init_and_main_basenames: TestCache#test_targeted_scan_skips_init_and_main_basenames().
  TestCache.test_write_cache_logs_os_errors: TestCache#test_write_cache_logs_os_errors().
  TestVerdictMapping.test_unsafe_threshold_is_inclusive: TestVerdictMapping#test_unsafe_threshold_is_inclusive().
  TestListFixtures.test_empty_project_returns_empty_list: TestListFixtures#test_empty_project_returns_empty_list().
  _frontmatter: _frontmatter().
  TestCache.flaky_read_text: TestCache#flaky_read_text().
  TestCache.test_cache_readability_accepts_legacy_schema_and_rejects_bad_shapes: TestCache#test_cache_readability_accepts_legacy_schema_and_rejects_bad_shapes().
  REPO_ROOT: REPO_ROOT.
  TestCache.fail_write_text: TestCache#fail_write_text().
  TestAllowlist: TestAllowlist#
  TestTier2Scan: TestTier2Scan#
  TestRealRepoRegression: TestRealRepoRegression#
  TestCache: TestCache#
  TestVerdictMapping: TestVerdictMapping#
  TestDisableEnvVar: TestDisableEnvVar#
  TestListFixtures: TestListFixtures#
---
# Module: [`tests/unit/security/test_fixture_detector.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_fixture_detector.py)

## Classes
### `TestAllowlist`
- def: [`tests/unit/security/test_fixture_detector.py:74`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_fixture_detector.py#L74)
- signature: `class TestAllowlist:`
- members:
  - `test_allowlist_hit_returns_confidence_1(self, tmp_path: Path)` — [`L75`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_fixture_detector.py#L75)
  - `test_no_claude_md_returns_negative(self, tmp_path: Path)` — [`L92`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_fixture_detector.py#L92)
  - `test_path_outside_project_returns_negative(self, tmp_path: Path)` — [`L100`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_fixture_detector.py#L100)
- uses (calls/refs, reference-scoped): [`is_fixture`](../../../tree_sitter_analyzer/security/fixture_detector.md#is_fixture), [`FixtureFact`](../../../tree_sitter_analyzer/security/fixture_detector.md#FixtureFact), [`is_fixture`](../../../tree_sitter_analyzer/security/fixture_detector.md#FixtureFact.is_fixture), [`confidence`](../../../tree_sitter_analyzer/security/fixture_detector.md#FixtureFact.confidence), [`source`](../../../tree_sitter_analyzer/security/fixture_detector.md#FixtureFact.source), [`note`](../../../tree_sitter_analyzer/security/fixture_detector.md#FixtureFact.note)  (2 test-only)

### `TestCache`
- def: [`tests/unit/security/test_fixture_detector.py:206`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_fixture_detector.py#L206)
- signature: `class TestCache:`
- members:
  - `fail_write_text(self: Path, *_args, **_kwargs)` — [`L424`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_fixture_detector.py#L424)
  - `flaky_read_text(path: Path, *args, **kwargs)` — [`L346`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_fixture_detector.py#L346)
  - `test_basename_seen_in_tests_handles_unreadable_file(self, tmp_path: Path, monkeypatch: pytest.MonkeyPatch)` — [`L359`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_fixture_detector.py#L359)
  - `test_cache_corrupt_falls_through_to_scan(self, tmp_path: Path, caplog: pytest.LogCaptureFixture)` — [`L223`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_fixture_detector.py#L223)
  - `test_cache_readability_accepts_legacy_schema_and_rejects_bad_shapes(self, tmp_path: Path)` — [`L381`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_fixture_detector.py#L381)
  - `test_cache_written_on_first_scan(self, tmp_path: Path)` — [`L207`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_fixture_detector.py#L207)
  - `test_hidden_test_dirs_do_not_count_as_fixture_signals(self, tmp_path: Path)` — [`L275`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_fixture_detector.py#L275)
  - `test_readable_cache_uses_targeted_scan(self, tmp_path: Path)` — [`L253`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_fixture_detector.py#L253)
  - `test_scan_tests_skips_unreadable_and_syntax_broken_tests(self, tmp_path: Path, monkeypatch: pytest.MonkeyPatch)` — [`L393`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_fixture_detector.py#L393)
  - `test_targeted_scan_detects_exact_repo_relative_literal(self, tmp_path: Path)` — [`L299`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_fixture_detector.py#L299)
  - `test_targeted_scan_returns_none_without_tests_dir(self, tmp_path: Path)` — [`L290`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_fixture_detector.py#L290)
  - `test_targeted_scan_skips_init_and_main_basenames(self, tmp_path: Path)` — [`L318`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_fixture_detector.py#L318)
  - `test_targeted_scan_skips_unreadable_test_files(self, tmp_path: Path, monkeypatch: pytest.MonkeyPatch)` — [`L333`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_fixture_detector.py#L333)
  - `test_write_cache_logs_os_errors(self, tmp_path: Path, monkeypatch: pytest.MonkeyPatch, caplog: pytest.LogCaptureFixture)` — [`L416`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_fixture_detector.py#L416)
- uses (calls/refs, reference-scoped): [`is_fixture`](../../../tree_sitter_analyzer/security/fixture_detector.md#is_fixture), [`_scan_tests`](../../../tree_sitter_analyzer/security/fixture_detector.md#_scan_tests), [`_targeted_fixture_scan`](../../../tree_sitter_analyzer/security/fixture_detector.md#_targeted_fixture_scan), [`_write_cache`](../../../tree_sitter_analyzer/security/fixture_detector.md#_write_cache), [`is_fixture`](../../../tree_sitter_analyzer/security/fixture_detector.md#FixtureFact.is_fixture), [`confidence`](../../../tree_sitter_analyzer/security/fixture_detector.md#FixtureFact.confidence), [`source`](../../../tree_sitter_analyzer/security/fixture_detector.md#FixtureFact.source), [`_cache_is_readable`](../../../tree_sitter_analyzer/security/fixture_detector.md#_cache_is_readable), [`_basename_seen_in_tests`](../../../tree_sitter_analyzer/security/fixture_detector.md#_basename_seen_in_tests)  (1 test-only)

### `TestDisableEnvVar`
- def: [`tests/unit/security/test_fixture_detector.py:481`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_fixture_detector.py#L481)
- signature: `class TestDisableEnvVar:`
- members:
  - `test_disable_short_circuits_detection(self, tmp_path: Path, monkeypatch: pytest.MonkeyPatch)` — [`L482`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_fixture_detector.py#L482)
- uses (calls/refs, reference-scoped): [`is_fixture`](../../../tree_sitter_analyzer/security/fixture_detector.md#is_fixture), [`is_fixture`](../../../tree_sitter_analyzer/security/fixture_detector.md#FixtureFact.is_fixture), [`list_fixtures`](../../../tree_sitter_analyzer/security/fixture_detector.md#list_fixtures), [`source`](../../../tree_sitter_analyzer/security/fixture_detector.md#FixtureFact.source)  (2 test-only)

### `TestListFixtures`
- def: [`tests/unit/security/test_fixture_detector.py:509`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_fixture_detector.py#L509)
- signature: `class TestListFixtures:`
- members:
  - `test_empty_project_returns_empty_list(self, tmp_path: Path)` — [`L541`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_fixture_detector.py#L541)
  - `test_list_includes_allowlist_and_scanned(self, tmp_path: Path)` — [`L510`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_fixture_detector.py#L510)
- uses (calls/refs, reference-scoped): [`confidence`](../../../tree_sitter_analyzer/security/fixture_detector.md#FixtureFact.confidence), [`list_fixtures`](../../../tree_sitter_analyzer/security/fixture_detector.md#list_fixtures), [`source`](../../../tree_sitter_analyzer/security/fixture_detector.md#FixtureFact.source)  (2 test-only)

### `TestRealRepoRegression`
- def: [`tests/unit/security/test_fixture_detector.py:185`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_fixture_detector.py#L185)
- signature: `class TestRealRepoRegression:`
- members:
  - `test_real_repo_finds_java_plugin(self)` — [`L186`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_fixture_detector.py#L186)
- uses (calls/refs, reference-scoped): [`is_fixture`](../../../tree_sitter_analyzer/security/fixture_detector.md#is_fixture), [`is_fixture`](../../../tree_sitter_analyzer/security/fixture_detector.md#FixtureFact.is_fixture), [`confidence`](../../../tree_sitter_analyzer/security/fixture_detector.md#FixtureFact.confidence), [`evidence`](../../../tree_sitter_analyzer/security/fixture_detector.md#FixtureFact.evidence)  (1 test-only)

### `TestTier2Scan`
- def: [`tests/unit/security/test_fixture_detector.py:112`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_fixture_detector.py#L112)
- signature: `class TestTier2Scan:`
- members:
  - `test_bare_repo_relative_literal_is_caution(self, tmp_path: Path)` — [`L136`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_fixture_detector.py#L136)
  - `test_no_signal_returns_negative(self, tmp_path: Path)` — [`L172`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_fixture_detector.py#L172)
  - `test_plugin_manifest_exclusion(self, tmp_path: Path)` — [`L153`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_fixture_detector.py#L153)
  - `test_sample_python_constant_idiom(self, tmp_path: Path)` — [`L113`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_fixture_detector.py#L113)
- uses (calls/refs, reference-scoped): [`is_fixture`](../../../tree_sitter_analyzer/security/fixture_detector.md#is_fixture), [`is_fixture`](../../../tree_sitter_analyzer/security/fixture_detector.md#FixtureFact.is_fixture), [`confidence`](../../../tree_sitter_analyzer/security/fixture_detector.md#FixtureFact.confidence), [`fixture_to_verdict`](../../../tree_sitter_analyzer/security/fixture_detector.md#fixture_to_verdict), [`source`](../../../tree_sitter_analyzer/security/fixture_detector.md#FixtureFact.source), [`evidence`](../../../tree_sitter_analyzer/security/fixture_detector.md#FixtureFact.evidence)  (1 test-only)

### `TestVerdictMapping`
- def: [`tests/unit/security/test_fixture_detector.py:445`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_fixture_detector.py#L445)
- signature: `class TestVerdictMapping:`
- members:
  - `test_threshold_mapping(self, confidence: float, expected: str | None)` — [`L459`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_fixture_detector.py#L459)
  - `test_unsafe_threshold_is_inclusive(self)` — [`L469`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_fixture_detector.py#L469)
- uses (calls/refs, reference-scoped): [`FixtureFact`](../../../tree_sitter_analyzer/security/fixture_detector.md#FixtureFact), [`is_fixture`](../../../tree_sitter_analyzer/security/fixture_detector.md#FixtureFact.is_fixture), [`confidence`](../../../tree_sitter_analyzer/security/fixture_detector.md#FixtureFact.confidence), [`fixture_to_verdict`](../../../tree_sitter_analyzer/security/fixture_detector.md#fixture_to_verdict), [`source`](../../../tree_sitter_analyzer/security/fixture_detector.md#FixtureFact.source), [`evidence`](../../../tree_sitter_analyzer/security/fixture_detector.md#FixtureFact.evidence), [`note`](../../../tree_sitter_analyzer/security/fixture_detector.md#FixtureFact.note)

## Functions
- `_frontmatter(allowlist: list[dict[str, str]])` — [`L56`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_fixture_detector.py#L56) — Render an ``intentional_design``-style CLAUDE.md frontmatter block.
- `_make_project(tmp_path: Path, files: dict[str, str])` — [`L40`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_fixture_detector.py#L40) — Materialise a fake project tree under ``tmp_path``.

## Module values
- `REPO_ROOT` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_fixture_detector.py#L32)

