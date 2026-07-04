---
title: 'Module: tree_sitter_analyzer/formatters/sql_formatters.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/formatters/sql_formatters.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.formatters.sql_formatters`/SQL
symbols:
  SQLFullFormatter._format_element_details: FullFormatter#_format_element_details().
  SQLFormatterBase.format_elements: FormatterBase#format_elements().
  SQLFullFormatter: FullFormatter#
  SQLFullFormatter._format_grouped_elements: FullFormatter#_format_grouped_elements().
  SQLFullFormatter._format_overview_table: FullFormatter#_format_overview_table().
  SQLCSVFormatter._format_grouped_elements: CSVFormatter#_format_grouped_elements().
  SQLFullFormatter._format_table_details: FullFormatter#_format_table_details().
  SQLFullFormatter._get_section_title: FullFormatter#_get_section_title().
  SQLFormatterBase._format_grouped_elements: FormatterBase#_format_grouped_elements().
  SQLFullFormatter._format_element_section: FullFormatter#_format_element_section().
  SQLFullFormatter._format_function_details: FullFormatter#_format_function_details().
  SQLFullFormatter._format_trigger_details: FullFormatter#_format_trigger_details().
  SQLFormatterBase: FormatterBase#
  SQLCompactFormatter: CompactFormatter#
  SQLCSVFormatter: CSVFormatter#
  SQLCSVFormatter.format_elements: CSVFormatter#format_elements().
  SQLFullFormatter._format_view_details: FullFormatter#_format_view_details().
  SQLFullFormatter._format_procedure_details: FullFormatter#_format_procedure_details().
  SQLFullFormatter._format_index_details: FullFormatter#_format_index_details().
  SQLFormatterBase.group_elements_by_type: FormatterBase#group_elements_by_type().
  SQLFullFormatter.format_analysis_result: FullFormatter#format_analysis_result().
  SQLCompactFormatter._format_grouped_elements: CompactFormatter#_format_grouped_elements().
  SQLCompactFormatter._format_compact_details: CompactFormatter#_format_compact_details().
  SQLFormatterBase._format_empty_file: FormatterBase#_format_empty_file().
  SQLCompactFormatter.format_analysis_result: CompactFormatter#format_analysis_result().
  SQLCSVFormatter.format_analysis_result: CSVFormatter#format_analysis_result().
---
# Module: [`tree_sitter_analyzer/formatters/sql_formatters.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/sql_formatters.py)

## Classes
### `SQLCSVFormatter`  ·  implements/extends SQLFormatterBase
- def: [`tree_sitter_analyzer/formatters/sql_formatters.py:356`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/sql_formatters.py#L356)
- doc: CSV format for data processing
- signature: `class SQLCSVFormatter(SQLFormatterBase):`
- members:
  - `_format_grouped_elements(self, grouped_elements: dict[SQLElementType, list[SQLElement]], file_path: str)` — [`L388`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/sql_formatters.py#L388) — Format elements as CSV
  - `format_analysis_result(self, analysis_result: Any, table_type: str = "csv")` — [`L359`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/sql_formatters.py#L359) — Format AnalysisResult directly for SQL files.
  - `format_elements(self, elements: list[SQLElement], file_path: str = "")` — [`L376`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/sql_formatters.py#L376) — Format SQL elements as CSV - override to always include header
- uses (calls/refs, reference-scoped): [`name`](../models/base.md#CodeElement.name), [`start_line`](../models/base.md#CodeElement.start_line), [`end_line`](../models/base.md#CodeElement.end_line), [`SQLElementType`](../models/sql_models.md#SQLElementType), [`SQLElement`](../models/sql_models.md#SQLElement), [`sql_element_type`](../models/sql_models.md#SQLElement.sql_element_type), [`SQLFormatterBase`](sql_formatters.md#SQLFormatterBase), [`format_sql_csv_details`](_sql_formatters_helpers.md#format_sql_csv_details), [`group_elements_by_type`](sql_formatters.md#SQLFormatterBase.group_elements_by_type), [`iter_sql_elements_by_line`](_sql_formatters_helpers.md#iter_sql_elements_by_line), [`format_sql_csv_dependencies`](_sql_formatters_helpers.md#format_sql_csv_dependencies)
- used by: [`format_elements`](sql_formatters.md#SQLFormatterBase.format_elements), [`_format_grouped_elements`](sql_formatters.md#SQLFormatterBase._format_grouped_elements), [`_formatters`](sql_formatter_wrapper.md#SQLFormatterWrapper._formatters), [`SQLFormatterBase`](sql_formatters.md#SQLFormatterBase)  (5 test-only)

### `SQLCompactFormatter`  ·  implements/extends SQLFormatterBase
- def: [`tree_sitter_analyzer/formatters/sql_formatters.py:302`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/sql_formatters.py#L302)
- doc: Compact SQL format for quick overview
- signature: `class SQLCompactFormatter(SQLFormatterBase):`
- members:
  - `_format_compact_details(self, element: SQLElement)` — [`L351`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/sql_formatters.py#L351) — Format compact details for an element
  - `_format_grouped_elements(self, grouped_elements: dict[SQLElementType, list[SQLElement]], file_path: str)` — [`L324`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/sql_formatters.py#L324) — Format elements in compact table format
  - `format_analysis_result(self, analysis_result: Any, table_type: str = "compact")` — [`L305`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/sql_formatters.py#L305) — Format AnalysisResult directly for SQL files.
- uses (calls/refs, reference-scoped): [`SQLElementType`](../models/sql_models.md#SQLElementType), [`SQLElement`](../models/sql_models.md#SQLElement), [`format_elements`](sql_formatters.md#SQLFormatterBase.format_elements), [`format_sql_compact_details`](_sql_formatters_helpers.md#format_sql_compact_details), [`SQLFormatterBase`](sql_formatters.md#SQLFormatterBase), [`_format_empty_file`](sql_formatters.md#SQLFormatterBase._format_empty_file)
- used by: [`_format_grouped_elements`](sql_formatters.md#SQLFormatterBase._format_grouped_elements), [`_formatters`](sql_formatter_wrapper.md#SQLFormatterWrapper._formatters), [`SQLFormatterBase`](sql_formatters.md#SQLFormatterBase)  (5 test-only)

### `SQLFormatterBase`
- def: [`tree_sitter_analyzer/formatters/sql_formatters.py:32`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/sql_formatters.py#L32)
- doc: Base class for SQL-specific formatters
- signature: `class SQLFormatterBase:`
- members:
  - `_format_empty_file(self, file_path: str)` — [`L63`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/sql_formatters.py#L63) — Format empty SQL file
  - `_format_grouped_elements(self, grouped_elements: dict[SQLElementType, list[SQLElement]], file_path: str)` — [`L68`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/sql_formatters.py#L68) — Format grouped elements - to be implemented by subclasses
  - `format_elements(self, elements: list[SQLElement], file_path: str = "")` — [`L35`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/sql_formatters.py#L35) — Format SQL elements with appropriate terminology — documented in [tree_sitter_analyzer-models-sql_models](../../../concepts/tree_sitter_analyzer-models-sql_models.md)
  - `group_elements_by_type(self, elements: list[Any])` — [`L46`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/sql_formatters.py#L46) — Group elements by SQL type
- uses (calls/refs, reference-scoped): [`SQLElementType`](../models/sql_models.md#SQLElementType), [`SQLElement`](../models/sql_models.md#SQLElement), [`SQLFullFormatter`](sql_formatters.md#SQLFullFormatter), [`_format_grouped_elements`](sql_formatters.md#SQLFullFormatter._format_grouped_elements), [`_format_grouped_elements`](sql_formatters.md#SQLCSVFormatter._format_grouped_elements), [`sql_element_type`](../models/sql_models.md#SQLElement.sql_element_type), [`SQLCSVFormatter`](sql_formatters.md#SQLCSVFormatter), [`SQLCompactFormatter`](sql_formatters.md#SQLCompactFormatter), [`format_elements`](sql_formatters.md#SQLCSVFormatter.format_elements), [`_format_grouped_elements`](sql_formatters.md#SQLCompactFormatter._format_grouped_elements)
- used by: [`SQLFullFormatter`](sql_formatters.md#SQLFullFormatter), [`SQLCSVFormatter`](sql_formatters.md#SQLCSVFormatter), [`SQLCompactFormatter`](sql_formatters.md#SQLCompactFormatter), [`format_elements`](sql_formatters.md#SQLCSVFormatter.format_elements), [`format_analysis_result`](sql_formatters.md#SQLFullFormatter.format_analysis_result), [`format_analysis_result`](sql_formatters.md#SQLCompactFormatter.format_analysis_result)  (21 test-only)

### `SQLFullFormatter`  ·  implements/extends SQLFormatterBase
- def: [`tree_sitter_analyzer/formatters/sql_formatters.py:75`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/sql_formatters.py#L75)
- doc: Comprehensive SQL format with detailed metadata
- signature: `class SQLFullFormatter(SQLFormatterBase):`
- members:
  - `_format_element_details(self, element: SQLElement)` — [`L178`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/sql_formatters.py#L178) — Format detailed information for a single element — documented in [tree_sitter_analyzer-models-sql_models](../../../concepts/tree_sitter_analyzer-models-sql_models.md)
  - `_format_element_section(self, element_type: SQLElementType, elements: list[SQLElement])` — [`L150`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/sql_formatters.py#L150) — Format detailed section for specific element type
  - `_format_function_details(self, function: SQLFunction)` — [`L251`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/sql_formatters.py#L251) — Format function-specific details
  - `_format_grouped_elements(self, grouped_elements: dict[SQLElementType, list[SQLElement]], file_path: str)` — [`L97`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/sql_formatters.py#L97) — Format elements in full detail format
  - `_format_index_details(self, index: SQLIndex)` — [`L284`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/sql_formatters.py#L284) — Format index-specific details
  - `_format_overview_table(self, grouped_elements: dict[SQLElementType, list[SQLElement]])` — [`L130`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/sql_formatters.py#L130) — Create overview table with SQL terminology
  - `_format_procedure_details(self, procedure: SQLProcedure)` — [`L238`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/sql_formatters.py#L238) — Format procedure-specific details
  - `_format_table_details(self, table: SQLTable)` — [`L197`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/sql_formatters.py#L197) — Format table-specific details
  - `_format_trigger_details(self, trigger: SQLTrigger)` — [`L267`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/sql_formatters.py#L267) — Format trigger-specific details
  - `_format_view_details(self, view: SQLView)` — [`L225`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/sql_formatters.py#L225) — Format view-specific details
  - `_get_section_title(self, element_type: SQLElementType)` — [`L166`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/sql_formatters.py#L166) — Get section title for element type
  - `format_analysis_result(self, analysis_result: Any, table_type: str = "full")` — [`L78`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/sql_formatters.py#L78) — Format AnalysisResult directly for SQL files.
- uses (calls/refs, reference-scoped): [`name`](../models/base.md#CodeElement.name), [`start_line`](../models/base.md#CodeElement.start_line), [`end_line`](../models/base.md#CodeElement.end_line), [`SQLElementType`](../models/sql_models.md#SQLElementType), [`SQLElement`](../models/sql_models.md#SQLElement), [`SQLTable`](../models/sql_models.md#SQLTable), [`SQLFunction`](../models/sql_models.md#SQLFunction), [`SQLTrigger`](../models/sql_models.md#SQLTrigger), [`dependencies`](../models/sql_models.md#SQLElement.dependencies), [`SQLView`](../models/sql_models.md#SQLView), [`SQLIndex`](../models/sql_models.md#SQLIndex), [`parameters`](../models/sql_models.md#SQLElement.parameters), [`columns`](../models/sql_models.md#SQLElement.columns), [`format_elements`](sql_formatters.md#SQLFormatterBase.format_elements), [`SQLProcedure`](../models/sql_models.md#SQLProcedure), [`TABLE`](../models/sql_models.md#SQLElementType.TABLE), [`name`](../models/sql_models.md#SQLColumn.name), [`table_name`](../models/sql_models.md#SQLElement.table_name), [`TRIGGER`](../models/sql_models.md#SQLElementType.TRIGGER), [`table_name`](../models/sql_models.md#SQLTrigger.table_name), [`trigger_timing`](../models/sql_models.md#SQLTrigger.trigger_timing), [`format_sql_overview_details`](_sql_formatters_helpers.md#format_sql_overview_details), [`format_sql_table_foreign_keys`](_sql_formatters_helpers.md#format_sql_table_foreign_keys), [`trigger_event`](../models/sql_models.md#SQLTrigger.trigger_event), [`indexed_columns`](../models/sql_models.md#SQLIndex.indexed_columns), [`return_type`](../models/sql_models.md#SQLElement.return_type), [`source_tables`](../models/sql_models.md#SQLView.source_tables), [`sql_element_type`](../models/sql_models.md#SQLElement.sql_element_type), [`SQLFormatterBase`](sql_formatters.md#SQLFormatterBase), [`FUNCTION`](../models/sql_models.md#SQLElementType.FUNCTION), [`VIEW`](../models/sql_models.md#SQLElementType.VIEW), [`constraints`](../models/sql_models.md#SQLElement.constraints), [`is_unique`](../models/sql_models.md#SQLIndex.is_unique), [`get_primary_key_columns`](../models/sql_models.md#SQLTable.get_primary_key_columns), [`iter_sql_elements_by_line`](_sql_formatters_helpers.md#iter_sql_elements_by_line), [`get_foreign_key_columns`](../models/sql_models.md#SQLTable.get_foreign_key_columns), [`INDEX`](../models/sql_models.md#SQLElementType.INDEX), [`PROCEDURE`](../models/sql_models.md#SQLElementType.PROCEDURE), [`_format_empty_file`](sql_formatters.md#SQLFormatterBase._format_empty_file), [`constraint_type`](../models/sql_models.md#SQLConstraint.constraint_type)  (+1 more)
- used by: [`_format_grouped_elements`](sql_formatters.md#SQLFormatterBase._format_grouped_elements), [`_formatters`](sql_formatter_wrapper.md#SQLFormatterWrapper._formatters), [`SQLFormatterBase`](sql_formatters.md#SQLFormatterBase)  (22 test-only)

