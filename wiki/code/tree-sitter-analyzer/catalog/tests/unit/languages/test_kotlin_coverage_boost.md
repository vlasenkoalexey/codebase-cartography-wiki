---
title: 'Module: tests/unit/languages/test_kotlin_coverage_boost.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_kotlin_coverage_boost.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_kotlin_coverage_boost`/TestKotlin
symbols:
  TestKotlinExtractorParameters.extractor: ExtractorParameters#extractor().
  TestKotlinExtractorVisibility.extractor: ExtractorVisibility#extractor().
  TestKotlinExtractorProperties.extractor: ExtractorProperties#extractor().
  TestKotlinExtractorImports.extractor: ExtractorImports#extractor().
  TestKotlinExtractorDocstrings.extractor: ExtractorDocstrings#extractor().
  TestKotlinExtractorErrorPaths.extractor: ExtractorErrorPaths#extractor().
  TestKotlinPluginEdgeCases.plugin: PluginEdgeCases#plugin().
  TestKotlinExtractorInternalMethods.extractor: ExtractorInternalMethods#extractor().
  TestKotlinTextExtractionEdgeCases.extractor: TextExtractionEdgeCases#extractor().
  TestKotlinExtractorExceptionPaths.extractor: ExtractorExceptionPaths#extractor().
  TestKotlinExtractorParameters: ExtractorParameters#
  TestKotlinExtractorParameters.parser: ExtractorParameters#parser().
  TestKotlinExtractorParameters.test_function_parameter_shapes: ExtractorParameters#test_function_parameter_shapes().
  TestKotlinExtractorVisibility: ExtractorVisibility#
  TestKotlinExtractorVisibility.parser: ExtractorVisibility#parser().
  TestKotlinExtractorVisibility.test_visibility_shapes: ExtractorVisibility#test_visibility_shapes().
  TestKotlinExtractorProperties: ExtractorProperties#
  TestKotlinExtractorProperties.parser: ExtractorProperties#parser().
  TestKotlinExtractorProperties.test_property_shapes: ExtractorProperties#test_property_shapes().
  TestKotlinExtractorImports: ExtractorImports#
  TestKotlinExtractorImports.parser: ExtractorImports#parser().
  TestKotlinExtractorImports.test_import_shapes: ExtractorImports#test_import_shapes().
  TestKotlinExtractorDocstrings: ExtractorDocstrings#
  TestKotlinExtractorDocstrings.parser: ExtractorDocstrings#parser().
  TestKotlinExtractorDocstrings.test_kdoc_shapes: ExtractorDocstrings#test_kdoc_shapes().
  TestKotlinExtractorErrorPaths: ExtractorErrorPaths#
  TestKotlinExtractorErrorPaths.parser: ExtractorErrorPaths#parser().
  TestKotlinExtractorErrorPaths.test_extract_with_malformed_declarations: ExtractorErrorPaths#test_extract_with_malformed_declarations().
  TestKotlinExtractorErrorPaths.test_node_text_extraction_edge_cases: ExtractorErrorPaths#test_node_text_extraction_edge_cases().
  TestKotlinExtractorErrorPaths.test_extract_function_with_exception: ExtractorErrorPaths#test_extract_function_with_exception().
  TestKotlinPluginEdgeCases: PluginEdgeCases#
  TestKotlinPluginEdgeCases.parser: PluginEdgeCases#parser().
  TestKotlinPluginEdgeCases.test_extract_elements_empty_or_whitespace_code: PluginEdgeCases#test_extract_elements_empty_or_whitespace_code().
  TestKotlinExtractorInternalMethods: ExtractorInternalMethods#
  TestKotlinExtractorInternalMethods.parser: ExtractorInternalMethods#parser().
  TestKotlinExtractorInternalMethods.test_class_shapes: ExtractorInternalMethods#test_class_shapes().
  TestKotlinTextExtractionEdgeCases: TextExtractionEdgeCases#
  TestKotlinTextExtractionEdgeCases.test_get_node_text_edge_cases: TextExtractionEdgeCases#test_get_node_text_edge_cases().
  TestKotlinExtractorExceptionPaths: ExtractorExceptionPaths#
  TestKotlinExtractorExceptionPaths.parser: ExtractorExceptionPaths#parser().
  TestKotlinExtractorExceptionPaths.test_extractors_return_none_on_error: ExtractorExceptionPaths#test_extractors_return_none_on_error().
  TestKotlinExtractorExceptionPaths.test_extract_import_unknown_name: ExtractorExceptionPaths#test_extract_import_unknown_name().
  TestKotlinExtractorExceptionPaths.test_extract_docstring: ExtractorExceptionPaths#test_extract_docstring().
---
# Module: [`tests/unit/languages/test_kotlin_coverage_boost.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_coverage_boost.py)

## Classes
### `TestKotlinExtractorDocstrings`
- def: [`tests/unit/languages/test_kotlin_coverage_boost.py:143`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_coverage_boost.py#L143)
- doc: Test docstring extraction.
- signature: `class TestKotlinExtractorDocstrings:`
- members:
  - `extractor(self)` — [`L147`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_coverage_boost.py#L147)
  - `parser(self)` — [`L151`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_coverage_boost.py#L151)
  - `test_kdoc_shapes(self, extractor, parser)` — [`L155`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_coverage_boost.py#L155) — Test function and class KDoc comments together.
- uses (calls/refs, reference-scoped): [`KotlinElementExtractor`](../../../tree_sitter_analyzer/languages/kotlin_plugin.md#KotlinElementExtractor)

### `TestKotlinExtractorErrorPaths`
- def: [`tests/unit/languages/test_kotlin_coverage_boost.py:179`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_coverage_boost.py#L179)
- doc: Test error handling paths.
- signature: `class TestKotlinExtractorErrorPaths:`
- members:
  - `extractor(self)` — [`L183`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_coverage_boost.py#L183)
  - `parser(self)` — [`L187`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_coverage_boost.py#L187)
  - `test_extract_function_with_exception(self, extractor, parser)` — [`L223`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_coverage_boost.py#L223) — Test function extraction with simulated error.
  - `test_extract_with_malformed_declarations(self, extractor, parser)` — [`L191`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_coverage_boost.py#L191) — Malformed declarations should return lists rather than crashing.
  - `test_node_text_extraction_edge_cases(self, extractor)` — [`L207`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_coverage_boost.py#L207) — Test node text extraction edge cases.
- uses (calls/refs, reference-scoped): [`KotlinElementExtractor`](../../../tree_sitter_analyzer/languages/kotlin_plugin.md#KotlinElementExtractor)

### `TestKotlinExtractorExceptionPaths`
- def: [`tests/unit/languages/test_kotlin_coverage_boost.py:378`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_coverage_boost.py#L378)
- doc: Test exception handling paths to boost coverage.
- signature: `class TestKotlinExtractorExceptionPaths:`
- members:
  - `extractor(self)` — [`L382`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_coverage_boost.py#L382)
  - `parser(self)` — [`L386`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_coverage_boost.py#L386)
  - `test_extract_docstring(self, extractor)` — [`L420`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_coverage_boost.py#L420) — Test docstring extraction.
  - `test_extract_import_unknown_name(self, extractor)` — [`L404`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_coverage_boost.py#L404) — Test import with unparseable name.
  - `test_extractors_return_none_on_error(self, extractor)` — [`L390`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_coverage_boost.py#L390) — Private extractors should return None on unexpected node errors.
- uses (calls/refs, reference-scoped): [`KotlinElementExtractor`](../../../tree_sitter_analyzer/languages/kotlin_plugin.md#KotlinElementExtractor)

### `TestKotlinExtractorImports`
- def: [`tests/unit/languages/test_kotlin_coverage_boost.py:119`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_coverage_boost.py#L119)
- doc: Test import extraction paths.
- signature: `class TestKotlinExtractorImports:`
- members:
  - `extractor(self)` — [`L123`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_coverage_boost.py#L123)
  - `parser(self)` — [`L127`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_coverage_boost.py#L127)
  - `test_import_shapes(self, extractor, parser)` — [`L131`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_coverage_boost.py#L131) — Test single, wildcard, and alias imports together.
- uses (calls/refs, reference-scoped): [`KotlinElementExtractor`](../../../tree_sitter_analyzer/languages/kotlin_plugin.md#KotlinElementExtractor)

### `TestKotlinExtractorInternalMethods`
- def: [`tests/unit/languages/test_kotlin_coverage_boost.py:257`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_coverage_boost.py#L257)
- doc: Test internal extractor methods.
- signature: `class TestKotlinExtractorInternalMethods:`
- members:
  - `extractor(self)` — [`L261`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_coverage_boost.py#L261)
  - `parser(self)` — [`L265`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_coverage_boost.py#L265)
  - `test_class_shapes(self, extractor, parser)` — [`L269`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_coverage_boost.py#L269) — Test class body, abstract, interface, inheritance, and object shapes.
- uses (calls/refs, reference-scoped): [`KotlinElementExtractor`](../../../tree_sitter_analyzer/languages/kotlin_plugin.md#KotlinElementExtractor)

### `TestKotlinExtractorParameters`
- def: [`tests/unit/languages/test_kotlin_coverage_boost.py:19`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_coverage_boost.py#L19)
- doc: Test parameter extraction paths.
- signature: `class TestKotlinExtractorParameters:`
- members:
  - `extractor(self)` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_coverage_boost.py#L23)
  - `parser(self)` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_coverage_boost.py#L27)
  - `test_function_parameter_shapes(self, extractor, parser)` — [`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_coverage_boost.py#L31) — Test representative parameter shapes in one parse.
- uses (calls/refs, reference-scoped): [`KotlinElementExtractor`](../../../tree_sitter_analyzer/languages/kotlin_plugin.md#KotlinElementExtractor)

### `TestKotlinExtractorProperties`
- def: [`tests/unit/languages/test_kotlin_coverage_boost.py:87`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_coverage_boost.py#L87)
- doc: Test property extraction paths.
- signature: `class TestKotlinExtractorProperties:`
- members:
  - `extractor(self)` — [`L91`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_coverage_boost.py#L91)
  - `parser(self)` — [`L95`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_coverage_boost.py#L95)
  - `test_property_shapes(self, extractor, parser)` — [`L99`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_coverage_boost.py#L99) — Test getter/setter, lateinit, and const property shapes together.
- uses (calls/refs, reference-scoped): [`KotlinElementExtractor`](../../../tree_sitter_analyzer/languages/kotlin_plugin.md#KotlinElementExtractor)

### `TestKotlinExtractorVisibility`
- def: [`tests/unit/languages/test_kotlin_coverage_boost.py:57`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_coverage_boost.py#L57)
- doc: Test visibility modifier extraction.
- signature: `class TestKotlinExtractorVisibility:`
- members:
  - `extractor(self)` — [`L61`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_coverage_boost.py#L61)
  - `parser(self)` — [`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_coverage_boost.py#L65)
  - `test_visibility_shapes(self, extractor, parser)` — [`L69`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_coverage_boost.py#L69) — Test protected/internal/private visibility shapes in one parse.
- uses (calls/refs, reference-scoped): [`KotlinElementExtractor`](../../../tree_sitter_analyzer/languages/kotlin_plugin.md#KotlinElementExtractor)

### `TestKotlinPluginEdgeCases`
- def: [`tests/unit/languages/test_kotlin_coverage_boost.py:235`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_coverage_boost.py#L235)
- doc: Test KotlinPlugin edge cases.
- signature: `class TestKotlinPluginEdgeCases:`
- members:
  - `parser(self)` — [`L243`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_coverage_boost.py#L243)
  - `plugin(self)` — [`L239`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_coverage_boost.py#L239)
  - `test_extract_elements_empty_or_whitespace_code(self, plugin, parser)` — [`L247`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_coverage_boost.py#L247) — Empty and whitespace-only code should return an element dict.
- uses (calls/refs, reference-scoped): [`KotlinPlugin`](../../../tree_sitter_analyzer/languages/kotlin_plugin.md#KotlinPlugin)

### `TestKotlinTextExtractionEdgeCases`
- def: [`tests/unit/languages/test_kotlin_coverage_boost.py:322`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_coverage_boost.py#L322)
- doc: Test text extraction edge cases.
- signature: `class TestKotlinTextExtractionEdgeCases:`
- members:
  - `extractor(self)` — [`L326`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_coverage_boost.py#L326)
  - `test_get_node_text_edge_cases(self, extractor)` — [`L329`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_coverage_boost.py#L329) — Test cached, multiline, and out-of-bounds text extraction.
- uses (calls/refs, reference-scoped): [`KotlinElementExtractor`](../../../tree_sitter_analyzer/languages/kotlin_plugin.md#KotlinElementExtractor)

