---
title: 'Module: tests/unit/test_symbol_search_conceptual_demotion.py'
type: catalog
provenance: extracted
module: tests/unit/test_symbol_search_conceptual_demotion.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_symbol_search_conceptual_demotion`/
symbols:
  q3_shaped_project: q3_shaped_project().
  TestConceptualQueryTestDemotion.test_production_symbol_tops_conceptual_query: TestConceptualQueryTestDemotion#test_production_symbol_tops_conceptual_query().
  TestConceptualQueryTestDemotion.test_test_intent_query_still_surfaces_test_symbols: TestConceptualQueryTestDemotion#test_test_intent_query_still_surfaces_test_symbols().
  _Q3_STYLE_QUERY: _Q3_STYLE_QUERY.
  _PROD_SOURCE: _PROD_SOURCE.
  _TEST_SOURCE: _TEST_SOURCE.
  TestConceptualQueryTestDemotion: TestConceptualQueryTestDemotion#
---
# Module: [`tests/unit/test_symbol_search_conceptual_demotion.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbol_search_conceptual_demotion.py)

## Classes
### `TestConceptualQueryTestDemotion`
- def: [`tests/unit/test_symbol_search_conceptual_demotion.py:49`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbol_search_conceptual_demotion.py#L49)
- signature: `class TestConceptualQueryTestDemotion:`
- members:
  - `test_production_symbol_tops_conceptual_query(self, q3_shaped_project)` — [`L51`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbol_search_conceptual_demotion.py#L51) — #607 RED: top-5 was all test functions; production must rank first.
  - `test_test_intent_query_still_surfaces_test_symbols(self, q3_shaped_project)` — [`L71`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbol_search_conceptual_demotion.py#L71) — Counter-direction pin: explicit test-seeking queries keep tests on top.
- uses (calls/refs, reference-scoped): [`CodeGraphSymbolSearchTool`](../../tree_sitter_analyzer/mcp/tools/symbol_search_tool.md#CodeGraphSymbolSearchTool), [`execute`](../../tree_sitter_analyzer/mcp/tools/symbol_search_tool.md#CodeGraphSymbolSearchTool.execute)  (1 test-only)

## Functions
- `q3_shaped_project(tmp_path)` — [`L34`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbol_search_conceptual_demotion.py#L34) — 1 production symbol + 6 token-richer test symbols (pilot Q3 shape).

## Module values
- `_PROD_SOURCE` — [`L21`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbol_search_conceptual_demotion.py#L21)
- `_Q3_STYLE_QUERY` — [`L19`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbol_search_conceptual_demotion.py#L19)
- `_TEST_SOURCE` — [`L23`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbol_search_conceptual_demotion.py#L23)

