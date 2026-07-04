---
title: 'Module: tests/unit/languages/test_sql_fixes.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_sql_fixes.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_sql_fixes`/
symbols:
  _extract: _extract().
  TREE_SITTER_SQL_AVAILABLE: TREE_SITTER_SQL_AVAILABLE.
  TestFunctionParamExtraction.test_function_with_mixed_param_types: TestFunctionParamExtraction#test_function_with_mixed_param_types().
  TestCreateTableErrorNodeCascade.test_no_schema_name_on_simple_tables: TestCreateTableErrorNodeCascade#test_no_schema_name_on_simple_tables().
  TestRegexFallbackColumnsPopulated.test_not_null_constraint_captured: TestRegexFallbackColumnsPopulated#test_not_null_constraint_captured().
  TestFunctionParamExtraction.test_simple_function_params_names: TestFunctionParamExtraction#test_simple_function_params_names().
  TestFunctionParamExtraction.test_simple_function_params_types: TestFunctionParamExtraction#test_simple_function_params_types().
  TestFunctionParamExtraction.test_schema_qualified_function_params_extracted: TestFunctionParamExtraction#test_schema_qualified_function_params_extracted().
  TestCreateTableAsSelect.test_create_table_with_schema_no_as_select: TestCreateTableAsSelect#test_create_table_with_schema_no_as_select().
  TestCreateTableErrorNodeCascade.test_all_three_tables_extracted: TestCreateTableErrorNodeCascade#test_all_three_tables_extracted().
  TestCreateTableErrorNodeCascade.test_customer_table_name_correct: TestCreateTableErrorNodeCascade#test_customer_table_name_correct().
  TestQuotedTableNameRegex.test_quoted_schema_plus_quoted_table: TestQuotedTableNameRegex#test_quoted_schema_plus_quoted_table().
  TestRegexFallbackColumnsPopulated.test_recovered_table_column_names: TestRegexFallbackColumnsPopulated#test_recovered_table_column_names().
  TestRegexFallbackColumnsPopulated.test_recovered_table_column_types: TestRegexFallbackColumnsPopulated#test_recovered_table_column_types().
  TestRegexFallbackColumnsPopulated.test_primary_key_constraint_line_excluded_from_columns: TestRegexFallbackColumnsPopulated#test_primary_key_constraint_line_excluded_from_columns().
  TestFunctionParamExtraction.test_simple_function_with_two_params_extracted: TestFunctionParamExtraction#test_simple_function_with_two_params_extracted().
  TestFunctionParamExtraction.test_schema_qualified_function_name_is_function_not_schema: TestFunctionParamExtraction#test_schema_qualified_function_name_is_function_not_schema().
  TestCreateTableAsSelect.test_create_table_as_select_name_is_table_not_schema: TestCreateTableAsSelect#test_create_table_as_select_name_is_table_not_schema().
  TestCreateTableAsSelect.test_create_table_as_select_schema_captured: TestCreateTableAsSelect#test_create_table_as_select_schema_captured().
  TestCreateTableAsSelect.test_create_table_no_schema_still_works: TestCreateTableAsSelect#test_create_table_no_schema_still_works().
  TestCreateTableAsSelect.test_create_table_as_select_single_schema: TestCreateTableAsSelect#test_create_table_as_select_single_schema().
  TestCreateTableErrorNodeCascade.test_table_count_is_exactly_three: TestCreateTableErrorNodeCascade#test_table_count_is_exactly_three().
  TestFillMissingTablesCommentSkip.test_commented_create_table_is_ignored: TestFillMissingTablesCommentSkip#test_commented_create_table_is_ignored().
  TestFillMissingTablesCommentSkip.test_block_commented_create_table_is_ignored: TestFillMissingTablesCommentSkip#test_block_commented_create_table_is_ignored().
  TestFillMissingTablesSchemaDeduplciation.test_same_name_different_schemas_both_recovered: TestFillMissingTablesSchemaDeduplciation#test_same_name_different_schemas_both_recovered().
  TestQuotedTableNameRegex.test_ansi_double_quoted_name_extracted: TestQuotedTableNameRegex#test_ansi_double_quoted_name_extracted().
  TestQuotedTableNameRegex.test_mysql_backtick_quoted_name_extracted: TestQuotedTableNameRegex#test_mysql_backtick_quoted_name_extracted().
  TestQuotedTableNameRegex.test_sql_server_bracket_quoted_name_extracted: TestQuotedTableNameRegex#test_sql_server_bracket_quoted_name_extracted().
  TestQuotedTableNameRegex.test_bare_identifier_still_works_after_regex_change: TestQuotedTableNameRegex#test_bare_identifier_still_works_after_regex_change().
  TestQuotedTableNameRegex.test_case_sensitive_quoted_names_not_deduped: TestQuotedTableNameRegex#test_case_sensitive_quoted_names_not_deduped().
  TestRegexFallbackColumnsPopulated.test_recovered_table_has_correct_column_count: TestRegexFallbackColumnsPopulated#test_recovered_table_has_correct_column_count().
  TestRegexFallbackColumnsPopulated.test_table_without_column_list_has_empty_columns: TestRegexFallbackColumnsPopulated#test_table_without_column_list_has_empty_columns().
  TestRegexFallbackColumnsPopulated.test_ctas_with_parenthesized_select_expression_produces_no_columns: TestRegexFallbackColumnsPopulated#test_ctas_with_parenthesized_select_expression_produces_no_columns().
  TestFunctionParamExtraction.test_schema_qualified_function_is_extracted: TestFunctionParamExtraction#test_schema_qualified_function_is_extracted().
  TestCreateTableAsSelect.test_create_table_as_select_produces_one_table: TestCreateTableAsSelect#test_create_table_as_select_produces_one_table().
  TestFillMissingTablesSchemaDeduplciation.test_duplicate_same_schema_not_added_twice: TestFillMissingTablesSchemaDeduplciation#test_duplicate_same_schema_not_added_twice().
  _SQL_FOREIGN_KEY_CASCADE: _SQL_FOREIGN_KEY_CASCADE.
  _parse: _parse().
  TestIsInSqlComment.test_not_in_comment_plain_text: TestIsInSqlComment#test_not_in_comment_plain_text().
  TestIsInSqlComment.test_inside_line_comment: TestIsInSqlComment#test_inside_line_comment().
  TestIsInSqlComment.test_after_line_comment_on_same_line: TestIsInSqlComment#test_after_line_comment_on_same_line().
  TestIsInSqlComment.test_inside_block_comment: TestIsInSqlComment#test_inside_block_comment().
  TestIsInSqlComment.test_after_closed_block_comment: TestIsInSqlComment#test_after_closed_block_comment().
  TestFunctionParamExtraction: TestFunctionParamExtraction#
  TestCreateTableAsSelect: TestCreateTableAsSelect#
  TestCreateTableErrorNodeCascade: TestCreateTableErrorNodeCascade#
  TestIsInSqlComment: TestIsInSqlComment#
  TestFillMissingTablesCommentSkip: TestFillMissingTablesCommentSkip#
  TestFillMissingTablesSchemaDeduplciation: TestFillMissingTablesSchemaDeduplciation#
  TestQuotedTableNameRegex: TestQuotedTableNameRegex#
  TestRegexFallbackColumnsPopulated: TestRegexFallbackColumnsPopulated#
---
# Module: [`tests/unit/languages/test_sql_fixes.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_sql_fixes.py)

## Classes
### `TestCreateTableAsSelect`
- def: [`tests/unit/languages/test_sql_fixes.py:154`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_sql_fixes.py#L154)
- doc: #808: CREATE TABLE schema.name AS SELECT must extract the table.
- signature: `class TestCreateTableAsSelect:`
- members:
  - `test_create_table_as_select_name_is_table_not_schema(self)` — [`L167`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_sql_fixes.py#L167) — #808: extracted name must be 'daily_stats', not 'reporting'.
  - `test_create_table_as_select_produces_one_table(self)` — [`L157`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_sql_fixes.py#L157) — #808: 'CREATE TABLE reporting.daily_stats AS SELECT ...' must yield 1 table.
  - `test_create_table_as_select_schema_captured(self)` — [`L178`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_sql_fixes.py#L178) — #808: schema_name field must contain 'reporting'.
  - `test_create_table_as_select_single_schema(self)` — [`L211`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_sql_fixes.py#L211) — Non-schema-qualified CREATE TABLE AS SELECT works too.
  - `test_create_table_no_schema_still_works(self)` — [`L189`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_sql_fixes.py#L189) — Plain CREATE TABLE (no schema) is unaffected by the fix.
  - `test_create_table_with_schema_no_as_select(self)` — [`L197`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_sql_fixes.py#L197) — Schema-qualified CREATE TABLE with column list (no AS SELECT).
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`SQLTable`](../../../tree_sitter_analyzer/models/sql_models.md#SQLTable), [`schema_name`](../../../tree_sitter_analyzer/models/sql_models.md#SQLElement.schema_name)  (1 test-only)

### `TestCreateTableErrorNodeCascade`
- def: [`tests/unit/languages/test_sql_fixes.py:256`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_sql_fixes.py#L256)
- doc: #808: CREATE TABLE absorbed into ERROR node must be recovered via regex fallback.
- signature: `class TestCreateTableErrorNodeCascade:`
- members:
  - `test_all_three_tables_extracted(self)` — [`L259`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_sql_fixes.py#L259) — Artist + Album + Customer must all appear — Customer is the cascade victim.
  - `test_customer_table_name_correct(self)` — [`L272`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_sql_fixes.py#L272) — Customer table must have name='Customer', not 'CustomerId' or similar.
  - `test_no_schema_name_on_simple_tables(self)` — [`L280`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_sql_fixes.py#L280) — None of the three tables use schema-qualified names — schema_name must be None.
  - `test_table_count_is_exactly_three(self)` — [`L266`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_sql_fixes.py#L266) — Exact count — ensures no duplicates from regex + AST overlap.
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`SQLTable`](../../../tree_sitter_analyzer/models/sql_models.md#SQLTable), [`schema_name`](../../../tree_sitter_analyzer/models/sql_models.md#SQLElement.schema_name)  (2 test-only)

### `TestFillMissingTablesCommentSkip`
- def: [`tests/unit/languages/test_sql_fixes.py:321`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_sql_fixes.py#L321)
- doc: Regex fallback must not add tables found only inside SQL comments.
- signature: `class TestFillMissingTablesCommentSkip:`
- members:
  - `test_block_commented_create_table_is_ignored(self)` — [`L336`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_sql_fixes.py#L336)
  - `test_commented_create_table_is_ignored(self)` — [`L324`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_sql_fixes.py#L324)
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`SQLTable`](../../../tree_sitter_analyzer/models/sql_models.md#SQLTable), [`fill_missing_sql_tables_from_regex`](../../../tree_sitter_analyzer/languages/sql_plugin/table_extractor.md#fill_missing_sql_tables_from_regex)

### `TestFillMissingTablesSchemaDeduplciation`
- def: [`tests/unit/languages/test_sql_fixes.py:349`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_sql_fixes.py#L349)
- doc: Regex fallback must distinguish same table name in different schemas.
- signature: `class TestFillMissingTablesSchemaDeduplciation:`
- members:
  - `test_duplicate_same_schema_not_added_twice(self)` — [`L364`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_sql_fixes.py#L364)
  - `test_same_name_different_schemas_both_recovered(self)` — [`L352`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_sql_fixes.py#L352)
- uses (calls/refs, reference-scoped): [`SQLTable`](../../../tree_sitter_analyzer/models/sql_models.md#SQLTable), [`fill_missing_sql_tables_from_regex`](../../../tree_sitter_analyzer/languages/sql_plugin/table_extractor.md#fill_missing_sql_tables_from_regex), [`schema_name`](../../../tree_sitter_analyzer/models/sql_models.md#SQLElement.schema_name)

### `TestFunctionParamExtraction`
- def: [`tests/unit/languages/test_sql_fixes.py:49`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_sql_fixes.py#L49)
- doc: #775: CREATE FUNCTION with parameters must be extracted correctly.
- signature: `class TestFunctionParamExtraction:`
- members:
  - `test_function_with_mixed_param_types(self)` — [`L130`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_sql_fixes.py#L130) — Function with INT and TEXT params — both captured.
  - `test_schema_qualified_function_is_extracted(self)` — [`L91`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_sql_fixes.py#L91) — #775: schema.function(params) must NOT silently return 0 results.
  - `test_schema_qualified_function_name_is_function_not_schema(self)` — [`L103`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_sql_fixes.py#L103) — #775: extracted name must be 'get_count', not 'myschema'.
  - `test_schema_qualified_function_params_extracted(self)` — [`L116`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_sql_fixes.py#L116) — #775: schema-qualified function must carry its parameters.
  - `test_simple_function_params_names(self)` — [`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_sql_fixes.py#L65)
  - `test_simple_function_params_types(self)` — [`L78`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_sql_fixes.py#L78)
  - `test_simple_function_with_two_params_extracted(self)` — [`L52`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_sql_fixes.py#L52) — A simple (non-schema) function with params returns 1 SQLFunction.
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`SQLFunction`](../../../tree_sitter_analyzer/models/sql_models.md#SQLFunction), [`parameters`](../../../tree_sitter_analyzer/models/sql_models.md#SQLElement.parameters), [`name`](../../../tree_sitter_analyzer/models/sql_models.md#SQLParameter.name), [`data_type`](../../../tree_sitter_analyzer/models/sql_models.md#SQLParameter.data_type)  (1 test-only)

### `TestIsInSqlComment`
- def: [`tests/unit/languages/test_sql_fixes.py:295`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_sql_fixes.py#L295)
- doc: Unit tests for _is_in_sql_comment helper.
- signature: `class TestIsInSqlComment:`
- members:
  - `test_after_closed_block_comment(self)` — [`L315`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_sql_fixes.py#L315)
  - `test_after_line_comment_on_same_line(self)` — [`L306`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_sql_fixes.py#L306)
  - `test_inside_block_comment(self)` — [`L311`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_sql_fixes.py#L311)
  - `test_inside_line_comment(self)` — [`L302`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_sql_fixes.py#L302)
  - `test_not_in_comment_plain_text(self)` — [`L298`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_sql_fixes.py#L298)
- uses (calls/refs, reference-scoped): [`_is_in_sql_comment`](../../../tree_sitter_analyzer/languages/sql_plugin/table_extractor.md#_is_in_sql_comment)

### `TestQuotedTableNameRegex`
- def: [`tests/unit/languages/test_sql_fixes.py:380`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_sql_fixes.py#L380)
- doc: #881: regex fallback must match ANSI, MySQL, and SQL Server quoted table names.
- signature: `class TestQuotedTableNameRegex:`
- members:
  - `test_ansi_double_quoted_name_extracted(self)` — [`L383`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_sql_fixes.py#L383) — ANSI SQL: CREATE TABLE "Order Details" (...) must be recovered.
  - `test_bare_identifier_still_works_after_regex_change(self)` — [`L420`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_sql_fixes.py#L420) — Regression: bare CREATE TABLE orders (...) still extracted.
  - `test_case_sensitive_quoted_names_not_deduped(self)` — [`L429`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_sql_fixes.py#L429) — Quoted table names differing only in case must both be recovered (Codex P2).
  - `test_mysql_backtick_quoted_name_extracted(self)` — [`L392`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_sql_fixes.py#L392) — MySQL style: CREATE TABLE `order details` (...) must be recovered.
  - `test_quoted_schema_plus_quoted_table(self)` — [`L410`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_sql_fixes.py#L410) — ANSI: CREATE TABLE "my schema"."my table" (...) — both stripped.
  - `test_sql_server_bracket_quoted_name_extracted(self)` — [`L401`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_sql_fixes.py#L401) — SQL Server: CREATE TABLE [Order Details] (...) must be recovered.
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`SQLTable`](../../../tree_sitter_analyzer/models/sql_models.md#SQLTable), [`fill_missing_sql_tables_from_regex`](../../../tree_sitter_analyzer/languages/sql_plugin/table_extractor.md#fill_missing_sql_tables_from_regex), [`schema_name`](../../../tree_sitter_analyzer/models/sql_models.md#SQLElement.schema_name)

### `TestRegexFallbackColumnsPopulated`
- def: [`tests/unit/languages/test_sql_fixes.py:445`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_sql_fixes.py#L445)
- doc: #880: regex-recovered tables must have their columns populated, not empty.
- signature: `class TestRegexFallbackColumnsPopulated:`
- members:
  - `test_ctas_with_parenthesized_select_expression_produces_no_columns(self)` — [`L504`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_sql_fixes.py#L504) — CTAS with CAST(...) in SELECT must not produce bogus columns (Codex P2).
  - `test_not_null_constraint_captured(self)` — [`L484`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_sql_fixes.py#L484) — NOT NULL constraint on a recovered column must set nullable=False.
  - `test_primary_key_constraint_line_excluded_from_columns(self)` — [`L513`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_sql_fixes.py#L513) — PRIMARY KEY constraint lines must not produce spurious columns.
  - `test_recovered_table_column_names(self)` — [`L459`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_sql_fixes.py#L459) — Column names must match the original DDL.
  - `test_recovered_table_column_types(self)` — [`L471`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_sql_fixes.py#L471) — Column data types must be captured.
  - `test_recovered_table_has_correct_column_count(self)` — [`L448`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_sql_fixes.py#L448) — A 3-column table recovered via regex fallback must yield 3 columns.
  - `test_table_without_column_list_has_empty_columns(self)` — [`L495`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_sql_fixes.py#L495) — AS SELECT form produces 0 columns (no column-list body).
- uses (calls/refs, reference-scoped): [`SQLTable`](../../../tree_sitter_analyzer/models/sql_models.md#SQLTable), [`fill_missing_sql_tables_from_regex`](../../../tree_sitter_analyzer/languages/sql_plugin/table_extractor.md#fill_missing_sql_tables_from_regex), [`columns`](../../../tree_sitter_analyzer/models/sql_models.md#SQLElement.columns), [`name`](../../../tree_sitter_analyzer/models/sql_models.md#SQLColumn.name), [`data_type`](../../../tree_sitter_analyzer/models/sql_models.md#SQLColumn.data_type), [`nullable`](../../../tree_sitter_analyzer/models/sql_models.md#SQLColumn.nullable)

## Functions
- `_extract(sql: str)` — [`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_sql_fixes.py#L37) — Parse SQL and run extract_sql_elements; return the element list.
- `_parse(sql: str)` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_sql_fixes.py#L29) — Return a tree-sitter Tree for the given SQL string.

## Module values
- `TREE_SITTER_SQL_AVAILABLE` — [`L17`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_sql_fixes.py#L17)
- `_SQL_FOREIGN_KEY_CASCADE` — [`L230`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_sql_fixes.py#L230)

