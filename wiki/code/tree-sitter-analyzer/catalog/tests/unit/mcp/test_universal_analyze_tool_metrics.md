---
title: 'Module: tests/unit/mcp/test_universal_analyze_tool_metrics.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_universal_analyze_tool_metrics.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_universal_analyze_tool_metrics`/
symbols:
  TestUniversalAnalyzeFindings.test_universal_analyze_counts_comments_and_blanks: TestUniversalAnalyzeFindings#test_universal_analyze_counts_comments_and_blanks().
  TestUniversalAnalyzeFindings.test_universal_analyze_envelope_includes_success_and_summary: TestUniversalAnalyzeFindings#test_universal_analyze_envelope_includes_success_and_summary().
  tool: tool().
  TestUniversalAnalyzeToolExtractBasicMetrics: TestUniversalAnalyzeToolExtractBasicMetrics#
  TestUniversalAnalyzeToolExtractBasicMetrics.test_extract_basic_metrics_empty_elements: TestUniversalAnalyzeToolExtractBasicMetrics#test_extract_basic_metrics_empty_elements().
  TestUniversalAnalyzeToolExtractBasicMetrics.test_extract_basic_metrics_with_elements: TestUniversalAnalyzeToolExtractBasicMetrics#test_extract_basic_metrics_with_elements().
  TestUniversalAnalyzeToolExtractDetailedMetrics: TestUniversalAnalyzeToolExtractDetailedMetrics#
  TestUniversalAnalyzeToolExtractDetailedMetrics.test_extract_detailed_metrics_includes_complexity: TestUniversalAnalyzeToolExtractDetailedMetrics#test_extract_detailed_metrics_includes_complexity().
  TestUniversalAnalyzeToolExtractStructureInfo: TestUniversalAnalyzeToolExtractStructureInfo#
  TestUniversalAnalyzeToolExtractStructureInfo.test_extract_structure_info_empty: TestUniversalAnalyzeToolExtractStructureInfo#test_extract_structure_info_empty().
  TestUniversalAnalyzeToolExtractStructureInfo.test_extract_structure_info_with_classes: TestUniversalAnalyzeToolExtractStructureInfo#test_extract_structure_info_with_classes().
  TestUniversalAnalyzeToolExtractUniversalBasicMetrics: TestUniversalAnalyzeToolExtractUniversalBasicMetrics#
  TestUniversalAnalyzeToolExtractUniversalBasicMetrics.test_extract_universal_basic_metrics_empty: TestUniversalAnalyzeToolExtractUniversalBasicMetrics#test_extract_universal_basic_metrics_empty().
  TestUniversalAnalyzeToolExtractUniversalBasicMetrics.test_extract_universal_basic_metrics_with_elements: TestUniversalAnalyzeToolExtractUniversalBasicMetrics#test_extract_universal_basic_metrics_with_elements().
  TestUniversalAnalyzeToolExtractUniversalDetailedMetrics: TestUniversalAnalyzeToolExtractUniversalDetailedMetrics#
  TestUniversalAnalyzeToolExtractUniversalDetailedMetrics.test_extract_universal_detailed_metrics_with_query_results: TestUniversalAnalyzeToolExtractUniversalDetailedMetrics#test_extract_universal_detailed_metrics_with_query_results().
  TestUniversalAnalyzeToolExtractUniversalStructureInfo: TestUniversalAnalyzeToolExtractUniversalStructureInfo#
  TestUniversalAnalyzeToolExtractUniversalStructureInfo.test_extract_universal_structure_info: TestUniversalAnalyzeToolExtractUniversalStructureInfo#test_extract_universal_structure_info().
  TestUniversalAnalyzeToolGetAvailableQueries: TestUniversalAnalyzeToolGetAvailableQueries#
  TestUniversalAnalyzeToolGetAvailableQueries.test_get_available_queries_java: TestUniversalAnalyzeToolGetAvailableQueries#test_get_available_queries_java().
  TestUniversalAnalyzeToolGetAvailableQueries.test_get_available_queries_python: TestUniversalAnalyzeToolGetAvailableQueries#test_get_available_queries_python().
  TestUniversalAnalyzeFindings: TestUniversalAnalyzeFindings#
---
# Module: [`tests/unit/mcp/test_universal_analyze_tool_metrics.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_universal_analyze_tool_metrics.py)

## Classes
### `TestUniversalAnalyzeFindings`
- def: [`tests/unit/mcp/test_universal_analyze_tool_metrics.py:208`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_universal_analyze_tool_metrics.py#L208)
- doc: Regression tests for round-16b dogfood findings 1 and 2.
- signature: `class TestUniversalAnalyzeFindings:`
- members:
  - `test_universal_analyze_counts_comments_and_blanks(self, tmp_path)` — [`L260`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_universal_analyze_tool_metrics.py#L260) — Finding 1: comment/blank line counts must match analyze_scale.
  - `test_universal_analyze_envelope_includes_success_and_summary(self, tmp_path)` — [`L212`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_universal_analyze_tool_metrics.py#L212) — Finding 2: response must carry success, summary_line, agent_summary.
- uses (calls/refs, reference-scoped): [`AnalyzeScaleTool`](../../../tree_sitter_analyzer/mcp/tools/analyze_scale_tool.md#AnalyzeScaleTool), [`UniversalAnalyzeTool`](../../../tree_sitter_analyzer/mcp/tools/universal_analyze_tool.md#UniversalAnalyzeTool), [`execute`](../../../tree_sitter_analyzer/mcp/tools/analyze_scale_tool.md#AnalyzeScaleTool.execute), [`execute`](../../../tree_sitter_analyzer/mcp/tools/universal_analyze_tool.md#UniversalAnalyzeTool.execute)

### `TestUniversalAnalyzeToolExtractBasicMetrics`
- def: [`tests/unit/mcp/test_universal_analyze_tool_metrics.py:21`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_universal_analyze_tool_metrics.py#L21)
- doc: Tests for _extract_basic_metrics method.
- signature: `class TestUniversalAnalyzeToolExtractBasicMetrics:`
- members:
  - `test_extract_basic_metrics_empty_elements(self, tool)` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_universal_analyze_tool_metrics.py#L24) — Test extracting basic metrics with empty elements.
  - `test_extract_basic_metrics_with_elements(self, tool)` — [`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_universal_analyze_tool_metrics.py#L38) — Test extracting basic metrics with elements.

### `TestUniversalAnalyzeToolExtractDetailedMetrics`
- def: [`tests/unit/mcp/test_universal_analyze_tool_metrics.py:71`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_universal_analyze_tool_metrics.py#L71)
- doc: Tests for _extract_detailed_metrics method.
- signature: `class TestUniversalAnalyzeToolExtractDetailedMetrics:`
- members:
  - `test_extract_detailed_metrics_includes_complexity(self, tool)` — [`L74`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_universal_analyze_tool_metrics.py#L74) — Test detailed metrics include complexity information.

### `TestUniversalAnalyzeToolExtractStructureInfo`
- def: [`tests/unit/mcp/test_universal_analyze_tool_metrics.py:91`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_universal_analyze_tool_metrics.py#L91)
- doc: Tests for _extract_structure_info method.
- signature: `class TestUniversalAnalyzeToolExtractStructureInfo:`
- members:
  - `test_extract_structure_info_empty(self, tool)` — [`L94`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_universal_analyze_tool_metrics.py#L94) — Test extracting structure info with empty elements.
  - `test_extract_structure_info_with_classes(self, tool)` — [`L106`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_universal_analyze_tool_metrics.py#L106) — Test extracting structure info with class elements.

### `TestUniversalAnalyzeToolExtractUniversalBasicMetrics`
- def: [`tests/unit/mcp/test_universal_analyze_tool_metrics.py:123`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_universal_analyze_tool_metrics.py#L123)
- doc: Tests for _extract_universal_basic_metrics method.
- signature: `class TestUniversalAnalyzeToolExtractUniversalBasicMetrics:`
- members:
  - `test_extract_universal_basic_metrics_empty(self, tool)` — [`L126`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_universal_analyze_tool_metrics.py#L126) — Test extracting universal basic metrics with empty elements.
  - `test_extract_universal_basic_metrics_with_elements(self, tool)` — [`L135`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_universal_analyze_tool_metrics.py#L135) — Test extracting universal basic metrics with elements.

### `TestUniversalAnalyzeToolExtractUniversalDetailedMetrics`
- def: [`tests/unit/mcp/test_universal_analyze_tool_metrics.py:153`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_universal_analyze_tool_metrics.py#L153)
- doc: Tests for _extract_universal_detailed_metrics method.
- signature: `class TestUniversalAnalyzeToolExtractUniversalDetailedMetrics:`
- members:
  - `test_extract_universal_detailed_metrics_with_query_results(self, tool)` — [`L156`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_universal_analyze_tool_metrics.py#L156) — Test extracting universal detailed metrics with query results.

### `TestUniversalAnalyzeToolExtractUniversalStructureInfo`
- def: [`tests/unit/mcp/test_universal_analyze_tool_metrics.py:164`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_universal_analyze_tool_metrics.py#L164)
- doc: Tests for _extract_universal_structure_info method.
- signature: `class TestUniversalAnalyzeToolExtractUniversalStructureInfo:`
- members:
  - `test_extract_universal_structure_info(self, tool)` — [`L167`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_universal_analyze_tool_metrics.py#L167) — Test extracting universal structure info.

### `TestUniversalAnalyzeToolGetAvailableQueries`
- def: [`tests/unit/mcp/test_universal_analyze_tool_metrics.py:181`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_universal_analyze_tool_metrics.py#L181)
- doc: Tests for _get_available_queries method.
- signature: `class TestUniversalAnalyzeToolGetAvailableQueries:`
- members:
  - `test_get_available_queries_java(self, tool)` — [`L185`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_universal_analyze_tool_metrics.py#L185) — Test getting available queries for Java.
  - `test_get_available_queries_python(self, tool)` — [`L193`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_universal_analyze_tool_metrics.py#L193) — Test getting available queries for Python.

## Functions
- `tool()` — [`L16`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_universal_analyze_tool_metrics.py#L16) — Create a UniversalAnalyzeTool instance for testing.

