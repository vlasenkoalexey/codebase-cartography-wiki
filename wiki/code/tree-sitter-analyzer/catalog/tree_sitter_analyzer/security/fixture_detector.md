---
title: 'Module: tree_sitter_analyzer/security/fixture_detector.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/security/fixture_detector.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.security.fixture_detector`/
symbols:
  is_fixture: is_fixture().
  _scan_tests: _scan_tests().
  _targeted_fixture_scan: _targeted_fixture_scan().
  _allowlist_facts: _allowlist_facts().
  _process_assign: _process_assign().
  FixtureFact: FixtureFact#
  FixtureFact.is_fixture: FixtureFact#is_fixture.
  _write_cache: _write_cache().
  FixtureFact.confidence: FixtureFact#confidence.
  _read_cache: _read_cache().
  list_fixtures: list_fixtures().
  _walk_module: _walk_module().
  _NEGATIVE: _NEGATIVE.
  _load_or_build_index: _load_or_build_index().
  _DISABLED: _DISABLED.
  fixture_to_verdict: fixture_to_verdict().
  _process_repo_relative_literals: _process_repo_relative_literals().
  FixtureFact.source: FixtureFact#source.
  FixtureFact.evidence: FixtureFact#evidence.
  _Aggregator.record: _Aggregator#record().
  _expr_is_path_like: _expr_is_path_like().
  FixtureFact.note: FixtureFact#note.
  _Aggregator: _Aggregator#
  _cache_is_readable: _cache_is_readable().
  _check_allowlist: _check_allowlist().
  _basename_to_repo_relative: _basename_to_repo_relative().
  _basename_seen_in_tests: _basename_seen_in_tests().
  _iter_test_files: _iter_test_files().
  _Aggregator.suppressed: _Aggregator#suppressed.
  _tests_signature: _tests_signature().
  _record_path_binding: _record_path_binding().
  _plugin_manifest_basenames: _plugin_manifest_basenames().
  logger: logger.
  _CONFIDENCE_CAUTION: _CONFIDENCE_CAUTION.
  _REPO_RELATIVE_CONFIDENCE: _REPO_RELATIVE_CONFIDENCE.
  _CACHE_SCHEMA_VERSION: _CACHE_SCHEMA_VERSION.
  _Aggregator.confidence: _Aggregator#confidence.
  _Aggregator.evidence: _Aggregator#evidence.
  _safe_relative: _safe_relative().
  _CONFIDENCE_UNSAFE: _CONFIDENCE_UNSAFE.
  _CONSTANT_ASSIGNMENT_CONFIDENCE: _CONSTANT_ASSIGNMENT_CONFIDENCE.
  _REPO_RELATIVE_PATTERN: _REPO_RELATIVE_PATTERN.
  _CACHE_PATH_SUFFIX: _CACHE_PATH_SUFFIX.
  _DISABLE_ENV_VAR: _DISABLE_ENV_VAR.
  _Aggregator.source: _Aggregator#source.
  _ALLOWLIST_CONFIDENCE: _ALLOWLIST_CONFIDENCE.
  _PATH_LITERAL_CONFIDENCE: _PATH_LITERAL_CONFIDENCE.
  _FIXTURE_NAME_PREFIX: _FIXTURE_NAME_PREFIX.
  _PLUGIN_MANIFEST_PATTERN: _PLUGIN_MANIFEST_PATTERN.
  _TARGETED_SKIP_BASENAMES: _TARGETED_SKIP_BASENAMES.
  _assignment_target_name: _assignment_target_name().
  _collect_strings: _collect_strings().
  _to_relative: _to_relative().
  __all__: __all__.
---
# Module: [`tree_sitter_analyzer/security/fixture_detector.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/fixture_detector.py)

## Classes
### `FixtureFact`
- def: [`tree_sitter_analyzer/security/fixture_detector.py:109`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/fixture_detector.py#L109)
- doc: Result of asking "is this file a fixture?".
- signature: `class FixtureFact:`
- members:
  - `confidence` — [`L119`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/fixture_detector.py#L119)
  - `evidence` — [`L121`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/fixture_detector.py#L121)
  - `is_fixture` — [`L118`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/fixture_detector.py#L118)
  - `note` — [`L122`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/fixture_detector.py#L122)
  - `source` — [`L120`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/fixture_detector.py#L120)
- used by: [`_format_safe_to_edit_result`](../mcp/tools/utils/safe_to_edit_helpers.md#_format_safe_to_edit_result), [`is_fixture`](fixture_detector.md#is_fixture), [`_scan_tests`](fixture_detector.md#_scan_tests), [`_targeted_fixture_scan`](fixture_detector.md#_targeted_fixture_scan), [`_allowlist_facts`](fixture_detector.md#_allowlist_facts), [`_write_cache`](fixture_detector.md#_write_cache), [`_read_cache`](fixture_detector.md#_read_cache), [`list_fixtures`](fixture_detector.md#list_fixtures), [`_NEGATIVE`](fixture_detector.md#_NEGATIVE), [`_load_or_build_index`](fixture_detector.md#_load_or_build_index), [`_DISABLED`](fixture_detector.md#_DISABLED), [`fixture_to_verdict`](fixture_detector.md#fixture_to_verdict), [`_check_allowlist`](fixture_detector.md#_check_allowlist)  (16 test-only)

### `_Aggregator`
- def: [`tree_sitter_analyzer/security/fixture_detector.py:508`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/fixture_detector.py#L508)
- members:
  - `record(self, signal: str, confidence: float, where: str)` — [`L516`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/fixture_detector.py#L516)
  - `confidence` — [`L511`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/fixture_detector.py#L511)
  - `evidence` — [`L513`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/fixture_detector.py#L513)
  - `source` — [`L512`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/fixture_detector.py#L512)
  - `suppressed` — [`L514`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/fixture_detector.py#L514)
- used by: [`_scan_tests`](fixture_detector.md#_scan_tests), [`_process_assign`](fixture_detector.md#_process_assign), [`_walk_module`](fixture_detector.md#_walk_module), [`_process_repo_relative_literals`](fixture_detector.md#_process_repo_relative_literals)

## Functions
- `_allowlist_facts(project_root: Path)` — [`L239`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/fixture_detector.py#L239) — Return ``{relative_path: FixtureFact}`` for every allowlist entry.
- `_assignment_target_name(node: ast.Assign)` — [`L660`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/fixture_detector.py#L660) — Return the LHS name for ``X = ...``; ``None`` for tuple/attr targets.
- `_basename_seen_in_tests(project_root: Path, basename: str)` — [`L345`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/fixture_detector.py#L345) — Return whether the filename appears anywhere in tests/ source.
- `_basename_to_repo_relative(basename: str, project_root: Path)` — [`L744`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/fixture_detector.py#L744) — Find the project-relative path for ``basename`` if exactly one exists.
- `_cache_is_readable(cache_path: Path)` — [`L671`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/fixture_detector.py#L671) — Return ``True`` when the fixture cache file parses as expected JSON.
- `_check_allowlist(project_root: Path, relative: str)` — [`L267`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/fixture_detector.py#L267) — Quick path-equality check against the allowlist.
- `_collect_strings(expr: ast.expr)` — [`L686`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/fixture_detector.py#L686) — All ``str`` constants reachable inside ``expr``.
- `_expr_is_path_like(expr: ast.expr, path_names: set[str])` — [`L575`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/fixture_detector.py#L575) — Heuristic: does ``expr`` evaluate to something on the filesystem?
- `_iter_test_files(tests_dir: Path)` — [`L282`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/fixture_detector.py#L282) — Return Python test files while pruning generated and hidden dirs.
- `_load_or_build_index(project_root: Path)` — [`L359`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/fixture_detector.py#L359) — Return the Tier-2 index, building (and caching) on signature change.
- `_plugin_manifest_basenames(node: ast.AST)` — [`L696`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/fixture_detector.py#L696) — If ``node`` is a list/tuple of ≥3 ``*_plugin.py`` literals, return them.
- `_process_assign(node: ast.Assign, source: str, path_names: set[str], relative_test: str, project_root: Path, aggregator: dict[str, _Aggregator])` — [`L597`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/fixture_detector.py#L597) — Extract signals from a top-level ``name = ...`` statement.
- `_process_repo_relative_literals(node: ast.AST, source: str, relative_test: str, project_root: Path, aggregator: dict[str, _Aggregator])` — [`L632`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/fixture_detector.py#L632) — Catch repo-relative string literals outside of fixture-style assigns.
- `_read_cache(cache_path: Path, signature: str)` — [`L391`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/fixture_detector.py#L391) — Return the cached index for ``signature`` or ``None`` on mismatch.
- `_record_path_binding(node: ast.Assign, path_names: set[str])` — [`L565`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/fixture_detector.py#L565) — If ``node`` assigns from ``Path(...)`` or a known path-name, remember it.
- `_safe_relative(path: Path, project_root: Path)` — [`L735`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/fixture_detector.py#L735) — Resolve ``path`` relative to ``project_root`` with a string fallback.
- `_scan_tests(tests_dir: Path, project_root: Path)` — [`L467`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/fixture_detector.py#L467) — Walk ``tests_dir`` and merge signals from every ``*.py`` file.
- `_targeted_fixture_scan(project_root: Path, relative: str)` — [`L305`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/fixture_detector.py#L305) — Fast exact-path scan for the common single-file ``is_fixture`` query.
- `_tests_signature(tests_dir: Path)` — [`L378`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/fixture_detector.py#L378) — Compute a SHA-1 over every ``tests/**/*.py``'s ``(mtime_ns, size)``.
- `_to_relative(file_path: str, project_root: Path)` — [`L723`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/fixture_detector.py#L723) — Best-effort conversion of ``file_path`` to a project-relative form.
- `_walk_module(tree: ast.Module, source: str, relative_test: str, project_root: Path, aggregator: dict[str, _Aggregator])` — [`L524`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/fixture_detector.py#L524) — Inspect the top-level nodes of ``tree`` and update ``aggregator``.
- `_write_cache(cache_path: Path, signature: str, index: dict[str, FixtureFact])` — [`L437`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/fixture_detector.py#L437) — Persist the rebuilt index, swallowing OS-level write failures.
- `fixture_to_verdict(fact: FixtureFact)` — [`L184`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/fixture_detector.py#L184) — Map a :class:`FixtureFact` to a ``safe_to_edit`` verdict override.
- `is_fixture(file_path: str, project_root: str | Path)` — [`L147`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/fixture_detector.py#L147) — Return whether ``file_path`` is a registered or detected fixture.
- `list_fixtures(project_root: str | Path)` — [`L205`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/fixture_detector.py#L205) — Return every detected fixture (Tier 1 ∪ Tier 2) for diagnostics.

## Module values
- `_ALLOWLIST_CONFIDENCE` — [`L76`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/fixture_detector.py#L76)
- `_CACHE_PATH_SUFFIX` — [`L96`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/fixture_detector.py#L96)
- `_CACHE_SCHEMA_VERSION` — [`L97`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/fixture_detector.py#L97)
- `_CONFIDENCE_CAUTION` — [`L74`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/fixture_detector.py#L74)
- `_CONFIDENCE_UNSAFE` — [`L73`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/fixture_detector.py#L73)
- `_CONSTANT_ASSIGNMENT_CONFIDENCE` — [`L78`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/fixture_detector.py#L78)
- `_DISABLED` — [`L133`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/fixture_detector.py#L133)
- `_DISABLE_ENV_VAR` — [`L100`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/fixture_detector.py#L100)
- `_FIXTURE_NAME_PREFIX` — [`L83`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/fixture_detector.py#L83)
- `_NEGATIVE` — [`L125`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/fixture_detector.py#L125)
- `_PATH_LITERAL_CONFIDENCE` — [`L77`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/fixture_detector.py#L77)
- `_PLUGIN_MANIFEST_PATTERN` — [`L88`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/fixture_detector.py#L88)
- `_REPO_RELATIVE_CONFIDENCE` — [`L79`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/fixture_detector.py#L79)
- `_REPO_RELATIVE_PATTERN` — [`L91`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/fixture_detector.py#L91)
- `_TARGETED_SKIP_BASENAMES` — [`L93`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/fixture_detector.py#L93)
- `__all__` — [`L767`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/fixture_detector.py#L767)
- `logger` — [`L68`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/fixture_detector.py#L68)

