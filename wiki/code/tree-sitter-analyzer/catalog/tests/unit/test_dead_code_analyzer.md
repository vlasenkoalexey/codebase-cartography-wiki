---
title: 'Module: tests/unit/test_dead_code_analyzer.py'
type: catalog
provenance: extracted
module: tests/unit/test_dead_code_analyzer.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_dead_code_analyzer`/
symbols:
  TestDeadCodeErrorHandling.test_nonexistent_directory_returns_empty: TestDeadCodeErrorHandling#test_nonexistent_directory_returns_empty().
  test_excludes_dot_prefixed_vendored_dirs: test_excludes_dot_prefixed_vendored_dirs().
  TestFindTransitiveDeadCode.test_propagates_to_callees: TestFindTransitiveDeadCode#test_propagates_to_callees().
  TestFindUnusedImports.test_detects_unused_import: TestFindUnusedImports#test_detects_unused_import().
  TestFindUnreferencedVariables.test_detects_unreferenced_assignment: TestFindUnreferencedVariables#test_detects_unreferenced_assignment().
  TestFindTransitiveDeadCode.test_finds_root_dead_function: TestFindTransitiveDeadCode#test_finds_root_dead_function().
  TestFindUnusedImports.test_multiple_unused_names: TestFindUnusedImports#test_multiple_unused_names().
  TestAnalyzeDeadCode.test_returns_dead_code_result: TestAnalyzeDeadCode#test_returns_dead_code_result().
  TestAnalyzeDeadCode.test_excludes_dirs: TestAnalyzeDeadCode#test_excludes_dirs().
  TestFindTransitiveDeadCode.test_excludes_test_files_when_flag_set: TestFindTransitiveDeadCode#test_excludes_test_files_when_flag_set().
  TestFindTransitiveDeadCode.test_entry_points_are_not_dead: TestFindTransitiveDeadCode#test_entry_points_are_not_dead().
  TestAnalyzeDeadCode.test_stats_populated: TestAnalyzeDeadCode#test_stats_populated().
  TestDeadCodeErrorHandling.test_binary_file_skipped: TestDeadCodeErrorHandling#test_binary_file_skipped().
  TestDeadCodeErrorHandling.test_symlink_handled: TestDeadCodeErrorHandling#test_symlink_handled().
  test_exclude_dirs_is_canonical_constant: test_exclude_dirs_is_canonical_constant().
  TestIsTestFile.test_prefixed_test_file: TestIsTestFile#test_prefixed_test_file().
  TestIsTestFile.test_suffixed_test_file: TestIsTestFile#test_suffixed_test_file().
  TestIsTestFile.test_spec_file: TestIsTestFile#test_spec_file().
  TestIsTestFile.test_test_directory: TestIsTestFile#test_test_directory().
  TestIsTestFile.test_regular_file: TestIsTestFile#test_regular_file().
  TestIsTestFile.test_nested_test_dir: TestIsTestFile#test_nested_test_dir().
  TestIsKnownEntry.test_python_main: TestIsKnownEntry#test_python_main().
  TestIsKnownEntry.test_python_setup: TestIsKnownEntry#test_python_setup().
  TestIsKnownEntry.test_java_init: TestIsKnownEntry#test_java_init().
  TestIsKnownEntry.test_javascript_handler: TestIsKnownEntry#test_javascript_handler().
  TestIsKnownEntry.test_go_testmain: TestIsKnownEntry#test_go_testmain().
  TestIsKnownEntry.test_unknown_language: TestIsKnownEntry#test_unknown_language().
  TestIsKnownEntry.test_non_entry_name: TestIsKnownEntry#test_non_entry_name().
  TestFindTransitiveDeadCode.simple_graph: TestFindTransitiveDeadCode#simple_graph().
  TestFindUnusedImports.test_used_import_not_flagged: TestFindUnusedImports#test_used_import_not_flagged().
  TestFindUnusedImports.test_unreadable_file_returns_empty: TestFindUnusedImports#test_unreadable_file_returns_empty().
  TestFindUnreferencedVariables.test_referenced_variable_not_flagged: TestFindUnreferencedVariables#test_referenced_variable_not_flagged().
  TestFindUnreferencedVariables.test_class_attribute_not_flagged_as_unreferenced: TestFindUnreferencedVariables#test_class_attribute_not_flagged_as_unreferenced().
  test_exclude_dirs_covers_previously_excluded_dirs: test_exclude_dirs_covers_previously_excluded_dirs().
  TestIsTestFile: TestIsTestFile#
  TestIsKnownEntry: TestIsKnownEntry#
  TestFindTransitiveDeadCode: TestFindTransitiveDeadCode#
  TestFindUnusedImports: TestFindUnusedImports#
  TestFindUnreferencedVariables: TestFindUnreferencedVariables#
  TestAnalyzeDeadCode: TestAnalyzeDeadCode#
  TestDeadCodeErrorHandling: TestDeadCodeErrorHandling#
---
# Module: [`tests/unit/test_dead_code_analyzer.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_dead_code_analyzer.py)

## Classes
### `TestAnalyzeDeadCode`
- def: [`tests/unit/test_dead_code_analyzer.py:225`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_dead_code_analyzer.py#L225)
- signature: `class TestAnalyzeDeadCode:`
- members:
  - `test_excludes_dirs(self, tmp_path)` — [`L251`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_dead_code_analyzer.py#L251) — node_modules/.git etc. should be excluded from analysis.
  - `test_returns_dead_code_result(self, tmp_path)` — [`L226`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_dead_code_analyzer.py#L226) — Top-level entry should return a DeadCodeResult.
  - `test_stats_populated(self, tmp_path)` — [`L236`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_dead_code_analyzer.py#L236) — The stats dict should contain file/function counts.
- uses (calls/refs, reference-scoped): [`analyze_dead_code`](../../tree_sitter_analyzer/dead_code_analyzer.md#analyze_dead_code), [`dead_functions`](../../tree_sitter_analyzer/dead_code_analyzer.md#DeadCodeResult.dead_functions), [`DeadCodeResult`](../../tree_sitter_analyzer/dead_code_analyzer.md#DeadCodeResult), [`stats`](../../tree_sitter_analyzer/dead_code_analyzer.md#DeadCodeResult.stats)

### `TestDeadCodeErrorHandling`
- def: [`tests/unit/test_dead_code_analyzer.py:269`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_dead_code_analyzer.py#L269)
- signature: `class TestDeadCodeErrorHandling:`
- members:
  - `test_binary_file_skipped(self, tmp_path)` — [`L279`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_dead_code_analyzer.py#L279) — Binary files should be silently skipped.
  - `test_nonexistent_directory_returns_empty(self)` — [`L270`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_dead_code_analyzer.py#L270) — Passing a path that does not exist should not crash.
  - `test_symlink_handled(self, tmp_path)` — [`L288`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_dead_code_analyzer.py#L288) — Symlinked files should not cause infinite loops.
- uses (calls/refs, reference-scoped): [`analyze_dead_code`](../../tree_sitter_analyzer/dead_code_analyzer.md#analyze_dead_code), [`dead_functions`](../../tree_sitter_analyzer/dead_code_analyzer.md#DeadCodeResult.dead_functions), [`stats`](../../tree_sitter_analyzer/dead_code_analyzer.md#DeadCodeResult.stats), [`unreferenced_variables`](../../tree_sitter_analyzer/dead_code_analyzer.md#DeadCodeResult.unreferenced_variables), [`unused_imports`](../../tree_sitter_analyzer/dead_code_analyzer.md#DeadCodeResult.unused_imports)

### `TestFindTransitiveDeadCode`
- def: [`tests/unit/test_dead_code_analyzer.py:76`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_dead_code_analyzer.py#L76)
- doc: Test transitive dead-code detection via a mock CallGraph.
- signature: `class TestFindTransitiveDeadCode:`
- members:
  - `simple_graph(self, tmp_path)` — [`L80`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_dead_code_analyzer.py#L80) — Create a project with two files: one calling the other.
  - `test_entry_points_are_not_dead(self, tmp_path)` — [`L121`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_dead_code_analyzer.py#L121) — Known entry-point names should not be flagged.
  - `test_excludes_test_files_when_flag_set(self, tmp_path)` — [`L112`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_dead_code_analyzer.py#L112) — When include_test_files=False, test-file functions are excluded.
  - `test_finds_root_dead_function(self, simple_graph)` — [`L95`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_dead_code_analyzer.py#L95) — Functions never called from outside should be flagged dead.
  - `test_propagates_to_callees(self, simple_graph)` — [`L103`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_dead_code_analyzer.py#L103) — Functions only called from dead functions should also be dead.
- uses (calls/refs, reference-scoped): [`FunctionRef`](../../tree_sitter_analyzer/call_graph.md#FunctionRef), [`CallGraph`](../../tree_sitter_analyzer/call_graph.md#CallGraph), [`find_transitive_dead_code`](../../tree_sitter_analyzer/dead_code_analyzer.md#find_transitive_dead_code), [`dead_callees`](../../tree_sitter_analyzer/dead_code_analyzer.md#DeadFunction.dead_callees), [`reason`](../../tree_sitter_analyzer/dead_code_analyzer.md#DeadFunction.reason)

### `TestFindUnreferencedVariables`
- def: [`tests/unit/test_dead_code_analyzer.py:193`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_dead_code_analyzer.py#L193)
- signature: `class TestFindUnreferencedVariables:`
- members:
  - `test_class_attribute_not_flagged_as_unreferenced(self, tmp_path)` — [`L212`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_dead_code_analyzer.py#L212) — Class body assignments are NOT module-level variables.
  - `test_detects_unreferenced_assignment(self, tmp_path)` — [`L194`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_dead_code_analyzer.py#L194) — A module-level variable never referenced should be flagged.
  - `test_referenced_variable_not_flagged(self, tmp_path)` — [`L205`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_dead_code_analyzer.py#L205) — A variable used in a function body should NOT be flagged.
- uses (calls/refs, reference-scoped): [`find_unreferenced_variables`](../../tree_sitter_analyzer/dead_code_analyzer.md#find_unreferenced_variables), [`file`](../../tree_sitter_analyzer/dead_code_analyzer.md#UnreferencedVariable.file), [`line`](../../tree_sitter_analyzer/dead_code_analyzer.md#UnreferencedVariable.line), [`name`](../../tree_sitter_analyzer/dead_code_analyzer.md#UnreferencedVariable.name)

### `TestFindUnusedImports`
- def: [`tests/unit/test_dead_code_analyzer.py:136`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_dead_code_analyzer.py#L136)
- signature: `class TestFindUnusedImports:`
- members:
  - `test_detects_unused_import(self, tmp_path)` — [`L137`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_dead_code_analyzer.py#L137) — A file importing `os` but never referencing it should report unused.
  - `test_multiple_unused_names(self, tmp_path)` — [`L159`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_dead_code_analyzer.py#L159) — `from x import a, b, c` where only a is used should flag b, c.
  - `test_unreadable_file_returns_empty(self, tmp_path)` — [`L180`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_dead_code_analyzer.py#L180) — A binary or unreadable file should produce an empty list, not crash.
  - `test_used_import_not_flagged(self, tmp_path)` — [`L150`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_dead_code_analyzer.py#L150) — An import that IS referenced in code should not be flagged.
- uses (calls/refs, reference-scoped): [`find_unused_imports`](../../tree_sitter_analyzer/dead_code_analyzer.md#find_unused_imports), [`file`](../../tree_sitter_analyzer/dead_code_analyzer.md#UnusedImport.file), [`line`](../../tree_sitter_analyzer/dead_code_analyzer.md#UnusedImport.line), [`unused_names`](../../tree_sitter_analyzer/dead_code_analyzer.md#UnusedImport.unused_names)

### `TestIsKnownEntry`
- def: [`tests/unit/test_dead_code_analyzer.py:48`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_dead_code_analyzer.py#L48)
- signature: `class TestIsKnownEntry:`
- members:
  - `test_go_testmain(self)` — [`L61`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_dead_code_analyzer.py#L61)
  - `test_java_init(self)` — [`L55`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_dead_code_analyzer.py#L55)
  - `test_javascript_handler(self)` — [`L58`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_dead_code_analyzer.py#L58)
  - `test_non_entry_name(self)` — [`L67`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_dead_code_analyzer.py#L67)
  - `test_python_main(self)` — [`L49`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_dead_code_analyzer.py#L49)
  - `test_python_setup(self)` — [`L52`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_dead_code_analyzer.py#L52)
  - `test_unknown_language(self)` — [`L64`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_dead_code_analyzer.py#L64)
- uses (calls/refs, reference-scoped): [`_is_known_entry`](../../tree_sitter_analyzer/dead_code_analyzer.md#_is_known_entry)

### `TestIsTestFile`
- def: [`tests/unit/test_dead_code_analyzer.py:23`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_dead_code_analyzer.py#L23)
- signature: `class TestIsTestFile:`
- members:
  - `test_nested_test_dir(self)` — [`L39`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_dead_code_analyzer.py#L39)
  - `test_prefixed_test_file(self)` — [`L24`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_dead_code_analyzer.py#L24)
  - `test_regular_file(self)` — [`L36`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_dead_code_analyzer.py#L36)
  - `test_spec_file(self)` — [`L30`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_dead_code_analyzer.py#L30)
  - `test_suffixed_test_file(self)` — [`L27`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_dead_code_analyzer.py#L27)
  - `test_test_directory(self)` — [`L33`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_dead_code_analyzer.py#L33)
- uses (calls/refs, reference-scoped): [`_is_test_file`](../../tree_sitter_analyzer/dead_code_analyzer.md#_is_test_file)

## Functions
- `test_exclude_dirs_covers_previously_excluded_dirs()` — [`L350`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_dead_code_analyzer.py#L350) — Migrating to the canonical constant must not lose any directory that
- `test_exclude_dirs_is_canonical_constant()` — [`L340`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_dead_code_analyzer.py#L340) — dead_code_analyzer must source its excluded-dir set from the single
- `test_excludes_dot_prefixed_vendored_dirs(tmp_path)` — [`L300`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_dead_code_analyzer.py#L300) — F2 regression: dead-code analysis must not walk into hidden/vendored

