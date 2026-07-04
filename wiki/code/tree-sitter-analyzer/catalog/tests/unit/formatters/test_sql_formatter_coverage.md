---
title: 'Module: tests/unit/formatters/test_sql_formatter_coverage.py'
type: catalog
provenance: extracted
module: tests/unit/formatters/test_sql_formatter_coverage.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.formatters.test_sql_formatter_coverage`/TestSQLFormatterCoverage#
symbols:
  TestSQLFormatterCoverage.test_format_overview_table_complex_elements: test_format_overview_table_complex_elements().
  TestSQLFormatterCoverage.test_format_analysis_result_empty: test_format_analysis_result_empty().
  TestSQLFormatterCoverage.test_format_analysis_result_no_sql_elements.DummyElement.name: test_format_analysis_result_no_sql_elements().DummyElement#name.
  TestSQLFormatterCoverage.test_format_empty_file: test_format_empty_file().
  TestSQLFormatterCoverage.test_base_formatter_not_implemented: test_base_formatter_not_implemented().
  TestSQLFormatterCoverage.test_format_analysis_result_no_sql_elements: test_format_analysis_result_no_sql_elements().
  TestSQLFormatterCoverage.test_format_analysis_result_no_sql_elements.DummyElement: test_format_analysis_result_no_sql_elements().DummyElement#
  TestSQLFormatterCoverage: ''
---
# Module: [`tests/unit/formatters/test_sql_formatter_coverage.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_coverage.py)

## Classes
### `DummyElement`
- def: [`tests/unit/formatters/test_sql_formatter_coverage.py:49`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_coverage.py#L49)
- signature: `class DummyElement:`
- members:
  - `name` — [`L50`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_coverage.py#L50)
- uses (calls/refs, reference-scoped): [`AnalysisResult`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult), [`elements`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.elements), [`language`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.language), [`file_path`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.file_path), [`success`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.success), [`line_count`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.line_count), [`error_message`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.error_message), [`source_code`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.source_code), [`node_count`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.node_count), [`query_results`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.query_results), [`format_analysis_result`](../../../tree_sitter_analyzer/formatters/sql_formatters.md#SQLFullFormatter.format_analysis_result)

### `TestSQLFormatterCoverage`
- def: [`tests/unit/formatters/test_sql_formatter_coverage.py:18`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_coverage.py#L18)
- signature: `class TestSQLFormatterCoverage:`
- members:
  - `test_base_formatter_not_implemented(self)` — [`L123`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_coverage.py#L123)
  - `test_format_analysis_result_empty(self)` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_coverage.py#L25)
  - `test_format_analysis_result_no_sql_elements(self)` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_coverage.py#L45)
  - `test_format_empty_file(self)` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_coverage.py#L19)
  - `test_format_overview_table_complex_elements(self)` — [`L66`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_coverage.py#L66)
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`start_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`end_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.end_line), [`language`](../../../tree_sitter_analyzer/models/base.md#CodeElement.language), [`AnalysisResult`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult), [`raw_text`](../../../tree_sitter_analyzer/models/base.md#CodeElement.raw_text), [`elements`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.elements), [`language`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.language), [`file_path`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.file_path), [`success`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.success), [`line_count`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.line_count), [`error_message`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.error_message), [`SQLTable`](../../../tree_sitter_analyzer/models/sql_models.md#SQLTable), [`source_code`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.source_code), [`node_count`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.node_count), [`SQLFunction`](../../../tree_sitter_analyzer/models/sql_models.md#SQLFunction), [`dependencies`](../../../tree_sitter_analyzer/models/sql_models.md#SQLElement.dependencies), [`SQLView`](../../../tree_sitter_analyzer/models/sql_models.md#SQLView), [`SQLIndex`](../../../tree_sitter_analyzer/models/sql_models.md#SQLIndex), [`parameters`](../../../tree_sitter_analyzer/models/sql_models.md#SQLElement.parameters), [`columns`](../../../tree_sitter_analyzer/models/sql_models.md#SQLElement.columns), [`format_elements`](../../../tree_sitter_analyzer/formatters/sql_formatters.md#SQLFormatterBase.format_elements), [`query_results`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.query_results), [`SQLParameter`](../../../tree_sitter_analyzer/models/sql_models.md#SQLParameter), [`SQLFullFormatter`](../../../tree_sitter_analyzer/formatters/sql_formatters.md#SQLFullFormatter), [`SQLColumn`](../../../tree_sitter_analyzer/models/sql_models.md#SQLColumn), [`name`](../../../tree_sitter_analyzer/models/sql_models.md#SQLColumn.name), [`table_name`](../../../tree_sitter_analyzer/models/sql_models.md#SQLElement.table_name), [`data_type`](../../../tree_sitter_analyzer/models/sql_models.md#SQLColumn.data_type), [`name`](../../../tree_sitter_analyzer/models/sql_models.md#SQLParameter.name), [`_format_grouped_elements`](../../../tree_sitter_analyzer/formatters/sql_formatters.md#SQLFormatterBase._format_grouped_elements), [`data_type`](../../../tree_sitter_analyzer/models/sql_models.md#SQLParameter.data_type), [`indexed_columns`](../../../tree_sitter_analyzer/models/sql_models.md#SQLIndex.indexed_columns), [`source_tables`](../../../tree_sitter_analyzer/models/sql_models.md#SQLView.source_tables), [`SQLFormatterBase`](../../../tree_sitter_analyzer/formatters/sql_formatters.md#SQLFormatterBase), [`constraints`](../../../tree_sitter_analyzer/models/sql_models.md#SQLElement.constraints), [`is_unique`](../../../tree_sitter_analyzer/models/sql_models.md#SQLIndex.is_unique), [`format_analysis_result`](../../../tree_sitter_analyzer/formatters/sql_formatters.md#SQLFullFormatter.format_analysis_result)

