---
title: 'Module: tests/unit/languages/test_plugin_encoding_propagation.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_plugin_encoding_propagation.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_plugin_encoding_propagation`/
symbols:
  TestJavaPluginEncodingPropagation.test_analyze_file_sets_extractor_file_encoding: TestJavaPluginEncodingPropagation#test_analyze_file_sets_extractor_file_encoding().
  TestCPluginEncodingPropagation.test_analyze_file_sets_extractor_file_encoding: TestCPluginEncodingPropagation#test_analyze_file_sets_extractor_file_encoding().
  TestCPluginEncodingPropagation.test_analyze_file_propagates_utf8_encoding: TestCPluginEncodingPropagation#test_analyze_file_propagates_utf8_encoding().
  TestJavaPluginEncodingPropagation.test_analyze_file_propagates_utf8_encoding: TestJavaPluginEncodingPropagation#test_analyze_file_propagates_utf8_encoding().
  _RecordingCExtractor: _RecordingCExtractor#
  _RecordingJavaExtractor: _RecordingJavaExtractor#
  _RecordingExtractorMixin.seen_encoding: _RecordingExtractorMixin#seen_encoding.
  _RecordingExtractorMixin: _RecordingExtractorMixin#
  TestExtractorEncodingAttribute.test_c_extractor_default_none: TestExtractorEncodingAttribute#test_c_extractor_default_none().
  TestExtractorEncodingAttribute.test_java_extractor_default_none: TestExtractorEncodingAttribute#test_java_extractor_default_none().
  TestExtractorEncodingAttribute.test_c_extractor_accepts_encoding: TestExtractorEncodingAttribute#test_c_extractor_accepts_encoding().
  TestExtractorEncodingAttribute.test_java_extractor_accepts_encoding: TestExtractorEncodingAttribute#test_java_extractor_accepts_encoding().
  _RecordingExtractorMixin.extract_functions: _RecordingExtractorMixin#extract_functions().
  TestPhpRubyNoDeadEncodingAttr.test_php_extractor_has_no_file_encoding_attr: TestPhpRubyNoDeadEncodingAttr#test_php_extractor_has_no_file_encoding_attr().
  TestPhpRubyNoDeadEncodingAttr.test_ruby_extractor_has_no_file_encoding_attr: TestPhpRubyNoDeadEncodingAttr#test_ruby_extractor_has_no_file_encoding_attr().
  TestJavaPluginEncodingPropagation._fake_read: TestJavaPluginEncodingPropagation#_fake_read().
  TestExtractorEncodingAttribute: TestExtractorEncodingAttribute#
  _RecordingExtractorMixin.extract_classes: _RecordingExtractorMixin#extract_classes().
  _RecordingExtractorMixin.extract_variables: _RecordingExtractorMixin#extract_variables().
  _RecordingExtractorMixin.extract_imports: _RecordingExtractorMixin#extract_imports().
  c_source_file: c_source_file().
  java_source_file: java_source_file().
  TestCPluginEncodingPropagation: TestCPluginEncodingPropagation#
  TestJavaPluginEncodingPropagation: TestJavaPluginEncodingPropagation#
  TestPhpRubyNoDeadEncodingAttr: TestPhpRubyNoDeadEncodingAttr#
---
# Module: [`tests/unit/languages/test_plugin_encoding_propagation.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugin_encoding_propagation.py)

## Classes
### `TestCPluginEncodingPropagation`
- def: [`tests/unit/languages/test_plugin_encoding_propagation.py:116`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugin_encoding_propagation.py#L116)
- signature: `class TestCPluginEncodingPropagation:`
- members:
  - `test_analyze_file_propagates_utf8_encoding(self, monkeypatch: pytest.MonkeyPatch, c_source_file: Path)` — [`L147`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugin_encoding_propagation.py#L147) — Even for the default utf-8 path the attribute must be set, not left None.
  - `test_analyze_file_sets_extractor_file_encoding(self, monkeypatch: pytest.MonkeyPatch, c_source_file: Path)` — [`L117`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugin_encoding_propagation.py#L117) — KI-1 regression: extractor._file_encoding must be set before extract calls.
- uses (calls/refs, reference-scoped): [`AnalysisRequest`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest), [`file_path`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest.file_path), [`language`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest.language), [`analyze_file`](../../../tree_sitter_analyzer/languages/c_plugin.md#CPlugin.analyze_file), [`include_complexity`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest.include_complexity), [`include_details`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest.include_details), [`CPlugin`](../../../tree_sitter_analyzer/languages/c_plugin.md#CPlugin)  (2 test-only)

### `TestExtractorEncodingAttribute`
- def: [`tests/unit/languages/test_plugin_encoding_propagation.py:31`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugin_encoding_propagation.py#L31)
- doc: C and Java extractors declare _file_encoding for byte-level slicing.
- signature: `class TestExtractorEncodingAttribute:`
- members:
  - `test_c_extractor_accepts_encoding(self)` — [`L44`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugin_encoding_propagation.py#L44)
  - `test_c_extractor_default_none(self)` — [`L34`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugin_encoding_propagation.py#L34)
  - `test_java_extractor_accepts_encoding(self)` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugin_encoding_propagation.py#L49)
  - `test_java_extractor_default_none(self)` — [`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugin_encoding_propagation.py#L39)
- uses (calls/refs, reference-scoped): [`JavaElementExtractor`](../../../tree_sitter_analyzer/languages/java_plugin.md#JavaElementExtractor), [`CElementExtractor`](../../../tree_sitter_analyzer/languages/c_plugin.md#CElementExtractor), [`_file_encoding`](../../../tree_sitter_analyzer/languages/c_plugin.md#CElementExtractor._file_encoding), [`_file_encoding`](../../../tree_sitter_analyzer/languages/java_plugin.md#JavaElementExtractor._file_encoding)

### `TestJavaPluginEncodingPropagation`
- def: [`tests/unit/languages/test_plugin_encoding_propagation.py:167`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugin_encoding_propagation.py#L167)
- signature: `class TestJavaPluginEncodingPropagation:`
- members:
  - `test_analyze_file_propagates_utf8_encoding(self, monkeypatch: pytest.MonkeyPatch, java_source_file: Path)` — [`L198`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugin_encoding_propagation.py#L198)
  - `test_analyze_file_sets_extractor_file_encoding(self, monkeypatch: pytest.MonkeyPatch, java_source_file: Path)` — [`L168`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugin_encoding_propagation.py#L168) — KI-1 regression for Java: extractor._file_encoding must be set.
- protocol/private: `_fake_read`[`L180`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugin_encoding_propagation.py#L180)
- uses (calls/refs, reference-scoped): [`AnalysisRequest`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest), [`file_path`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest.file_path), [`language`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest.language), [`include_complexity`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest.include_complexity), [`include_details`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest.include_details), [`analyze_file`](../../../tree_sitter_analyzer/languages/java_plugin.md#JavaPlugin.analyze_file), [`JavaPlugin`](../../../tree_sitter_analyzer/languages/java_plugin.md#JavaPlugin)  (2 test-only)

### `TestPhpRubyNoDeadEncodingAttr`
- def: [`tests/unit/languages/test_plugin_encoding_propagation.py:224`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugin_encoding_propagation.py#L224)
- doc: KI-2 regression: PHP/Ruby extractors had a dead _file_encoding declaration
- signature: `class TestPhpRubyNoDeadEncodingAttr:`
- members:
  - `test_php_extractor_has_no_file_encoding_attr(self)` — [`L229`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugin_encoding_propagation.py#L229)
  - `test_ruby_extractor_has_no_file_encoding_attr(self)` — [`L236`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugin_encoding_propagation.py#L236)
- uses (calls/refs, reference-scoped): [`PHPElementExtractor`](../../../tree_sitter_analyzer/languages/php_plugin.md#PHPElementExtractor), [`RubyElementExtractor`](../../../tree_sitter_analyzer/languages/ruby_plugin.md#RubyElementExtractor)

### `_RecordingCExtractor`  ·  implements/extends CElementExtractor, _RecordingExtractorMixin
- def: [`tests/unit/languages/test_plugin_encoding_propagation.py:84`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugin_encoding_propagation.py#L84)
- signature: `class _RecordingCExtractor(_RecordingExtractorMixin, CElementExtractor):`
- uses (calls/refs, reference-scoped): [`CElementExtractor`](../../../tree_sitter_analyzer/languages/c_plugin.md#CElementExtractor)  (1 test-only)
- used by: [`CElementExtractor`](../../../tree_sitter_analyzer/languages/c_plugin.md#CElementExtractor)  (3 test-only)

### `_RecordingExtractorMixin`
- def: [`tests/unit/languages/test_plugin_encoding_propagation.py:60`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugin_encoding_propagation.py#L60)
- doc: Mixin that records _file_encoding at the moment extract_* is called.
- signature: `class _RecordingExtractorMixin:`
- members:
  - `extract_classes(self, tree, source_code)` — [`L74`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugin_encoding_propagation.py#L74)
  - `extract_functions(self, tree, source_code)` — [`L70`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugin_encoding_propagation.py#L70)
  - `extract_imports(self, tree, source_code)` — [`L80`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugin_encoding_propagation.py#L80)
  - `extract_variables(self, tree, source_code)` — [`L77`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugin_encoding_propagation.py#L77)
  - `seen_encoding` — [`L68`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugin_encoding_propagation.py#L68)
- uses (calls/refs, reference-scoped): (2 test-only callers)
- used by: (6 test-only callers)

### `_RecordingJavaExtractor`  ·  implements/extends JavaElementExtractor, _RecordingExtractorMixin
- def: [`tests/unit/languages/test_plugin_encoding_propagation.py:88`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugin_encoding_propagation.py#L88)
- signature: `class _RecordingJavaExtractor(_RecordingExtractorMixin, JavaElementExtractor):`
- uses (calls/refs, reference-scoped): [`JavaElementExtractor`](../../../tree_sitter_analyzer/languages/java_plugin.md#JavaElementExtractor)  (1 test-only)
- used by: [`JavaElementExtractor`](../../../tree_sitter_analyzer/languages/java_plugin.md#JavaElementExtractor)  (3 test-only)

## Functions
- `c_source_file(tmp_path: Path)` — [`L93`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugin_encoding_propagation.py#L93)
- `java_source_file(tmp_path: Path)` — [`L103`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_plugin_encoding_propagation.py#L103)

