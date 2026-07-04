---
title: 'Module: tree_sitter_analyzer/languages/sql_plugin/extractor.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/sql_plugin/extractor.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.sql_plugin.extractor`/
symbols:
  TREE_SITTER_AVAILABLE: TREE_SITTER_AVAILABLE.
  SQLElementExtractor.extract_sql_elements: SQLElementExtractor#extract_sql_elements().
  SQLElementExtractor: SQLElementExtractor#
  SQLElementExtractor.source_code: SQLElementExtractor#source_code.
  SQLElementExtractor._get_node_text: SQLElementExtractor#_get_node_text().
  SQLElementExtractor._is_valid_identifier: SQLElementExtractor#_is_valid_identifier().
  SQLElementExtractor.extract_functions: SQLElementExtractor#extract_functions().
  SQLElementExtractor._adapt_sql_elements: SQLElementExtractor#_adapt_sql_elements().
  SQLElementExtractor._extract_views: SQLElementExtractor#_extract_views().
  SQLElementExtractor.extract_classes: SQLElementExtractor#extract_classes().
  SQLElementExtractor._traverse_nodes: SQLElementExtractor#_traverse_nodes().
  SQLElementExtractor.content_lines: SQLElementExtractor#content_lines.
  SQLElementExtractor._reset_caches: SQLElementExtractor#_reset_caches().
  SQLElementExtractor.extract_variables: SQLElementExtractor#extract_variables().
  SQLElementExtractor.extract_imports: SQLElementExtractor#extract_imports().
  SQLElementExtractor._validate_and_fix_elements: SQLElementExtractor#_validate_and_fix_elements().
  SQLElementExtractor._extract_sql_views: SQLElementExtractor#_extract_sql_views().
  SQLElementExtractor._extract_sql_indexes: SQLElementExtractor#_extract_sql_indexes().
  SQLElementExtractor._extract_tables: SQLElementExtractor#_extract_tables().
  SQLElementExtractor._extract_sql_functions: SQLElementExtractor#_extract_sql_functions().
  SQLElementExtractor._extract_triggers: SQLElementExtractor#_extract_triggers().
  SQLElementExtractor.set_adapter: SQLElementExtractor#set_adapter().
  SQLElementExtractor._extract_sql_procedures: SQLElementExtractor#_extract_sql_procedures().
  SQLElementExtractor._extract_sql_functions_enhanced: SQLElementExtractor#_extract_sql_functions_enhanced().
  SQLElementExtractor._extract_sql_triggers: SQLElementExtractor#_extract_sql_triggers().
  SQLElementExtractor._extract_procedures: SQLElementExtractor#_extract_procedures().
  SQLElementExtractor._extract_indexes: SQLElementExtractor#_extract_indexes().
  SQLElementExtractor._extract_schema_references: SQLElementExtractor#_extract_schema_references().
  SQLElementExtractor.adapter: SQLElementExtractor#adapter.
  SQLElementExtractor._extract_sql_tables: SQLElementExtractor#_extract_sql_tables().
  SQLElementExtractor.diagnostic_mode: SQLElementExtractor#diagnostic_mode.
  SQLElementExtractor._extract_indexes_with_regex: SQLElementExtractor#_extract_indexes_with_regex().
  SQLElementExtractor._node_text_cache: SQLElementExtractor#_node_text_cache.
  SQLElementExtractor._extract_function_metadata: SQLElementExtractor#_extract_function_metadata().
  SQLElementExtractor._extract_procedure_parameters: SQLElementExtractor#_extract_procedure_parameters().
  SQLElementExtractor._processed_nodes: SQLElementExtractor#_processed_nodes.
  SQLElementExtractor.__init__: SQLElementExtractor#__init__().
  SQLElementExtractor._parse_column_definition: SQLElementExtractor#_parse_column_definition().
  SQLElementExtractor._split_column_definitions: SQLElementExtractor#_split_column_definitions().
  SQLElementExtractor._file_encoding: SQLElementExtractor#_file_encoding.
---
# Module: [`tree_sitter_analyzer/languages/sql_plugin/extractor.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/extractor.py)

## Classes
### `SQLElementExtractor`  ·  implements/extends ElementExtractor
- def: [`tree_sitter_analyzer/languages/sql_plugin/extractor.py:71`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/extractor.py#L71)
- doc: SQL-specific element extractor.
- signature: `class SQLElementExtractor(ElementExtractor):`
- members:
  - `_adapt_sql_elements(self, sql_elements: list[SQLElement])` — [`L144`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/extractor.py#L144) — Apply optional platform adapter with diagnostic logging.
  - `_extract_function_metadata(self, func_node: tree_sitter.Node, parameters: list[Any], return_type: str | None, dependencies: list[str])` — [`L332`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/extractor.py#L332) — Extract function metadata using this extractor's node text helper.
  - `_extract_indexes(self, root_node: tree_sitter.Node, variables: list[Variable])` — [`L459`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/extractor.py#L459) — Extract CREATE INDEX statements from SQL AST.
  - `_extract_indexes_with_regex(self, sql_elements: list[Any], processed_indexes: set[str])` — [`L378`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/extractor.py#L378) — Extract CREATE INDEX statements using regex as fallback.
  - `_extract_procedure_parameters(self, proc_text: str, parameters: list[Any])` — [`L348`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/extractor.py#L348) — Extract procedure parameters.
  - `_extract_procedures(self, root_node: tree_sitter.Node, functions: list[Function])` — [`L421`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/extractor.py#L421) — Extract CREATE PROCEDURE statements from SQL AST.
  - `_extract_schema_references(self, root_node: tree_sitter.Node, imports: list[Import])` — [`L471`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/extractor.py#L471) — Extract schema references (e.g., FROM schema.table).
  - `_extract_sql_functions(self, root_node: tree_sitter.Node, functions: list[Function])` — [`L433`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/extractor.py#L433) — Extract CREATE FUNCTION statements from SQL AST.
  - `_extract_sql_functions_enhanced(self, root_node: tree_sitter.Node, sql_elements: list[Any])` — [`L320`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/extractor.py#L320) — Extract enhanced SQL function elements.
  - `_extract_sql_indexes(self, root_node: tree_sitter.Node, sql_elements: list[Any])` — [`L365`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/extractor.py#L365) — Extract enhanced SQL index elements.
  - `_extract_sql_procedures(self, root_node: tree_sitter.Node, sql_elements: list[Any])` — [`L308`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/extractor.py#L308) — Extract enhanced SQL procedure elements.
  - `_extract_sql_tables(self, root_node: tree_sitter.Node, sql_elements: list[Any])` — [`L284`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/extractor.py#L284) — Extract enhanced SQL table elements.
  - `_extract_sql_triggers(self, root_node: tree_sitter.Node, sql_elements: list[Any])` — [`L354`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/extractor.py#L354) — Extract enhanced SQL trigger elements.
  - `_extract_sql_views(self, root_node: tree_sitter.Node, sql_elements: list[Any])` — [`L295`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/extractor.py#L295) — Extract enhanced SQL view elements.
  - `_extract_tables(self, root_node: tree_sitter.Node, classes: list[Class])` — [`L393`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/extractor.py#L393) — Extract CREATE TABLE statements from SQL AST.
  - `_extract_triggers(self, root_node: tree_sitter.Node, functions: list[Function])` — [`L446`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/extractor.py#L446) — Extract CREATE TRIGGER statements from SQL AST.
  - `_extract_views(self, root_node: tree_sitter.Node, classes: list[Class])` — [`L406`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/extractor.py#L406) — Extract CREATE VIEW statements from SQL AST.
  - `_get_node_text(self, node: tree_sitter.Node)` — [`L261`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/extractor.py#L261) — Get text content from a tree-sitter node with caching.
  - `extract_classes(self, tree: tree_sitter.Tree, source_code: str)` — [`L193`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/extractor.py#L193) — Extract tables and views from SQL code.
  - `extract_functions(self, tree: tree_sitter.Tree, source_code: str)` — [`L169`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/extractor.py#L169) — Extract stored procedures, functions, and triggers from SQL code.
  - `extract_imports(self, tree: tree_sitter.Tree, source_code: str)` — [`L234`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/extractor.py#L234) — Extract schema references and dependencies from SQL code.
  - `extract_sql_elements(self, tree: tree_sitter.Tree, source_code: str)` — [`L101`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/extractor.py#L101) — Extract all SQL elements with enhanced metadata. — documented in [tree_sitter_analyzer-models-sql_models](../../../../concepts/tree_sitter_analyzer-models-sql_models.md)
  - `extract_variables(self, tree: tree_sitter.Tree, source_code: str)` — [`L214`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/extractor.py#L214) — Extract indexes from SQL code.
  - `set_adapter(self, adapter: CompatibilityAdapter)` — [`L96`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/extractor.py#L96) — Set the compatibility adapter.
  - `adapter` — [`L94`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/extractor.py#L94)
  - `content_lines` — [`L86`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/extractor.py#L86)
  - `diagnostic_mode` — [`L87`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/extractor.py#L87)
  - `source_code` — [`L85`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/extractor.py#L85)
- protocol/private: `__init__`[`L83`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/extractor.py#L83), `_file_encoding`[`L92`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/extractor.py#L92), `_is_valid_identifier`[`L277`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/extractor.py#L277), `_node_text_cache`[`L90`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/extractor.py#L90), `_parse_column_definition`[`L483`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/extractor.py#L483), `_processed_nodes`[`L91`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/extractor.py#L91), `_reset_caches`[`L257`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/extractor.py#L257), `_split_column_definitions`[`L486`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/extractor.py#L486), `_traverse_nodes`[`L270`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/extractor.py#L270), `_validate_and_fix_elements`[`L163`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/extractor.py#L163)
- uses (calls/refs, reference-scoped): [`name`](../../models/base.md#CodeElement.name), [`log_debug`](../../utils/logging.md#log_debug), [`Function`](../../models/base.md#Function), [`log_error`](../../utils/logging.md#log_error), [`Class`](../../models/base.md#Class), [`Variable`](../../models/base.md#Variable), [`Import`](../../models/base.md#Import), [`ElementExtractor`](../../plugins/base.md#ElementExtractor), [`SQLElement`](../../models/sql_models.md#SQLElement), [`fill_missing_sql_tables_from_regex`](table_extractor.md#fill_missing_sql_tables_from_regex), [`SQLTrigger`](../../models/sql_models.md#SQLTrigger), [`SQLIndex`](../../models/sql_models.md#SQLIndex), [`extract_sql_tables`](table_extractor.md#extract_sql_tables), [`is_valid_identifier`](identifier_validator.md#is_valid_identifier), [`extract_sql_triggers`](trigger_extractor.md#extract_sql_triggers), [`extract_procedure_parameters`](procedure_extractor.md#extract_procedure_parameters), [`_parse_column_definition`](table_extractor.md#_parse_column_definition), [`CompatibilityAdapter`](../../platform_compat/adapter.md#CompatibilityAdapter), [`_extract_function_metadata`](function_extractor.md#_extract_function_metadata), [`extract_sql_procedures`](procedure_extractor.md#extract_sql_procedures), [`validate_and_fix_elements`](element_validator.md#validate_and_fix_elements), [`adapt_elements`](../../platform_compat/adapter.md#CompatibilityAdapter.adapt_elements), [`extract_class_views`](_class_view_extractor.md#extract_class_views), [`extract_legacy_functions`](function_extractor.md#extract_legacy_functions), [`extract_sql_indexes`](index_extractor.md#extract_sql_indexes), [`get_node_text`](_node_text.md#get_node_text), [`platform_info`](../../plugins/base.md#ElementExtractor.platform_info), [`extract_indexes_with_regex`](index_extractor.md#extract_indexes_with_regex), [`extract_class_tables`](_class_table_extractor.md#extract_class_tables), [`extract_legacy_indexes`](index_extractor.md#extract_legacy_indexes), [`extract_legacy_procedures`](procedure_extractor.md#extract_legacy_procedures), [`extract_legacy_triggers`](trigger_extractor.md#extract_legacy_triggers), [`extract_schema_references`](schema_reference_extractor.md#extract_schema_references), [`extract_sql_functions_enhanced`](function_extractor.md#extract_sql_functions_enhanced), [`extract_sql_views`](view_extractor.md#extract_sql_views), [`__init__`](../../plugins/base.md#ElementExtractor.__init__), [`_split_column_definitions`](table_extractor.md#_split_column_definitions)
- used by: [`ElementExtractor`](../../plugins/base.md#ElementExtractor), [`extract_functions`](../../plugins/base.md#ElementExtractor.extract_functions), [`extract_classes`](../../plugins/base.md#ElementExtractor.extract_classes), [`extract_variables`](../../plugins/base.md#ElementExtractor.extract_variables), [`extract_imports`](../../plugins/base.md#ElementExtractor.extract_imports), [`TREE_SITTER_AVAILABLE`](plugin.md#TREE_SITTER_AVAILABLE), [`create_extractor`](plugin.md#SQLPlugin.create_extractor), [`adapter`](plugin.md#SQLPlugin.adapter), [`extractor`](plugin.md#SQLPlugin.extractor)  (35 test-only)

## Module values
- `TREE_SITTER_AVAILABLE` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/extractor.py#L19) — documented in [tree_sitter_analyzer-plugins-base](../../../../concepts/tree_sitter_analyzer-plugins-base.md)

