---
title: 'Module: tests/unit/languages/test_html_plugin.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_html_plugin.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_html_plugin`/
symbols:
  TestHtmlIntegration.test_markup_element_summary: TestHtmlIntegration#test_markup_element_summary().
  TestHtmlIntegration.test_markup_element_creation: TestHtmlIntegration#test_markup_element_creation().
  TestHtmlIntegration.test_nested_elements: TestHtmlIntegration#test_nested_elements().
  MockRequest.query_filters: MockRequest#query_filters.
  TestHtmlElementExtractor.extractor: TestHtmlElementExtractor#extractor.
  TestHtmlPlugin.plugin: TestHtmlPlugin#plugin.
  TestHtmlElementExtractor.test_element_categories: TestHtmlElementExtractor#test_element_categories().
  TestHtmlElementExtractor.test_classify_element: TestHtmlElementExtractor#test_classify_element().
  TestHtmlElementExtractor.test_extract_functions_returns_empty: TestHtmlElementExtractor#test_extract_functions_returns_empty().
  TestHtmlElementExtractor.test_extract_classes_returns_empty: TestHtmlElementExtractor#test_extract_classes_returns_empty().
  TestHtmlElementExtractor.test_extract_variables_returns_empty: TestHtmlElementExtractor#test_extract_variables_returns_empty().
  TestHtmlElementExtractor.test_extract_imports_returns_empty: TestHtmlElementExtractor#test_extract_imports_returns_empty().
  TestHtmlPlugin.test_get_supported_element_types: TestHtmlPlugin#test_get_supported_element_types().
  TestHtmlPlugin.test_get_queries: TestHtmlPlugin#test_get_queries().
  TestHtmlPlugin.test_execute_query_strategy: TestHtmlPlugin#test_execute_query_strategy().
  TestHtmlPlugin.test_get_element_categories: TestHtmlPlugin#test_get_element_categories().
  TestHtmlPlugin.test_analyze_file_fallback.MockRequest: TestHtmlPlugin#test_analyze_file_fallback().MockRequest#
  TestHtmlElementExtractor: TestHtmlElementExtractor#
  TestHtmlElementExtractor.setup_method: TestHtmlElementExtractor#setup_method().
  TestHtmlPlugin: TestHtmlPlugin#
  TestHtmlPlugin.setup_method: TestHtmlPlugin#setup_method().
  TestHtmlPlugin.test_analyze_file_fallback: TestHtmlPlugin#test_analyze_file_fallback().
  TestHtmlPlugin.test_analyze_file_fallback.MockRequest.__init__: TestHtmlPlugin#test_analyze_file_fallback().MockRequest#__init__().
  MockRequest.include_source: MockRequest#include_source.
  TestHtmlIntegration: TestHtmlIntegration#
---
# Module: [`tests/unit/languages/test_html_plugin.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin.py)

## Classes
### `MockRequest`
- def: [`tests/unit/languages/test_html_plugin.py:119`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin.py#L119)
- signature: `class MockRequest:`
- members:
  - `include_source` — [`L121`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin.py#L121)
  - `query_filters` — [`L122`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin.py#L122)
- protocol/private: `__init__`[`L120`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin.py#L120)
- uses (calls/refs, reference-scoped): [`elements`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.elements), [`language`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.language), [`success`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.success), [`MarkupElement`](../../../tree_sitter_analyzer/models/markup_models.md#MarkupElement), [`line_count`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.line_count), [`source_code`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.source_code), [`analyze_file`](../../../tree_sitter_analyzer/languages/html_plugin.md#HtmlPlugin.analyze_file)  (1 test-only)

### `TestHtmlElementExtractor`
- def: [`tests/unit/languages/test_html_plugin.py:16`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin.py#L16)
- doc: Test HTML element extraction functionality
- signature: `class TestHtmlElementExtractor:`
- members:
  - `setup_method(self)` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin.py#L19) — Set up test fixtures
  - `test_classify_element(self)` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin.py#L30) — Test element classification
  - `test_element_categories(self)` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin.py#L23) — Test HTML element categorization
  - `test_extract_classes_returns_empty(self)` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin.py#L45) — Test that HTML extractor returns empty list for classes
  - `test_extract_functions_returns_empty(self)` — [`L40`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin.py#L40) — Test that HTML extractor returns empty list for functions
  - `test_extract_imports_returns_empty(self)` — [`L55`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin.py#L55) — Test that HTML extractor returns empty list for imports
  - `test_extract_variables_returns_empty(self)` — [`L50`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin.py#L50) — Test that HTML extractor returns empty list for variables
  - `extractor` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin.py#L21)
- uses (calls/refs, reference-scoped): [`_classify_element`](../../../tree_sitter_analyzer/languages/html_plugin.md#HtmlElementExtractor._classify_element), [`HtmlElementExtractor`](../../../tree_sitter_analyzer/languages/html_plugin.md#HtmlElementExtractor), [`element_categories`](../../../tree_sitter_analyzer/languages/html_plugin.md#HtmlElementExtractor.element_categories), [`extract_classes`](../../../tree_sitter_analyzer/languages/html_plugin.md#HtmlElementExtractor.extract_classes), [`extract_functions`](../../../tree_sitter_analyzer/languages/html_plugin.md#HtmlElementExtractor.extract_functions), [`extract_imports`](../../../tree_sitter_analyzer/languages/html_plugin.md#HtmlElementExtractor.extract_imports), [`extract_variables`](../../../tree_sitter_analyzer/languages/html_plugin.md#HtmlElementExtractor.extract_variables)

### `TestHtmlIntegration`
- def: [`tests/unit/languages/test_html_plugin.py:152`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin.py#L152)
- doc: Integration tests for HTML plugin
- signature: `class TestHtmlIntegration:`
- members:
  - `test_markup_element_creation(self)` — [`L155`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin.py#L155) — Test MarkupElement creation
  - `test_markup_element_summary(self)` — [`L176`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin.py#L176) — Test MarkupElement summary generation
  - `test_nested_elements(self)` — [`L199`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin.py#L199) — Test nested HTML elements
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`start_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`end_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.end_line), [`language`](../../../tree_sitter_analyzer/models/base.md#CodeElement.language), [`raw_text`](../../../tree_sitter_analyzer/models/base.md#CodeElement.raw_text), [`MarkupElement`](../../../tree_sitter_analyzer/models/markup_models.md#MarkupElement), [`tag_name`](../../../tree_sitter_analyzer/models/markup_models.md#MarkupElement.tag_name), [`element_class`](../../../tree_sitter_analyzer/models/markup_models.md#MarkupElement.element_class), [`attributes`](../../../tree_sitter_analyzer/models/markup_models.md#MarkupElement.attributes), [`children`](../../../tree_sitter_analyzer/models/markup_models.md#MarkupElement.children), [`parent`](../../../tree_sitter_analyzer/models/markup_models.md#MarkupElement.parent), [`to_summary_item`](../../../tree_sitter_analyzer/models/markup_models.md#MarkupElement.to_summary_item)

### `TestHtmlPlugin`
- def: [`tests/unit/languages/test_html_plugin.py:61`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin.py#L61)
- doc: Test HTML plugin functionality
- signature: `class TestHtmlPlugin:`
- members:
  - `setup_method(self)` — [`L64`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin.py#L64) — Set up test fixtures
  - `test_analyze_file_fallback(self)` — [`L101`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin.py#L101) — Test HTML file analysis with fallback parsing
  - `test_execute_query_strategy(self)` — [`L81`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin.py#L81) — Test query strategy execution
  - `test_get_element_categories(self)` — [`L92`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin.py#L92) — Test element categories
  - `test_get_queries(self)` — [`L73`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin.py#L73) — Test query retrieval
  - `test_get_supported_element_types(self)` — [`L68`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin.py#L68) — Test supported element types
  - `plugin` — [`L66`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_html_plugin.py#L66)
- uses (calls/refs, reference-scoped): [`HtmlPlugin`](../../../tree_sitter_analyzer/languages/html_plugin.md#HtmlPlugin), [`execute_query_strategy`](../../../tree_sitter_analyzer/languages/html_plugin.md#HtmlPlugin.execute_query_strategy), [`get_queries`](../../../tree_sitter_analyzer/languages/html_plugin.md#HtmlPlugin.get_queries), [`get_element_categories`](../../../tree_sitter_analyzer/languages/html_plugin.md#HtmlPlugin.get_element_categories), [`get_supported_element_types`](../../../tree_sitter_analyzer/languages/html_plugin.md#HtmlPlugin.get_supported_element_types)
- used by: (1 test-only callers)

