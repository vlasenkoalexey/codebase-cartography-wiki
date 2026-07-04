---
title: 'Module: tests/property/test_language_detection_properties.py'
type: catalog
provenance: extracted
module: tests/property/test_language_detection_properties.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.property.test_language_detection_properties`/
symbols:
  detector: detector.
  LanguageDetectionStatefulMachine.detect_language_for_file: LanguageDetectionStatefulMachine#detect_language_for_file().
  TestLanguageDetectionProperties.test_python_extension_detection: TestLanguageDetectionProperties#test_python_extension_detection().
  TestLanguageDetectionProperties.test_java_extension_detection: TestLanguageDetectionProperties#test_java_extension_detection().
  TestLanguageDetectionProperties.test_javascript_extension_detection: TestLanguageDetectionProperties#test_javascript_extension_detection().
  TestLanguageDetectionProperties.test_typescript_extension_detection: TestLanguageDetectionProperties#test_typescript_extension_detection().
  TestLanguageDetectionProperties.test_go_extension_detection: TestLanguageDetectionProperties#test_go_extension_detection().
  TestLanguageDetectionProperties.test_rust_extension_detection: TestLanguageDetectionProperties#test_rust_extension_detection().
  TestLanguageDetectionProperties.test_csharp_extension_detection: TestLanguageDetectionProperties#test_csharp_extension_detection().
  TestLanguageDetectionProperties.test_css_extension_detection: TestLanguageDetectionProperties#test_css_extension_detection().
  TestLanguageDetectionProperties.test_html_extension_detection: TestLanguageDetectionProperties#test_html_extension_detection().
  TestLanguageDetectionProperties.test_yaml_extension_detection: TestLanguageDetectionProperties#test_yaml_extension_detection().
  TestLanguageDetectionProperties.test_yml_extension_detection: TestLanguageDetectionProperties#test_yml_extension_detection().
  TestLanguageDetectionProperties.test_sql_extension_detection: TestLanguageDetectionProperties#test_sql_extension_detection().
  TestLanguageDetectionProperties.test_unknown_extension_detection: TestLanguageDetectionProperties#test_unknown_extension_detection().
  TestLanguageDetectionProperties.test_no_extension_detection: TestLanguageDetectionProperties#test_no_extension_detection().
  TestLanguageDetectionProperties.test_detection_idempotency: TestLanguageDetectionProperties#test_detection_idempotency().
  TestLanguageDetectionProperties.test_same_extension_same_language: TestLanguageDetectionProperties#test_same_extension_same_language().
  TestLanguageDetectionProperties.test_multiple_extensions_detection: TestLanguageDetectionProperties#test_multiple_extensions_detection().
  TestLanguageDetectionEdgeCases.test_empty_filename: TestLanguageDetectionEdgeCases#test_empty_filename().
  TestLanguageDetectionEdgeCases.test_dotfile: TestLanguageDetectionEdgeCases#test_dotfile().
  TestLanguageDetectionEdgeCases.test_multiple_dots: TestLanguageDetectionEdgeCases#test_multiple_dots().
  TestLanguageDetectionEdgeCases.test_uppercase_extension: TestLanguageDetectionEdgeCases#test_uppercase_extension().
  TestLanguageDetectionEdgeCases.test_mixed_case_extension: TestLanguageDetectionEdgeCases#test_mixed_case_extension().
  TestLanguageDetectionEdgeCases.test_extension_with_numbers: TestLanguageDetectionEdgeCases#test_extension_with_numbers().
  LanguageDetectionStatefulMachine.detected_languages: LanguageDetectionStatefulMachine#detected_languages.
  LanguageDetectionStatefulMachine.all_detections_are_valid: LanguageDetectionStatefulMachine#all_detections_are_valid().
  LanguageDetectionStatefulMachine.same_extension_same_language: LanguageDetectionStatefulMachine#same_extension_same_language().
  LanguageDetectionStatefulMachine: LanguageDetectionStatefulMachine#
  TestLanguageDetectionProperties: TestLanguageDetectionProperties#
  LanguageDetectionStatefulMachine.__init__: LanguageDetectionStatefulMachine#__init__().
  TestLanguageDetectionEdgeCases: TestLanguageDetectionEdgeCases#
---
# Module: [`tests/property/test_language_detection_properties.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_language_detection_properties.py)

## Classes
### `LanguageDetectionStatefulMachine`
- def: [`tests/property/test_language_detection_properties.py:386`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_language_detection_properties.py#L386)
- doc: 语言检测状态机测试。
- signature: `class LanguageDetectionStatefulMachine(RuleBasedStateMachine):`
- members:
  - `all_detections_are_valid(self)` — [`L427`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_language_detection_properties.py#L427) — 验证所有检测结果都是有效的。
  - `detect_language_for_file(self, file_name: str, extension: str)` — [`L415`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_language_detection_properties.py#L415) — 为文件检测语言。
  - `same_extension_same_language(self)` — [`L435`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_language_detection_properties.py#L435) — 验证相同扩展名返回相同语言。
  - `detected_languages` — [`L391`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_language_detection_properties.py#L391)
- protocol/private: `__init__`[`L389`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_language_detection_properties.py#L389)
- uses (calls/refs, reference-scoped): [`detect_from_extension`](../../tree_sitter_analyzer/language_detector.md#LanguageDetector.detect_from_extension)  (1 test-only)

### `TestLanguageDetectionEdgeCases`
- def: [`tests/property/test_language_detection_properties.py:451`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_language_detection_properties.py#L451)
- doc: 语言检测边界情况测试。
- signature: `class TestLanguageDetectionEdgeCases:`
- members:
  - `test_dotfile(self)` — [`L460`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_language_detection_properties.py#L460) — 测试点文件。
  - `test_empty_filename(self)` — [`L454`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_language_detection_properties.py#L454) — 测试空文件名。
  - `test_extension_with_numbers(self)` — [`L486`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_language_detection_properties.py#L486) — 测试带数字的扩展名。
  - `test_mixed_case_extension(self)` — [`L479`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_language_detection_properties.py#L479) — 测试混合大小写扩展名。
  - `test_multiple_dots(self)` — [`L466`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_language_detection_properties.py#L466) — 测试多个点。
  - `test_uppercase_extension(self)` — [`L472`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_language_detection_properties.py#L472) — 测试大写扩展名。
- uses (calls/refs, reference-scoped): [`detect_from_extension`](../../tree_sitter_analyzer/language_detector.md#LanguageDetector.detect_from_extension)  (1 test-only)

### `TestLanguageDetectionProperties`
- def: [`tests/property/test_language_detection_properties.py:18`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_language_detection_properties.py#L18)
- doc: 语言检测属性测试类。
- signature: `class TestLanguageDetectionProperties:`
- members:
  - `test_csharp_extension_detection(self, file_path: Path)` — [`L144`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_language_detection_properties.py#L144) — 测试C#扩展名检测的属性。
  - `test_css_extension_detection(self, file_path: Path)` — [`L163`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_language_detection_properties.py#L163) — 测试CSS扩展名检测的属性。
  - `test_detection_idempotency(self, file_path: Path)` — [`L302`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_language_detection_properties.py#L302) — 测试语言检测的幂等性。
  - `test_go_extension_detection(self, file_path: Path)` — [`L106`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_language_detection_properties.py#L106) — 测试Go扩展名检测的属性。
  - `test_html_extension_detection(self, file_path: Path)` — [`L182`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_language_detection_properties.py#L182) — 测试HTML扩展名检测的属性。
  - `test_java_extension_detection(self, file_path: Path)` — [`L49`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_language_detection_properties.py#L49) — 测试Java扩展名检测的属性。
  - `test_javascript_extension_detection(self, file_path: Path)` — [`L68`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_language_detection_properties.py#L68) — 测试JavaScript扩展名检测的属性。
  - `test_multiple_extensions_detection(self, extensions: list[str])` — [`L367`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_language_detection_properties.py#L367) — 测试多个扩展名检测的属性。
  - `test_no_extension_detection(self, file_path: Path)` — [`L278`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_language_detection_properties.py#L278) — 测试无扩展名检测的属性。
  - `test_python_extension_detection(self, file_path: Path)` — [`L29`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_language_detection_properties.py#L29) — 测试Python扩展名检测的属性。
  - `test_rust_extension_detection(self, file_path: Path)` — [`L125`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_language_detection_properties.py#L125) — 测试Rust扩展名检测的属性。
  - `test_same_extension_same_language(self, file_path1: Path, file_path2: Path)` — [`L329`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_language_detection_properties.py#L329) — 测试相同扩展名返回相同语言的属性。
  - `test_sql_extension_detection(self, file_path: Path)` — [`L239`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_language_detection_properties.py#L239) — 测试SQL扩展名检测的属性。
  - `test_typescript_extension_detection(self, file_path: Path)` — [`L87`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_language_detection_properties.py#L87) — 测试TypeScript扩展名检测的属性。
  - `test_unknown_extension_detection(self, file_path: Path)` — [`L258`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_language_detection_properties.py#L258) — 测试未知扩展名检测的属性。
  - `test_yaml_extension_detection(self, file_path: Path)` — [`L201`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_language_detection_properties.py#L201) — 测试YAML扩展名检测的属性。
  - `test_yml_extension_detection(self, file_path: Path)` — [`L220`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_language_detection_properties.py#L220) — 测试.yml扩展名检测的属性。
- uses (calls/refs, reference-scoped): [`detect_from_extension`](../../tree_sitter_analyzer/language_detector.md#LanguageDetector.detect_from_extension)  (1 test-only)

## Module values
- `detector` — [`L15`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_language_detection_properties.py#L15)

