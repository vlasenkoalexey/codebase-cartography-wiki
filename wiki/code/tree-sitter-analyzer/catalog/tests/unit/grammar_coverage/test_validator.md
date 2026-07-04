---
title: 'Module: tests/unit/grammar_coverage/test_validator.py'
type: catalog
provenance: extracted
module: tests/unit/grammar_coverage/test_validator.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.grammar_coverage.test_validator`/Test
symbols:
  TestGenerateCoverageReport.test_generate_report_with_uncovered_types: GenerateCoverageReport#test_generate_report_with_uncovered_types().
  TestGenerateCoverageReport.test_generate_report_full_coverage: GenerateCoverageReport#test_generate_report_full_coverage().
  TestGenerateCoverageReport.test_generate_report_zero_coverage: GenerateCoverageReport#test_generate_report_zero_coverage().
  TestEdgeCases.test_coverage_with_zero_total_types: EdgeCases#test_coverage_with_zero_total_types().
  TestCoverageReport.test_coverage_report_creation: CoverageReport#test_coverage_report_creation().
  TestCoverageReport.test_coverage_report_zero_coverage: CoverageReport#test_coverage_report_zero_coverage().
  TestCoverageReport.test_coverage_report_full_coverage: CoverageReport#test_coverage_report_full_coverage().
  TestValidatePluginCoverage.test_validate_plugin_coverage_mocked: ValidatePluginCoverage#test_validate_plugin_coverage_mocked().
  TestValidatePluginCoverage.test_validate_python_coverage_real_files: ValidatePluginCoverage#test_validate_python_coverage_real_files().
  TestCheckCoverageThreshold.test_coverage_meets_threshold: CheckCoverageThreshold#test_coverage_meets_threshold().
  TestCheckCoverageThreshold.test_coverage_below_threshold: CheckCoverageThreshold#test_coverage_below_threshold().
  TestCheckCoverageThreshold.test_threshold_defaults_to_100: CheckCoverageThreshold#test_threshold_defaults_to_100().
  TestCheckCoverageThreshold.test_edge_cases: CheckCoverageThreshold#test_edge_cases().
  TestCountNodeTypes.test_count_node_types_with_mock_tree: CountNodeTypes#test_count_node_types_with_mock_tree().
  TestCountNodeTypes.test_count_node_types_ignores_unnamed_nodes: CountNodeTypes#test_count_node_types_ignores_unnamed_nodes().
  TestCountNodeTypes.test_count_node_types_nested_structure: CountNodeTypes#test_count_node_types_nested_structure().
  TestGetLanguageExtension.test_get_supported_extensions: GetLanguageExtension#test_get_supported_extensions().
  TestGetLanguageExtension.test_get_unsupported_extension_raises_error: GetLanguageExtension#test_get_unsupported_extension_raises_error().
  TestLoadExpectedJson.test_load_valid_json: LoadExpectedJson#test_load_valid_json().
  TestLoadExpectedJson.test_load_missing_file_raises_error: LoadExpectedJson#test_load_missing_file_raises_error().
  TestLoadExpectedJson.test_load_invalid_json_raises_error: LoadExpectedJson#test_load_invalid_json_raises_error().
  TestEdgeCases.test_empty_corpus_file: EdgeCases#test_empty_corpus_file().
  TestCoverageReport: CoverageReport#
  TestGenerateCoverageReport: GenerateCoverageReport#
  TestCheckCoverageThreshold: CheckCoverageThreshold#
  TestCountNodeTypes: CountNodeTypes#
  TestGetLanguageExtension: GetLanguageExtension#
  TestLoadExpectedJson: LoadExpectedJson#
  TestValidatePluginCoverage: ValidatePluginCoverage#
  TestEdgeCases: EdgeCases#
---
# Module: [`tests/unit/grammar_coverage/test_validator.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator.py)

## Classes
### `TestCheckCoverageThreshold`
- def: [`tests/unit/grammar_coverage/test_validator.py:153`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator.py#L153)
- doc: 测试 check_coverage_threshold 函数
- signature: `class TestCheckCoverageThreshold:`
- members:
  - `test_coverage_below_threshold(self)` — [`L162`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator.py#L162) — 测试覆盖率低于阈值
  - `test_coverage_meets_threshold(self)` — [`L156`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator.py#L156) — 测试覆盖率达到阈值
  - `test_edge_cases(self)` — [`L173`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator.py#L173) — 测试边缘情况
  - `test_threshold_defaults_to_100(self)` — [`L168`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator.py#L168) — 测试默认阈值为 100%
- uses (calls/refs, reference-scoped): [`check_coverage_threshold`](../../../tree_sitter_analyzer/grammar_coverage/validator.md#check_coverage_threshold)

### `TestCountNodeTypes`
- def: [`tests/unit/grammar_coverage/test_validator.py:181`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator.py#L181)
- doc: 测试 _count_node_types 函数（通过 validate_plugin_coverage 间接测试）
- signature: `class TestCountNodeTypes:`
- members:
  - `test_count_node_types_ignores_unnamed_nodes(self)` — [`L216`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator.py#L216) — 测试统计时忽略未命名节点
  - `test_count_node_types_nested_structure(self)` — [`L242`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator.py#L242) — 测试嵌套结构的节点统计
  - `test_count_node_types_with_mock_tree(self)` — [`L184`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator.py#L184) — 测试节点类型统计（使用 mock tree）
- uses (calls/refs, reference-scoped): [`_count_node_types`](../../../tree_sitter_analyzer/grammar_coverage/validator.md#_count_node_types)

### `TestCoverageReport`
- def: [`tests/unit/grammar_coverage/test_validator.py:32`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator.py#L32)
- doc: 测试 CoverageReport 数据结构
- signature: `class TestCoverageReport:`
- members:
  - `test_coverage_report_creation(self)` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator.py#L35) — 测试创建 CoverageReport 实例
  - `test_coverage_report_full_coverage(self)` — [`L71`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator.py#L71) — 测试 100% 覆盖率的报告
  - `test_coverage_report_zero_coverage(self)` — [`L55`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator.py#L55) — 测试 0% 覆盖率的报告
- uses (calls/refs, reference-scoped): [`uncovered_types`](../../../tree_sitter_analyzer/grammar_coverage/validator.md#CoverageReport.uncovered_types), [`coverage_percentage`](../../../tree_sitter_analyzer/grammar_coverage/validator.md#CoverageReport.coverage_percentage), [`covered_node_types`](../../../tree_sitter_analyzer/grammar_coverage/validator.md#CoverageReport.covered_node_types), [`total_node_types`](../../../tree_sitter_analyzer/grammar_coverage/validator.md#CoverageReport.total_node_types), [`CoverageReport`](../../../tree_sitter_analyzer/grammar_coverage/validator.md#CoverageReport), [`language`](../../../tree_sitter_analyzer/grammar_coverage/validator.md#CoverageReport.language), [`corpus_file`](../../../tree_sitter_analyzer/grammar_coverage/validator.md#CoverageReport.corpus_file), [`actual_node_types`](../../../tree_sitter_analyzer/grammar_coverage/validator.md#CoverageReport.actual_node_types), [`expected_node_types`](../../../tree_sitter_analyzer/grammar_coverage/validator.md#CoverageReport.expected_node_types)

### `TestEdgeCases`
- def: [`tests/unit/grammar_coverage/test_validator.py:402`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator.py#L402)
- doc: 测试边缘情况和错误处理
- signature: `class TestEdgeCases:`
- members:
  - `test_coverage_with_zero_total_types(self)` — [`L422`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator.py#L422) — 测试总类型数为 0 的情况
  - `test_empty_corpus_file(self)` — [`L405`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator.py#L405) — 测试空的 corpus 文件
- uses (calls/refs, reference-scoped): [`uncovered_types`](../../../tree_sitter_analyzer/grammar_coverage/validator.md#CoverageReport.uncovered_types), [`generate_coverage_report`](../../../tree_sitter_analyzer/grammar_coverage/validator.md#generate_coverage_report), [`coverage_percentage`](../../../tree_sitter_analyzer/grammar_coverage/validator.md#CoverageReport.coverage_percentage), [`covered_node_types`](../../../tree_sitter_analyzer/grammar_coverage/validator.md#CoverageReport.covered_node_types), [`total_node_types`](../../../tree_sitter_analyzer/grammar_coverage/validator.md#CoverageReport.total_node_types), [`CoverageReport`](../../../tree_sitter_analyzer/grammar_coverage/validator.md#CoverageReport), [`language`](../../../tree_sitter_analyzer/grammar_coverage/validator.md#CoverageReport.language), [`_count_node_types`](../../../tree_sitter_analyzer/grammar_coverage/validator.md#_count_node_types), [`corpus_file`](../../../tree_sitter_analyzer/grammar_coverage/validator.md#CoverageReport.corpus_file), [`actual_node_types`](../../../tree_sitter_analyzer/grammar_coverage/validator.md#CoverageReport.actual_node_types), [`expected_node_types`](../../../tree_sitter_analyzer/grammar_coverage/validator.md#CoverageReport.expected_node_types)

### `TestGenerateCoverageReport`
- def: [`tests/unit/grammar_coverage/test_validator.py:88`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator.py#L88)
- doc: 测试 generate_coverage_report 函数
- signature: `class TestGenerateCoverageReport:`
- members:
  - `test_generate_report_full_coverage(self)` — [`L113`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator.py#L113) — 测试生成 100% 覆盖的报告
  - `test_generate_report_with_uncovered_types(self)` — [`L91`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator.py#L91) — 测试生成包含未覆盖类型的报告
  - `test_generate_report_zero_coverage(self)` — [`L133`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator.py#L133) — 测试生成 0% 覆盖的报告
- uses (calls/refs, reference-scoped): [`uncovered_types`](../../../tree_sitter_analyzer/grammar_coverage/validator.md#CoverageReport.uncovered_types), [`generate_coverage_report`](../../../tree_sitter_analyzer/grammar_coverage/validator.md#generate_coverage_report), [`coverage_percentage`](../../../tree_sitter_analyzer/grammar_coverage/validator.md#CoverageReport.coverage_percentage), [`covered_node_types`](../../../tree_sitter_analyzer/grammar_coverage/validator.md#CoverageReport.covered_node_types), [`total_node_types`](../../../tree_sitter_analyzer/grammar_coverage/validator.md#CoverageReport.total_node_types), [`CoverageReport`](../../../tree_sitter_analyzer/grammar_coverage/validator.md#CoverageReport), [`language`](../../../tree_sitter_analyzer/grammar_coverage/validator.md#CoverageReport.language), [`corpus_file`](../../../tree_sitter_analyzer/grammar_coverage/validator.md#CoverageReport.corpus_file), [`actual_node_types`](../../../tree_sitter_analyzer/grammar_coverage/validator.md#CoverageReport.actual_node_types), [`expected_node_types`](../../../tree_sitter_analyzer/grammar_coverage/validator.md#CoverageReport.expected_node_types)

### `TestGetLanguageExtension`
- def: [`tests/unit/grammar_coverage/test_validator.py:269`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator.py#L269)
- doc: 测试 _get_language_extension 函数
- signature: `class TestGetLanguageExtension:`
- members:
  - `test_get_supported_extensions(self)` — [`L272`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator.py#L272) — 测试获取支持的文件扩展名
  - `test_get_unsupported_extension_raises_error(self)` — [`L285`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator.py#L285) — 测试不支持的语言抛出 ValueError
- uses (calls/refs, reference-scoped): [`_get_language_extension`](../../../tree_sitter_analyzer/grammar_coverage/validator.md#_get_language_extension)

### `TestLoadExpectedJson`
- def: [`tests/unit/grammar_coverage/test_validator.py:295`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator.py#L295)
- doc: 测试 _load_expected_json 函数
- signature: `class TestLoadExpectedJson:`
- members:
  - `test_load_invalid_json_raises_error(self)` — [`L328`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator.py#L328) — 测试无效 JSON 抛出 JSONDecodeError
  - `test_load_missing_file_raises_error(self)` — [`L318`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator.py#L318) — 测试文件不存在抛出 FileNotFoundError
  - `test_load_valid_json(self)` — [`L298`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator.py#L298) — 测试加载有效的 JSON 文件
- uses (calls/refs, reference-scoped): [`_load_expected_json`](../../../tree_sitter_analyzer/grammar_coverage/validator.md#_load_expected_json)

### `TestValidatePluginCoverage`
- def: [`tests/unit/grammar_coverage/test_validator.py:340`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator.py#L340)
- doc: 测试 validate_plugin_coverage 函数（集成测试风格，使用真实文件）
- signature: `class TestValidatePluginCoverage:`
- members:
  - `test_validate_plugin_coverage_mocked(self, mock_get_ext, mock_get_covered, mock_load_expected, mock_parse_corpus)` — [`L371`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator.py#L371) — 测试 validate_plugin_coverage 逻辑（使用 mock）
  - `test_validate_python_coverage_real_files(self)` — [`L349`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_validator.py#L349) — 测试使用真实 Python corpus 文件验证覆盖率
- uses (calls/refs, reference-scoped): [`uncovered_types`](../../../tree_sitter_analyzer/grammar_coverage/validator.md#CoverageReport.uncovered_types), [`coverage_percentage`](../../../tree_sitter_analyzer/grammar_coverage/validator.md#CoverageReport.coverage_percentage), [`validate_plugin_coverage_sync`](../../../tree_sitter_analyzer/grammar_coverage/validator.md#validate_plugin_coverage_sync), [`covered_node_types`](../../../tree_sitter_analyzer/grammar_coverage/validator.md#CoverageReport.covered_node_types), [`total_node_types`](../../../tree_sitter_analyzer/grammar_coverage/validator.md#CoverageReport.total_node_types), [`language`](../../../tree_sitter_analyzer/grammar_coverage/validator.md#CoverageReport.language)

