---
title: 'Module: tests/unit/mcp/test_tools/test_read_partial_tool.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_tools/test_read_partial_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_tools.test_read_partial_tool`/TestReadPartialTool
symbols:
  TestReadPartialToolBatchExtra: BatchExtra#
  TestReadPartialToolCoverageGaps: CoverageGaps#
  TestReadPartialToolExecuteBatch: ExecuteBatch#
  TestReadPartialToolInit: Init#
  TestReadPartialToolGetToolSchema: GetToolSchema#
  TestReadPartialToolGetToolDefinition: GetToolDefinition#
  TestReadPartialToolValidateArguments: ValidateArguments#
  TestReadPartialToolExecute: Execute#
  TestReadPartialToolReadFilePartial: ReadFilePartial#
  TestReadPartialToolExecuteExtra: ExecuteExtra#
  TestReadPartialToolExecuteExtraContinued: ExecuteExtraContinued#
  TestReadPartialToolValidateExtra: ValidateExtra#
  TestReadPartialToolInit.__test__: Init#__test__.
  TestReadPartialToolGetToolSchema.__test__: GetToolSchema#__test__.
  TestReadPartialToolGetToolDefinition.__test__: GetToolDefinition#__test__.
  TestReadPartialToolValidateArguments.__test__: ValidateArguments#__test__.
  TestReadPartialToolExecute.__test__: Execute#__test__.
  TestReadPartialToolExecuteBatch.__test__: ExecuteBatch#__test__.
  TestReadPartialToolReadFilePartial.__test__: ReadFilePartial#__test__.
  TestReadPartialToolExecuteExtra.__test__: ExecuteExtra#__test__.
  TestReadPartialToolExecuteExtraContinued.__test__: ExecuteExtraContinued#__test__.
  TestReadPartialToolBatchExtra.__test__: BatchExtra#__test__.
  TestReadPartialToolValidateExtra.__test__: ValidateExtra#__test__.
  TestReadPartialToolCoverageGaps.__test__: CoverageGaps#__test__.
---
# Module: [`tests/unit/mcp/test_tools/test_read_partial_tool.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_read_partial_tool.py)

## Classes
### `TestReadPartialToolBatchExtra`  ·  implements/extends ReadPartialToolBatchExtraFileErrorMixin, ReadPartialToolBatchExtraLimitMixin, ReadPartialToolBatchExtraValidationMixin
- def: [`tests/unit/mcp/test_tools/test_read_partial_tool.py:98`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_read_partial_tool.py#L98)
- doc: Additional tests for uncovered _execute_batch() paths.
- signature: `class TestReadPartialToolBatchExtra(ReadPartialToolBatchExtraFileErrorMixin, ReadPartialToolBatchExtraLimitMixin, ReadPartialToolBatchExtraValidationMixin):`
- protocol/private: `__test__`[`L105`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_read_partial_tool.py#L105)
- uses (calls/refs, reference-scoped): (3 test-only callers)
- used by: (3 test-only callers)

### `TestReadPartialToolCoverageGaps`  ·  implements/extends ReadPartialToolCoverageBatchMixin, ReadPartialToolCoverageExecuteMixin, ReadPartialToolCoverageValidateMixin
- def: [`tests/unit/mcp/test_tools/test_read_partial_tool.py:114`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_read_partial_tool.py#L114)
- doc: Tests targeting specific uncovered lines in read_partial_tool.py.
- signature: `class TestReadPartialToolCoverageGaps(ReadPartialToolCoverageExecuteMixin, ReadPartialToolCoverageBatchMixin, ReadPartialToolCoverageValidateMixin):`
- protocol/private: `__test__`[`L121`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_read_partial_tool.py#L121)
- uses (calls/refs, reference-scoped): (3 test-only callers)
- used by: (3 test-only callers)

### `TestReadPartialToolExecute`  ·  implements/extends ReadPartialToolExecuteMixin
- def: [`tests/unit/mcp/test_tools/test_read_partial_tool.py:63`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_read_partial_tool.py#L63)
- doc: Tests for execute method (single mode).
- signature: `class TestReadPartialToolExecute(ReadPartialToolExecuteMixin):`
- protocol/private: `__test__`[`L66`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_read_partial_tool.py#L66)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `TestReadPartialToolExecuteBatch`  ·  implements/extends ReadPartialToolExecuteBatchProcessingMixin, ReadPartialToolExecuteBatchValidationMixin
- def: [`tests/unit/mcp/test_tools/test_read_partial_tool.py:69`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_read_partial_tool.py#L69)
- doc: Tests for _execute_batch method (batch mode).
- signature: `class TestReadPartialToolExecuteBatch(ReadPartialToolExecuteBatchValidationMixin, ReadPartialToolExecuteBatchProcessingMixin):`
- protocol/private: `__test__`[`L75`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_read_partial_tool.py#L75)
- uses (calls/refs, reference-scoped): (2 test-only callers)
- used by: (2 test-only callers)

### `TestReadPartialToolExecuteExtra`  ·  implements/extends ReadPartialToolExecuteExtraMixin
- def: [`tests/unit/mcp/test_tools/test_read_partial_tool.py:84`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_read_partial_tool.py#L84)
- doc: Additional tests for uncovered execute() paths.
- signature: `class TestReadPartialToolExecuteExtra(ReadPartialToolExecuteExtraMixin):`
- protocol/private: `__test__`[`L87`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_read_partial_tool.py#L87)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `TestReadPartialToolExecuteExtraContinued`  ·  implements/extends ReadPartialToolExecuteExtraContinuedMixin
- def: [`tests/unit/mcp/test_tools/test_read_partial_tool.py:90`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_read_partial_tool.py#L90)
- doc: Additional read_partial execute and agent summary tests.
- signature: `class TestReadPartialToolExecuteExtraContinued(ReadPartialToolExecuteExtraContinuedMixin):`
- protocol/private: `__test__`[`L95`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_read_partial_tool.py#L95)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `TestReadPartialToolGetToolDefinition`  ·  implements/extends ReadPartialToolGetToolDefinitionMixin
- def: [`tests/unit/mcp/test_tools/test_read_partial_tool.py:51`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_read_partial_tool.py#L51)
- doc: Tests for get_tool_definition method.
- signature: `class TestReadPartialToolGetToolDefinition(ReadPartialToolGetToolDefinitionMixin):`
- protocol/private: `__test__`[`L54`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_read_partial_tool.py#L54)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `TestReadPartialToolGetToolSchema`  ·  implements/extends ReadPartialToolGetToolSchemaMixin
- def: [`tests/unit/mcp/test_tools/test_read_partial_tool.py:45`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_read_partial_tool.py#L45)
- doc: Tests for get_tool_schema method.
- signature: `class TestReadPartialToolGetToolSchema(ReadPartialToolGetToolSchemaMixin):`
- protocol/private: `__test__`[`L48`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_read_partial_tool.py#L48)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `TestReadPartialToolInit`  ·  implements/extends ReadPartialToolInitMixin
- def: [`tests/unit/mcp/test_tools/test_read_partial_tool.py:39`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_read_partial_tool.py#L39)
- doc: Tests for ReadPartialTool initialization.
- signature: `class TestReadPartialToolInit(ReadPartialToolInitMixin):`
- protocol/private: `__test__`[`L42`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_read_partial_tool.py#L42)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `TestReadPartialToolReadFilePartial`  ·  implements/extends ReadPartialToolReadFilePartialMixin
- def: [`tests/unit/mcp/test_tools/test_read_partial_tool.py:78`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_read_partial_tool.py#L78)
- doc: Tests for _read_file_partial method.
- signature: `class TestReadPartialToolReadFilePartial(ReadPartialToolReadFilePartialMixin):`
- protocol/private: `__test__`[`L81`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_read_partial_tool.py#L81)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `TestReadPartialToolValidateArguments`  ·  implements/extends ReadPartialToolValidateArgumentsMixin
- def: [`tests/unit/mcp/test_tools/test_read_partial_tool.py:57`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_read_partial_tool.py#L57)
- doc: Tests for validate_arguments method.
- signature: `class TestReadPartialToolValidateArguments(ReadPartialToolValidateArgumentsMixin):`
- protocol/private: `__test__`[`L60`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_read_partial_tool.py#L60)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `TestReadPartialToolValidateExtra`  ·  implements/extends ReadPartialToolValidateExtraMixin
- def: [`tests/unit/mcp/test_tools/test_read_partial_tool.py:108`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_read_partial_tool.py#L108)
- doc: Additional tests for uncovered validate_arguments paths.
- signature: `class TestReadPartialToolValidateExtra(ReadPartialToolValidateExtraMixin):`
- protocol/private: `__test__`[`L111`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_read_partial_tool.py#L111)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

