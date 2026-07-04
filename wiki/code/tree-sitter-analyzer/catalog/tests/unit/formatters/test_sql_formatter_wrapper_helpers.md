---
title: 'Module: tests/unit/formatters/test_sql_formatter_wrapper_helpers.py'
type: catalog
provenance: extracted
module: tests/unit/formatters/test_sql_formatter_wrapper_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.formatters.test_sql_formatter_wrapper_helpers`/
symbols:
  _noop_extractor: _noop_extractor().
  TestConvertAnalysisResultToSqlElements.test_trigger_extractor_populates_timing: TestConvertAnalysisResultToSqlElements#test_trigger_extractor_populates_timing().
  TestConvertAnalysisResultToSqlElements.test_index_extractor_populates_unique: TestConvertAnalysisResultToSqlElements#test_index_extractor_populates_unique().
  TestConvertAnalysisResultToSqlElements.test_sql_element_passthrough: TestConvertAnalysisResultToSqlElements#test_sql_element_passthrough().
  TestConvertAnalysisResultToSqlElements.test_view_extractor_populates_source_tables: TestConvertAnalysisResultToSqlElements#test_view_extractor_populates_source_tables().
  TestConvertAnalysisResultToSqlElements.test_procedure_extractor_populates_params: TestConvertAnalysisResultToSqlElements#test_procedure_extractor_populates_params().
  TestElementToDict.test_full_attributes: TestElementToDict#test_full_attributes().
  TestConvertAnalysisResultToSqlElements.test_extractor_populates_columns: TestConvertAnalysisResultToSqlElements#test_extractor_populates_columns().
  TestConvertAnalysisResultToSqlElements.test_function_extractor_populates_return_type: TestConvertAnalysisResultToSqlElements#test_function_extractor_populates_return_type().
  TestCreateSqlElementFromDict.test_missing_fields_uses_defaults: TestCreateSqlElementFromDict#test_missing_fields_uses_defaults().
  TestCreateSqlElementFromDict.test_all_dict_factory_types_produce_correct_classes: TestCreateSqlElementFromDict#test_all_dict_factory_types_produce_correct_classes().
  _make_element: _make_element().
  TestConvertAnalysisResultToSqlElements._make_result: TestConvertAnalysisResultToSqlElements#_make_result().
  TestConvertAnalysisResultToSqlElements._convert: TestConvertAnalysisResultToSqlElements#_convert().
  TestConvertAnalysisResultToSqlElements.test_index_no_table_name_no_dependency: TestConvertAnalysisResultToSqlElements#test_index_no_table_name_no_dependency().
  TestConvertAnalysisResultToSqlElements.test_multiple_elements: TestConvertAnalysisResultToSqlElements#test_multiple_elements().
  TestConvertAnalysisResultToSqlElements.test_table_element: TestConvertAnalysisResultToSqlElements#test_table_element().
  TestConvertAnalysisResultToSqlElements.test_view_element: TestConvertAnalysisResultToSqlElements#test_view_element().
  TestConvertAnalysisResultToSqlElements.test_procedure_element: TestConvertAnalysisResultToSqlElements#test_procedure_element().
  TestConvertAnalysisResultToSqlElements.test_function_element: TestConvertAnalysisResultToSqlElements#test_function_element().
  TestConvertAnalysisResultToSqlElements.test_trigger_element: TestConvertAnalysisResultToSqlElements#test_trigger_element().
  TestConvertAnalysisResultToSqlElements.test_index_element: TestConvertAnalysisResultToSqlElements#test_index_element().
  TestConvertAnalysisResultToSqlElements.test_unknown_type_skipped: TestConvertAnalysisResultToSqlElements#test_unknown_type_skipped().
  TestCreateSqlElementFromDict.test_table: TestCreateSqlElementFromDict#test_table().
  TestCreateSqlElementFromDict.test_create_table_prefix: TestCreateSqlElementFromDict#test_create_table_prefix().
  TestCreateSqlElementFromDict.test_unknown_type_falls_back_to_table: TestCreateSqlElementFromDict#test_unknown_type_falls_back_to_table().
  TestConvertAnalysisResultToSqlElements.test_empty_elements: TestConvertAnalysisResultToSqlElements#test_empty_elements().
  TestCreateSqlElementFromDict.test_view: TestCreateSqlElementFromDict#test_view().
  TestCreateSqlElementFromDict.test_create_view_prefix: TestCreateSqlElementFromDict#test_create_view_prefix().
  TestCreateSqlElementFromDict.test_procedure: TestCreateSqlElementFromDict#test_procedure().
  TestCreateSqlElementFromDict.test_create_procedure_prefix: TestCreateSqlElementFromDict#test_create_procedure_prefix().
  TestCreateSqlElementFromDict.test_function: TestCreateSqlElementFromDict#test_function().
  TestCreateSqlElementFromDict.test_create_function_prefix: TestCreateSqlElementFromDict#test_create_function_prefix().
  TestCreateSqlElementFromDict.test_trigger: TestCreateSqlElementFromDict#test_trigger().
  TestCreateSqlElementFromDict.test_create_trigger_prefix: TestCreateSqlElementFromDict#test_create_trigger_prefix().
  TestCreateSqlElementFromDict.test_index: TestCreateSqlElementFromDict#test_index().
  TestCreateSqlElementFromDict.test_create_index_prefix: TestCreateSqlElementFromDict#test_create_index_prefix().
  TestElementToDict.test_missing_attributes_use_defaults: TestElementToDict#test_missing_attributes_use_defaults().
  TestElementToDict.test_sql_type_fallback: TestElementToDict#test_sql_type_fallback().
  TestCreateSqlElementFromDict.test_exception_returns_none: TestCreateSqlElementFromDict#test_exception_returns_none().
  TestConvertAnalysisResultToSqlElements.extract_idx: TestConvertAnalysisResultToSqlElements#extract_idx().
  TestConvertAnalysisResultToSqlElements.extract_columns: TestConvertAnalysisResultToSqlElements#extract_columns().
  TestConvertAnalysisResultToSqlElements.extract_view: TestConvertAnalysisResultToSqlElements#extract_view().
  TestConvertAnalysisResultToSqlElements.extract_proc: TestConvertAnalysisResultToSqlElements#extract_proc().
  TestConvertAnalysisResultToSqlElements.extract_fn: TestConvertAnalysisResultToSqlElements#extract_fn().
  TestConvertAnalysisResultToSqlElements.extract_trg: TestConvertAnalysisResultToSqlElements#extract_trg().
  TestElementToDict: TestElementToDict#
  TestConvertAnalysisResultToSqlElements: TestConvertAnalysisResultToSqlElements#
  TestCreateSqlElementFromDict: TestCreateSqlElementFromDict#
---
# Module: [`tests/unit/formatters/test_sql_formatter_wrapper_helpers.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_helpers.py)

## Classes
### `TestConvertAnalysisResultToSqlElements`
- def: [`tests/unit/formatters/test_sql_formatter_wrapper_helpers.py:64`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_helpers.py#L64)
- signature: `class TestConvertAnalysisResultToSqlElements:`
- members:
  - `extract_columns(raw_text, name)` — [`L132`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_helpers.py#L132)
  - `extract_fn(raw_text, name)` — [`L185`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_helpers.py#L185)
  - `extract_idx(raw_text, name)` — [`L222`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_helpers.py#L222)
  - `extract_proc(raw_text, name)` — [`L167`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_helpers.py#L167)
  - `extract_trg(raw_text, name)` — [`L202`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_helpers.py#L202)
  - `extract_view(raw_text, name)` — [`L149`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_helpers.py#L149)
  - `test_empty_elements(self)` — [`L265`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_helpers.py#L265)
  - `test_extractor_populates_columns(self)` — [`L128`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_helpers.py#L128)
  - `test_function_element(self)` — [`L98`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_helpers.py#L98)
  - `test_function_extractor_populates_return_type(self)` — [`L181`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_helpers.py#L181)
  - `test_index_element(self)` — [`L110`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_helpers.py#L110)
  - `test_index_extractor_populates_unique(self)` — [`L218`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_helpers.py#L218)
  - `test_index_no_table_name_no_dependency(self)` — [`L237`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_helpers.py#L237)
  - `test_multiple_elements(self)` — [`L253`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_helpers.py#L253)
  - `test_procedure_element(self)` — [`L92`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_helpers.py#L92)
  - `test_procedure_extractor_populates_params(self)` — [`L163`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_helpers.py#L163)
  - `test_sql_element_passthrough(self)` — [`L121`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_helpers.py#L121)
  - `test_table_element(self)` — [`L79`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_helpers.py#L79)
  - `test_trigger_element(self)` — [`L104`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_helpers.py#L104)
  - `test_trigger_extractor_populates_timing(self)` — [`L198`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_helpers.py#L198)
  - `test_unknown_type_skipped(self)` — [`L116`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_helpers.py#L116)
  - `test_view_element(self)` — [`L86`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_helpers.py#L86)
  - `test_view_extractor_populates_source_tables(self)` — [`L145`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_helpers.py#L145)
- protocol/private: `_convert`[`L68`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_helpers.py#L68), `_make_result`[`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_helpers.py#L65)
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`start_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`end_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.end_line), [`language`](../../../tree_sitter_analyzer/models/base.md#CodeElement.language), [`raw_text`](../../../tree_sitter_analyzer/models/base.md#CodeElement.raw_text), [`SQLTable`](../../../tree_sitter_analyzer/models/sql_models.md#SQLTable), [`SQLFunction`](../../../tree_sitter_analyzer/models/sql_models.md#SQLFunction), [`SQLTrigger`](../../../tree_sitter_analyzer/models/sql_models.md#SQLTrigger), [`dependencies`](../../../tree_sitter_analyzer/models/sql_models.md#SQLElement.dependencies), [`SQLView`](../../../tree_sitter_analyzer/models/sql_models.md#SQLView), [`SQLIndex`](../../../tree_sitter_analyzer/models/sql_models.md#SQLIndex), [`parameters`](../../../tree_sitter_analyzer/models/sql_models.md#SQLElement.parameters), [`columns`](../../../tree_sitter_analyzer/models/sql_models.md#SQLElement.columns), [`SQLProcedure`](../../../tree_sitter_analyzer/models/sql_models.md#SQLProcedure), [`convert_analysis_result_to_sql_elements`](../../../tree_sitter_analyzer/formatters/_sql_formatter_wrapper_helpers.md#convert_analysis_result_to_sql_elements), [`table_name`](../../../tree_sitter_analyzer/models/sql_models.md#SQLTrigger.table_name), [`trigger_timing`](../../../tree_sitter_analyzer/models/sql_models.md#SQLTrigger.trigger_timing), [`trigger_event`](../../../tree_sitter_analyzer/models/sql_models.md#SQLTrigger.trigger_event), [`indexed_columns`](../../../tree_sitter_analyzer/models/sql_models.md#SQLIndex.indexed_columns), [`return_type`](../../../tree_sitter_analyzer/models/sql_models.md#SQLElement.return_type), [`source_tables`](../../../tree_sitter_analyzer/models/sql_models.md#SQLView.source_tables), [`constraints`](../../../tree_sitter_analyzer/models/sql_models.md#SQLElement.constraints), [`is_unique`](../../../tree_sitter_analyzer/models/sql_models.md#SQLIndex.is_unique)  (2 test-only)

### `TestCreateSqlElementFromDict`
- def: [`tests/unit/formatters/test_sql_formatter_wrapper_helpers.py:270`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_helpers.py#L270)
- signature: `class TestCreateSqlElementFromDict:`
- members:
  - `test_all_dict_factory_types_produce_correct_classes(self)` — [`L378`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_helpers.py#L378)
  - `test_create_function_prefix(self)` — [`L322`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_helpers.py#L322)
  - `test_create_index_prefix(self)` — [`L350`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_helpers.py#L350)
  - `test_create_procedure_prefix(self)` — [`L308`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_helpers.py#L308)
  - `test_create_table_prefix(self)` — [`L279`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_helpers.py#L279)
  - `test_create_trigger_prefix(self)` — [`L336`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_helpers.py#L336)
  - `test_create_view_prefix(self)` — [`L294`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_helpers.py#L294)
  - `test_exception_returns_none(self)` — [`L365`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_helpers.py#L365)
  - `test_function(self)` — [`L315`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_helpers.py#L315)
  - `test_index(self)` — [`L343`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_helpers.py#L343)
  - `test_missing_fields_uses_defaults(self)` — [`L369`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_helpers.py#L369)
  - `test_procedure(self)` — [`L301`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_helpers.py#L301)
  - `test_table(self)` — [`L271`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_helpers.py#L271)
  - `test_trigger(self)` — [`L329`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_helpers.py#L329)
  - `test_unknown_type_falls_back_to_table(self)` — [`L357`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_helpers.py#L357)
  - `test_view(self)` — [`L287`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_helpers.py#L287)
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`start_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`end_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.end_line), [`language`](../../../tree_sitter_analyzer/models/base.md#CodeElement.language), [`raw_text`](../../../tree_sitter_analyzer/models/base.md#CodeElement.raw_text), [`SQLTable`](../../../tree_sitter_analyzer/models/sql_models.md#SQLTable), [`SQLFunction`](../../../tree_sitter_analyzer/models/sql_models.md#SQLFunction), [`SQLTrigger`](../../../tree_sitter_analyzer/models/sql_models.md#SQLTrigger), [`SQLView`](../../../tree_sitter_analyzer/models/sql_models.md#SQLView), [`SQLIndex`](../../../tree_sitter_analyzer/models/sql_models.md#SQLIndex), [`SQLProcedure`](../../../tree_sitter_analyzer/models/sql_models.md#SQLProcedure), [`create_sql_element_from_dict`](../../../tree_sitter_analyzer/formatters/_sql_formatter_wrapper_helpers.md#create_sql_element_from_dict)

### `TestElementToDict`
- def: [`tests/unit/formatters/test_sql_formatter_wrapper_helpers.py:38`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_helpers.py#L38)
- signature: `class TestElementToDict:`
- members:
  - `test_full_attributes(self)` — [`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_helpers.py#L39)
  - `test_missing_attributes_use_defaults(self)` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_helpers.py#L49)
  - `test_sql_type_fallback(self)` — [`L58`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_helpers.py#L58)
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`start_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`end_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.end_line), [`language`](../../../tree_sitter_analyzer/models/base.md#CodeElement.language), [`raw_text`](../../../tree_sitter_analyzer/models/base.md#CodeElement.raw_text), [`SQLTable`](../../../tree_sitter_analyzer/models/sql_models.md#SQLTable), [`element_to_dict`](../../../tree_sitter_analyzer/formatters/_sql_formatter_wrapper_helpers.md#element_to_dict)

## Functions
- `_make_element(name="test", element_type="table", start_line=1, end_line=10, raw_text="CREATE TABLE test (id INT);", language="sql")` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_helpers.py#L26)
- `_noop_extractor(raw_text, name)` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_sql_formatter_wrapper_helpers.py#L22)

