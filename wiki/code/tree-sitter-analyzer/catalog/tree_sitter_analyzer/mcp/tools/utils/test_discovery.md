---
title: 'Module: tree_sitter_analyzer/mcp/tools/utils/test_discovery.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/utils/test_discovery.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.utils.test_discovery`/
symbols:
  find_test_files: find_test_files().
  detect_language_from_ext: detect_language_from_ext().
  _find_pattern_tests: _find_pattern_tests().
  _find_symbol_reference_tests: _find_symbol_reference_tests().
  _find_colocated_tests: _find_colocated_tests().
  _add_direct_test_candidate: _add_direct_test_candidate().
  _add_result: _add_result().
  _find_recursive_test_candidates: _find_recursive_test_candidates().
  _TEST_DIRS._TEST_DIRS: _TEST_DIRS._TEST_DIRS.
  _format_pattern: _format_pattern().
  _python_public_symbols: _python_public_symbols().
  _TEST_PATTERNS._TEST_PATTERNS: _TEST_PATTERNS._TEST_PATTERNS.
  _EXT_TO_LANG._EXT_TO_LANG: _EXT_TO_LANG._EXT_TO_LANG.
  __all__: __all__.
---
# Module: [`tree_sitter_analyzer/mcp/tools/utils/test_discovery.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/test_discovery.py)

## Functions
- `_add_direct_test_candidate(candidate: Path, root: Path, results: list[str])` — [`L149`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/test_discovery.py#L149) — Add a candidate path when it exists.
- `_add_result(results: list[str], candidate: Path, root: Path)` — [`L188`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/test_discovery.py#L188) — Add a test file to results if not already present.
- `_find_colocated_tests(source_path: Path, stem: str, patterns: list[str], root: Path, results: list[str])` — [`L170`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/test_discovery.py#L170) — Find tests next to the source file.
- `_find_pattern_tests(root: Path, stem: str, patterns: list[str], test_dirs: list[str], results: list[str])` — [`L132`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/test_discovery.py#L132) — Find tests in common test directories using language patterns.
- `_find_recursive_test_candidates(test_dir: Path, test_filename: str, root: Path, results: list[str])` — [`L155`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/test_discovery.py#L155) — Find matching tests recursively within a test directory.
- `_find_symbol_reference_tests(source_path: Path, language: str, root: Path, results: list[str])` — [`L204`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/test_discovery.py#L204) — Union proximity matches with tests that reference public source symbols.
- `_format_pattern(pattern: str, stem: str)` — [`L183`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/test_discovery.py#L183) — Format a test file pattern with the source file stem.
- `_python_public_symbols(source_path: Path)` — [`L236`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/test_discovery.py#L236) — Extract public Python def/class names with a cheap line-based scan.
- `detect_language_from_ext(ext: str)` — [`L91`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/test_discovery.py#L91) — Map file extension to language name.
- `find_test_files(file_path: str, project_root: str)` — [`L96`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/test_discovery.py#L96) — Find test files for the given source file, language-aware.

## Module values
- `_EXT_TO_LANG` — [`L70`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/test_discovery.py#L70)
- `_TEST_DIRS` — [`L54`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/test_discovery.py#L54)
- `_TEST_PATTERNS` — [`L33`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/test_discovery.py#L33)
- `__all__` — [`L22`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/test_discovery.py#L22)

