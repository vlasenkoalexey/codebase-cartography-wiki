---
title: 'Module: tests/unit/core/test_language_detector.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_language_detector.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_language_detector`/test_
symbols:
  test_add_extension_mapping: add_extension_mapping().
  test_detector_methods: detector_methods().
  test_detect_from_extension_java: detect_from_extension_java().
  test_detect_from_extension_javascript: detect_from_extension_javascript().
  test_detect_from_extension_python: detect_from_extension_python().
  test_detect_from_extension_typescript: detect_from_extension_typescript().
  test_detect_from_extension_unknown: detect_from_extension_unknown().
  test_detect_language_with_content: detect_language_with_content().
  test_detector_content_heuristics: detector_content_heuristics().
  test_ambiguous_extensions: ambiguous_extensions().
  test_detect_language_non_string_path: detect_language_non_string_path().
  test_detect_from_extension_empty_and_none: detect_from_extension_empty_and_none().
  test_detect_language_h_extension_map_overrides_ambiguity: detect_language_h_extension_map_overrides_ambiguity().
  test_resolve_ambiguity_h_no_match: resolve_ambiguity_h_no_match().
  test_detect_language_m_extension_map_returns_objc: detect_language_m_extension_map_returns_objc().
  test_resolve_ambiguity_m_objc_content: resolve_ambiguity_m_objc_content().
  test_resolve_ambiguity_m_matlab_content: resolve_ambiguity_m_matlab_content().
  test_resolve_ambiguity_m_tie_falls_to_first_candidate: resolve_ambiguity_m_tie_falls_to_first_candidate().
  test_detect_language_sql_ambiguous_with_content: detect_language_sql_ambiguous_with_content().
  test_detect_language_sql_without_content: detect_language_sql_without_content().
  test_resolve_ambiguity_non_ambiguous_extension: resolve_ambiguity_non_ambiguous_extension().
  test_detect_language_unknown_extension_returns_unknown: detect_language_unknown_extension_returns_unknown().
  test_is_supported_unknown_language: is_supported_unknown_language().
  test_get_language_info: get_language_info().
  test_get_language_info_unknown: get_language_info_unknown().
  test_detect_c_family_no_match: detect_c_family_no_match().
  test_detect_from_file_with_temp_files: detect_from_file_with_temp_files().
  test_is_language_supported: is_language_supported().
  test_detect_language_from_file_nonexistent: detect_language_from_file_nonexistent().
  test_detect_language_from_file_relative_with_project_root: detect_language_from_file_relative_with_project_root().
---
# Module: [`tests/unit/core/test_language_detector.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector.py)

## Functions
- `test_add_extension_mapping()` — [`L245`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector.py#L245)
- `test_ambiguous_extensions()` — [`L143`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector.py#L143) — Test handling of ambiguous file extensions
- `test_detect_c_family_no_match()` — [`L268`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector.py#L268)
- `test_detect_from_extension_empty_and_none()` — [`L159`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector.py#L159)
- `test_detect_from_extension_java()` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector.py#L21) — Test Java file detection
- `test_detect_from_extension_javascript()` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector.py#L27) — Test JavaScript file detection
- `test_detect_from_extension_python()` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector.py#L33) — Test Python file detection
- `test_detect_from_extension_typescript()` — [`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector.py#L39) — Test TypeScript file detection
- `test_detect_from_extension_unknown()` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector.py#L45) — Test unknown extension handling
- `test_detect_from_file_with_temp_files()` — [`L74`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector.py#L74) — Test file detection with temporary files
- `test_detect_language_from_file_nonexistent()` — [`L220`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector.py#L220)
- `test_detect_language_from_file_relative_with_project_root()` — [`L225`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector.py#L225)
- `test_detect_language_h_extension_map_overrides_ambiguity()` — [`L165`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector.py#L165)
- `test_detect_language_m_extension_map_returns_objc()` — [`L177`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector.py#L177)
- `test_detect_language_non_string_path()` — [`L154`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector.py#L154)
- `test_detect_language_sql_ambiguous_with_content()` — [`L200`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector.py#L200)
- `test_detect_language_sql_without_content()` — [`L205`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector.py#L205)
- `test_detect_language_unknown_extension_returns_unknown()` — [`L216`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector.py#L216)
- `test_detect_language_with_content()` — [`L51`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector.py#L51) — Test language detection using content analysis
- `test_detector_content_heuristics()` — [`L119`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector.py#L119) — Test content-based heuristics with detect_language method
- `test_detector_methods()` — [`L106`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector.py#L106) — Test detector instance methods
- `test_get_language_info()` — [`L253`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector.py#L253)
- `test_get_language_info_unknown()` — [`L261`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector.py#L261)
- `test_is_language_supported()` — [`L97`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector.py#L97) — Test language support checking
- `test_is_supported_unknown_language()` — [`L240`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector.py#L240)
- `test_resolve_ambiguity_h_no_match()` — [`L172`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector.py#L172)
- `test_resolve_ambiguity_m_matlab_content()` — [`L189`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector.py#L189)
- `test_resolve_ambiguity_m_objc_content()` — [`L183`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector.py#L183)
- `test_resolve_ambiguity_m_tie_falls_to_first_candidate()` — [`L195`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector.py#L195)
- `test_resolve_ambiguity_non_ambiguous_extension()` — [`L211`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector.py#L211)

