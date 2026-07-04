---
title: 'Module: tests/unit/mcp/test_server_missing_branches.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_server_missing_branches.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_server_missing_branches`/Test
symbols:
  TestCreateServerToolHandlers.test_set_project_path: CreateServerToolHandlers#test_set_project_path().
  TestHandleAnalyzeCode.test_analysis_failure: HandleAnalyzeCode#test_analysis_failure().
  TestHandleAnalyzeCode.test_analysis_none_result: HandleAnalyzeCode#test_analysis_none_result().
  TestCreateServerToolHandlers.test_project_root_stored: CreateServerToolHandlers#test_project_root_stored().
  TestHandleAnalyzeCode.test_missing_file_path_uses_universal_tool: HandleAnalyzeCode#test_missing_file_path_uses_universal_tool().
  TestHandleAnalyzeCode.test_missing_file_path_no_universal_raises: HandleAnalyzeCode#test_missing_file_path_no_universal_raises().
  TestHandleAnalyzeCode.test_universal_tool_raises_valueerror: HandleAnalyzeCode#test_universal_tool_raises_valueerror().
  TestReadResource.test_read_code_file_resource: ReadResource#test_read_code_file_resource().
  TestReadResource.test_read_project_stats_resource: ReadResource#test_read_project_stats_resource().
  TestCreateServerToolHandlers.test_set_project_path_reinit: CreateServerToolHandlers#test_set_project_path_reinit().
  TestCalculateFileMetrics.test_calculate_metrics: CalculateFileMetrics#test_calculate_metrics().
  TestCalculateFileMetrics.test_calculate_metrics_nonexistent_file: CalculateFileMetrics#test_calculate_metrics_nonexistent_file().
  TestCalculateFileMetrics.test_calculate_metrics_empty_file: CalculateFileMetrics#test_calculate_metrics_empty_file().
  TestReadResource.test_read_resource_not_found: ReadResource#test_read_resource_not_found().
  TestCreateServerToolHandlers.test_create_server_returns_server: CreateServerToolHandlers#test_create_server_returns_server().
  TestRun.test_run_raises_when_mcp_not_available: Run#test_run_raises_when_mcp_not_available().
  TestParseMcpArgs.test_no_args: ParseMcpArgs#test_no_args().
  TestParseMcpArgs.test_unknown_args_raises: ParseMcpArgs#test_unknown_args_raises().
  TestParseMcpArgs.test_with_project_root: ParseMcpArgs#test_with_project_root().
  TestMainFunction.test_main_keyboard_interrupt: MainFunction#test_main_keyboard_interrupt().
  TestMainFunction.test_main_exception: MainFunction#test_main_exception().
  TestMainFunction.test_main_sync: MainFunction#test_main_sync().
  TestParseMcpArgs: ParseMcpArgs#
  TestHandleAnalyzeCode: HandleAnalyzeCode#
  TestHandleAnalyzeCode.tmp_path: HandleAnalyzeCode#tmp_path().
  TestCalculateFileMetrics: CalculateFileMetrics#
  TestCalculateFileMetrics.tmp_path: CalculateFileMetrics#tmp_path().
  TestReadResource: ReadResource#
  TestReadResource.tmp_path: ReadResource#tmp_path().
  TestCreateServerToolHandlers: CreateServerToolHandlers#
  TestCreateServerToolHandlers.tmp_path: CreateServerToolHandlers#tmp_path().
  TestRun: Run#
  TestRun.tmp_path: Run#tmp_path().
  TestMainFunction: MainFunction#
---
# Module: [`tests/unit/mcp/test_server_missing_branches.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_missing_branches.py)

## Classes
### `TestCalculateFileMetrics`
- def: [`tests/unit/mcp/test_server_missing_branches.py:128`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_missing_branches.py#L128)
- signature: `class TestCalculateFileMetrics:`
- members:
  - `test_calculate_metrics(self, tmp_path)` — [`L134`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_missing_branches.py#L134)
  - `test_calculate_metrics_empty_file(self, tmp_path)` — [`L153`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_missing_branches.py#L153)
  - `test_calculate_metrics_nonexistent_file(self, tmp_path)` — [`L145`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_missing_branches.py#L145)
  - `tmp_path(self)` — [`L130`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_missing_branches.py#L130)
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerMCPServer`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer), [`_calculate_file_metrics`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer._calculate_file_metrics)

### `TestCreateServerToolHandlers`
- def: [`tests/unit/mcp/test_server_missing_branches.py:214`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_missing_branches.py#L214)
- signature: `class TestCreateServerToolHandlers:`
- members:
  - `test_create_server_returns_server(self, tmp_path)` — [`L220`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_missing_branches.py#L220)
  - `test_project_root_stored(self, tmp_path)` — [`L237`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_missing_branches.py#L237)
  - `test_set_project_path(self, tmp_path)` — [`L228`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_missing_branches.py#L228)
  - `test_set_project_path_reinit(self, tmp_path)` — [`L245`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_missing_branches.py#L245)
  - `tmp_path(self)` — [`L216`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_missing_branches.py#L216)
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerMCPServer`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer), [`UnifiedAnalysisEngine`](../../../tree_sitter_analyzer/core/analysis_engine.md#UnifiedAnalysisEngine), [`set_project_path`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.set_project_path), [`create_server`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.create_server), [`analysis_engine`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.analysis_engine), [`_project_root`](../../../tree_sitter_analyzer/core/analysis_engine.md#UnifiedAnalysisEngine._project_root)

### `TestHandleAnalyzeCode`
- def: [`tests/unit/mcp/test_server_missing_branches.py:50`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_missing_branches.py#L50)
- signature: `class TestHandleAnalyzeCode:`
- members:
  - `test_analysis_failure(self, tmp_path)` — [`L93`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_missing_branches.py#L93) — analysis_result.success == False
  - `test_analysis_none_result(self, tmp_path)` — [`L109`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_missing_branches.py#L109) — analysis_result is None
  - `test_missing_file_path_no_universal_raises(self, tmp_path)` — [`L70`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_missing_branches.py#L70) — no file_path and no universal tool
  - `test_missing_file_path_uses_universal_tool(self, tmp_path)` — [`L57`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_missing_branches.py#L57) — no file_path, universal tool available, succeeds
  - `test_universal_tool_raises_valueerror(self, tmp_path)` — [`L80`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_missing_branches.py#L80) — Universal tool re-raises ValueError
  - `tmp_path(self)` — [`L52`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_missing_branches.py#L52)
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerMCPServer`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer), [`analyze`](../../../tree_sitter_analyzer/core/_analysis_engine_analysis_mixin.md#UnifiedAnalysisEngineAnalysisMixin.analyze), [`_analyze_code_scale`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer._analyze_code_scale), [`universal_analyze_tool`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.universal_analyze_tool), [`analysis_engine`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.analysis_engine)

### `TestMainFunction`
- def: [`tests/unit/mcp/test_server_missing_branches.py:280`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_missing_branches.py#L280)
- signature: `class TestMainFunction:`
- members:
  - `test_main_exception(self)` — [`L302`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_missing_branches.py#L302)
  - `test_main_keyboard_interrupt(self)` — [`L282`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_missing_branches.py#L282)
  - `test_main_sync(self)` — [`L321`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_missing_branches.py#L321)
- uses (calls/refs, reference-scoped): [`main`](../../../tree_sitter_analyzer/mcp/server.md#main), [`main_sync`](../../../tree_sitter_analyzer/mcp/server.md#main_sync)

### `TestParseMcpArgs`
- def: [`tests/unit/mcp/test_server_missing_branches.py:21`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_missing_branches.py#L21)
- signature: `class TestParseMcpArgs:`
- members:
  - `test_no_args(self)` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_missing_branches.py#L22)
  - `test_unknown_args_raises(self)` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_missing_branches.py#L28)
  - `test_with_project_root(self)` — [`L34`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_missing_branches.py#L34)
- uses (calls/refs, reference-scoped): [`parse_mcp_args`](../../../tree_sitter_analyzer/mcp/server.md#parse_mcp_args)

### `TestReadResource`
- def: [`tests/unit/mcp/test_server_missing_branches.py:170`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_missing_branches.py#L170)
- signature: `class TestReadResource:`
- members:
  - `test_read_code_file_resource(self, tmp_path)` — [`L177`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_missing_branches.py#L177)
  - `test_read_project_stats_resource(self, tmp_path)` — [`L189`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_missing_branches.py#L189)
  - `test_read_resource_not_found(self, tmp_path)` — [`L201`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_missing_branches.py#L201)
  - `tmp_path(self)` — [`L172`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_missing_branches.py#L172)
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerMCPServer`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer), [`project_stats_resource`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.project_stats_resource), [`code_file_resource`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.code_file_resource), [`_read_resource`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer._read_resource)

### `TestRun`
- def: [`tests/unit/mcp/test_server_missing_branches.py:259`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_missing_branches.py#L259)
- signature: `class TestRun:`
- members:
  - `test_run_raises_when_mcp_not_available(self, tmp_path)` — [`L266`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_missing_branches.py#L266)
  - `tmp_path(self)` — [`L261`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_server_missing_branches.py#L261)
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerMCPServer`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer), [`run`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.run)

