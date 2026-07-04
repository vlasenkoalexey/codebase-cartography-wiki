---
title: 'Module: tests/unit/test_project_graph_coverage.py'
type: catalog
provenance: extracted
module: tests/unit/test_project_graph_coverage.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_project_graph_coverage`/
symbols:
  TestImportResolverPathNormalization.test_file_resolvers_keep_posix_paths_when_path_is_windows: TestImportResolverPathNormalization#test_file_resolvers_keep_posix_paths_when_path_is_windows().
  TestBlastRadiusEdgeCases.test_reverse_nonexistent: TestBlastRadiusEdgeCases#test_reverse_nonexistent().
  TestBlastRadiusEdgeCases.test_analyze_nonexistent: TestBlastRadiusEdgeCases#test_analyze_nonexistent().
  TestDependencyGraphSourceFileIteration.test_iter_source_files_prunes_hidden_and_generated_dirs: TestDependencyGraphSourceFileIteration#test_iter_source_files_prunes_hidden_and_generated_dirs().
  TestDependencyGraphSourceFileIteration.test_is_excluded_handles_paths_outside_project_root: TestDependencyGraphSourceFileIteration#test_is_excluded_handles_paths_outside_project_root().
  TestExtractImportsEdgeCases.test_parse_error_returns_empty: TestExtractImportsEdgeCases#test_parse_error_returns_empty().
  TestDependencyGraphResolvePaths.test_go_resolve_from_fixture: TestDependencyGraphResolvePaths#test_go_resolve_from_fixture().
  FIXTURES_DIR: FIXTURES_DIR.
  TestDependencyGraphResolvePaths._clear_cache: TestDependencyGraphResolvePaths#_clear_cache().
  TestDependencyGraphResolvePaths.test_js_resolve_with_extension: TestDependencyGraphResolvePaths#test_js_resolve_with_extension().
  TestDependencyGraphResolvePaths.test_ts_resolve: TestDependencyGraphResolvePaths#test_ts_resolve().
  TestDependencyGraphResolvePaths.test_go_absolute_import_no_resolve: TestDependencyGraphResolvePaths#test_go_absolute_import_no_resolve().
  TestDependencyGraphResolvePaths.test_rust_resolve_crate: TestDependencyGraphResolvePaths#test_rust_resolve_crate().
  TestDependencyGraphResolvePaths.test_cpp_resolve_include: TestDependencyGraphResolvePaths#test_cpp_resolve_include().
  TestDependencyGraphResolvePaths.test_java_resolve_package: TestDependencyGraphResolvePaths#test_java_resolve_package().
  TestDependencyGraphResolvePaths.test_excluded_dirs_skipped: TestDependencyGraphResolvePaths#test_excluded_dirs_skipped().
  TestCacheKeyFor.test_oserror_returns_none: TestCacheKeyFor#test_oserror_returns_none().
  PY_PROJECT: PY_PROJECT.
  GO_PROJECT: GO_PROJECT.
  JS_PROJECT: JS_PROJECT.
  RUST_PROJECT: RUST_PROJECT.
  CPP_PROJECT: CPP_PROJECT.
  JAVA_PROJECT: JAVA_PROJECT.
  TestLanguageFromExt.test_python: TestLanguageFromExt#test_python().
  TestLanguageFromExt.test_javascript: TestLanguageFromExt#test_javascript().
  TestLanguageFromExt.test_typescript: TestLanguageFromExt#test_typescript().
  TestLanguageFromExt.test_java: TestLanguageFromExt#test_java().
  TestLanguageFromExt.test_go: TestLanguageFromExt#test_go().
  TestLanguageFromExt.test_rust: TestLanguageFromExt#test_rust().
  TestLanguageFromExt.test_c: TestLanguageFromExt#test_c().
  TestLanguageFromExt.test_cpp: TestLanguageFromExt#test_cpp().
  TestLanguageFromExt.test_unknown: TestLanguageFromExt#test_unknown().
  TestLanguageFromExt.test_newly_unlocked_plugins: TestLanguageFromExt#test_newly_unlocked_plugins().
  TestLanguageFromExt.test_case_insensitive: TestLanguageFromExt#test_case_insensitive().
  TestResolveRelativeImport.test_absolute_returns_none: TestResolveRelativeImport#test_absolute_returns_none().
  TestResolveRelativeImport.test_single_dot: TestResolveRelativeImport#test_single_dot().
  TestResolveRelativeImport.test_double_dot: TestResolveRelativeImport#test_double_dot().
  TestResolveRelativeImport.test_triple_dot: TestResolveRelativeImport#test_triple_dot().
  TestResolveRelativeImport.test_with_submodule: TestResolveRelativeImport#test_with_submodule().
  TestExtractImportsEdgeCases.test_auto_detect_language_none: TestExtractImportsEdgeCases#test_auto_detect_language_none().
  TestLanguageFromExt: TestLanguageFromExt#
  TestDependencyGraphSourceFileIteration: TestDependencyGraphSourceFileIteration#
  TestResolveRelativeImport: TestResolveRelativeImport#
  TestImportResolverPathNormalization: TestImportResolverPathNormalization#
  TestExtractImportsEdgeCases: TestExtractImportsEdgeCases#
  TestDependencyGraphResolvePaths: TestDependencyGraphResolvePaths#
  TestCacheKeyFor: TestCacheKeyFor#
  TestBlastRadiusEdgeCases: TestBlastRadiusEdgeCases#
---
# Module: [`tests/unit/test_project_graph_coverage.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph_coverage.py)

## Classes
### `TestBlastRadiusEdgeCases`
- def: [`tests/unit/test_project_graph_coverage.py:280`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph_coverage.py#L280)
- signature: `class TestBlastRadiusEdgeCases:`
- members:
  - `test_analyze_nonexistent(self)` — [`L287`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph_coverage.py#L287)
  - `test_reverse_nonexistent(self)` — [`L281`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph_coverage.py#L281)
- uses (calls/refs, reference-scoped): [`DependencyGraph`](../../tree_sitter_analyzer/project_graph.md#DependencyGraph), [`BlastRadius`](../../tree_sitter_analyzer/project_graph.md#BlastRadius), [`reverse`](../../tree_sitter_analyzer/project_graph.md#BlastRadius.reverse), [`analyze`](../../tree_sitter_analyzer/project_graph.md#BlastRadius.analyze)  (1 test-only)

### `TestCacheKeyFor`
- def: [`tests/unit/test_project_graph_coverage.py:274`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph_coverage.py#L274)
- signature: `class TestCacheKeyFor:`
- members:
  - `test_oserror_returns_none(self)` — [`L275`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph_coverage.py#L275)
- uses (calls/refs, reference-scoped): [`DependencyGraph`](../../tree_sitter_analyzer/project_graph.md#DependencyGraph), [`_cache_key_for`](../../tree_sitter_analyzer/project_graph.md#DependencyGraph._cache_key_for)

### `TestDependencyGraphResolvePaths`
- def: [`tests/unit/test_project_graph_coverage.py:181`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph_coverage.py#L181)
- doc: Cover _resolve_to_project_file for JS/TS, Go, Rust, C/CPP, Java.
- signature: `class TestDependencyGraphResolvePaths:`
- members:
  - `test_cpp_resolve_include(self, tmp_path)` — [`L234`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph_coverage.py#L234)
  - `test_excluded_dirs_skipped(self, tmp_path)` — [`L257`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph_coverage.py#L257)
  - `test_go_absolute_import_no_resolve(self, tmp_path)` — [`L216`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph_coverage.py#L216)
  - `test_go_resolve_from_fixture(self)` — [`L211`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph_coverage.py#L211)
  - `test_java_resolve_package(self, tmp_path)` — [`L244`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph_coverage.py#L244)
  - `test_js_resolve_with_extension(self, tmp_path)` — [`L190`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph_coverage.py#L190)
  - `test_rust_resolve_crate(self, tmp_path)` — [`L223`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph_coverage.py#L223)
  - `test_ts_resolve(self, tmp_path)` — [`L202`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph_coverage.py#L202)
- protocol/private: `_clear_cache`[`L185`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph_coverage.py#L185)
- uses (calls/refs, reference-scoped): [`DependencyGraph`](../../tree_sitter_analyzer/project_graph.md#DependencyGraph), [`nodes`](../../tree_sitter_analyzer/project_graph.md#DependencyGraph.nodes), [`edges`](../../tree_sitter_analyzer/project_graph.md#DependencyGraph.edges), [`_global_cache`](../../tree_sitter_analyzer/project_graph.md#DependencyGraph._global_cache)  (1 test-only)

### `TestDependencyGraphSourceFileIteration`
- def: [`tests/unit/test_project_graph_coverage.py:74`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph_coverage.py#L74)
- signature: `class TestDependencyGraphSourceFileIteration:`
- members:
  - `test_is_excluded_handles_paths_outside_project_root(self, tmp_path)` — [`L94`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph_coverage.py#L94)
  - `test_iter_source_files_prunes_hidden_and_generated_dirs(self, tmp_path)` — [`L75`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph_coverage.py#L75)
- uses (calls/refs, reference-scoped): [`DependencyGraph`](../../tree_sitter_analyzer/project_graph.md#DependencyGraph), [`_global_cache`](../../tree_sitter_analyzer/project_graph.md#DependencyGraph._global_cache), [`is_excluded`](../../tree_sitter_analyzer/project_graph.md#DependencyGraph.is_excluded), [`iter_source_files`](../../tree_sitter_analyzer/project_graph.md#DependencyGraph.iter_source_files)

### `TestExtractImportsEdgeCases`
- def: [`tests/unit/test_project_graph_coverage.py:163`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph_coverage.py#L163)
- signature: `class TestExtractImportsEdgeCases:`
- members:
  - `test_auto_detect_language_none(self, tmp_path)` — [`L164`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph_coverage.py#L164)
  - `test_parse_error_returns_empty(self, tmp_path)` — [`L169`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph_coverage.py#L169)
- uses (calls/refs, reference-scoped): [`DependencyGraph`](../../tree_sitter_analyzer/project_graph.md#DependencyGraph), [`extract_imports_from_file`](../../tree_sitter_analyzer/project_graph.md#extract_imports_from_file), [`_global_cache`](../../tree_sitter_analyzer/project_graph.md#DependencyGraph._global_cache)

### `TestImportResolverPathNormalization`
- def: [`tests/unit/test_project_graph_coverage.py:127`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph_coverage.py#L127)
- signature: `class TestImportResolverPathNormalization:`
- members:
  - `test_file_resolvers_keep_posix_paths_when_path_is_windows(self, monkeypatch)` — [`L128`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph_coverage.py#L128)
- uses (calls/refs, reference-scoped): [`_resolve_js_ts_import`](../../tree_sitter_analyzer/project_graph.md#_resolve_js_ts_import), [`_resolve_c_cpp_import`](../../tree_sitter_analyzer/project_graph.md#_resolve_c_cpp_import), [`_resolve_go_import`](../../tree_sitter_analyzer/project_graph.md#_resolve_go_import), [`_resolve_rust_import`](../../tree_sitter_analyzer/project_graph.md#_resolve_rust_import)

### `TestLanguageFromExt`
- def: [`tests/unit/test_project_graph_coverage.py:26`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph_coverage.py#L26)
- signature: `class TestLanguageFromExt:`
- members:
  - `test_c(self)` — [`L47`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph_coverage.py#L47)
  - `test_case_insensitive(self)` — [`L70`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph_coverage.py#L70)
  - `test_cpp(self)` — [`L51`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph_coverage.py#L51)
  - `test_go(self)` — [`L41`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph_coverage.py#L41)
  - `test_java(self)` — [`L38`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph_coverage.py#L38)
  - `test_javascript(self)` — [`L30`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph_coverage.py#L30)
  - `test_newly_unlocked_plugins(self)` — [`L61`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph_coverage.py#L61)
  - `test_python(self)` — [`L27`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph_coverage.py#L27)
  - `test_rust(self)` — [`L44`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph_coverage.py#L44)
  - `test_typescript(self)` — [`L34`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph_coverage.py#L34)
  - `test_unknown(self)` — [`L55`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph_coverage.py#L55)
- uses (calls/refs, reference-scoped): [`_language_from_ext`](../../tree_sitter_analyzer/project_graph.md#_language_from_ext)

### `TestResolveRelativeImport`
- def: [`tests/unit/test_project_graph_coverage.py:105`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph_coverage.py#L105)
- signature: `class TestResolveRelativeImport:`
- members:
  - `test_absolute_returns_none(self)` — [`L106`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph_coverage.py#L106)
  - `test_double_dot(self)` — [`L114`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph_coverage.py#L114)
  - `test_single_dot(self)` — [`L110`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph_coverage.py#L110)
  - `test_triple_dot(self)` — [`L118`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph_coverage.py#L118)
  - `test_with_submodule(self)` — [`L122`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph_coverage.py#L122)
- uses (calls/refs, reference-scoped): [`_resolve_relative_import`](../../tree_sitter_analyzer/project_graph.md#_resolve_relative_import)

## Module values
- `CPP_PROJECT` — [`L22`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph_coverage.py#L22)
- `FIXTURES_DIR` — [`L17`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph_coverage.py#L17)
- `GO_PROJECT` — [`L20`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph_coverage.py#L20)
- `JAVA_PROJECT` — [`L23`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph_coverage.py#L23)
- `JS_PROJECT` — [`L19`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph_coverage.py#L19)
- `PY_PROJECT` — [`L18`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph_coverage.py#L18)
- `RUST_PROJECT` — [`L21`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_project_graph_coverage.py#L21)

