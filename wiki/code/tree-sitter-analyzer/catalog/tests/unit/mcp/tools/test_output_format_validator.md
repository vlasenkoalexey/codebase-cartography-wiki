---
title: 'Module: tests/unit/mcp/tools/test_output_format_validator.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/tools/test_output_format_validator.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.tools.test_output_format_validator`/Test
symbols:
  TestOutputFormatValidatorDetectLanguage.test_detect_language_japanese_locale: OutputFormatValidatorDetectLanguage#test_detect_language_japanese_locale().
  TestOutputFormatValidatorDetectLanguage.test_detect_language_english_fallback: OutputFormatValidatorDetectLanguage#test_detect_language_english_fallback().
  TestOutputFormatValidatorDetectLanguage.test_detect_language_locale_exception: OutputFormatValidatorDetectLanguage#test_detect_language_locale_exception().
  TestOutputFormatValidatorDetectLanguage.test_detect_language_non_japanese_locale: OutputFormatValidatorDetectLanguage#test_detect_language_non_japanese_locale().
  TestOutputFormatValidatorJapaneseError.test_japanese_error_message: OutputFormatValidatorJapaneseError#test_japanese_error_message().
  TestOutputFormatValidatorJapaneseError.test_japanese_error_includes_efficiency_guide: OutputFormatValidatorJapaneseError#test_japanese_error_includes_efficiency_guide().
  TestOutputFormatValidatorEnglishError.test_english_error_message: OutputFormatValidatorEnglishError#test_english_error_message().
  TestOutputFormatValidatorEnglishError.test_english_error_includes_usage_patterns: OutputFormatValidatorEnglishError#test_english_error_includes_usage_patterns().
  TestOutputFormatValidatorExclusion.test_single_format_no_error: OutputFormatValidatorExclusion#test_single_format_no_error().
  TestOutputFormatValidatorExclusion.test_no_format_no_error: OutputFormatValidatorExclusion#test_no_format_no_error().
  TestOutputFormatValidatorExclusion.test_multiple_formats_raises_error: OutputFormatValidatorExclusion#test_multiple_formats_raises_error().
  TestOutputFormatValidatorExclusion.test_all_formats_raises_error: OutputFormatValidatorExclusion#test_all_formats_raises_error().
  TestOutputFormatValidatorActiveFormat.test_get_active_total_only: OutputFormatValidatorActiveFormat#test_get_active_total_only().
  TestOutputFormatValidatorActiveFormat.test_get_active_count_only_matches: OutputFormatValidatorActiveFormat#test_get_active_count_only_matches().
  TestOutputFormatValidatorActiveFormat.test_get_active_summary_only: OutputFormatValidatorActiveFormat#test_get_active_summary_only().
  TestOutputFormatValidatorActiveFormat.test_get_active_group_by_file: OutputFormatValidatorActiveFormat#test_get_active_group_by_file().
  TestOutputFormatValidatorActiveFormat.test_get_active_suppress_output: OutputFormatValidatorActiveFormat#test_get_active_suppress_output().
  TestOutputFormatValidatorActiveFormat.test_get_active_normal_default: OutputFormatValidatorActiveFormat#test_get_active_normal_default().
  TestOutputFormatValidatorActiveFormat.test_get_active_first_match: OutputFormatValidatorActiveFormat#test_get_active_first_match().
  TestGetDefaultValidator.test_returns_validator_instance: GetDefaultValidator#test_returns_validator_instance().
  TestGetDefaultValidator.test_singleton_behavior: GetDefaultValidator#test_singleton_behavior().
  TestOutputFormatValidatorDetectLanguage: OutputFormatValidatorDetectLanguage#
  TestOutputFormatValidatorJapaneseError: OutputFormatValidatorJapaneseError#
  TestOutputFormatValidatorEnglishError: OutputFormatValidatorEnglishError#
  TestOutputFormatValidatorExclusion: OutputFormatValidatorExclusion#
  TestOutputFormatValidatorActiveFormat: OutputFormatValidatorActiveFormat#
  TestGetDefaultValidator: GetDefaultValidator#
---
# Module: [`tests/unit/mcp/tools/test_output_format_validator.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_output_format_validator.py)

## Classes
### `TestGetDefaultValidator`
- def: [`tests/unit/mcp/tools/test_output_format_validator.py:187`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_output_format_validator.py#L187)
- doc: Tests for get_default_validator singleton
- signature: `class TestGetDefaultValidator:`
- members:
  - `test_returns_validator_instance(self)` — [`L190`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_output_format_validator.py#L190)
  - `test_singleton_behavior(self)` — [`L194`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_output_format_validator.py#L194)
- uses (calls/refs, reference-scoped): [`OutputFormatValidator`](../../../../tree_sitter_analyzer/mcp/tools/output_format_validator.md#OutputFormatValidator), [`get_default_validator`](../../../../tree_sitter_analyzer/mcp/tools/output_format_validator.md#get_default_validator)

### `TestOutputFormatValidatorActiveFormat`
- def: [`tests/unit/mcp/tools/test_output_format_validator.py:146`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_output_format_validator.py#L146)
- doc: Tests for get_active_format
- signature: `class TestOutputFormatValidatorActiveFormat:`
- members:
  - `test_get_active_count_only_matches(self)` — [`L153`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_output_format_validator.py#L153)
  - `test_get_active_first_match(self)` — [`L178`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_output_format_validator.py#L178) — Returns first matching format, not all
  - `test_get_active_group_by_file(self)` — [`L164`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_output_format_validator.py#L164)
  - `test_get_active_normal_default(self)` — [`L174`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_output_format_validator.py#L174)
  - `test_get_active_summary_only(self)` — [`L160`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_output_format_validator.py#L160)
  - `test_get_active_suppress_output(self)` — [`L168`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_output_format_validator.py#L168)
  - `test_get_active_total_only(self)` — [`L149`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_output_format_validator.py#L149)
- uses (calls/refs, reference-scoped): [`OutputFormatValidator`](../../../../tree_sitter_analyzer/mcp/tools/output_format_validator.md#OutputFormatValidator), [`get_active_format`](../../../../tree_sitter_analyzer/mcp/tools/output_format_validator.md#OutputFormatValidator.get_active_format)

### `TestOutputFormatValidatorDetectLanguage`
- def: [`tests/unit/mcp/tools/test_output_format_validator.py:21`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_output_format_validator.py#L21)
- doc: Tests for _detect_language method
- signature: `class TestOutputFormatValidatorDetectLanguage:`
- members:
  - `test_detect_language_english_fallback(self)` — [`L38`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_output_format_validator.py#L38) — Detect English as default when no Japanese indicators (line 51)
  - `test_detect_language_japanese_locale(self)` — [`L24`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_output_format_validator.py#L24) — ``_detect_language`` is intentionally hard-coded to ``"en"``
  - `test_detect_language_locale_exception(self)` — [`L46`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_output_format_validator.py#L46) — Handle locale exception gracefully (line 47-48)
  - `test_detect_language_non_japanese_locale(self)` — [`L56`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_output_format_validator.py#L56) — Detect English for non-Japanese locale
- uses (calls/refs, reference-scoped): [`OutputFormatValidator`](../../../../tree_sitter_analyzer/mcp/tools/output_format_validator.md#OutputFormatValidator), [`_detect_language`](../../../../tree_sitter_analyzer/mcp/tools/output_format_validator.md#OutputFormatValidator._detect_language)

### `TestOutputFormatValidatorEnglishError`
- def: [`tests/unit/mcp/tools/test_output_format_validator.py:90`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_output_format_validator.py#L90)
- doc: Tests for English error messages
- signature: `class TestOutputFormatValidatorEnglishError:`
- members:
  - `test_english_error_includes_usage_patterns(self)` — [`L102`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_output_format_validator.py#L102) — English error includes recommended usage patterns
  - `test_english_error_message(self)` — [`L93`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_output_format_validator.py#L93) — Generate English error message
- uses (calls/refs, reference-scoped): [`OutputFormatValidator`](../../../../tree_sitter_analyzer/mcp/tools/output_format_validator.md#OutputFormatValidator), [`_get_error_message`](../../../../tree_sitter_analyzer/mcp/tools/output_format_validator.md#OutputFormatValidator._get_error_message)

### `TestOutputFormatValidatorExclusion`
- def: [`tests/unit/mcp/tools/test_output_format_validator.py:110`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_output_format_validator.py#L110)
- doc: Tests for validate_output_format_exclusion
- signature: `class TestOutputFormatValidatorExclusion:`
- members:
  - `test_all_formats_raises_error(self)` — [`L131`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_output_format_validator.py#L131) — All format parameters together raises ValueError
  - `test_multiple_formats_raises_error(self)` — [`L123`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_output_format_validator.py#L123) — Multiple format parameters raises ValueError
  - `test_no_format_no_error(self)` — [`L118`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_output_format_validator.py#L118) — No format parameter raises no error
  - `test_single_format_no_error(self)` — [`L113`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_output_format_validator.py#L113) — Single format parameter raises no error
- uses (calls/refs, reference-scoped): [`OutputFormatValidator`](../../../../tree_sitter_analyzer/mcp/tools/output_format_validator.md#OutputFormatValidator), [`validate_output_format_exclusion`](../../../../tree_sitter_analyzer/mcp/tools/output_format_validator.md#OutputFormatValidator.validate_output_format_exclusion)

### `TestOutputFormatValidatorJapaneseError`
- def: [`tests/unit/mcp/tools/test_output_format_validator.py:67`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_output_format_validator.py#L67)
- doc: Tests for Japanese error messages (lines 81, 87-88, 90)
- signature: `class TestOutputFormatValidatorJapaneseError:`
- members:
  - `test_japanese_error_includes_efficiency_guide(self)` — [`L80`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_output_format_validator.py#L80) — Japanese error includes token efficiency guide
  - `test_japanese_error_message(self)` — [`L70`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_output_format_validator.py#L70) — Generate Japanese error message when language is ja
- uses (calls/refs, reference-scoped): [`OutputFormatValidator`](../../../../tree_sitter_analyzer/mcp/tools/output_format_validator.md#OutputFormatValidator), [`_get_error_message`](../../../../tree_sitter_analyzer/mcp/tools/output_format_validator.md#OutputFormatValidator._get_error_message)

