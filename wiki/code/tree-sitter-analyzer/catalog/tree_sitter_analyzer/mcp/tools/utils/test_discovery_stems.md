---
title: 'Module: tree_sitter_analyzer/mcp/tools/utils/test_discovery_stems.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/utils/test_discovery_stems.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.utils.test_discovery_stems`/
symbols:
  related_test_stems_for_path: related_test_stems_for_path().
  module_family_test_stems: module_family_test_stems().
  fixture_test_stems: fixture_test_stems().
  python_package_test_stems: python_package_test_stems().
  related_stem_matches: related_stem_matches().
  _unique_nonempty_stems: _unique_nonempty_stems().
  _special_module_family_stems: _special_module_family_stems().
  _stripped_fixture_stems: _stripped_fixture_stems().
  _strip_family_suffixes: _strip_family_suffixes().
---
# Module: [`tree_sitter_analyzer/mcp/tools/utils/test_discovery_stems.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/test_discovery_stems.py)

## Functions
- `_special_module_family_stems(stem: str)` — [`L109`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/test_discovery_stems.py#L109) — Return family stems for helper modules that do not share a direct name.
- `_strip_family_suffixes(stem: str, suffixes: tuple[str, ...])` — [`L134`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/test_discovery_stems.py#L134) — Return stems produced by peeling one or more helper suffixes.
- `_stripped_fixture_stems(part: str)` — [`L116`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/test_discovery_stems.py#L116) — Return useful stems after removing common fixture suffixes.
- `_unique_nonempty_stems(stems: list[str])` — [`L155`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/test_discovery_stems.py#L155) — Return stems without duplicates while preserving order.
- `fixture_test_stems(file_path: str | Path)` — [`L79`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/test_discovery_stems.py#L79) — Return test-name stems implied by a tests/fixtures path.
- `module_family_test_stems(file_path: str | Path)` — [`L32`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/test_discovery_stems.py#L32) — Return broader stems for extracted Python implementation modules.
- `python_package_test_stems(file_path: str | Path)` — [`L16`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/test_discovery_stems.py#L16) — Return package-level test stems for Python plugin-style source modules.
- `related_stem_matches(test_stem: str, related_stem: str)` — [`L100`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/test_discovery_stems.py#L100) — Return True when a derived stem is specific enough for a test name.
- `related_test_stems_for_path(file_path: str | Path)` — [`L8`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/test_discovery_stems.py#L8) — Return non-filename stems that can connect a file to tests.

