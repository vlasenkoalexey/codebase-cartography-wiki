---
title: 'Module: tree_sitter_analyzer/mcp/tools/utils/test_discovery_languages.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/utils/test_discovery_languages.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.utils.test_discovery_languages`/
symbols:
  find_language_specific_tests: find_language_specific_tests().
  _find_java_tests: _find_java_tests().
  _add_direct_test_candidate: _add_direct_test_candidate().
  _find_ruby_spec_tests: _find_ruby_spec_tests().
  _add_result: _add_result().
  _mirror_main_to_test_parts: _mirror_main_to_test_parts().
---
# Module: [`tree_sitter_analyzer/mcp/tools/utils/test_discovery_languages.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/test_discovery_languages.py)

## Functions
- `_add_direct_test_candidate(candidate: Path, root: Path, results: list[str])` — [`L78`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/test_discovery_languages.py#L78) — Add a candidate path when it exists.
- `_add_result(results: list[str], candidate: Path, root: Path)` — [`L84`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/test_discovery_languages.py#L84) — Add a test file to results if not already present.
- `_find_java_tests(source_path: Path, stem: str, root: Path, results: list[str])` — [`L44`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/test_discovery_languages.py#L44) — Find Java test files using Maven/Gradle directory conventions.
- `_find_ruby_spec_tests(stem: str, root: Path, results: list[str])` — [`L31`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/test_discovery_languages.py#L31) — Find Ruby spec files under the project spec directory.
- `_mirror_main_to_test_parts(parts: tuple[str, ...])` — [`L65`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/test_discovery_languages.py#L65) — Mirror a Java source path from src/main/java to src/test/java.
- `find_language_specific_tests(source_path: Path, stem: str, language: str, root: Path, python_test_dirs: list[str], results: list[str])` — [`L10`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/test_discovery_languages.py#L10) — Run extra test discovery conventions for languages that need them.

