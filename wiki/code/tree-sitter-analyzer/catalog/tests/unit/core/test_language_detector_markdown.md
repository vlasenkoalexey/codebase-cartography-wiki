---
title: 'Module: tests/unit/core/test_language_detector_markdown.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_language_detector_markdown.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_language_detector_markdown`/TestMarkdown
symbols:
  TestMarkdownLanguageDetection.detector: LanguageDetection#detector.
  TestMarkdownLanguageDetection.test_add_custom_markdown_extension: LanguageDetection#test_add_custom_markdown_extension().
  TestMarkdownLanguageDetection.test_markdown_language_support: LanguageDetection#test_markdown_language_support().
  TestMarkdownDetectionIntegration.detector: DetectionIntegration#detector.
  TestMarkdownLanguageDetection.test_markdown_extensions_detection: LanguageDetection#test_markdown_extensions_detection().
  TestMarkdownLanguageDetection.test_markdown_extensions_with_confidence: LanguageDetection#test_markdown_extensions_with_confidence().
  TestMarkdownLanguageDetection.test_markdown_content_patterns: LanguageDetection#test_markdown_content_patterns().
  TestMarkdownLanguageDetection.test_markdown_content_scoring: LanguageDetection#test_markdown_content_scoring().
  TestMarkdownLanguageDetection.test_markdown_vs_other_languages: LanguageDetection#test_markdown_vs_other_languages().
  TestMarkdownLanguageDetection.test_markdown_extension_mapping: LanguageDetection#test_markdown_extension_mapping().
  TestMarkdownLanguageDetection.test_markdown_language_info: LanguageDetection#test_markdown_language_info().
  TestMarkdownLanguageDetection.test_case_insensitive_extensions: LanguageDetection#test_case_insensitive_extensions().
  TestMarkdownLanguageDetection.test_markdown_with_path_variations: LanguageDetection#test_markdown_with_path_variations().
  TestMarkdownLanguageDetection.test_markdown_content_edge_cases: LanguageDetection#test_markdown_content_edge_cases().
  TestMarkdownLanguageDetection.test_markdown_pattern_regex: LanguageDetection#test_markdown_pattern_regex().
  TestMarkdownLanguageDetection.test_unknown_extension_not_markdown: LanguageDetection#test_unknown_extension_not_markdown().
  TestMarkdownDetectionIntegration.test_real_markdown_samples: DetectionIntegration#test_real_markdown_samples().
  TestMarkdownDetectionIntegration.test_documentation_markdown: DetectionIntegration#test_documentation_markdown().
  TestMarkdownDetectionIntegration.test_blog_post_markdown: DetectionIntegration#test_blog_post_markdown().
  TestMarkdownLanguageDetection: LanguageDetection#
  TestMarkdownLanguageDetection.setup_method: LanguageDetection#setup_method().
  TestMarkdownDetectionIntegration: DetectionIntegration#
  TestMarkdownDetectionIntegration.setup_method: DetectionIntegration#setup_method().
---
# Module: [`tests/unit/core/test_language_detector_markdown.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_markdown.py)

## Classes
### `TestMarkdownDetectionIntegration`
- def: [`tests/unit/core/test_language_detector_markdown.py:256`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_markdown.py#L256)
- doc: Integration tests for Markdown detection
- signature: `class TestMarkdownDetectionIntegration:`
- members:
  - `setup_method(self)` — [`L259`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_markdown.py#L259) — Setup test fixtures
  - `test_blog_post_markdown(self)` — [`L341`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_markdown.py#L341) — Test with blog post style Markdown
  - `test_documentation_markdown(self)` — [`L300`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_markdown.py#L300) — Test with documentation-style Markdown
  - `test_real_markdown_samples(self)` — [`L263`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_markdown.py#L263) — Test with realistic Markdown samples
  - `detector` — [`L261`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_markdown.py#L261)
- uses (calls/refs, reference-scoped): [`detect_language`](../../../tree_sitter_analyzer/language_detector.md#LanguageDetector.detect_language), [`LanguageDetector`](../../../tree_sitter_analyzer/language_detector.md#LanguageDetector)

### `TestMarkdownLanguageDetection`
- def: [`tests/unit/core/test_language_detector_markdown.py:13`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_markdown.py#L13)
- doc: Test Markdown language detection
- signature: `class TestMarkdownLanguageDetection:`
- members:
  - `setup_method(self)` — [`L16`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_markdown.py#L16) — Setup test fixtures
  - `test_add_custom_markdown_extension(self)` — [`L184`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_markdown.py#L184) — Test adding custom Markdown extension
  - `test_case_insensitive_extensions(self)` — [`L157`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_markdown.py#L157) — Test case-insensitive extension detection
  - `test_markdown_content_edge_cases(self)` — [`L198`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_markdown.py#L198) — Test Markdown content detection edge cases
  - `test_markdown_content_patterns(self)` — [`L53`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_markdown.py#L53) — Test Markdown content pattern detection
  - `test_markdown_content_scoring(self)` — [`L90`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_markdown.py#L90) — Test Markdown content pattern scoring
  - `test_markdown_extension_mapping(self)` — [`L139`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_markdown.py#L139) — Test Markdown extension mapping
  - `test_markdown_extensions_detection(self)` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_markdown.py#L20) — Test detection of Markdown file extensions
  - `test_markdown_extensions_with_confidence(self)` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_markdown.py#L35) — Test Markdown extension detection with confidence scores
  - `test_markdown_language_info(self)` — [`L147`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_markdown.py#L147) — Test Markdown language information
  - `test_markdown_language_support(self)` — [`L134`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_markdown.py#L134) — Test that Markdown is in supported languages
  - `test_markdown_pattern_regex(self)` — [`L219`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_markdown.py#L219) — Test Markdown pattern regex matching
  - `test_markdown_vs_other_languages(self)` — [`L119`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_markdown.py#L119) — Test Markdown detection vs other languages
  - `test_markdown_with_path_variations(self)` — [`L170`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_markdown.py#L170) — Test Markdown detection with various path formats
  - `test_unknown_extension_not_markdown(self)` — [`L241`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_markdown.py#L241) — Test that unknown extensions don't default to Markdown
  - `detector` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_markdown.py#L18)
- uses (calls/refs, reference-scoped): [`detect_from_extension`](../../../tree_sitter_analyzer/language_detector.md#LanguageDetector.detect_from_extension), [`detect_language`](../../../tree_sitter_analyzer/language_detector.md#LanguageDetector.detect_language), [`LanguageDetector`](../../../tree_sitter_analyzer/language_detector.md#LanguageDetector), [`is_supported`](../../../tree_sitter_analyzer/language_detector.md#LanguageDetector.is_supported), [`content_patterns`](../../../tree_sitter_analyzer/language_detector.md#LanguageDetector.content_patterns), [`get_language_info`](../../../tree_sitter_analyzer/language_detector.md#LanguageDetector.get_language_info), [`get_supported_extensions`](../../../tree_sitter_analyzer/language_detector.md#LanguageDetector.get_supported_extensions), [`get_supported_languages`](../../../tree_sitter_analyzer/language_detector.md#LanguageDetector.get_supported_languages), [`add_extension_mapping`](../../../tree_sitter_analyzer/language_detector.md#LanguageDetector.add_extension_mapping)

