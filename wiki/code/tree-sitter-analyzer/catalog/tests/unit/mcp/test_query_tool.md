---
title: 'Module: tests/unit/mcp/test_query_tool.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_query_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_query_tool`/
symbols:
  tool: tool().
  TestQueryToolInitialization: TestQueryToolInitialization#
  TestSetProjectPath: TestSetProjectPath#
  TestGetToolDefinition: TestGetToolDefinition#
  TestValidateArguments: TestValidateArguments#
  TestExecute: TestExecute#
  TestFormatSummary: TestFormatSummary#
  TestExtractNameFromContent: TestExtractNameFromContent#
  TestGetAvailableQueries: TestGetAvailableQueries#
  TestExecuteAdditionalCoverage: TestExecuteAdditionalCoverage#
  TestFormatSummaryAdditional: TestFormatSummaryAdditional#
  TestExtractNameAdditional: TestExtractNameAdditional#
  TestValidateArgumentsAdditional: TestValidateArgumentsAdditional#
  TestExecuteCoverageBoost: TestExecuteCoverageBoost#
  TestFormatSummaryCoverageBoost: TestFormatSummaryCoverageBoost#
  TestExtractNameCoverageBoost: TestExtractNameCoverageBoost#
  TestValidateArgumentsCoverageBoost: TestValidateArgumentsCoverageBoost#
  TestCategorizeQueries: TestCategorizeQueries#
  TestExecuteInvalidQueryKey: TestExecuteInvalidQueryKey#
  TestBuildNextSteps: TestBuildNextSteps#
  TestCategorizeQueriesCoverage: TestCategorizeQueriesCoverage#
  sample_python_file: sample_python_file().
  mock_query_results: mock_query_results().
---
# Module: [`tests/unit/mcp/test_query_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_query_tool.py)

## Classes
### `TestBuildNextSteps`  ·  implements/extends TestBuildNextStepsTestMixin
- def: [`tests/unit/mcp/test_query_tool.py:185`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_query_tool.py#L185)
- doc: Tests for _build_next_steps method.
- signature: `class TestBuildNextSteps(TestBuildNextStepsTestMixin):`
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `TestCategorizeQueries`  ·  implements/extends TestCategorizeQueriesTestMixin
- def: [`tests/unit/mcp/test_query_tool.py:173`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_query_tool.py#L173)
- doc: Tests for _categorize_queries.
- signature: `class TestCategorizeQueries(TestCategorizeQueriesTestMixin):`
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `TestCategorizeQueriesCoverage`  ·  implements/extends TestCategorizeQueriesCoverageTestMixin
- def: [`tests/unit/mcp/test_query_tool.py:191`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_query_tool.py#L191)
- doc: Coverage for _categorize_queries remaining branches.
- signature: `class TestCategorizeQueriesCoverage(TestCategorizeQueriesCoverageTestMixin):`
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `TestExecute`  ·  implements/extends TestExecuteTestMixin
- def: [`tests/unit/mcp/test_query_tool.py:101`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_query_tool.py#L101)
- doc: Tests for execute method.
- signature: `class TestExecute(TestExecuteTestMixin):`
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `TestExecuteAdditionalCoverage`  ·  implements/extends TestExecuteAdditionalCoverageTestMixin
- def: [`tests/unit/mcp/test_query_tool.py:125`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_query_tool.py#L125)
- doc: Additional coverage for execute.
- signature: `class TestExecuteAdditionalCoverage(TestExecuteAdditionalCoverageTestMixin):`
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `TestExecuteCoverageBoost`  ·  implements/extends TestExecuteCoverageBoostTestMixin
- def: [`tests/unit/mcp/test_query_tool.py:149`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_query_tool.py#L149)
- doc: Coverage for execute edge branches.
- signature: `class TestExecuteCoverageBoost(TestExecuteCoverageBoostTestMixin):`
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `TestExecuteInvalidQueryKey`  ·  implements/extends TestExecuteInvalidQueryKeyTestMixin
- def: [`tests/unit/mcp/test_query_tool.py:179`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_query_tool.py#L179)
- doc: Tests for execute when query_key/empty results handling.
- signature: `class TestExecuteInvalidQueryKey(TestExecuteInvalidQueryKeyTestMixin):`
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `TestExtractNameAdditional`  ·  implements/extends TestExtractNameAdditionalTestMixin
- def: [`tests/unit/mcp/test_query_tool.py:137`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_query_tool.py#L137)
- doc: Additional coverage for _extract_name_from_content.
- signature: `class TestExtractNameAdditional(TestExtractNameAdditionalTestMixin):`
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `TestExtractNameCoverageBoost`  ·  implements/extends TestExtractNameCoverageBoostTestMixin
- def: [`tests/unit/mcp/test_query_tool.py:161`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_query_tool.py#L161)
- doc: Coverage for _extract_name_from_content branches.
- signature: `class TestExtractNameCoverageBoost(TestExtractNameCoverageBoostTestMixin):`
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `TestExtractNameFromContent`  ·  implements/extends TestExtractNameFromContentTestMixin
- def: [`tests/unit/mcp/test_query_tool.py:113`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_query_tool.py#L113)
- doc: Tests for _extract_name_from_content method.
- signature: `class TestExtractNameFromContent(TestExtractNameFromContentTestMixin):`
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `TestFormatSummary`  ·  implements/extends TestFormatSummaryTestMixin
- def: [`tests/unit/mcp/test_query_tool.py:107`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_query_tool.py#L107)
- doc: Tests for _format_summary method.
- signature: `class TestFormatSummary(TestFormatSummaryTestMixin):`
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `TestFormatSummaryAdditional`  ·  implements/extends TestFormatSummaryAdditionalTestMixin
- def: [`tests/unit/mcp/test_query_tool.py:131`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_query_tool.py#L131)
- doc: Additional coverage for _format_summary.
- signature: `class TestFormatSummaryAdditional(TestFormatSummaryAdditionalTestMixin):`
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `TestFormatSummaryCoverageBoost`  ·  implements/extends TestFormatSummaryCoverageBoostTestMixin
- def: [`tests/unit/mcp/test_query_tool.py:155`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_query_tool.py#L155)
- doc: Coverage for _format_summary branches.
- signature: `class TestFormatSummaryCoverageBoost(TestFormatSummaryCoverageBoostTestMixin):`
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `TestGetAvailableQueries`  ·  implements/extends TestGetAvailableQueriesTestMixin
- def: [`tests/unit/mcp/test_query_tool.py:119`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_query_tool.py#L119)
- doc: Tests for get_available_queries method.
- signature: `class TestGetAvailableQueries(TestGetAvailableQueriesTestMixin):`
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `TestGetToolDefinition`  ·  implements/extends TestGetToolDefinitionTestMixin
- def: [`tests/unit/mcp/test_query_tool.py:89`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_query_tool.py#L89)
- doc: Tests for get_tool_definition method.
- signature: `class TestGetToolDefinition(TestGetToolDefinitionTestMixin):`
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `TestQueryToolInitialization`  ·  implements/extends TestQueryToolInitializationTestMixin
- def: [`tests/unit/mcp/test_query_tool.py:77`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_query_tool.py#L77)
- doc: Tests for tool initialization.
- signature: `class TestQueryToolInitialization(TestQueryToolInitializationTestMixin):`
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `TestSetProjectPath`  ·  implements/extends TestSetProjectPathTestMixin
- def: [`tests/unit/mcp/test_query_tool.py:83`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_query_tool.py#L83)
- doc: Tests for set_project_path method.
- signature: `class TestSetProjectPath(TestSetProjectPathTestMixin):`
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `TestValidateArguments`  ·  implements/extends TestValidateArgumentsTestMixin
- def: [`tests/unit/mcp/test_query_tool.py:95`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_query_tool.py#L95)
- doc: Tests for validate_arguments method.
- signature: `class TestValidateArguments(TestValidateArgumentsTestMixin):`
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `TestValidateArgumentsAdditional`  ·  implements/extends TestValidateArgumentsAdditionalTestMixin
- def: [`tests/unit/mcp/test_query_tool.py:143`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_query_tool.py#L143)
- doc: Additional coverage for validate_arguments.
- signature: `class TestValidateArgumentsAdditional(TestValidateArgumentsAdditionalTestMixin):`
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `TestValidateArgumentsCoverageBoost`  ·  implements/extends TestValidateArgumentsCoverageBoostTestMixin
- def: [`tests/unit/mcp/test_query_tool.py:167`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_query_tool.py#L167)
- doc: Coverage for validate_arguments branches.
- signature: `class TestValidateArgumentsCoverageBoost(TestValidateArgumentsCoverageBoostTestMixin):`
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

## Functions
- `mock_query_results()` — [`L57`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_query_tool.py#L57) — Create mock query results.
- `sample_python_file(tmp_path: Path)` — [`L47`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_query_tool.py#L47) — Create a sample Python file for testing.
- `tool()` — [`L41`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_query_tool.py#L41) — Create a fresh tool instance for each test.

