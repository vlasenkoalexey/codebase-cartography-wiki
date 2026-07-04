---
title: 'Module: tree_sitter_analyzer/platform_compat/fixtures.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/platform_compat/fixtures.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.platform_compat.fixtures`/
symbols:
  ALL_FIXTURES: ALL_FIXTURES.
  FIXTURE_FUNCTION_WITH_SELECT: FIXTURE_FUNCTION_WITH_SELECT.
  FIXTURE_TRIGGER_WITH_DESCRIPTION: FIXTURE_TRIGGER_WITH_DESCRIPTION.
  FIXTURE_FUNCTION_WITH_AUTO_INCREMENT: FIXTURE_FUNCTION_WITH_AUTO_INCREMENT.
  FIXTURE_PHANTOM_TRIGGER: FIXTURE_PHANTOM_TRIGGER.
  SQLTestFixture.id: SQLTestFixture#id.
  SQLTestFixture: SQLTestFixture#
  FIXTURE_VIEW_IN_ERROR_NODE: FIXTURE_VIEW_IN_ERROR_NODE.
  FIXTURE_PROCEDURE_WITH_COMMENTS: FIXTURE_PROCEDURE_WITH_COMMENTS.
  FIXTURE_INDEX_ON_EXPRESSION: FIXTURE_INDEX_ON_EXPRESSION.
  SQLTestFixture.sql: SQLTestFixture#sql.
  SQLTestFixture.expected_constructs: SQLTestFixture#expected_constructs.
  SQLTestFixture.description: SQLTestFixture#description.
  FIXTURE_SIMPLE_TABLE: FIXTURE_SIMPLE_TABLE.
  FIXTURE_COMPLEX_TABLE: FIXTURE_COMPLEX_TABLE.
  FIXTURE_VIEW_WITH_JOIN: FIXTURE_VIEW_WITH_JOIN.
  FIXTURE_STORED_PROCEDURE: FIXTURE_STORED_PROCEDURE.
  FIXTURE_FUNCTION_WITH_PARAMS: FIXTURE_FUNCTION_WITH_PARAMS.
  FIXTURE_TRIGGER_BEFORE_INSERT: FIXTURE_TRIGGER_BEFORE_INSERT.
  FIXTURE_INDEX_UNIQUE: FIXTURE_INDEX_UNIQUE.
  SQLTestFixture.is_edge_case: SQLTestFixture#is_edge_case.
  SQLTestFixture.known_platform_issues: SQLTestFixture#known_platform_issues.
---
# Module: [`tree_sitter_analyzer/platform_compat/fixtures.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/fixtures.py)

## Classes
### `SQLTestFixture`
- def: [`tree_sitter_analyzer/platform_compat/fixtures.py:5`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/fixtures.py#L5)
- doc: A SQL code sample for testing platform compatibility.
- signature: `class SQLTestFixture:`
- members:
  - `description` — [`L10`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/fixtures.py#L10)
  - `expected_constructs` — [`L11`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/fixtures.py#L11)
  - `id` — [`L8`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/fixtures.py#L8)
  - `is_edge_case` — [`L14`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/fixtures.py#L14)
  - `known_platform_issues` — [`L15`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/fixtures.py#L15)
  - `sql` — [`L9`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/fixtures.py#L9)
- used by: [`record_all`](recorder.md#BehaviorRecorder.record_all), [`record_fixture`](recorder.md#BehaviorRecorder.record_fixture), [`FIXTURE_FUNCTION_WITH_AUTO_INCREMENT`](fixtures.md#FIXTURE_FUNCTION_WITH_AUTO_INCREMENT), [`FIXTURE_FUNCTION_WITH_SELECT`](fixtures.md#FIXTURE_FUNCTION_WITH_SELECT), [`FIXTURE_PHANTOM_TRIGGER`](fixtures.md#FIXTURE_PHANTOM_TRIGGER), [`FIXTURE_TRIGGER_WITH_DESCRIPTION`](fixtures.md#FIXTURE_TRIGGER_WITH_DESCRIPTION), [`FIXTURE_INDEX_ON_EXPRESSION`](fixtures.md#FIXTURE_INDEX_ON_EXPRESSION), [`FIXTURE_PROCEDURE_WITH_COMMENTS`](fixtures.md#FIXTURE_PROCEDURE_WITH_COMMENTS), [`FIXTURE_VIEW_IN_ERROR_NODE`](fixtures.md#FIXTURE_VIEW_IN_ERROR_NODE), [`FIXTURE_COMPLEX_TABLE`](fixtures.md#FIXTURE_COMPLEX_TABLE), [`FIXTURE_FUNCTION_WITH_PARAMS`](fixtures.md#FIXTURE_FUNCTION_WITH_PARAMS), [`FIXTURE_INDEX_UNIQUE`](fixtures.md#FIXTURE_INDEX_UNIQUE), [`FIXTURE_SIMPLE_TABLE`](fixtures.md#FIXTURE_SIMPLE_TABLE), [`FIXTURE_STORED_PROCEDURE`](fixtures.md#FIXTURE_STORED_PROCEDURE), [`FIXTURE_TRIGGER_BEFORE_INSERT`](fixtures.md#FIXTURE_TRIGGER_BEFORE_INSERT), [`FIXTURE_VIEW_WITH_JOIN`](fixtures.md#FIXTURE_VIEW_WITH_JOIN)  (2 test-only)

## Module values
- `ALL_FIXTURES` — [`L213`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/fixtures.py#L213)
- `FIXTURE_COMPLEX_TABLE` — [`L33`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/fixtures.py#L33)
- `FIXTURE_FUNCTION_WITH_AUTO_INCREMENT` — [`L142`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/fixtures.py#L142)
- `FIXTURE_FUNCTION_WITH_PARAMS` — [`L72`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/fixtures.py#L72)
- `FIXTURE_FUNCTION_WITH_SELECT` — [`L110`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/fixtures.py#L110)
- `FIXTURE_INDEX_ON_EXPRESSION` — [`L203`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/fixtures.py#L203)
- `FIXTURE_INDEX_UNIQUE` — [`L99`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/fixtures.py#L99)
- `FIXTURE_PHANTOM_TRIGGER` — [`L173`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/fixtures.py#L173)
- `FIXTURE_PROCEDURE_WITH_COMMENTS` — [`L186`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/fixtures.py#L186)
- `FIXTURE_SIMPLE_TABLE` — [`L20`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/fixtures.py#L20)
- `FIXTURE_STORED_PROCEDURE` — [`L60`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/fixtures.py#L60)
- `FIXTURE_TRIGGER_BEFORE_INSERT` — [`L85`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/fixtures.py#L85)
- `FIXTURE_TRIGGER_WITH_DESCRIPTION` — [`L126`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/fixtures.py#L126)
- `FIXTURE_VIEW_IN_ERROR_NODE` — [`L160`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/fixtures.py#L160)
- `FIXTURE_VIEW_WITH_JOIN` — [`L48`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/fixtures.py#L48)

