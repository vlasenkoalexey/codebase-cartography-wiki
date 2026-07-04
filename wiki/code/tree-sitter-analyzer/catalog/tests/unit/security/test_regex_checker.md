---
title: 'Module: tests/unit/security/test_regex_checker.py'
type: catalog
provenance: extracted
module: tests/unit/security/test_regex_checker.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.security.test_regex_checker`/Test
symbols:
  TestIntegration.test_complete_validation_workflow: Integration#test_complete_validation_workflow().
  TestValidatePattern.test_validate_pattern_too_long: ValidatePattern#test_validate_pattern_too_long().
  TestValidatePattern.test_validate_pattern_at_max_length: ValidatePattern#test_validate_pattern_at_max_length().
  TestCheckDangerousPatterns.test_check_dangerous_patterns_nested_plus: CheckDangerousPatterns#test_check_dangerous_patterns_nested_plus().
  TestCheckDangerousPatterns.test_check_dangerous_patterns_nested_star: CheckDangerousPatterns#test_check_dangerous_patterns_nested_star().
  TestCheckDangerousPatterns.test_check_dangerous_patterns_alternation_overlap: CheckDangerousPatterns#test_check_dangerous_patterns_alternation_overlap().
  TestCheckDangerousPatterns.test_check_dangerous_patterns_lookahead: CheckDangerousPatterns#test_check_dangerous_patterns_lookahead().
  TestCheckDangerousPatterns.test_check_dangerous_patterns_lookbehind: CheckDangerousPatterns#test_check_dangerous_patterns_lookbehind().
  TestCheckDangerousPatterns.test_check_dangerous_patterns_negative_lookahead: CheckDangerousPatterns#test_check_dangerous_patterns_negative_lookahead().
  TestCheckDangerousPatterns.test_check_dangerous_patterns_negative_lookbehind: CheckDangerousPatterns#test_check_dangerous_patterns_negative_lookbehind().
  TestMissingCoverage.test_check_performance_slow_execution: MissingCoverage#test_check_performance_slow_execution().
  TestMissingCoverage.test_create_safe_pattern_compilation_failure_after_validation: MissingCoverage#test_create_safe_pattern_compilation_failure_after_validation().
  TestIntegration.test_dangerous_pattern_detection_workflow: Integration#test_dangerous_pattern_detection_workflow().
  TestRegexSafetyCheckerInitialization.test_max_pattern_length_constant: RegexSafetyCheckerInitialization#test_max_pattern_length_constant().
  TestRegexSafetyCheckerInitialization.test_max_execution_time_constant: RegexSafetyCheckerInitialization#test_max_execution_time_constant().
  TestRegexSafetyCheckerInitialization.test_dangerous_patterns_list: RegexSafetyCheckerInitialization#test_dangerous_patterns_list().
  TestValidatePattern.test_validate_pattern_safe: ValidatePattern#test_validate_pattern_safe().
  TestValidatePattern.test_validate_pattern_simple: ValidatePattern#test_validate_pattern_simple().
  TestValidatePattern.test_validate_pattern_empty_string: ValidatePattern#test_validate_pattern_empty_string().
  TestValidatePattern.test_validate_pattern_none: ValidatePattern#test_validate_pattern_none().
  TestValidatePattern.test_validate_pattern_non_string: ValidatePattern#test_validate_pattern_non_string().
  TestValidatePattern.test_validate_pattern_invalid_regex: ValidatePattern#test_validate_pattern_invalid_regex().
  TestValidatePattern.test_validate_pattern_dangerous_nested_quantifiers: ValidatePattern#test_validate_pattern_dangerous_nested_quantifiers().
  TestValidatePattern.test_validate_pattern_dangerous_alternation_overlap: ValidatePattern#test_validate_pattern_dangerous_alternation_overlap().
  TestValidatePattern.test_validate_pattern_dangerous_backreference: ValidatePattern#test_validate_pattern_dangerous_backreference().
  TestValidatePattern.test_validate_pattern_dangerous_lookahead: ValidatePattern#test_validate_pattern_dangerous_lookahead().
  TestValidatePattern.test_validate_pattern_dangerous_lookbehind: ValidatePattern#test_validate_pattern_dangerous_lookbehind().
  TestValidatePattern.test_validate_pattern_with_escaped_chars: ValidatePattern#test_validate_pattern_with_escaped_chars().
  TestValidatePattern.test_validate_pattern_with_character_class: ValidatePattern#test_validate_pattern_with_character_class().
  TestValidatePattern.test_validate_pattern_with_anchors: ValidatePattern#test_validate_pattern_with_anchors().
  TestValidatePattern.test_validate_pattern_with_groups: ValidatePattern#test_validate_pattern_with_groups().
  TestValidatePattern.test_validate_pattern_exception_handling: ValidatePattern#test_validate_pattern_exception_handling().
  TestCheckDangerousPatterns.test_check_dangerous_patterns_safe: CheckDangerousPatterns#test_check_dangerous_patterns_safe().
  TestCheckDangerousPatterns.test_check_dangerous_patterns_backreference: CheckDangerousPatterns#test_check_dangerous_patterns_backreference().
  TestCheckDangerousPatterns.test_check_dangerous_patterns_invalid_dangerous_pattern: CheckDangerousPatterns#test_check_dangerous_patterns_invalid_dangerous_pattern().
  TestCheckCompilation.test_check_compilation_valid: CheckCompilation#test_check_compilation_valid().
  TestCheckCompilation.test_check_compilation_invalid: CheckCompilation#test_check_compilation_invalid().
  TestCheckCompilation.test_check_compilation_unclosed_bracket: CheckCompilation#test_check_compilation_unclosed_bracket().
  TestCheckCompilation.test_check_compilation_unclosed_paren: CheckCompilation#test_check_compilation_unclosed_paren().
  TestCheckCompilation.test_check_compilation_invalid_quantifier: CheckCompilation#test_check_compilation_invalid_quantifier().
  TestCheckPerformance.test_check_performance_safe_pattern: CheckPerformance#test_check_performance_safe_pattern().
  TestCheckPerformance.test_check_performance_simple_pattern: CheckPerformance#test_check_performance_simple_pattern().
  TestCheckPerformance.test_check_performance_with_long_string: CheckPerformance#test_check_performance_with_long_string().
  TestCheckPerformance.test_check_performance_exception_handling: CheckPerformance#test_check_performance_exception_handling().
  TestCheckPerformance.test_check_performance_execution_error: CheckPerformance#test_check_performance_execution_error().
  TestAnalyzeComplexity.test_analyze_complexity_simple: AnalyzeComplexity#test_analyze_complexity_simple().
  TestAnalyzeComplexity.test_analyze_complexity_with_quantifiers: AnalyzeComplexity#test_analyze_complexity_with_quantifiers().
  TestAnalyzeComplexity.test_analyze_complexity_with_groups: AnalyzeComplexity#test_analyze_complexity_with_groups().
  TestAnalyzeComplexity.test_analyze_complexity_with_alternations: AnalyzeComplexity#test_analyze_complexity_with_alternations().
  TestAnalyzeComplexity.test_analyze_complexity_with_character_classes: AnalyzeComplexity#test_analyze_complexity_with_character_classes().
  TestAnalyzeComplexity.test_analyze_complexity_with_anchors: AnalyzeComplexity#test_analyze_complexity_with_anchors().
  TestAnalyzeComplexity.test_analyze_complexity_score_calculation: AnalyzeComplexity#test_analyze_complexity_score_calculation().
  TestAnalyzeComplexity.test_analyze_complexity_exception_handling: AnalyzeComplexity#test_analyze_complexity_exception_handling().
  TestSuggestSaferPattern.test_suggest_safer_pattern_safe_pattern: SuggestSaferPattern#test_suggest_safer_pattern_safe_pattern().
  TestSuggestSaferPattern.test_suggest_safer_pattern_nested_plus: SuggestSaferPattern#test_suggest_safer_pattern_nested_plus().
  TestSuggestSaferPattern.test_suggest_safer_pattern_nested_star: SuggestSaferPattern#test_suggest_safer_pattern_nested_star().
  TestSuggestSaferPattern.test_suggest_safer_pattern_no_suggestion: SuggestSaferPattern#test_suggest_safer_pattern_no_suggestion().
  TestSuggestSaferPattern.test_suggest_safer_pattern_partial_match: SuggestSaferPattern#test_suggest_safer_pattern_partial_match().
  TestGetSafeFlags.test_get_safe_flags: GetSafeFlags#test_get_safe_flags().
  TestCreateSafePattern.test_create_safe_pattern_valid: CreateSafePattern#test_create_safe_pattern_valid().
  TestCreateSafePattern.test_create_safe_pattern_with_flags: CreateSafePattern#test_create_safe_pattern_with_flags().
  TestCreateSafePattern.test_create_safe_pattern_dangerous: CreateSafePattern#test_create_safe_pattern_dangerous().
  TestCreateSafePattern.test_create_safe_pattern_invalid: CreateSafePattern#test_create_safe_pattern_invalid().
  TestCreateSafePattern.test_create_safe_pattern_compilation_failure: CreateSafePattern#test_create_safe_pattern_compilation_failure().
  TestEdgeCases.test_pattern_with_unicode: EdgeCases#test_pattern_with_unicode().
  TestEdgeCases.test_pattern_with_special_chars: EdgeCases#test_pattern_with_special_chars().
  TestEdgeCases.test_pattern_with_comments: EdgeCases#test_pattern_with_comments().
  TestEdgeCases.test_pattern_with_named_groups: EdgeCases#test_pattern_with_named_groups().
  TestEdgeCases.test_pattern_with_non_capturing_groups: EdgeCases#test_pattern_with_non_capturing_groups().
  TestEdgeCases.test_pattern_with_atomic_groups: EdgeCases#test_pattern_with_atomic_groups().
  TestEdgeCases.test_pattern_with_conditional: EdgeCases#test_pattern_with_conditional().
  TestEdgeCases.test_pattern_with_recursive: EdgeCases#test_pattern_with_recursive().
  TestMissingCoverage.test_validate_pattern_performance_error_path: MissingCoverage#test_validate_pattern_performance_error_path().
  TestMissingCoverage.test_suggest_safer_pattern_dangerous_no_replacement: MissingCoverage#test_suggest_safer_pattern_dangerous_no_replacement().
  TestIntegration.test_complexity_analysis_workflow: Integration#test_complexity_analysis_workflow().
  TestRegexSafetyCheckerInitialization.test_default_initialization: RegexSafetyCheckerInitialization#test_default_initialization().
  TestMissingCoverage.fake_time: MissingCoverage#fake_time().
  TestMissingCoverage.compile_side_effect: MissingCoverage#compile_side_effect().
  TestRegexSafetyCheckerInitialization: RegexSafetyCheckerInitialization#
  TestValidatePattern: ValidatePattern#
  TestCheckDangerousPatterns: CheckDangerousPatterns#
  TestCheckCompilation: CheckCompilation#
  TestCheckPerformance: CheckPerformance#
  TestAnalyzeComplexity: AnalyzeComplexity#
  TestSuggestSaferPattern: SuggestSaferPattern#
  TestGetSafeFlags: GetSafeFlags#
  TestCreateSafePattern: CreateSafePattern#
  TestEdgeCases: EdgeCases#
  TestMissingCoverage: MissingCoverage#
  TestIntegration: Integration#
---
# Module: [`tests/unit/security/test_regex_checker.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py)

## Classes
### `TestAnalyzeComplexity`
- def: [`tests/unit/security/test_regex_checker.py:338`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L338)
- doc: 测试 analyze_complexity 方法
- signature: `class TestAnalyzeComplexity:`
- members:
  - `test_analyze_complexity_exception_handling(self)` — [`L398`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L398) — 测试异常处理
  - `test_analyze_complexity_score_calculation(self)` — [`L383`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L383) — 测试复杂度分数计算
  - `test_analyze_complexity_simple(self)` — [`L341`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L341) — 测试简单模式复杂度分析
  - `test_analyze_complexity_with_alternations(self)` — [`L365`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L365) — 测试带交替的模式复杂度分析
  - `test_analyze_complexity_with_anchors(self)` — [`L377`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L377) — 测试带锚点的模式复杂度分析
  - `test_analyze_complexity_with_character_classes(self)` — [`L371`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L371) — 测试带字符类的模式复杂度分析
  - `test_analyze_complexity_with_groups(self)` — [`L359`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L359) — 测试带分组的模式复杂度分析
  - `test_analyze_complexity_with_quantifiers(self)` — [`L352`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L352) — 测试带量词的模式复杂度分析
- uses (calls/refs, reference-scoped): [`RegexSafetyChecker`](../../../tree_sitter_analyzer/security/regex_checker.md#RegexSafetyChecker), [`analyze_complexity`](../../../tree_sitter_analyzer/security/regex_checker.md#RegexSafetyChecker.analyze_complexity)

### `TestCheckCompilation`
- def: [`tests/unit/security/test_regex_checker.py:258`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L258)
- doc: 测试 _check_compilation 方法
- signature: `class TestCheckCompilation:`
- members:
  - `test_check_compilation_invalid(self)` — [`L267`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L267) — 测试无效模式编译
  - `test_check_compilation_invalid_quantifier(self)` — [`L285`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L285) — 测试无效量词
  - `test_check_compilation_unclosed_bracket(self)` — [`L273`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L273) — 测试未闭合的方括号
  - `test_check_compilation_unclosed_paren(self)` — [`L279`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L279) — 测试未闭合的圆括号
  - `test_check_compilation_valid(self)` — [`L261`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L261) — 测试有效模式编译
- uses (calls/refs, reference-scoped): [`RegexSafetyChecker`](../../../tree_sitter_analyzer/security/regex_checker.md#RegexSafetyChecker), [`_check_compilation`](../../../tree_sitter_analyzer/security/regex_checker.md#RegexSafetyChecker._check_compilation)

### `TestCheckDangerousPatterns`
- def: [`tests/unit/security/test_regex_checker.py:181`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L181)
- doc: 测试 _check_dangerous_patterns 方法
- signature: `class TestCheckDangerousPatterns:`
- members:
  - `test_check_dangerous_patterns_alternation_overlap(self)` — [`L204`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L204) — 检测交替重叠
  - `test_check_dangerous_patterns_backreference(self)` — [`L211`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L211) — 检测反向引用
  - `test_check_dangerous_patterns_invalid_dangerous_pattern(self)` — [`L248`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L248) — 测试无效的危险模式处理
  - `test_check_dangerous_patterns_lookahead(self)` — [`L220`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L220) — 检测前瞻断言
  - `test_check_dangerous_patterns_lookbehind(self)` — [`L227`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L227) — 检测后顾断言
  - `test_check_dangerous_patterns_negative_lookahead(self)` — [`L234`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L234) — 检测负向前瞻
  - `test_check_dangerous_patterns_negative_lookbehind(self)` — [`L241`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L241) — 检测负向后顾
  - `test_check_dangerous_patterns_nested_plus(self)` — [`L190`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L190) — 检测嵌套加号量词
  - `test_check_dangerous_patterns_nested_star(self)` — [`L197`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L197) — 检测嵌套星号量词
  - `test_check_dangerous_patterns_safe(self)` — [`L184`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L184) — 测试安全模式检查
- uses (calls/refs, reference-scoped): [`RegexSafetyChecker`](../../../tree_sitter_analyzer/security/regex_checker.md#RegexSafetyChecker), [`_check_dangerous_patterns`](../../../tree_sitter_analyzer/security/regex_checker.md#RegexSafetyChecker._check_dangerous_patterns), [`DANGEROUS_PATTERNS`](../../../tree_sitter_analyzer/security/regex_checker.md#RegexSafetyChecker.DANGEROUS_PATTERNS)

### `TestCheckPerformance`
- def: [`tests/unit/security/test_regex_checker.py:292`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L292)
- doc: 测试 _check_performance 方法
- signature: `class TestCheckPerformance:`
- members:
  - `test_check_performance_exception_handling(self)` — [`L313`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L313) — 测试异常处理
  - `test_check_performance_execution_error(self)` — [`L322`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L322) — 测试执行错误
  - `test_check_performance_safe_pattern(self)` — [`L295`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L295) — 测试安全模式性能
  - `test_check_performance_simple_pattern(self)` — [`L301`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L301) — 测试简单模式性能
  - `test_check_performance_with_long_string(self)` — [`L307`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L307) — 测试长字符串模式性能
- uses (calls/refs, reference-scoped): [`RegexSafetyChecker`](../../../tree_sitter_analyzer/security/regex_checker.md#RegexSafetyChecker), [`_check_performance`](../../../tree_sitter_analyzer/security/regex_checker.md#RegexSafetyChecker._check_performance)

### `TestCreateSafePattern`
- def: [`tests/unit/security/test_regex_checker.py:454`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L454)
- doc: 测试 create_safe_pattern 方法
- signature: `class TestCreateSafePattern:`
- members:
  - `test_create_safe_pattern_compilation_failure(self)` — [`L484`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L484) — 测试编译失败返回 None
  - `test_create_safe_pattern_dangerous(self)` — [`L472`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L472) — 测试创建危险模式返回 None
  - `test_create_safe_pattern_invalid(self)` — [`L478`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L478) — 测试创建无效模式返回 None
  - `test_create_safe_pattern_valid(self)` — [`L457`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L457) — 测试创建安全模式
  - `test_create_safe_pattern_with_flags(self)` — [`L464`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L464) — 测试带标志创建安全模式
- uses (calls/refs, reference-scoped): [`RegexSafetyChecker`](../../../tree_sitter_analyzer/security/regex_checker.md#RegexSafetyChecker), [`create_safe_pattern`](../../../tree_sitter_analyzer/security/regex_checker.md#RegexSafetyChecker.create_safe_pattern)

### `TestEdgeCases`
- def: [`tests/unit/security/test_regex_checker.py:493`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L493)
- doc: 测试边缘情况
- signature: `class TestEdgeCases:`
- members:
  - `test_pattern_with_atomic_groups(self)` — [`L528`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L528) — 测试原子分组模式
  - `test_pattern_with_comments(self)` — [`L508`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L508) — 测试带注释的模式
  - `test_pattern_with_conditional(self)` — [`L536`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L536) — 测试条件模式
  - `test_pattern_with_named_groups(self)` — [`L514`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L514) — 测试命名分组模式
  - `test_pattern_with_non_capturing_groups(self)` — [`L520`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L520) — 测试非捕获分组模式
  - `test_pattern_with_recursive(self)` — [`L543`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L543) — 测试递归模式
  - `test_pattern_with_special_chars(self)` — [`L502`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L502) — 测试特殊字符模式
  - `test_pattern_with_unicode(self)` — [`L496`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L496) — 测试 Unicode 模式
- uses (calls/refs, reference-scoped): [`RegexSafetyChecker`](../../../tree_sitter_analyzer/security/regex_checker.md#RegexSafetyChecker), [`validate_pattern`](../../../tree_sitter_analyzer/security/regex_checker.md#RegexSafetyChecker.validate_pattern)

### `TestGetSafeFlags`
- def: [`tests/unit/security/test_regex_checker.py:442`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L442)
- doc: 测试 get_safe_flags 方法
- signature: `class TestGetSafeFlags:`
- members:
  - `test_get_safe_flags(self)` — [`L445`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L445) — 测试获取安全标志
- uses (calls/refs, reference-scoped): [`RegexSafetyChecker`](../../../tree_sitter_analyzer/security/regex_checker.md#RegexSafetyChecker), [`get_safe_flags`](../../../tree_sitter_analyzer/security/regex_checker.md#RegexSafetyChecker.get_safe_flags)

### `TestIntegration`
- def: [`tests/unit/security/test_regex_checker.py:612`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L612)
- doc: 测试集成场景
- signature: `class TestIntegration:`
- members:
  - `test_complete_validation_workflow(self)` — [`L615`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L615) — 测试完整验证工作流
  - `test_complexity_analysis_workflow(self)` — [`L652`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L652) — 测试复杂度分析工作流
  - `test_dangerous_pattern_detection_workflow(self)` — [`L635`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L635) — 测试危险模式检测工作流
- uses (calls/refs, reference-scoped): [`RegexSafetyChecker`](../../../tree_sitter_analyzer/security/regex_checker.md#RegexSafetyChecker), [`validate_pattern`](../../../tree_sitter_analyzer/security/regex_checker.md#RegexSafetyChecker.validate_pattern), [`create_safe_pattern`](../../../tree_sitter_analyzer/security/regex_checker.md#RegexSafetyChecker.create_safe_pattern), [`analyze_complexity`](../../../tree_sitter_analyzer/security/regex_checker.md#RegexSafetyChecker.analyze_complexity), [`suggest_safer_pattern`](../../../tree_sitter_analyzer/security/regex_checker.md#RegexSafetyChecker.suggest_safer_pattern)

### `TestMissingCoverage`
- def: [`tests/unit/security/test_regex_checker.py:551`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L551)
- doc: Tests for uncovered lines: 103, 184-187, 262, 295-297
- signature: `class TestMissingCoverage:`
- members:
  - `compile_side_effect(pattern, flags=0)` — [`L599`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L599)
  - `fake_time()` — [`L577`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L577)
  - `test_check_performance_slow_execution(self)` — [`L566`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L566) — Lines 184-187: execution exceeds MAX_EXECUTION_TIME.
  - `test_create_safe_pattern_compilation_failure_after_validation(self)` — [`L593`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L593) — Lines 295-297: re.compile fails after validation passes.
  - `test_suggest_safer_pattern_dangerous_no_replacement(self)` — [`L586`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L586) — Line 262: dangerous pattern that has no replacement rule.
  - `test_validate_pattern_performance_error_path(self)` — [`L554`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L554) — Line 103: performance check returns error in validate_pattern.
- uses (calls/refs, reference-scoped): [`RegexSafetyChecker`](../../../tree_sitter_analyzer/security/regex_checker.md#RegexSafetyChecker), [`validate_pattern`](../../../tree_sitter_analyzer/security/regex_checker.md#RegexSafetyChecker.validate_pattern), [`create_safe_pattern`](../../../tree_sitter_analyzer/security/regex_checker.md#RegexSafetyChecker.create_safe_pattern), [`_check_performance`](../../../tree_sitter_analyzer/security/regex_checker.md#RegexSafetyChecker._check_performance), [`suggest_safer_pattern`](../../../tree_sitter_analyzer/security/regex_checker.md#RegexSafetyChecker.suggest_safer_pattern)

### `TestRegexSafetyCheckerInitialization`
- def: [`tests/unit/security/test_regex_checker.py:16`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L16)
- doc: 测试 RegexSafetyChecker 初始化
- signature: `class TestRegexSafetyCheckerInitialization:`
- members:
  - `test_dangerous_patterns_list(self)` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L35) — 测试危险模式列表
  - `test_default_initialization(self)` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L19) — 测试默认初始化
  - `test_max_execution_time_constant(self)` — [`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L31) — 测试最大执行时间常量
  - `test_max_pattern_length_constant(self)` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L27) — 测试最大模式长度常量
- uses (calls/refs, reference-scoped): [`RegexSafetyChecker`](../../../tree_sitter_analyzer/security/regex_checker.md#RegexSafetyChecker), [`DANGEROUS_PATTERNS`](../../../tree_sitter_analyzer/security/regex_checker.md#RegexSafetyChecker.DANGEROUS_PATTERNS), [`MAX_PATTERN_LENGTH`](../../../tree_sitter_analyzer/security/regex_checker.md#RegexSafetyChecker.MAX_PATTERN_LENGTH), [`MAX_EXECUTION_TIME`](../../../tree_sitter_analyzer/security/regex_checker.md#RegexSafetyChecker.MAX_EXECUTION_TIME)

### `TestSuggestSaferPattern`
- def: [`tests/unit/security/test_regex_checker.py:407`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L407)
- doc: 测试 suggest_safer_pattern 方法
- signature: `class TestSuggestSaferPattern:`
- members:
  - `test_suggest_safer_pattern_nested_plus(self)` — [`L416`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L416) — 测试嵌套加号量词的建议
  - `test_suggest_safer_pattern_nested_star(self)` — [`L422`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L422) — 测试嵌套星号量词的建议
  - `test_suggest_safer_pattern_no_suggestion(self)` — [`L428`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L428) — 测试无建议的情况
  - `test_suggest_safer_pattern_partial_match(self)` — [`L435`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L435) — 测试部分匹配的建议
  - `test_suggest_safer_pattern_safe_pattern(self)` — [`L410`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L410) — 测试安全模式不提供建议
- uses (calls/refs, reference-scoped): [`RegexSafetyChecker`](../../../tree_sitter_analyzer/security/regex_checker.md#RegexSafetyChecker), [`suggest_safer_pattern`](../../../tree_sitter_analyzer/security/regex_checker.md#RegexSafetyChecker.suggest_safer_pattern)

### `TestValidatePattern`
- def: [`tests/unit/security/test_regex_checker.py:42`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L42)
- doc: 测试 validate_pattern 方法
- signature: `class TestValidatePattern:`
- members:
  - `test_validate_pattern_at_max_length(self)` — [`L88`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L88) — 测试最大长度模式
  - `test_validate_pattern_dangerous_alternation_overlap(self)` — [`L110`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L110) — 测试危险交替重叠
  - `test_validate_pattern_dangerous_backreference(self)` — [`L117`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L117) — 测试危险反向引用
  - `test_validate_pattern_dangerous_lookahead(self)` — [`L126`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L126) — 测试危险前瞻断言
  - `test_validate_pattern_dangerous_lookbehind(self)` — [`L133`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L133) — 测试危险后顾断言
  - `test_validate_pattern_dangerous_nested_quantifiers(self)` — [`L103`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L103) — 测试危险嵌套量词
  - `test_validate_pattern_empty_string(self)` — [`L59`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L59) — 测试空字符串模式
  - `test_validate_pattern_exception_handling(self)` — [`L169`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L169) — 测试异常处理
  - `test_validate_pattern_invalid_regex(self)` — [`L96`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L96) — 测试无效的正则表达式
  - `test_validate_pattern_non_string(self)` — [`L73`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L73) — 测试非字符串模式
  - `test_validate_pattern_none(self)` — [`L66`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L66) — 测试 None 模式
  - `test_validate_pattern_safe(self)` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L45) — 测试安全模式验证
  - `test_validate_pattern_simple(self)` — [`L52`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L52) — 测试简单模式验证
  - `test_validate_pattern_too_long(self)` — [`L80`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L80) — 测试过长的模式
  - `test_validate_pattern_with_anchors(self)` — [`L154`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L154) — 测试带锚点的模式
  - `test_validate_pattern_with_character_class(self)` — [`L147`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L147) — 测试带字符类的模式
  - `test_validate_pattern_with_escaped_chars(self)` — [`L140`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L140) — 测试带转义字符的模式
  - `test_validate_pattern_with_groups(self)` — [`L161`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_regex_checker.py#L161) — 测试带分组的模式
- uses (calls/refs, reference-scoped): [`RegexSafetyChecker`](../../../tree_sitter_analyzer/security/regex_checker.md#RegexSafetyChecker), [`validate_pattern`](../../../tree_sitter_analyzer/security/regex_checker.md#RegexSafetyChecker.validate_pattern), [`MAX_PATTERN_LENGTH`](../../../tree_sitter_analyzer/security/regex_checker.md#RegexSafetyChecker.MAX_PATTERN_LENGTH)

