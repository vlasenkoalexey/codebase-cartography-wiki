---
title: 'Module: tests/unit/core/test_language_detector_html_css.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_language_detector_html_css.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_language_detector_html_css`/TestHtmlCss
symbols:
  TestHtmlCssLanguageDetection.detector: LanguageDetection#detector.
  TestHtmlCssLanguageDetection.test_html_content_detection: LanguageDetection#test_html_content_detection().
  TestHtmlCssLanguageDetection.test_css_content_detection: LanguageDetection#test_css_content_detection().
  TestHtmlCssContentPatterns.detector: ContentPatterns#detector.
  TestHtmlCssLanguageDetection.test_html_extension_detection: LanguageDetection#test_html_extension_detection().
  TestHtmlCssLanguageDetection.test_css_extension_detection: LanguageDetection#test_css_extension_detection().
  TestHtmlCssLanguageDetection.test_html_css_supported_languages: LanguageDetection#test_html_css_supported_languages().
  TestHtmlCssLanguageDetection.test_html_css_is_supported: LanguageDetection#test_html_css_is_supported().
  TestHtmlCssLanguageDetection.test_html_css_extensions_in_mapping: LanguageDetection#test_html_css_extensions_in_mapping().
  TestHtmlCssLanguageDetection.test_detect_from_extension_html_css: LanguageDetection#test_detect_from_extension_html_css().
  TestHtmlCssLanguageDetection.test_get_language_info_html_css: LanguageDetection#test_get_language_info_html_css().
  TestHtmlCssLanguageDetection.test_invalid_input_handling: LanguageDetection#test_invalid_input_handling().
  TestHtmlCssLanguageDetection.test_unknown_extension: LanguageDetection#test_unknown_extension().
  TestHtmlCssLanguageDetection.test_case_insensitive_extensions: LanguageDetection#test_case_insensitive_extensions().
  TestHtmlCssContentPatterns.test_html_doctype_pattern: ContentPatterns#test_html_doctype_pattern().
  TestHtmlCssContentPatterns.test_html_tag_patterns: ContentPatterns#test_html_tag_patterns().
  TestHtmlCssContentPatterns.test_css_selector_patterns: ContentPatterns#test_css_selector_patterns().
  TestHtmlCssContentPatterns.test_css_at_rule_patterns: ContentPatterns#test_css_at_rule_patterns().
  TestHtmlCssLanguageDetection.test_global_detect_function_html_css: LanguageDetection#test_global_detect_function_html_css().
  TestHtmlCssLanguageDetection: LanguageDetection#
  TestHtmlCssLanguageDetection.setup_method: LanguageDetection#setup_method().
  TestHtmlCssContentPatterns: ContentPatterns#
  TestHtmlCssContentPatterns.setup_method: ContentPatterns#setup_method().
---
# Module: [`tests/unit/core/test_language_detector_html_css.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_html_css.py)

## Classes
### `TestHtmlCssContentPatterns`
- def: [`tests/unit/core/test_language_detector_html_css.py:246`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_html_css.py#L246)
- doc: Test HTML and CSS content pattern matching
- signature: `class TestHtmlCssContentPatterns:`
- members:
  - `setup_method(self)` — [`L249`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_html_css.py#L249) — Set up test fixtures
  - `test_css_at_rule_patterns(self)` — [`L292`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_html_css.py#L292) — Test CSS at-rule pattern matching
  - `test_css_selector_patterns(self)` — [`L278`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_html_css.py#L278) — Test CSS selector pattern matching
  - `test_html_doctype_pattern(self)` — [`L253`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_html_css.py#L253) — Test HTML DOCTYPE pattern matching
  - `test_html_tag_patterns(self)` — [`L264`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_html_css.py#L264) — Test HTML tag pattern matching
  - `detector` — [`L251`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_html_css.py#L251)
- uses (calls/refs, reference-scoped): [`LanguageDetector`](../../../tree_sitter_analyzer/language_detector.md#LanguageDetector), [`content_patterns`](../../../tree_sitter_analyzer/language_detector.md#LanguageDetector.content_patterns)

### `TestHtmlCssLanguageDetection`
- def: [`tests/unit/core/test_language_detector_html_css.py:16`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_html_css.py#L16)
- doc: Test HTML and CSS language detection
- signature: `class TestHtmlCssLanguageDetection:`
- members:
  - `setup_method(self)` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_html_css.py#L19) — Set up test fixtures
  - `test_case_insensitive_extensions(self)` — [`L229`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_html_css.py#L229) — Test case-insensitive extension handling
  - `test_css_content_detection(self)` — [`L98`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_html_css.py#L98) — Test CSS content-based detection
  - `test_css_extension_detection(self)` — [`L40`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_html_css.py#L40) — Test CSS file extension detection
  - `test_detect_from_extension_html_css(self)` — [`L172`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_html_css.py#L172) — Test quick detection using extension only
  - `test_get_language_info_html_css(self)` — [`L182`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_html_css.py#L182) — Test language info retrieval for HTML and CSS
  - `test_global_detect_function_html_css(self)` — [`L200`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_html_css.py#L200) — Test global detection function for HTML and CSS
  - `test_html_content_detection(self)` — [`L62`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_html_css.py#L62) — Test HTML content-based detection
  - `test_html_css_extensions_in_mapping(self)` — [`L161`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_html_css.py#L161) — Test that HTML and CSS extensions are in extension mapping
  - `test_html_css_is_supported(self)` — [`L156`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_html_css.py#L156) — Test HTML and CSS support status
  - `test_html_css_supported_languages(self)` — [`L150`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_html_css.py#L150) — Test that HTML and CSS are in supported languages
  - `test_html_extension_detection(self)` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_html_css.py#L23) — Test HTML file extension detection
  - `test_invalid_input_handling(self)` — [`L206`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_html_css.py#L206) — Test handling of invalid inputs
  - `test_unknown_extension(self)` — [`L223`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_html_css.py#L223) — Test handling of unknown extensions
  - `detector` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_detector_html_css.py#L21)
- uses (calls/refs, reference-scoped): [`detect_language_from_file`](../../../tree_sitter_analyzer/language_detector.md#detect_language_from_file), [`detect_from_extension`](../../../tree_sitter_analyzer/language_detector.md#LanguageDetector.detect_from_extension), [`detect_language`](../../../tree_sitter_analyzer/language_detector.md#LanguageDetector.detect_language), [`LanguageDetector`](../../../tree_sitter_analyzer/language_detector.md#LanguageDetector), [`is_supported`](../../../tree_sitter_analyzer/language_detector.md#LanguageDetector.is_supported), [`content_patterns`](../../../tree_sitter_analyzer/language_detector.md#LanguageDetector.content_patterns), [`get_language_info`](../../../tree_sitter_analyzer/language_detector.md#LanguageDetector.get_language_info), [`get_supported_extensions`](../../../tree_sitter_analyzer/language_detector.md#LanguageDetector.get_supported_extensions), [`get_supported_languages`](../../../tree_sitter_analyzer/language_detector.md#LanguageDetector.get_supported_languages)

