---
title: 'Module: tests/unit/languages/test_markdown_plugin_comprehensive.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_markdown_plugin_comprehensive.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_markdown_plugin_comprehensive`/TestMarkdown
symbols:
  TestMarkdownPluginIntegration.test_analyze_file_success: PluginIntegration#test_analyze_file_success().
  TestMarkdownElementExtractor.extractor: ElementExtractor#extractor.
  TestMarkdownElement.test_markdown_element_creation: Element#test_markdown_element_creation().
  TestMarkdownPlugin.plugin: Plugin#plugin.
  TestMarkdownElementExtractor.test_extractor_initialization: ElementExtractor#test_extractor_initialization().
  TestMarkdownPlugin.test_analyze_file_no_tree_sitter: Plugin#test_analyze_file_no_tree_sitter().
  TestMarkdownElement.test_markdown_element_with_all_attributes: Element#test_markdown_element_with_all_attributes().
  TestMarkdownPlugin.test_plugin_initialization: Plugin#test_plugin_initialization().
  TestMarkdownPlugin.test_legacy_compatibility_methods: Plugin#test_legacy_compatibility_methods().
  TestMarkdownPluginIntegration.test_analyze_file_no_language: PluginIntegration#test_analyze_file_no_language().
  TestMarkdownElementExtractor.test_reset_caches: ElementExtractor#test_reset_caches().
  TestMarkdownPluginIntegration.test_analyze_file_file_not_found: PluginIntegration#test_analyze_file_file_not_found().
  TestMarkdownElementExtractor.mock_root_node: ElementExtractor#mock_root_node.
  TestMarkdownPluginEdgeCases.extractor: PluginEdgeCases#extractor.
  TestMarkdownElementExtractor.test_extract_headers_with_exception: ElementExtractor#test_extract_headers_with_exception().
  TestMarkdownPlugin.test_get_tree_sitter_language_general_error: Plugin#test_get_tree_sitter_language_general_error().
  TestMarkdownPlugin.test_get_tree_sitter_language_success: Plugin#test_get_tree_sitter_language_success().
  TestMarkdownPluginEdgeCases.test_very_long_content: PluginEdgeCases#test_very_long_content().
  TestMarkdownPluginEdgeCases.test_unicode_content: PluginEdgeCases#test_unicode_content().
  TestMarkdownElementExtractor.test_get_node_text_optimized_with_cache: ElementExtractor#test_get_node_text_optimized_with_cache().
  TestMarkdownElementExtractor.test_get_node_text_optimized_fallback: ElementExtractor#test_get_node_text_optimized_fallback().
  TestMarkdownElementExtractor.test_get_node_text_optimized_multiline: ElementExtractor#test_get_node_text_optimized_multiline().
  TestMarkdownElementExtractor.test_get_node_text_optimized_out_of_bounds: ElementExtractor#test_get_node_text_optimized_out_of_bounds().
  TestMarkdownPlugin.test_get_tree_sitter_language_import_error: Plugin#test_get_tree_sitter_language_import_error().
  TestMarkdownPlugin.test_extract_elements: Plugin#test_extract_elements().
  TestMarkdownPluginIntegration.plugin: PluginIntegration#plugin.
  TestMarkdownElementExtractor.test_extract_functions_with_none_tree: ElementExtractor#test_extract_functions_with_none_tree().
  TestMarkdownElementExtractor.test_extract_classes_with_none_tree: ElementExtractor#test_extract_classes_with_none_tree().
  TestMarkdownElementExtractor.test_extract_variables_with_none_tree: ElementExtractor#test_extract_variables_with_none_tree().
  TestMarkdownElementExtractor.test_extract_imports_with_none_tree: ElementExtractor#test_extract_imports_with_none_tree().
  TestMarkdownElementExtractor.test_traverse_nodes: ElementExtractor#test_traverse_nodes().
  TestMarkdownPlugin.test_get_extractor_cached: Plugin#test_get_extractor_cached().
  TestMarkdownPlugin.test_get_supported_queries: Plugin#test_get_supported_queries().
  TestMarkdownPlugin.test_extract_elements_exception: Plugin#test_extract_elements_exception().
  TestMarkdownPluginEdgeCases.test_empty_content: PluginEdgeCases#test_empty_content().
  TestMarkdownPluginEdgeCases.test_malformed_markdown: PluginEdgeCases#test_malformed_markdown().
  TestMarkdownPluginIntegration.extract_all_mock: PluginIntegration#extract_all_mock().
  TestMarkdownElementExtractor.test_parse_link_components_valid: ElementExtractor#test_parse_link_components_valid().
  TestMarkdownElementExtractor.test_parse_link_components_no_title: ElementExtractor#test_parse_link_components_no_title().
  TestMarkdownElementExtractor.test_parse_link_components_invalid: ElementExtractor#test_parse_link_components_invalid().
  TestMarkdownElementExtractor.test_parse_image_components_valid: ElementExtractor#test_parse_image_components_valid().
  TestMarkdownElementExtractor.test_parse_image_components_no_title: ElementExtractor#test_parse_image_components_no_title().
  TestMarkdownElementExtractor.test_parse_image_components_invalid: ElementExtractor#test_parse_image_components_invalid().
  TestMarkdownPluginIntegration.setup_method: PluginIntegration#setup_method().
  TestMarkdownPluginEdgeCases.plugin: PluginEdgeCases#plugin.
  TestMarkdownElementExtractor.mock_tree: ElementExtractor#mock_tree.
  TestMarkdownPlugin.import_side_effect: Plugin#import_side_effect().
  TestMarkdownElement: Element#
  TestMarkdownElementExtractor: ElementExtractor#
  TestMarkdownElementExtractor.setup_method: ElementExtractor#setup_method().
  TestMarkdownPlugin: Plugin#
  TestMarkdownPlugin.setup_method: Plugin#setup_method().
  TestMarkdownPluginIntegration: PluginIntegration#
  TestMarkdownPluginEdgeCases: PluginEdgeCases#
  TestMarkdownPluginEdgeCases.setup_method: PluginEdgeCases#setup_method().
---
# Module: [`tests/unit/languages/test_markdown_plugin_comprehensive.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_comprehensive.py)

## Classes
### `TestMarkdownElement`
- def: [`tests/unit/languages/test_markdown_plugin_comprehensive.py:26`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_comprehensive.py#L26)
- doc: Test MarkdownElement class
- signature: `class TestMarkdownElement:`
- members:
  - `test_markdown_element_creation(self)` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_comprehensive.py#L29) — Test basic MarkdownElement creation
  - `test_markdown_element_with_all_attributes(self)` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_comprehensive.py#L48) — Test MarkdownElement with all optional attributes
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`start_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`end_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.end_line), [`language`](../../../tree_sitter_analyzer/models/base.md#CodeElement.language), [`raw_text`](../../../tree_sitter_analyzer/models/base.md#CodeElement.raw_text), [`MarkdownElement`](../../../tree_sitter_analyzer/languages/markdown_plugin/elements.md#MarkdownElement), [`element_type`](../../../tree_sitter_analyzer/models/base.md#CodeElement.element_type), [`alt_text`](../../../tree_sitter_analyzer/languages/markdown_plugin/elements.md#MarkdownElement.alt_text), [`url`](../../../tree_sitter_analyzer/languages/markdown_plugin/elements.md#MarkdownElement.url), [`is_checked`](../../../tree_sitter_analyzer/languages/markdown_plugin/elements.md#MarkdownElement.is_checked), [`language_info`](../../../tree_sitter_analyzer/languages/markdown_plugin/elements.md#MarkdownElement.language_info), [`level`](../../../tree_sitter_analyzer/languages/markdown_plugin/elements.md#MarkdownElement.level), [`title`](../../../tree_sitter_analyzer/languages/markdown_plugin/elements.md#MarkdownElement.title)

### `TestMarkdownElementExtractor`
- def: [`tests/unit/languages/test_markdown_plugin_comprehensive.py:70`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_comprehensive.py#L70)
- doc: Test MarkdownElementExtractor class
- signature: `class TestMarkdownElementExtractor:`
- members:
  - `setup_method(self)` — [`L73`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_comprehensive.py#L73) — Setup test fixtures
  - `test_extract_classes_with_none_tree(self)` — [`L107`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_comprehensive.py#L107) — Test extract_classes with None tree
  - `test_extract_functions_with_none_tree(self)` — [`L102`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_comprehensive.py#L102) — Test extract_functions with None tree
  - `test_extract_headers_with_exception(self, mock_log)` — [`L125`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_comprehensive.py#L125) — Test header extraction with exception handling
  - `test_extract_imports_with_none_tree(self)` — [`L117`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_comprehensive.py#L117) — Test extract_imports with None tree
  - `test_extract_variables_with_none_tree(self)` — [`L112`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_comprehensive.py#L112) — Test extract_variables with None tree
  - `test_extractor_initialization(self)` — [`L80`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_comprehensive.py#L80) — Test extractor initialization
  - `test_get_node_text_optimized_fallback(self)` — [`L157`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_comprehensive.py#L157) — Test node text extraction fallback method
  - `test_get_node_text_optimized_multiline(self)` — [`L175`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_comprehensive.py#L175) — Test node text extraction for multiline content
  - `test_get_node_text_optimized_out_of_bounds(self)` — [`L195`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_comprehensive.py#L195) — Test node text extraction with out of bounds indices
  - `test_get_node_text_optimized_with_cache(self)` — [`L144`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_comprehensive.py#L144) — Test node text extraction with cache
  - `test_parse_image_components_invalid(self)` — [`L247`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_comprehensive.py#L247) — Test parsing invalid image components
  - `test_parse_image_components_no_title(self)` — [`L240`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_comprehensive.py#L240) — Test parsing image components without title
  - `test_parse_image_components_valid(self)` — [`L233`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_comprehensive.py#L233) — Test parsing valid image components
  - `test_parse_link_components_invalid(self)` — [`L226`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_comprehensive.py#L226) — Test parsing invalid link components
  - `test_parse_link_components_no_title(self)` — [`L219`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_comprehensive.py#L219) — Test parsing link components without title
  - `test_parse_link_components_valid(self)` — [`L212`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_comprehensive.py#L212) — Test parsing valid link components
  - `test_reset_caches(self)` — [`L90`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_comprehensive.py#L90) — Test cache reset functionality
  - `test_traverse_nodes(self)` — [`L254`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_comprehensive.py#L254) — Test node traversal
  - `extractor` — [`L75`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_comprehensive.py#L75)
  - `mock_root_node` — [`L77`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_comprehensive.py#L77)
  - `mock_tree` — [`L76`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_comprehensive.py#L76)
- uses (calls/refs, reference-scoped): [`MarkdownElementExtractor`](../../../tree_sitter_analyzer/languages/markdown_plugin/extractor.md#MarkdownElementExtractor), [`source_code`](../../../tree_sitter_analyzer/languages/markdown_plugin/extractor.md#MarkdownElementExtractor.source_code), [`extract_classes`](../../../tree_sitter_analyzer/languages/markdown_plugin/public_extraction.md#MarkdownModelExtractionMixin.extract_classes), [`extract_functions`](../../../tree_sitter_analyzer/languages/markdown_plugin/public_extraction.md#MarkdownModelExtractionMixin.extract_functions), [`extract_imports`](../../../tree_sitter_analyzer/languages/markdown_plugin/public_extraction.md#MarkdownModelExtractionMixin.extract_imports), [`extract_variables`](../../../tree_sitter_analyzer/languages/markdown_plugin/public_extraction.md#MarkdownModelExtractionMixin.extract_variables), [`_get_node_text_optimized`](../../../tree_sitter_analyzer/languages/markdown_plugin/private_extraction.md#MarkdownExtractorStateMixin._get_node_text_optimized), [`extract_headers`](../../../tree_sitter_analyzer/languages/markdown_plugin/public_extraction.md#MarkdownBlockExtractionMixin.extract_headers), [`content_lines`](../../../tree_sitter_analyzer/languages/markdown_plugin/extractor.md#MarkdownElementExtractor.content_lines), [`_node_text_cache`](../../../tree_sitter_analyzer/languages/markdown_plugin/extractor.md#MarkdownElementExtractor._node_text_cache), [`_element_cache`](../../../tree_sitter_analyzer/languages/markdown_plugin/extractor.md#MarkdownElementExtractor._element_cache), [`_processed_nodes`](../../../tree_sitter_analyzer/languages/markdown_plugin/extractor.md#MarkdownElementExtractor._processed_nodes), [`_traverse_nodes`](../../../tree_sitter_analyzer/languages/markdown_plugin/private_extraction.md#MarkdownExtractorStateMixin._traverse_nodes), [`parse_image_components`](../../../tree_sitter_analyzer/languages/markdown_plugin/link_image_extractor.md#parse_image_components), [`parse_link_components`](../../../tree_sitter_analyzer/languages/markdown_plugin/link_image_extractor.md#parse_link_components), [`_reset_caches`](../../../tree_sitter_analyzer/languages/markdown_plugin/private_extraction.md#MarkdownExtractorStateMixin._reset_caches), [`current_file`](../../../tree_sitter_analyzer/languages/markdown_plugin/extractor.md#MarkdownElementExtractor.current_file)

### `TestMarkdownPlugin`
- def: [`tests/unit/languages/test_markdown_plugin_comprehensive.py:275`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_comprehensive.py#L275)
- doc: Test MarkdownPlugin class
- signature: `class TestMarkdownPlugin:`
- members:
  - `import_side_effect(name, *args, **kwargs)` — [`L361`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_comprehensive.py#L361)
  - `setup_method(self)` — [`L278`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_comprehensive.py#L278) — Setup test fixtures
  - `test_analyze_file_no_tree_sitter(self)` — [`L325`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_comprehensive.py#L325) — Test analyze_file when tree-sitter is not available
  - `test_extract_elements(self)` — [`L405`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_comprehensive.py#L405) — Test extract_elements method
  - `test_extract_elements_exception(self)` — [`L444`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_comprehensive.py#L444) — Test extract_elements with exception
  - `test_get_extractor_cached(self)` — [`L291`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_comprehensive.py#L291) — Test get_extractor with caching
  - `test_get_supported_queries(self)` — [`L297`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_comprehensive.py#L297) — Test get_supported_queries method
  - `test_get_tree_sitter_language_general_error(self)` — [`L354`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_comprehensive.py#L354) — Test get_tree_sitter_language with general error
  - `test_get_tree_sitter_language_import_error(self)` — [`L338`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_comprehensive.py#L338) — Test get_tree_sitter_language with import error
  - `test_get_tree_sitter_language_success(self)` — [`L376`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_comprehensive.py#L376) — Test successful get_tree_sitter_language
  - `test_legacy_compatibility_methods(self)` — [`L456`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_comprehensive.py#L456) — Test extractor methods via create_extractor
  - `test_plugin_initialization(self)` — [`L282`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_comprehensive.py#L282) — Test plugin initialization
  - `plugin` — [`L280`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_comprehensive.py#L280)
- uses (calls/refs, reference-scoped): [`AnalysisResult`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult), [`AnalysisRequest`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest), [`success`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.success), [`file_path`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest.file_path), [`extract_functions`](../../../tree_sitter_analyzer/plugins/base.md#ElementExtractor.extract_functions), [`extract_classes`](../../../tree_sitter_analyzer/plugins/base.md#ElementExtractor.extract_classes), [`extract_variables`](../../../tree_sitter_analyzer/plugins/base.md#ElementExtractor.extract_variables), [`error_message`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.error_message), [`extract_imports`](../../../tree_sitter_analyzer/plugins/base.md#ElementExtractor.extract_imports), [`MarkdownElementExtractor`](../../../tree_sitter_analyzer/languages/markdown_plugin/extractor.md#MarkdownElementExtractor), [`analyze_file`](../../../tree_sitter_analyzer/languages/markdown_plugin/plugin.md#MarkdownPlugin.analyze_file), [`extract_elements`](../../../tree_sitter_analyzer/languages/markdown_plugin/plugin.md#MarkdownPlugin.extract_elements), [`MarkdownPlugin`](../../../tree_sitter_analyzer/languages/markdown_plugin/plugin.md#MarkdownPlugin), [`get_tree_sitter_language`](../../../tree_sitter_analyzer/languages/markdown_plugin/plugin.md#MarkdownPlugin.get_tree_sitter_language), [`create_extractor`](../../../tree_sitter_analyzer/languages/markdown_plugin/plugin.md#MarkdownPlugin.create_extractor), [`_language_cache`](../../../tree_sitter_analyzer/languages/markdown_plugin/plugin.md#MarkdownPlugin._language_cache), [`get_extractor`](../../../tree_sitter_analyzer/languages/markdown_plugin/plugin.md#MarkdownPlugin.get_extractor), [`_extractor`](../../../tree_sitter_analyzer/languages/markdown_plugin/plugin.md#MarkdownPlugin._extractor), [`get_language_name`](../../../tree_sitter_analyzer/languages/markdown_plugin/plugin.md#MarkdownPlugin.get_language_name), [`get_supported_queries`](../../../tree_sitter_analyzer/languages/markdown_plugin/plugin.md#MarkdownPlugin.get_supported_queries), [`language`](../../../tree_sitter_analyzer/languages/markdown_plugin/plugin.md#MarkdownPlugin.language)

### `TestMarkdownPluginEdgeCases`
- def: [`tests/unit/languages/test_markdown_plugin_comprehensive.py:561`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_comprehensive.py#L561)
- doc: Test edge cases and error conditions
- signature: `class TestMarkdownPluginEdgeCases:`
- members:
  - `setup_method(self)` — [`L564`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_comprehensive.py#L564) — Setup test fixtures
  - `test_empty_content(self)` — [`L569`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_comprehensive.py#L569) — Test handling of empty content
  - `test_malformed_markdown(self)` — [`L578`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_comprehensive.py#L578) — Test handling of malformed markdown
  - `test_unicode_content(self)` — [`L609`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_comprehensive.py#L609) — Test handling of Unicode content
  - `test_very_long_content(self)` — [`L588`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_comprehensive.py#L588) — Test handling of very long content
  - `extractor` — [`L567`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_comprehensive.py#L567)
  - `plugin` — [`L566`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_comprehensive.py#L566)
- uses (calls/refs, reference-scoped): [`MarkdownElementExtractor`](../../../tree_sitter_analyzer/languages/markdown_plugin/extractor.md#MarkdownElementExtractor), [`MarkdownPlugin`](../../../tree_sitter_analyzer/languages/markdown_plugin/plugin.md#MarkdownPlugin), [`extract_links`](../../../tree_sitter_analyzer/languages/markdown_plugin/public_extraction.md#MarkdownInlineExtractionMixin.extract_links), [`source_code`](../../../tree_sitter_analyzer/languages/markdown_plugin/extractor.md#MarkdownElementExtractor.source_code), [`_get_node_text_optimized`](../../../tree_sitter_analyzer/languages/markdown_plugin/private_extraction.md#MarkdownExtractorStateMixin._get_node_text_optimized), [`extract_headers`](../../../tree_sitter_analyzer/languages/markdown_plugin/public_extraction.md#MarkdownBlockExtractionMixin.extract_headers), [`content_lines`](../../../tree_sitter_analyzer/languages/markdown_plugin/extractor.md#MarkdownElementExtractor.content_lines)

### `TestMarkdownPluginIntegration`
- def: [`tests/unit/languages/test_markdown_plugin_comprehensive.py:469`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_comprehensive.py#L469)
- doc: Integration tests for Markdown plugin
- signature: `class TestMarkdownPluginIntegration:`
- members:
  - `extract_all_mock(tree, source)` — [`L534`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_comprehensive.py#L534)
  - `setup_method(self)` — [`L472`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_comprehensive.py#L472) — Setup test fixtures
  - `test_analyze_file_file_not_found(self)` — [`L477`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_comprehensive.py#L477) — Test analyze_file with non-existent file
  - `test_analyze_file_no_language(self)` — [`L487`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_comprehensive.py#L487) — Test analyze_file when language loading fails
  - `test_analyze_file_success(self, mock_ts, mock_ts_plugin, mock_read_file_safe)` — [`L500`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_comprehensive.py#L500) — Test successful analyze_file
  - `plugin` — [`L474`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_markdown_plugin_comprehensive.py#L474)
- uses (calls/refs, reference-scoped): [`AnalysisRequest`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest), [`elements`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.elements), [`language`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.language), [`file_path`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.file_path), [`success`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.success), [`file_path`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest.file_path), [`MarkdownElement`](../../../tree_sitter_analyzer/languages/markdown_plugin/elements.md#MarkdownElement), [`line_count`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.line_count), [`error_message`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.error_message), [`analyze_file`](../../../tree_sitter_analyzer/languages/markdown_plugin/plugin.md#MarkdownPlugin.analyze_file), [`MarkdownPlugin`](../../../tree_sitter_analyzer/languages/markdown_plugin/plugin.md#MarkdownPlugin)

