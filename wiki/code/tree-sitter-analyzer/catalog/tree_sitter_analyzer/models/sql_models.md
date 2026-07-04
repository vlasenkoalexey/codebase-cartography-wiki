---
title: 'Module: tree_sitter_analyzer/models/sql_models.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/models/sql_models.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.models.sql_models`/
symbols:
  SQLElementType: SQLElementType#
  SQLElement: SQLElement#
  SQLTable: SQLTable#
  SQLFunction: SQLFunction#
  SQLTrigger: SQLTrigger#
  SQLElement.dependencies: SQLElement#dependencies.
  SQLView: SQLView#
  SQLIndex: SQLIndex#
  SQLElement.parameters: SQLElement#parameters.
  SQLElement.columns: SQLElement#columns.
  SQLProcedure: SQLProcedure#
  SQLParameter: SQLParameter#
  SQLColumn: SQLColumn#
  SQLElementType.TABLE: SQLElementType#TABLE.
  SQLColumn.name: SQLColumn#name.
  SQLTable.sql_element_type: SQLTable#sql_element_type.
  SQLTrigger.sql_element_type: SQLTrigger#sql_element_type.
  SQLElement.to_summary_item: SQLElement#to_summary_item().
  SQLElement.table_name: SQLElement#table_name.
  SQLElementType.TRIGGER: SQLElementType#TRIGGER.
  SQLColumn.data_type: SQLColumn#data_type.
  SQLParameter.name: SQLParameter#name.
  SQLTrigger.table_name: SQLTrigger#table_name.
  SQLTrigger.trigger_timing: SQLTrigger#trigger_timing.
  SQLParameter.data_type: SQLParameter#data_type.
  SQLFunction.sql_element_type: SQLFunction#sql_element_type.
  SQLTrigger.trigger_event: SQLTrigger#trigger_event.
  SQLElement.sql_element_type: SQLElement#sql_element_type.
  SQLElement.return_type: SQLElement#return_type.
  SQLView.source_tables: SQLView#source_tables.
  SQLIndex.indexed_columns: SQLIndex#indexed_columns.
  SQLElementType.VIEW: SQLElementType#VIEW.
  SQLElementType.FUNCTION: SQLElementType#FUNCTION.
  SQLElement.constraints: SQLElement#constraints.
  SQLView.sql_element_type: SQLView#sql_element_type.
  SQLIndex.is_unique: SQLIndex#is_unique.
  SQLTable.get_primary_key_columns: SQLTable#get_primary_key_columns().
  SQLConstraint: SQLConstraint#
  SQLElement.schema_name: SQLElement#schema_name.
  SQLTable.get_foreign_key_columns: SQLTable#get_foreign_key_columns().
  SQLProcedure.sql_element_type: SQLProcedure#sql_element_type.
  SQLIndex.sql_element_type: SQLIndex#sql_element_type.
  SQLColumn.nullable: SQLColumn#nullable.
  SQLElementType.PROCEDURE: SQLElementType#PROCEDURE.
  SQLElementType.INDEX: SQLElementType#INDEX.
  SQLParameter.direction: SQLParameter#direction.
  SQLColumn.is_primary_key: SQLColumn#is_primary_key.
  SQLColumn.is_foreign_key: SQLColumn#is_foreign_key.
  SQLColumn.foreign_key_reference: SQLColumn#foreign_key_reference.
  SQLConstraint.constraint_type: SQLConstraint#constraint_type.
  SQLTrigger.element_type: SQLTrigger#element_type.
  SQLConstraint.name: SQLConstraint#name.
  SQLConstraint.columns: SQLConstraint#columns.
  SQLFunction.element_type: SQLFunction#element_type.
  SQLElement.element_type: SQLElement#element_type.
  SQLView.element_type: SQLView#element_type.
  SQLColumn.default_value: SQLColumn#default_value.
  SQLConstraint.reference_table: SQLConstraint#reference_table.
  SQLConstraint.reference_columns: SQLConstraint#reference_columns.
  SQLElement.trigger_timing: SQLElement#trigger_timing.
  SQLElement.trigger_event: SQLElement#trigger_event.
  SQLElement.index_type: SQLElement#index_type.
  SQLTable.element_type: SQLTable#element_type.
  SQLView.view_definition: SQLView#view_definition.
  SQLProcedure.element_type: SQLProcedure#element_type.
  SQLFunction.is_deterministic: SQLFunction#is_deterministic.
  SQLFunction.reads_sql_data: SQLFunction#reads_sql_data.
  SQLIndex.element_type: SQLIndex#element_type.
  __all__: __all__.
---
# Module: [`tree_sitter_analyzer/models/sql_models.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/sql_models.py)

## Classes
### `SQLColumn`
- def: [`tree_sitter_analyzer/models/sql_models.py:29`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/sql_models.py#L29)
- doc: SQL column definition
- signature: `class SQLColumn:`
- members:
  - `data_type` — [`L33`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/sql_models.py#L33)
  - `default_value` — [`L35`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/sql_models.py#L35)
  - `foreign_key_reference` — [`L38`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/sql_models.py#L38)
  - `is_foreign_key` — [`L37`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/sql_models.py#L37)
  - `is_primary_key` — [`L36`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/sql_models.py#L36)
  - `name` — [`L32`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/sql_models.py#L32)
  - `nullable` — [`L34`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/sql_models.py#L34)
- used by: [`columns`](sql_models.md#SQLElement.columns), [`extract_sql_tables`](../languages/sql_plugin/table_extractor.md#extract_sql_tables), [`_parse_column_definition`](../languages/sql_plugin/table_extractor.md#_parse_column_definition), [`_format_table_details`](../formatters/sql_formatters.md#SQLFullFormatter._format_table_details), [`format_sql_table_foreign_keys`](../formatters/_sql_formatters_helpers.md#format_sql_table_foreign_keys), [`_process_column_node`](../languages/sql_plugin/table_extractor.md#_process_column_node), [`extract_table_columns`](../languages/sql_plugin/table_extractor.md#extract_table_columns), [`_format_view_details`](../formatters/sql_formatters.md#SQLFullFormatter._format_view_details), [`get_primary_key_columns`](sql_models.md#SQLTable.get_primary_key_columns), [`get_foreign_key_columns`](sql_models.md#SQLTable.get_foreign_key_columns), [`_parse_columns_from_raw_text`](../languages/sql_plugin/table_extractor.md#_parse_columns_from_raw_text)  (10 test-only)

### `SQLConstraint`
- def: [`tree_sitter_analyzer/models/sql_models.py:51`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/sql_models.py#L51)
- doc: SQL constraint definition
- signature: `class SQLConstraint:`
- members:
  - `columns` — [`L56`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/sql_models.py#L56)
  - `constraint_type` — [`L55`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/sql_models.py#L55)
  - `name` — [`L54`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/sql_models.py#L54)
  - `reference_columns` — [`L58`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/sql_models.py#L58)
  - `reference_table` — [`L57`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/sql_models.py#L57)
- used by: [`extract_sql_tables`](../languages/sql_plugin/table_extractor.md#extract_sql_tables), [`_format_table_details`](../formatters/sql_formatters.md#SQLFullFormatter._format_table_details), [`extract_table_columns`](../languages/sql_plugin/table_extractor.md#extract_table_columns), [`constraints`](sql_models.md#SQLElement.constraints)  (2 test-only)

### `SQLElement`  ·  implements/extends CodeElement
- def: [`tree_sitter_analyzer/models/sql_models.py:62`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/sql_models.py#L62) — documented in [tree_sitter_analyzer-models-result](../../../concepts/tree_sitter_analyzer-models-result.md)
- doc: Base SQL element with database-specific metadata
- signature: `class SQLElement(CodeElement):`
- members:
  - `to_summary_item(self)` — [`L80`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/sql_models.py#L80) — Return dictionary for summary item with SQL-specific information
  - `columns` — [`L66`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/sql_models.py#L66)
  - `constraints` — [`L69`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/sql_models.py#L69)
  - `dependencies` — [`L68`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/sql_models.py#L68)
  - `element_type` — [`L70`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/sql_models.py#L70)
  - `index_type` — [`L78`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/sql_models.py#L78)
  - `parameters` — [`L67`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/sql_models.py#L67)
  - `return_type` — [`L75`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/sql_models.py#L75)
  - `schema_name` — [`L73`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/sql_models.py#L73)
  - `sql_element_type` — [`L65`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/sql_models.py#L65)
  - `table_name` — [`L74`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/sql_models.py#L74)
  - `trigger_event` — [`L77`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/sql_models.py#L77)
  - `trigger_timing` — [`L76`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/sql_models.py#L76)
- uses (calls/refs, reference-scoped): [`name`](base.md#CodeElement.name), [`start_line`](base.md#CodeElement.start_line), [`end_line`](base.md#CodeElement.end_line), [`CodeElement`](base.md#CodeElement), [`SQLElementType`](sql_models.md#SQLElementType), [`SQLTable`](sql_models.md#SQLTable), [`SQLFunction`](sql_models.md#SQLFunction), [`SQLTrigger`](sql_models.md#SQLTrigger), [`SQLView`](sql_models.md#SQLView), [`SQLIndex`](sql_models.md#SQLIndex), [`SQLProcedure`](sql_models.md#SQLProcedure), [`SQLParameter`](sql_models.md#SQLParameter), [`SQLColumn`](sql_models.md#SQLColumn), [`TABLE`](sql_models.md#SQLElementType.TABLE), [`SQLConstraint`](sql_models.md#SQLConstraint)
- used by: [`CodeElement`](base.md#CodeElement), [`SQLTable`](sql_models.md#SQLTable), [`TREE_SITTER_AVAILABLE`](../languages/sql_plugin/extractor.md#TREE_SITTER_AVAILABLE), [`fill_missing_sql_tables_from_regex`](../languages/sql_plugin/table_extractor.md#fill_missing_sql_tables_from_regex), [`SQLFunction`](sql_models.md#SQLFunction), [`SQLTrigger`](sql_models.md#SQLTrigger), [`extract_sql_elements`](../languages/sql_plugin/extractor.md#SQLElementExtractor.extract_sql_elements), [`SQLView`](sql_models.md#SQLView), [`SQLIndex`](sql_models.md#SQLIndex), [`_sql_index_from_analysis`](../formatters/_sql_formatter_wrapper_helpers.md#_sql_index_from_analysis), [`_sql_trigger_from_analysis`](../formatters/_sql_formatter_wrapper_helpers.md#_sql_trigger_from_analysis), [`_sql_index_from_dict`](../formatters/_sql_formatter_wrapper_helpers.md#_sql_index_from_dict), [`_sql_trigger_from_dict`](../formatters/_sql_formatter_wrapper_helpers.md#_sql_trigger_from_dict), [`_convert_analysis_element`](../formatters/_sql_formatter_wrapper_helpers.md#_convert_analysis_element), [`_format_element_details`](../formatters/sql_formatters.md#SQLFullFormatter._format_element_details), [`_sql_function_from_analysis`](../formatters/_sql_formatter_wrapper_helpers.md#_sql_function_from_analysis), [`_sql_table_from_analysis`](../formatters/_sql_formatter_wrapper_helpers.md#_sql_table_from_analysis), [`_sql_view_from_analysis`](../formatters/_sql_formatter_wrapper_helpers.md#_sql_view_from_analysis), [`_sql_table_from_dict`](../formatters/_sql_formatter_wrapper_helpers.md#_sql_table_from_dict), [`_sql_function_from_dict`](../formatters/_sql_formatter_wrapper_helpers.md#_sql_function_from_dict), [`_sql_view_from_dict`](../formatters/_sql_formatter_wrapper_helpers.md#_sql_view_from_dict), [`_sql_procedure_from_analysis`](../formatters/_sql_formatter_wrapper_helpers.md#_sql_procedure_from_analysis), [`format_elements`](../formatters/sql_formatters.md#SQLFormatterBase.format_elements), [`_sql_procedure_from_dict`](../formatters/_sql_formatter_wrapper_helpers.md#_sql_procedure_from_dict), [`extract_sql_tables`](../languages/sql_plugin/table_extractor.md#extract_sql_tables), [`SQLProcedure`](sql_models.md#SQLProcedure), [`format_sql_compact_details`](../formatters/_sql_formatters_helpers.md#format_sql_compact_details), [`create_sql_element_from_dict`](../formatters/_sql_formatter_wrapper_helpers.md#create_sql_element_from_dict), [`_append_source_function`](../languages/sql_plugin/function_extractor.md#_append_source_function), [`_append_ast_function`](../languages/sql_plugin/function_extractor.md#_append_ast_function), [`_append_fallback_procedure`](../languages/sql_plugin/_procedure_extractor_helpers.md#_append_fallback_procedure), [`_extract_view_from_create_node`](../languages/sql_plugin/view_extractor.md#_extract_view_from_create_node), [`to_summary_item`](base.md#CodeElement.to_summary_item), [`_append_source_procedure`](../languages/sql_plugin/_procedure_extractor_helpers.md#_append_source_procedure), [`_extract_views_from_error_node`](../languages/sql_plugin/view_extractor.md#_extract_views_from_error_node), [`generate_elements`](../platform_compat/adapter.md#RecoverViewsFromErrorsRule.generate_elements), [`_format_grouped_elements`](../formatters/sql_formatters.md#SQLFullFormatter._format_grouped_elements), [`_build_recovered_view`](../languages/sql_plugin/element_validator.md#_build_recovered_view), [`_format_grouped_elements`](../formatters/sql_formatters.md#SQLCSVFormatter._format_grouped_elements), [`_format_overview_table`](../formatters/sql_formatters.md#SQLFullFormatter._format_overview_table)  (+41 more; 37 test-only)

### `SQLElementType`  ·  implements/extends Enum
- def: [`tree_sitter_analyzer/models/sql_models.py:17`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/sql_models.py#L17) — documented in [tree_sitter_analyzer-models-sql_models](../../../concepts/tree_sitter_analyzer-models-sql_models.md)
- doc: SQL element types for database objects
- signature: `class SQLElementType(Enum):`
- members:
  - `FUNCTION` — [`L23`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/sql_models.py#L23)
  - `INDEX` — [`L25`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/sql_models.py#L25)
  - `PROCEDURE` — [`L22`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/sql_models.py#L22)
  - `TABLE` — [`L20`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/sql_models.py#L20)
  - `TRIGGER` — [`L24`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/sql_models.py#L24)
  - `VIEW` — [`L21`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/sql_models.py#L21)
- used by: [`generate_elements`](../platform_compat/adapter.md#RecoverViewsFromErrorsRule.generate_elements), [`_format_grouped_elements`](../formatters/sql_formatters.md#SQLFullFormatter._format_grouped_elements), [`_format_grouped_elements`](../formatters/sql_formatters.md#SQLCSVFormatter._format_grouped_elements), [`_format_overview_table`](../formatters/sql_formatters.md#SQLFullFormatter._format_overview_table), [`sql_element_type`](sql_models.md#SQLTable.sql_element_type), [`_get_section_title`](../formatters/sql_formatters.md#SQLFullFormatter._get_section_title), [`sql_element_type`](sql_models.md#SQLTrigger.sql_element_type), [`_format_grouped_elements`](../formatters/sql_formatters.md#SQLFormatterBase._format_grouped_elements), [`sql_element_type`](sql_models.md#SQLFunction.sql_element_type), [`_format_element_section`](../formatters/sql_formatters.md#SQLFullFormatter._format_element_section), [`sql_element_type`](sql_models.md#SQLElement.sql_element_type), [`sql_element_type`](sql_models.md#SQLView.sql_element_type), [`group_elements_by_type`](../formatters/sql_formatters.md#SQLFormatterBase.group_elements_by_type), [`iter_sql_elements_by_line`](../formatters/_sql_formatters_helpers.md#iter_sql_elements_by_line), [`sql_element_type`](sql_models.md#SQLIndex.sql_element_type), [`sql_element_type`](sql_models.md#SQLProcedure.sql_element_type), [`_format_grouped_elements`](../formatters/sql_formatters.md#SQLCompactFormatter._format_grouped_elements)  (31 test-only)

### `SQLFunction`  ·  implements/extends SQLElement
- def: [`tree_sitter_analyzer/models/sql_models.py:127`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/sql_models.py#L127) — documented in [tree_sitter_analyzer-models-sql_models](../../../concepts/tree_sitter_analyzer-models-sql_models.md)
- doc: SQL function representation
- signature: `class SQLFunction(SQLElement):`
- members:
  - `element_type` — [`L131`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/sql_models.py#L131)
  - `is_deterministic` — [`L132`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/sql_models.py#L132)
  - `reads_sql_data` — [`L133`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/sql_models.py#L133)
  - `sql_element_type` — [`L130`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/sql_models.py#L130)
- uses (calls/refs, reference-scoped): [`SQLElementType`](sql_models.md#SQLElementType), [`SQLElement`](sql_models.md#SQLElement), [`FUNCTION`](sql_models.md#SQLElementType.FUNCTION)
- used by: [`SQLElement`](sql_models.md#SQLElement), [`_format_element_details`](../formatters/sql_formatters.md#SQLFullFormatter._format_element_details), [`_sql_function_from_analysis`](../formatters/_sql_formatter_wrapper_helpers.md#_sql_function_from_analysis), [`_sql_function_from_dict`](../formatters/_sql_formatter_wrapper_helpers.md#_sql_function_from_dict), [`format_sql_compact_details`](../formatters/_sql_formatters_helpers.md#format_sql_compact_details), [`_append_source_function`](../languages/sql_plugin/function_extractor.md#_append_source_function), [`_append_ast_function`](../languages/sql_plugin/function_extractor.md#_append_ast_function), [`_format_function_details`](../formatters/sql_formatters.md#SQLFullFormatter._format_function_details), [`apply`](../platform_compat/adapter.md#FixFunctionNameKeywordsRule.apply), [`_format_compact_function_details`](../formatters/_sql_formatters_helpers.md#_format_compact_function_details), [`apply`](../platform_compat/adapter.md#RemovePhantomFunctionsRule.apply)  (27 test-only)

### `SQLIndex`  ·  implements/extends SQLElement
- def: [`tree_sitter_analyzer/models/sql_models.py:148`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/sql_models.py#L148) — documented in [tree_sitter_analyzer-models-sql_models](../../../concepts/tree_sitter_analyzer-models-sql_models.md)
- doc: SQL index representation
- signature: `class SQLIndex(SQLElement):`
- members:
  - `element_type` — [`L152`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/sql_models.py#L152)
  - `indexed_columns` — [`L153`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/sql_models.py#L153)
  - `is_unique` — [`L154`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/sql_models.py#L154)
  - `sql_element_type` — [`L151`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/sql_models.py#L151)
- uses (calls/refs, reference-scoped): [`SQLElementType`](sql_models.md#SQLElementType), [`SQLElement`](sql_models.md#SQLElement), [`INDEX`](sql_models.md#SQLElementType.INDEX)
- used by: [`SQLElement`](sql_models.md#SQLElement), [`TREE_SITTER_AVAILABLE`](../languages/sql_plugin/extractor.md#TREE_SITTER_AVAILABLE), [`_sql_index_from_analysis`](../formatters/_sql_formatter_wrapper_helpers.md#_sql_index_from_analysis), [`_sql_index_from_dict`](../formatters/_sql_formatter_wrapper_helpers.md#_sql_index_from_dict), [`_format_element_details`](../formatters/sql_formatters.md#SQLFullFormatter._format_element_details), [`format_sql_compact_details`](../formatters/_sql_formatters_helpers.md#format_sql_compact_details), [`_append_sql_index`](../languages/sql_plugin/index_extractor.md#_append_sql_index), [`_extract_index_metadata`](../languages/sql_plugin/index_extractor.md#_extract_index_metadata), [`_extract_sql_indexes`](../languages/sql_plugin/extractor.md#SQLElementExtractor._extract_sql_indexes), [`_format_compact_index_details`](../formatters/_sql_formatters_helpers.md#_format_compact_index_details), [`_format_index_details`](../formatters/sql_formatters.md#SQLFullFormatter._format_index_details), [`extract_sql_indexes`](../languages/sql_plugin/index_extractor.md#extract_sql_indexes), [`extract_indexes_with_regex`](../languages/sql_plugin/index_extractor.md#extract_indexes_with_regex), [`_extract_indexes_with_regex`](../languages/sql_plugin/extractor.md#SQLElementExtractor._extract_indexes_with_regex), [`_append_regex_index`](../languages/sql_plugin/index_extractor.md#_append_regex_index)  (12 test-only)

### `SQLParameter`
- def: [`tree_sitter_analyzer/models/sql_models.py:42`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/sql_models.py#L42)
- doc: SQL procedure/function parameter
- signature: `class SQLParameter:`
- members:
  - `data_type` — [`L46`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/sql_models.py#L46)
  - `direction` — [`L47`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/sql_models.py#L47)
  - `name` — [`L45`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/sql_models.py#L45)
- used by: [`parameters`](sql_models.md#SQLElement.parameters), [`_append_source_function`](../languages/sql_plugin/function_extractor.md#_append_source_function), [`_append_ast_function`](../languages/sql_plugin/function_extractor.md#_append_ast_function), [`_append_fallback_procedure`](../languages/sql_plugin/_procedure_extractor_helpers.md#_append_fallback_procedure), [`_append_source_procedure`](../languages/sql_plugin/_procedure_extractor_helpers.md#_append_source_procedure), [`extract_procedure_parameters`](../languages/sql_plugin/procedure_extractor.md#extract_procedure_parameters), [`append_source_procedures`](../languages/sql_plugin/_procedure_extractor_helpers.md#append_source_procedures), [`_extract_function_metadata`](../languages/sql_plugin/function_extractor.md#_extract_function_metadata), [`append_tree_sitter_procedures`](../languages/sql_plugin/_procedure_extractor_helpers.md#append_tree_sitter_procedures)  (10 test-only)

### `SQLProcedure`  ·  implements/extends SQLElement
- def: [`tree_sitter_analyzer/models/sql_models.py:119`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/sql_models.py#L119) — documented in [tree_sitter_analyzer-models-sql_models](../../../concepts/tree_sitter_analyzer-models-sql_models.md)
- doc: SQL stored procedure representation
- signature: `class SQLProcedure(SQLElement):`
- members:
  - `element_type` — [`L123`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/sql_models.py#L123)
  - `sql_element_type` — [`L122`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/sql_models.py#L122)
- uses (calls/refs, reference-scoped): [`SQLElementType`](sql_models.md#SQLElementType), [`SQLElement`](sql_models.md#SQLElement), [`PROCEDURE`](sql_models.md#SQLElementType.PROCEDURE)
- used by: [`SQLElement`](sql_models.md#SQLElement), [`_format_element_details`](../formatters/sql_formatters.md#SQLFullFormatter._format_element_details), [`_sql_procedure_from_analysis`](../formatters/_sql_formatter_wrapper_helpers.md#_sql_procedure_from_analysis), [`_sql_procedure_from_dict`](../formatters/_sql_formatter_wrapper_helpers.md#_sql_procedure_from_dict), [`format_sql_compact_details`](../formatters/_sql_formatters_helpers.md#format_sql_compact_details), [`_append_fallback_procedure`](../languages/sql_plugin/_procedure_extractor_helpers.md#_append_fallback_procedure), [`_append_source_procedure`](../languages/sql_plugin/_procedure_extractor_helpers.md#_append_source_procedure), [`_format_procedure_details`](../formatters/sql_formatters.md#SQLFullFormatter._format_procedure_details), [`_format_compact_procedure_details`](../formatters/_sql_formatters_helpers.md#_format_compact_procedure_details)  (13 test-only)

### `SQLTable`  ·  implements/extends SQLElement
- def: [`tree_sitter_analyzer/models/sql_models.py:93`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/sql_models.py#L93) — documented in [tree_sitter_analyzer-models-result](../../../concepts/tree_sitter_analyzer-models-result.md)
- doc: SQL table representation
- signature: `class SQLTable(SQLElement):`
- members:
  - `get_foreign_key_columns(self)` — [`L103`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/sql_models.py#L103) — Get foreign key column names
  - `get_primary_key_columns(self)` — [`L99`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/sql_models.py#L99) — Get primary key column names
  - `element_type` — [`L97`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/sql_models.py#L97)
  - `sql_element_type` — [`L96`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/sql_models.py#L96)
- uses (calls/refs, reference-scoped): [`SQLElementType`](sql_models.md#SQLElementType), [`SQLElement`](sql_models.md#SQLElement), [`columns`](sql_models.md#SQLElement.columns), [`TABLE`](sql_models.md#SQLElementType.TABLE), [`name`](sql_models.md#SQLColumn.name), [`is_primary_key`](sql_models.md#SQLColumn.is_primary_key), [`is_foreign_key`](sql_models.md#SQLColumn.is_foreign_key)
- used by: [`SQLElement`](sql_models.md#SQLElement), [`fill_missing_sql_tables_from_regex`](../languages/sql_plugin/table_extractor.md#fill_missing_sql_tables_from_regex), [`_format_element_details`](../formatters/sql_formatters.md#SQLFullFormatter._format_element_details), [`_sql_table_from_analysis`](../formatters/_sql_formatter_wrapper_helpers.md#_sql_table_from_analysis), [`_sql_table_from_dict`](../formatters/_sql_formatter_wrapper_helpers.md#_sql_table_from_dict), [`extract_sql_tables`](../languages/sql_plugin/table_extractor.md#extract_sql_tables), [`format_sql_compact_details`](../formatters/_sql_formatters_helpers.md#format_sql_compact_details), [`_format_table_details`](../formatters/sql_formatters.md#SQLFullFormatter._format_table_details), [`format_sql_table_foreign_keys`](../formatters/_sql_formatters_helpers.md#format_sql_table_foreign_keys), [`_format_compact_table_details`](../formatters/_sql_formatters_helpers.md#_format_compact_table_details)  (62 test-only)

### `SQLTrigger`  ·  implements/extends SQLElement
- def: [`tree_sitter_analyzer/models/sql_models.py:137`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/sql_models.py#L137) — documented in [tree_sitter_analyzer-models-sql_models](../../../concepts/tree_sitter_analyzer-models-sql_models.md)
- doc: SQL trigger representation
- signature: `class SQLTrigger(SQLElement):`
- members:
  - `element_type` — [`L141`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/sql_models.py#L141)
  - `sql_element_type` — [`L140`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/sql_models.py#L140)
  - `table_name` — [`L142`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/sql_models.py#L142)
  - `trigger_event` — [`L144`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/sql_models.py#L144)
  - `trigger_timing` — [`L143`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/sql_models.py#L143)
- uses (calls/refs, reference-scoped): [`SQLElementType`](sql_models.md#SQLElementType), [`SQLElement`](sql_models.md#SQLElement), [`TRIGGER`](sql_models.md#SQLElementType.TRIGGER)
- used by: [`SQLElement`](sql_models.md#SQLElement), [`TREE_SITTER_AVAILABLE`](../languages/sql_plugin/extractor.md#TREE_SITTER_AVAILABLE), [`_sql_trigger_from_analysis`](../formatters/_sql_formatter_wrapper_helpers.md#_sql_trigger_from_analysis), [`_sql_trigger_from_dict`](../formatters/_sql_formatter_wrapper_helpers.md#_sql_trigger_from_dict), [`_format_element_details`](../formatters/sql_formatters.md#SQLFullFormatter._format_element_details), [`format_sql_compact_details`](../formatters/_sql_formatters_helpers.md#format_sql_compact_details), [`extract_sql_triggers`](../languages/sql_plugin/trigger_extractor.md#extract_sql_triggers), [`apply`](../platform_compat/adapter.md#RemovePhantomTriggersRule.apply), [`_format_trigger_details`](../formatters/sql_formatters.md#SQLFullFormatter._format_trigger_details), [`apply`](../platform_compat/adapter.md#FixTriggerNameDescriptionRule.apply), [`_extract_sql_triggers`](../languages/sql_plugin/extractor.md#SQLElementExtractor._extract_sql_triggers), [`_format_compact_trigger_details`](../formatters/_sql_formatters_helpers.md#_format_compact_trigger_details), [`trigger_factory`](../languages/sql_plugin/trigger_extractor.md#_SQLTriggerExtractionContext.trigger_factory)  (21 test-only)

### `SQLView`  ·  implements/extends SQLElement
- def: [`tree_sitter_analyzer/models/sql_models.py:109`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/sql_models.py#L109) — documented in [tree_sitter_analyzer-models-sql_models](../../../concepts/tree_sitter_analyzer-models-sql_models.md)
- doc: SQL view representation
- signature: `class SQLView(SQLElement):`
- members:
  - `element_type` — [`L113`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/sql_models.py#L113)
  - `source_tables` — [`L114`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/sql_models.py#L114)
  - `sql_element_type` — [`L112`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/sql_models.py#L112)
  - `view_definition` — [`L115`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/sql_models.py#L115)
- uses (calls/refs, reference-scoped): [`SQLElementType`](sql_models.md#SQLElementType), [`SQLElement`](sql_models.md#SQLElement), [`VIEW`](sql_models.md#SQLElementType.VIEW)
- used by: [`SQLElement`](sql_models.md#SQLElement), [`_format_element_details`](../formatters/sql_formatters.md#SQLFullFormatter._format_element_details), [`_sql_view_from_analysis`](../formatters/_sql_formatter_wrapper_helpers.md#_sql_view_from_analysis), [`_sql_view_from_dict`](../formatters/_sql_formatter_wrapper_helpers.md#_sql_view_from_dict), [`format_sql_compact_details`](../formatters/_sql_formatters_helpers.md#format_sql_compact_details), [`_extract_view_from_create_node`](../languages/sql_plugin/view_extractor.md#_extract_view_from_create_node), [`_extract_views_from_error_node`](../languages/sql_plugin/view_extractor.md#_extract_views_from_error_node), [`generate_elements`](../platform_compat/adapter.md#RecoverViewsFromErrorsRule.generate_elements), [`_build_recovered_view`](../languages/sql_plugin/element_validator.md#_build_recovered_view), [`_format_view_details`](../formatters/sql_formatters.md#SQLFullFormatter._format_view_details), [`_format_compact_view_details`](../formatters/_sql_formatters_helpers.md#_format_compact_view_details)  (16 test-only)

## Module values
- `__all__` — [`L157`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/sql_models.py#L157)

