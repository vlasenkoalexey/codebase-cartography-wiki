---
title: 'Module: tests/unit/core/test_language_detector_extended.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_language_detector_extended.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_language_detector_extended`/
symbols:
  test_global_detector_instance: test_global_detector_instance().
  language_detector: language_detector().
  test_detect_language_from_file: test_detect_language_from_file().
  test_is_language_supported_global: test_is_language_supported_global().
  test_detect_language_from_file_with_project_root: test_detect_language_from_file_with_project_root().
  test_detect_language_from_file_empty: test_detect_language_from_file_empty().
  test_detect_language_from_file_none: test_detect_language_from_file_none().
  test_is_language_supported_with_plugin_manager_failure: test_is_language_supported_with_plugin_manager_failure().
  test_detect_language_with_content_java: test_detect_language_with_content_java().
  test_detect_language_with_content_python: test_detect_language_with_content_python().
  test_detect_language_with_content_javascript: test_detect_language_with_content_javascript().
  test_detect_language_with_content_typescript: test_detect_language_with_content_typescript().
  test_detect_language_ambiguous_h_file_cpp: test_detect_language_ambiguous_h_file_cpp().
  test_detect_language_ambiguous_h_file_c: test_detect_language_ambiguous_h_file_c().
  test_detect_language_ambiguous_h_file_objc: test_detect_language_ambiguous_h_file_objc().
  test_detect_language_ambiguous_m_file_objc: test_detect_language_ambiguous_m_file_objc().
  test_detect_language_ambiguous_m_file_matlab: test_detect_language_ambiguous_m_file_matlab().
  test_detect_language_ambiguous_without_content: test_detect_language_ambiguous_without_content().
  test_detect_language_unknown_extension: test_detect_language_unknown_extension().
  test_detect_from_extension_various_files: test_detect_from_extension_various_files().
  test_is_supported_supported_languages: test_is_supported_supported_languages().
  test_is_supported_unsupported_languages: test_is_supported_unsupported_languages().
  test_get_supported_extensions: test_get_supported_extensions().
  test_get_supported_languages: test_get_supported_languages().
  test_add_extension_mapping: test_add_extension_mapping().
  test_get_language_info_supported: test_get_language_info_supported().
  test_get_language_info_swift_supported: test_get_language_info_swift_supported().
  test_resolve_ambiguity_non_ambiguous: test_resolve_ambiguity_non_ambiguous().
  test_resolve_ambiguity_unknown_extension: test_resolve_ambiguity_unknown_extension().
  test_detect_c_family_with_no_matches: test_detect_c_family_with_no_matches().
  test_detect_objc_vs_matlab_tie: test_detect_objc_vs_matlab_tie().
  test_detect_c_family_objc_not_in_candidates: test_detect_c_family_objc_not_in_candidates().
  test_empty_file_path: test_empty_file_path().
  test_file_path_without_extension: test_file_path_without_extension().
  test_file_path_with_multiple_dots: test_file_path_with_multiple_dots().
  test_case_insensitive_extensions: test_case_insensitive_extensions().
  test_empty_content_for_ambiguous_extension: test_empty_content_for_ambiguous_extension().
  test_none_content_for_ambiguous_extension: test_none_content_for_ambiguous_extension().
  test_resolve_ambiguity_h_with_cpp_content: test_resolve_ambiguity_h_with_cpp_content().
  test_resolve_ambiguity_h_with_c_content: test_resolve_ambiguity_h_with_c_content().
  test_resolve_ambiguity_h_with_objc_content: test_resolve_ambiguity_h_with_objc_content().
  test_resolve_ambiguity_m_with_objc_content: test_resolve_ambiguity_m_with_objc_content().
  test_resolve_ambiguity_m_with_matlab_content: test_resolve_ambiguity_m_with_matlab_content().
  test_resolve_ambiguity_sql_fallback: test_resolve_ambiguity_sql_fallback().
  test_resolve_ambiguity_json_fallback: test_resolve_ambiguity_json_fallback().
  test_detect_c_family_cpp_wins: test_detect_c_family_cpp_wins().
  test_detect_c_family_c_wins: test_detect_c_family_c_wins().
  test_detect_c_family_objc_wins: test_detect_c_family_objc_wins().
  test_detect_objc_vs_matlab_objc_wins: test_detect_objc_vs_matlab_objc_wins().
  test_detect_objc_vs_matlab_matlab_wins: test_detect_objc_vs_matlab_matlab_wins().
  test_detect_from_extension_none_input: test_detect_from_extension_none_input().
  test_detect_from_extension_non_string_input: test_detect_from_extension_non_string_input().
  test_detect_language_with_content_ambiguity_path: test_detect_language_with_content_ambiguity_path().
  test_detect_language_with_content_ambiguity_without_content: test_detect_language_with_content_ambiguity_without_content().
  test_detect_language_empty_string_path: test_detect_language_empty_string_path().
  test_detect_language_non_string_input: test_detect_language_non_string_input().
  test_is_supported_with_plugin_manager_failure: test_is_supported_with_plugin_manager_failure().
---
# Module: [`tests/unit/core/test_language_detector_extended.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_extended.py)

## Functions
- `language_detector()` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_extended.py#L24) — Fixture to provide a LanguageDetector instance
- `test_add_extension_mapping(language_detector)` — [`L343`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_extended.py#L343) — Test adding custom extension mapping
- `test_case_insensitive_extensions(language_detector, file_path, expected_language)` — [`L480`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_extended.py#L480) — Test case insensitive extension handling
- `test_detect_c_family_c_wins(language_detector)` — [`L562`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_extended.py#L562) — _detect_c_family with strong C patterns
- `test_detect_c_family_cpp_wins(language_detector)` — [`L555`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_extended.py#L555) — _detect_c_family with strong C++ patterns
- `test_detect_c_family_objc_not_in_candidates(language_detector)` — [`L410`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_extended.py#L410) — Test C family detection when objc wins but not in candidates
- `test_detect_c_family_objc_wins(language_detector)` — [`L569`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_extended.py#L569) — _detect_c_family with ObjC patterns winning
- `test_detect_c_family_with_no_matches(language_detector)` — [`L392`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_extended.py#L392) — Test C family detection with no pattern matches
- `test_detect_from_extension_non_string_input(language_detector)` — [`L595`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_extended.py#L595) — detect_from_extension with non-string returns unknown
- `test_detect_from_extension_none_input(language_detector)` — [`L590`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_extended.py#L590) — detect_from_extension with None returns unknown
- `test_detect_from_extension_various_files(language_detector, file_path, expected_language)` — [`L272`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_extended.py#L272) — Test extension-based detection for various files
- `test_detect_language_ambiguous_h_file_c(language_detector)` — [`L138`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_extended.py#L138) — Test ambiguous .h file detection as C
- `test_detect_language_ambiguous_h_file_cpp(language_detector)` — [`L110`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_extended.py#L110) — Test ambiguous .h file detection as C++
- `test_detect_language_ambiguous_h_file_objc(language_detector)` — [`L163`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_extended.py#L163) — Test ambiguous .h file detection as Objective-C
- `test_detect_language_ambiguous_m_file_matlab(language_detector)` — [`L208`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_extended.py#L208) — Test ambiguous .m file detection as MATLAB
- `test_detect_language_ambiguous_m_file_objc(language_detector)` — [`L189`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_extended.py#L189) — Test ambiguous .m file detection as Objective-C
- `test_detect_language_ambiguous_without_content(language_detector)` — [`L234`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_extended.py#L234) — Test ambiguous extension without content
- `test_detect_language_empty_string_path(language_detector)` — [`L618`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_extended.py#L618) — detect_language with empty string
- `test_detect_language_from_file()` — [`L420`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_extended.py#L420) — Test global detect_language_from_file function
- `test_detect_language_from_file_empty()` — [`L646`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_extended.py#L646) — detect_language_from_file with empty string
- `test_detect_language_from_file_none()` — [`L651`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_extended.py#L651) — detect_language_from_file with None
- `test_detect_language_from_file_with_project_root()` — [`L632`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_extended.py#L632) — detect_language_from_file with relative path and project_root
- `test_detect_language_non_string_input(language_detector)` — [`L625`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_extended.py#L625) — detect_language with non-string input
- `test_detect_language_unknown_extension(language_detector)` — [`L244`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_extended.py#L244) — Test unknown file extension
- `test_detect_language_with_content_ambiguity_path(language_detector)` — [`L600`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_extended.py#L600) — Force ambiguity resolution by removing .sql from extension_map
- `test_detect_language_with_content_ambiguity_without_content(language_detector)` — [`L610`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_extended.py#L610) — Force ambiguity path without content returns 0.7 confidence
- `test_detect_language_with_content_java(language_detector)` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_extended.py#L29) — Test language detection with Java content
- `test_detect_language_with_content_javascript(language_detector)` — [`L67`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_extended.py#L67) — Test language detection with JavaScript content
- `test_detect_language_with_content_python(language_detector)` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_extended.py#L49) — Test language detection with Python content
- `test_detect_language_with_content_typescript(language_detector)` — [`L86`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_extended.py#L86) — Test language detection with TypeScript content
- `test_detect_objc_vs_matlab_matlab_wins(language_detector)` — [`L583`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_extended.py#L583) — _detect_objc_vs_matlab with clear MATLAB content
- `test_detect_objc_vs_matlab_objc_wins(language_detector)` — [`L576`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_extended.py#L576) — _detect_objc_vs_matlab with clear ObjC content
- `test_detect_objc_vs_matlab_tie(language_detector)` — [`L401`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_extended.py#L401) — Test Objective-C vs MATLAB detection with tie
- `test_empty_content_for_ambiguous_extension(language_detector)` — [`L486`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_extended.py#L486) — Test empty content for ambiguous extension
- `test_empty_file_path(language_detector)` — [`L450`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_extended.py#L450) — Test empty file path
- `test_file_path_with_multiple_dots(language_detector)` — [`L464`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_extended.py#L464) — Test file path with multiple dots
- `test_file_path_without_extension(language_detector)` — [`L457`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_extended.py#L457) — Test file path without extension
- `test_get_language_info_supported(language_detector)` — [`L358`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_extended.py#L358) — Test getting language information for supported language
- `test_get_language_info_swift_supported(language_detector)` — [`L370`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_extended.py#L370) — Test getting language information for Swift.
- `test_get_supported_extensions(language_detector)` — [`L312`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_extended.py#L312) — Test getting supported extensions
- `test_get_supported_languages(language_detector)` — [`L326`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_extended.py#L326) — Test getting supported languages
- `test_global_detector_instance()` — [`L440`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_extended.py#L440) — Test global detector instance
- `test_is_language_supported_global()` — [`L432`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_extended.py#L432) — Test global is_language_supported function
- `test_is_language_supported_with_plugin_manager_failure()` — [`L667`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_extended.py#L667) — is_language_supported falls back when PluginManager raises
- `test_is_supported_supported_languages(language_detector, language)` — [`L296`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_extended.py#L296) — Test support status for supported languages
- `test_is_supported_unsupported_languages(language_detector, language)` — [`L302`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_extended.py#L302) — Test support status for unsupported languages.
- `test_is_supported_with_plugin_manager_failure(language_detector)` — [`L656`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_extended.py#L656) — is_supported falls back when PluginManager raises
- `test_none_content_for_ambiguous_extension(language_detector)` — [`L493`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_extended.py#L493) — Test None content for ambiguous extension
- `test_resolve_ambiguity_h_with_c_content(language_detector)` — [`L511`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_extended.py#L511) — _resolve_ambiguity for .h with C content returns c
- `test_resolve_ambiguity_h_with_cpp_content(language_detector)` — [`L503`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_extended.py#L503) — _resolve_ambiguity for .h with C++ content returns cpp
- `test_resolve_ambiguity_h_with_objc_content(language_detector)` — [`L519`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_extended.py#L519) — _resolve_ambiguity for .h with ObjC content returns objc
- `test_resolve_ambiguity_json_fallback(language_detector)` — [`L549`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_extended.py#L549) — _resolve_ambiguity for .json returns first candidate
- `test_resolve_ambiguity_m_with_matlab_content(language_detector)` — [`L535`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_extended.py#L535) — _resolve_ambiguity for .m with MATLAB content
- `test_resolve_ambiguity_m_with_objc_content(language_detector)` — [`L527`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_extended.py#L527) — _resolve_ambiguity for .m with ObjC content
- `test_resolve_ambiguity_non_ambiguous(language_detector)` — [`L380`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_extended.py#L380) — Test resolve ambiguity for non-ambiguous extension
- `test_resolve_ambiguity_sql_fallback(language_detector)` — [`L543`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_extended.py#L543) — _resolve_ambiguity for .sql returns first candidate
- `test_resolve_ambiguity_unknown_extension(language_detector)` — [`L386`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_extended.py#L386) — Test resolve ambiguity for unknown extension

