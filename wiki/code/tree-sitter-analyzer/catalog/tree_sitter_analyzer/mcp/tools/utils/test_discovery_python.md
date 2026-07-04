---
title: 'Module: tree_sitter_analyzer/mcp/tools/utils/test_discovery_python.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/utils/test_discovery_python.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.utils.test_discovery_python`/
symbols:
  _find_python_package_tests: _find_python_package_tests().
  find_python_specific_tests: find_python_specific_tests().
  _add_stem_named_tests: _add_stem_named_tests().
  _find_fixture_tests: _find_fixture_tests().
  _find_python_family_tests: _find_python_family_tests().
  _add_pattern_matches: _add_pattern_matches().
  _iter_pattern_matches: _iter_pattern_matches().
  _iter_python_test_files: _iter_python_test_files().
  _matches_any_stem: _matches_any_stem().
  _existing_test_dirs: _existing_test_dirs().
  _relative_to_root: _relative_to_root().
  _add_result: _add_result().
  _unique_stems: _unique_stems().
---
# Module: [`tree_sitter_analyzer/mcp/tools/utils/test_discovery_python.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/test_discovery_python.py)

## Functions
- `_add_pattern_matches(root: Path, test_dirs: list[str], patterns: list[str], results: list[str])` — [`L80`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/test_discovery_python.py#L80) — Add tests matching one of the provided glob patterns.
- `_add_result(results: list[str], candidate: Path, root: Path)` — [`L160`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/test_discovery_python.py#L160) — Add a test file to results if not already present.
- `_add_stem_named_tests(root: Path, test_dirs: list[str], stems: list[str], results: list[str])` — [`L93`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/test_discovery_python.py#L93) — Add tests whose test module stem matches one of the source stems.
- `_existing_test_dirs(root: Path, test_dirs: list[str])` — [`L130`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/test_discovery_python.py#L130) — Return test directories that exist in the project.
- `_find_fixture_tests(source_path: Path, root: Path, test_dirs: list[str], results: list[str])` — [`L51`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/test_discovery_python.py#L51) — Find tests that name the domain of a file under tests/fixtures.
- `_find_python_family_tests(source_path: Path, root: Path, test_dirs: list[str], results: list[str])` — [`L68`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/test_discovery_python.py#L68) — Find tests for extracted helper modules that share a family stem.
- `_find_python_package_tests(source_path: Path, root: Path, test_dirs: list[str], results: list[str])` — [`L32`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/test_discovery_python.py#L32) — Find package-level tests for plugin-style source modules.
- `_iter_pattern_matches(root: Path, test_dirs: list[str], patterns: list[str])` — [`L107`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/test_discovery_python.py#L107) — Return sorted test files matching any glob pattern.
- `_iter_python_test_files(root: Path, test_dirs: list[str])` — [`L121`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/test_discovery_python.py#L121) — Return sorted Python test files from existing test directories.
- `_matches_any_stem(test_stem: str, stems: list[str])` — [`L135`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/test_discovery_python.py#L135) — Return True when a test stem is related to any source stem.
- `_relative_to_root(path: Path, root: Path)` — [`L152`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/test_discovery_python.py#L152) — Return path relative to root, or None for external paths.
- `_unique_stems(stems: list[str])` — [`L140`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/test_discovery_python.py#L140) — Return non-empty stems without duplicates, preserving order.
- `find_python_specific_tests(source_path: Path, root: Path, test_dirs: list[str], results: list[str])` — [`L15`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/test_discovery_python.py#L15) — Find Python tests that need project-aware conventions.

