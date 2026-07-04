---
title: 'Module: tests/integration/test_real_treesitter_e2e.py'
type: catalog
provenance: extracted
module: tests/integration/test_real_treesitter_e2e.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.test_real_treesitter_e2e`/
symbols:
  TestRealTreeSitterIntegration.test_full_pipeline_parser_output_manager: TestRealTreeSitterIntegration#test_full_pipeline_parser_output_manager().
  TestRealTreeSitterIntegration.test_parse_python_extracts_functions: TestRealTreeSitterIntegration#test_parse_python_extracts_functions().
  TestRealTreeSitterIntegration.test_parse_python_extracts_classes: TestRealTreeSitterIntegration#test_parse_python_extracts_classes().
  SAMPLE_PYTHON: SAMPLE_PYTHON.
  REQUIRES_PYTHON: REQUIRES_PYTHON.
  TestRealTreeSitterIntegration.walk: TestRealTreeSitterIntegration#walk().
  TestRealTreeSitterIntegration.test_parse_python_returns_valid_tree: TestRealTreeSitterIntegration#test_parse_python_returns_valid_tree().
  PYTHON_AVAILABLE: PYTHON_AVAILABLE.
  pytestmark: pytestmark.
  SAMPLE_JAVA: SAMPLE_JAVA.
  TestRealTreeSitterIntegration: TestRealTreeSitterIntegration#
---
# Module: [`tests/integration/test_real_treesitter_e2e.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_real_treesitter_e2e.py)

## Classes
### `TestRealTreeSitterIntegration`
- def: [`tests/integration/test_real_treesitter_e2e.py:88`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_real_treesitter_e2e.py#L88)
- doc: End-to-end: real parse → structured data → formatter output.
- signature: `class TestRealTreeSitterIntegration:`
- members:
  - `test_full_pipeline_parser_output_manager(self)` — [`L156`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_real_treesitter_e2e.py#L156) — Real TSParser parses Python, formatter produces output.
  - `test_parse_python_extracts_classes(self)` — [`L129`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_real_treesitter_e2e.py#L129) — Real parse extracts class nodes.
  - `test_parse_python_extracts_functions(self)` — [`L102`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_real_treesitter_e2e.py#L102) — Real parse extracts function nodes.
  - `test_parse_python_returns_valid_tree(self)` — [`L92`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_real_treesitter_e2e.py#L92) — Real tree-sitter parse yields valid AST.
  - `walk(node)` — [`L110`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_real_treesitter_e2e.py#L110)
- uses (calls/refs, reference-scoped): [`Parser`](../../tree_sitter_analyzer/core/parser.md#Parser), [`FormatterRegistry`](../../tree_sitter_analyzer/formatters/formatter_registry.md#FormatterRegistry), [`tree`](../../tree_sitter_analyzer/core/parser.md#ParseResult.tree), [`success`](../../tree_sitter_analyzer/core/parser.md#ParseResult.success), [`parse_file`](../../tree_sitter_analyzer/core/parser.md#Parser.parse_file), [`format`](../../tree_sitter_analyzer/formatters/_formatter_interface.md#IFormatter.format), [`source_code`](../../tree_sitter_analyzer/core/parser.md#ParseResult.source_code), [`get_formatter`](../../tree_sitter_analyzer/formatters/formatter_registry.md#FormatterRegistry.get_formatter)  (2 test-only)

## Module values
- `PYTHON_AVAILABLE` — [`L25`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_real_treesitter_e2e.py#L25)
- `REQUIRES_PYTHON` — [`L29`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_real_treesitter_e2e.py#L29)
- `SAMPLE_JAVA` — [`L62`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_real_treesitter_e2e.py#L62)
- `SAMPLE_PYTHON` — [`L33`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_real_treesitter_e2e.py#L33)
- `pytestmark` — [`L20`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_real_treesitter_e2e.py#L20)

