---
title: 'Module: tests/unit/core/test_language_detector_helpers.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_language_detector_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_language_detector_helpers`/Test
symbols:
  TestCachedLanguage.test_store_and_retrieve: CachedLanguage#test_store_and_retrieve().
  TestCachedLanguage.test_get_with_wrong_mtime: CachedLanguage#test_get_with_wrong_mtime().
  TestCachedLanguage.test_store_with_project_root: CachedLanguage#test_store_with_project_root().
  TestBuildExtensionConfidenceMap.test_returns_dict: BuildExtensionConfidenceMap#test_returns_dict().
  TestBuildExtensionConfidenceMap.test_entry_structure: BuildExtensionConfidenceMap#test_entry_structure().
  TestBuildExtensionConfidenceMap.test_common_extensions_present: BuildExtensionConfidenceMap#test_common_extensions_present().
  TestBuildExtensionConfidenceMap.test_high_confidence_for_primary_extensions: BuildExtensionConfidenceMap#test_high_confidence_for_primary_extensions().
  TestBuildExtensionConfidenceMap.test_ambiguous_extensions_have_lower_confidence: BuildExtensionConfidenceMap#test_ambiguous_extensions_have_lower_confidence().
  TestBuildExtensionConfidenceMap.test_markdown_variants: BuildExtensionConfidenceMap#test_markdown_variants().
  TestBuildExtensionConfidenceMap.test_deterministic: BuildExtensionConfidenceMap#test_deterministic().
  TestBuildContentPatternWeights.test_returns_dict: BuildContentPatternWeights#test_returns_dict().
  TestBuildContentPatternWeights.test_entry_structure: BuildContentPatternWeights#test_entry_structure().
  TestBuildContentPatternWeights.test_key_languages_have_patterns: BuildContentPatternWeights#test_key_languages_have_patterns().
  TestBuildContentPatternWeights.test_regex_patterns_compile: BuildContentPatternWeights#test_regex_patterns_compile().
  TestBuildContentPatternWeights.test_java_patterns: BuildContentPatternWeights#test_java_patterns().
  TestBuildContentPatternWeights.test_python_patterns: BuildContentPatternWeights#test_python_patterns().
  TestBuildContentPatternWeights.test_markdown_patterns: BuildContentPatternWeights#test_markdown_patterns().
  TestBuildContentPatternWeights.test_deterministic: BuildContentPatternWeights#test_deterministic().
  TestNormalizeDetectionPath.test_absolute_path_unchanged_no_root: NormalizeDetectionPath#test_absolute_path_unchanged_no_root().
  TestNormalizeDetectionPath.test_relative_path_with_root: NormalizeDetectionPath#test_relative_path_with_root().
  TestNormalizeDetectionPath.test_tilde_expansion: NormalizeDetectionPath#test_tilde_expansion().
  TestNormalizeDetectionPath.test_tilde_with_root: NormalizeDetectionPath#test_tilde_with_root().
  TestNormalizeDetectionPath.test_absolute_path_ignores_root: NormalizeDetectionPath#test_absolute_path_ignores_root().
  TestNormalizeDetectionPath.test_empty_string: NormalizeDetectionPath#test_empty_string().
  TestNormalizeDetectionPath.test_dot_path: NormalizeDetectionPath#test_dot_path().
  TestNormalizeDetectionPath.test_double_dot_path_with_root: NormalizeDetectionPath#test_double_dot_path_with_root().
  TestNormalizeDetectionPath.test_exception_fallback: NormalizeDetectionPath#test_exception_fallback().
  TestGetPathMtimeNs.test_existing_file: GetPathMtimeNs#test_existing_file().
  TestGetPathMtimeNs.test_nonexistent_file: GetPathMtimeNs#test_nonexistent_file().
  TestGetPathMtimeNs.test_directory: GetPathMtimeNs#test_directory().
  TestGetPathMtimeNs.test_permission_error_returns_none: GetPathMtimeNs#test_permission_error_returns_none().
  TestGetPathMtimeNs.test_os_error_returns_none: GetPathMtimeNs#test_os_error_returns_none().
  TestCachedLanguage.test_get_nonexistent_key: CachedLanguage#test_get_nonexistent_key().
  TestCachedLanguage.test_store_with_none_mtime_is_noop: CachedLanguage#test_store_with_none_mtime_is_noop().
  TestBuildExtensionConfidenceMap: BuildExtensionConfidenceMap#
  TestBuildContentPatternWeights: BuildContentPatternWeights#
  TestNormalizeDetectionPath: NormalizeDetectionPath#
  TestGetPathMtimeNs: GetPathMtimeNs#
  TestCachedLanguage: CachedLanguage#
---
# Module: [`tests/unit/core/test_language_detector_helpers.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_helpers.py)

## Classes
### `TestBuildContentPatternWeights`
- def: [`tests/unit/core/test_language_detector_helpers.py:79`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_helpers.py#L79)
- signature: `class TestBuildContentPatternWeights:`
- members:
  - `test_deterministic(self)` — [`L145`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_helpers.py#L145)
  - `test_entry_structure(self)` — [`L85`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_helpers.py#L85)
  - `test_java_patterns(self)` — [`L123`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_helpers.py#L123)
  - `test_key_languages_have_patterns(self)` — [`L96`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_helpers.py#L96)
  - `test_markdown_patterns(self)` — [`L138`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_helpers.py#L138)
  - `test_python_patterns(self)` — [`L131`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_helpers.py#L131)
  - `test_regex_patterns_compile(self)` — [`L115`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_helpers.py#L115)
  - `test_returns_dict(self)` — [`L80`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_helpers.py#L80)
- uses (calls/refs, reference-scoped): [`build_content_pattern_weights`](../../../tree_sitter_analyzer/_language_detector_helpers.md#build_content_pattern_weights)

### `TestBuildExtensionConfidenceMap`
- def: [`tests/unit/core/test_language_detector_helpers.py:19`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_helpers.py#L19)
- signature: `class TestBuildExtensionConfidenceMap:`
- members:
  - `test_ambiguous_extensions_have_lower_confidence(self)` — [`L63`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_helpers.py#L63)
  - `test_common_extensions_present(self)` — [`L34`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_helpers.py#L34)
  - `test_deterministic(self)` — [`L75`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_helpers.py#L75)
  - `test_entry_structure(self)` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_helpers.py#L25)
  - `test_high_confidence_for_primary_extensions(self)` — [`L56`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_helpers.py#L56)
  - `test_markdown_variants(self)` — [`L69`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_helpers.py#L69)
  - `test_returns_dict(self)` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_helpers.py#L20)
- uses (calls/refs, reference-scoped): [`build_extension_confidence_map`](../../../tree_sitter_analyzer/_language_detector_helpers.md#build_extension_confidence_map)

### `TestCachedLanguage`
- def: [`tests/unit/core/test_language_detector_helpers.py:236`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_helpers.py#L236)
- signature: `class TestCachedLanguage:`
- members:
  - `test_get_nonexistent_key(self)` — [`L237`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_helpers.py#L237)
  - `test_get_with_wrong_mtime(self)` — [`L258`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_helpers.py#L258)
  - `test_store_and_retrieve(self)` — [`L241`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_helpers.py#L241)
  - `test_store_with_none_mtime_is_noop(self)` — [`L255`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_helpers.py#L255)
  - `test_store_with_project_root(self)` — [`L272`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_helpers.py#L272)
- uses (calls/refs, reference-scoped): [`get_cached_language`](../../../tree_sitter_analyzer/_language_detector_helpers.md#get_cached_language), [`store_cached_language`](../../../tree_sitter_analyzer/_language_detector_helpers.md#store_cached_language), [`get_path_mtime_ns`](../../../tree_sitter_analyzer/_language_detector_helpers.md#get_path_mtime_ns)

### `TestGetPathMtimeNs`
- def: [`tests/unit/core/test_language_detector_helpers.py:194`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_helpers.py#L194)
- signature: `class TestGetPathMtimeNs:`
- members:
  - `test_directory(self)` — [`L214`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_helpers.py#L214)
  - `test_existing_file(self)` — [`L195`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_helpers.py#L195)
  - `test_nonexistent_file(self)` — [`L210`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_helpers.py#L210)
  - `test_os_error_returns_none(self)` — [`L228`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_helpers.py#L228)
  - `test_permission_error_returns_none(self)` — [`L219`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_helpers.py#L219)
- uses (calls/refs, reference-scoped): [`get_path_mtime_ns`](../../../tree_sitter_analyzer/_language_detector_helpers.md#get_path_mtime_ns)

### `TestNormalizeDetectionPath`
- def: [`tests/unit/core/test_language_detector_helpers.py:154`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_helpers.py#L154)
- signature: `class TestNormalizeDetectionPath:`
- members:
  - `test_absolute_path_ignores_root(self)` — [`L173`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_helpers.py#L173)
  - `test_absolute_path_unchanged_no_root(self)` — [`L155`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_helpers.py#L155)
  - `test_dot_path(self)` — [`L181`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_helpers.py#L181)
  - `test_double_dot_path_with_root(self)` — [`L185`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_helpers.py#L185)
  - `test_empty_string(self)` — [`L177`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_helpers.py#L177)
  - `test_exception_fallback(self)` — [`L189`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_helpers.py#L189)
  - `test_relative_path_with_root(self)` — [`L159`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_helpers.py#L159)
  - `test_tilde_expansion(self)` — [`L164`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_helpers.py#L164)
  - `test_tilde_with_root(self)` — [`L169`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_helpers.py#L169)
- uses (calls/refs, reference-scoped): [`normalize_detection_path`](../../../tree_sitter_analyzer/_language_detector_helpers.md#normalize_detection_path)

