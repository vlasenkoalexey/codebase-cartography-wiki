---
title: 'Module: tests/unit/grammar_coverage/test_introspector.py'
type: catalog
provenance: extracted
module: tests/unit/grammar_coverage/test_introspector.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.grammar_coverage.test_introspector`/
symbols:
  TestGetAllNodeTypes.test_all_supported_languages_work: TestGetAllNodeTypes#test_all_supported_languages_work().
  TestGetLanguageSummary.test_all_languages_summary: TestGetLanguageSummary#test_all_languages_summary().
  TestCrossLanguageConsistency.test_all_languages_have_function_definitions: TestCrossLanguageConsistency#test_all_languages_have_function_definitions().
  TestCrossLanguageConsistency.test_all_languages_have_reasonable_node_count: TestCrossLanguageConsistency#test_all_languages_have_reasonable_node_count().
  TestGetStructuralTypes.test_structural_and_extractable_are_complementary: TestGetStructuralTypes#test_structural_and_extractable_are_complementary().
  TestAutoDetectExtractableTypes.test_python_extractable_detection: TestAutoDetectExtractableTypes#test_python_extractable_detection().
  TestAutoDetectExtractableTypes.test_javascript_extractable_detection: TestAutoDetectExtractableTypes#test_javascript_extractable_detection().
  TestAutoDetectExtractableTypes.test_go_extractable_detection: TestAutoDetectExtractableTypes#test_go_extractable_detection().
  TestGetStructuralTypes.test_python_structural_detection: TestGetStructuralTypes#test_python_structural_detection().
  TestEdgeCases.test_empty_node_types_list: TestEdgeCases#test_empty_node_types_list().
  EXPECTED_GRAMMAR_COUNTS: EXPECTED_GRAMMAR_COUNTS.
  TestGetAllNodeTypes.test_python_node_extraction: TestGetAllNodeTypes#test_python_node_extraction().
  TestGetAllNodeTypes.test_javascript_node_extraction: TestGetAllNodeTypes#test_javascript_node_extraction().
  TestGetAllNodeTypes.test_go_node_extraction: TestGetAllNodeTypes#test_go_node_extraction().
  TestGetAllNodeTypes.test_unsupported_language_raises: TestGetAllNodeTypes#test_unsupported_language_raises().
  TestAutoDetectExtractableTypes.test_pattern_matching_logic: TestAutoDetectExtractableTypes#test_pattern_matching_logic().
  TestGetLanguageSummary.test_python_summary: TestGetLanguageSummary#test_python_summary().
  TestEdgeCases.test_no_extractable_types: TestEdgeCases#test_no_extractable_types().
  TestEdgeCases.test_no_structural_types: TestEdgeCases#test_no_structural_types().
  TestGetAllNodeTypes: TestGetAllNodeTypes#
  TestAutoDetectExtractableTypes: TestAutoDetectExtractableTypes#
  TestGetStructuralTypes: TestGetStructuralTypes#
  TestGetLanguageSummary: TestGetLanguageSummary#
  TestEdgeCases: TestEdgeCases#
  TestCrossLanguageConsistency: TestCrossLanguageConsistency#
---
# Module: [`tests/unit/grammar_coverage/test_introspector.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_introspector.py)

## Classes
### `TestAutoDetectExtractableTypes`
- def: [`tests/unit/grammar_coverage/test_introspector.py:122`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_introspector.py#L122)
- doc: 测试自动检测可提取节点类型。
- signature: `class TestAutoDetectExtractableTypes:`
- members:
  - `test_go_extractable_detection(self)` — [`L163`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_introspector.py#L163) — 测试 Go 语言的可提取节点检测。
  - `test_javascript_extractable_detection(self)` — [`L149`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_introspector.py#L149) — 测试 JavaScript 语言的可提取节点检测。
  - `test_pattern_matching_logic(self)` — [`L177`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_introspector.py#L177) — 测试模式匹配逻辑的正确性。
  - `test_python_extractable_detection(self)` — [`L125`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_introspector.py#L125) — 测试 Python 语言的可提取节点检测。
- uses (calls/refs, reference-scoped): [`get_all_node_types`](../../../tree_sitter_analyzer/grammar_coverage/introspector.md#get_all_node_types), [`auto_detect_extractable_types`](../../../tree_sitter_analyzer/grammar_coverage/introspector.md#auto_detect_extractable_types)

### `TestCrossLanguageConsistency`
- def: [`tests/unit/grammar_coverage/test_introspector.py:346`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_introspector.py#L346)
- doc: 测试跨语言一致性。
- signature: `class TestCrossLanguageConsistency:`
- members:
  - `test_all_languages_have_function_definitions(self)` — [`L349`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_introspector.py#L349) — 测试所有编程语言都有函数定义节点（数据格式语言除外）。
  - `test_all_languages_have_reasonable_node_count(self)` — [`L374`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_introspector.py#L374) — 测试所有语言的节点数量在合理范围内。
- uses (calls/refs, reference-scoped): [`loader`](../../../tree_sitter_analyzer/language_loader.md#loader), [`is_language_available`](../../../tree_sitter_analyzer/language_loader.md#LanguageLoader.is_language_available), [`get_all_node_types`](../../../tree_sitter_analyzer/grammar_coverage/introspector.md#get_all_node_types), [`auto_detect_extractable_types`](../../../tree_sitter_analyzer/grammar_coverage/introspector.md#auto_detect_extractable_types), [`get_language_summary`](../../../tree_sitter_analyzer/grammar_coverage/introspector.md#get_language_summary), [`LANGUAGE_MODULE_MAP`](../../../tree_sitter_analyzer/grammar_coverage/introspector.md#LANGUAGE_MODULE_MAP)  (1 test-only)

### `TestEdgeCases`
- def: [`tests/unit/grammar_coverage/test_introspector.py:313`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_introspector.py#L313)
- doc: 测试边界情况和错误处理。
- signature: `class TestEdgeCases:`
- members:
  - `test_empty_node_types_list(self)` — [`L316`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_introspector.py#L316) — 测试空节点列表的处理。
  - `test_no_extractable_types(self)` — [`L324`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_introspector.py#L324) — 测试无可提取节点的情况。
  - `test_no_structural_types(self)` — [`L331`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_introspector.py#L331) — 测试无结构性节点的情况（理论上不存在）。
- uses (calls/refs, reference-scoped): [`auto_detect_extractable_types`](../../../tree_sitter_analyzer/grammar_coverage/introspector.md#auto_detect_extractable_types), [`get_structural_types`](../../../tree_sitter_analyzer/grammar_coverage/introspector.md#get_structural_types)

### `TestGetAllNodeTypes`
- def: [`tests/unit/grammar_coverage/test_introspector.py:39`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_introspector.py#L39)
- doc: 测试从 tree-sitter 语法中提取所有节点类型。
- signature: `class TestGetAllNodeTypes:`
- members:
  - `test_all_supported_languages_work(self)` — [`L106`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_introspector.py#L106) — 测试所有支持的语言都能正常提取节点类型。
  - `test_go_node_extraction(self)` — [`L84`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_introspector.py#L84) — 测试 Go 语言的节点类型提取。
  - `test_javascript_node_extraction(self)` — [`L67`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_introspector.py#L67) — 测试 JavaScript 语言的节点类型提取。
  - `test_python_node_extraction(self)` — [`L42`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_introspector.py#L42) — 测试 Python 语言的节点类型提取。
  - `test_unsupported_language_raises(self)` — [`L101`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_introspector.py#L101) — 测试不支持的语言抛出异常。
- uses (calls/refs, reference-scoped): [`loader`](../../../tree_sitter_analyzer/language_loader.md#loader), [`is_language_available`](../../../tree_sitter_analyzer/language_loader.md#LanguageLoader.is_language_available), [`get_all_node_types`](../../../tree_sitter_analyzer/grammar_coverage/introspector.md#get_all_node_types), [`LANGUAGE_MODULE_MAP`](../../../tree_sitter_analyzer/grammar_coverage/introspector.md#LANGUAGE_MODULE_MAP)  (1 test-only)

### `TestGetLanguageSummary`
- def: [`tests/unit/grammar_coverage/test_introspector.py:249`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_introspector.py#L249)
- doc: 测试获取语言摘要功能。
- signature: `class TestGetLanguageSummary:`
- members:
  - `test_all_languages_summary(self)` — [`L279`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_introspector.py#L279) — 测试所有支持语言的摘要生成。
  - `test_python_summary(self)` — [`L252`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_introspector.py#L252) — 测试 Python 语言摘要生成。
- uses (calls/refs, reference-scoped): [`loader`](../../../tree_sitter_analyzer/language_loader.md#loader), [`is_language_available`](../../../tree_sitter_analyzer/language_loader.md#LanguageLoader.is_language_available), [`get_language_summary`](../../../tree_sitter_analyzer/grammar_coverage/introspector.md#get_language_summary), [`LANGUAGE_MODULE_MAP`](../../../tree_sitter_analyzer/grammar_coverage/introspector.md#LANGUAGE_MODULE_MAP)  (1 test-only)

### `TestGetStructuralTypes`
- def: [`tests/unit/grammar_coverage/test_introspector.py:202`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_introspector.py#L202)
- doc: 测试识别结构性节点类型。
- signature: `class TestGetStructuralTypes:`
- members:
  - `test_python_structural_detection(self)` — [`L205`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_introspector.py#L205) — 测试 Python 语言的结构性节点检测。
  - `test_structural_and_extractable_are_complementary(self)` — [`L232`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_introspector.py#L232) — 测试结构性节点和可提取节点是否互补（覆盖所有节点）。
- uses (calls/refs, reference-scoped): [`get_all_node_types`](../../../tree_sitter_analyzer/grammar_coverage/introspector.md#get_all_node_types), [`auto_detect_extractable_types`](../../../tree_sitter_analyzer/grammar_coverage/introspector.md#auto_detect_extractable_types), [`get_structural_types`](../../../tree_sitter_analyzer/grammar_coverage/introspector.md#get_structural_types)

## Module values
- `EXPECTED_GRAMMAR_COUNTS` — [`L17`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_introspector.py#L17)

