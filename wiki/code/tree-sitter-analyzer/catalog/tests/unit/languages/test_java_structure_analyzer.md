---
title: 'Module: tests/unit/languages/test_java_structure_analyzer.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_java_structure_analyzer.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_java_structure_analyzer`/
symbols:
  test_complex_structure_analysis: test_complex_structure_analysis().
  test_output_schema_validation: test_output_schema_validation().
  test_cli_structure_option_with_sample_file: test_cli_structure_option_with_sample_file().
  test_cli_structure_option_json_format: test_cli_structure_option_json_format().
  analyzer: analyzer().
  test_cli_structure_option_text_format: test_cli_structure_option_text_format().
  _extract_json_from_cli_output: _extract_json_from_cli_output().
  _verify_package_fallback: _verify_package_fallback().
  _verify_imports_fallback: _verify_imports_fallback().
  _verify_classes_fallback: _verify_classes_fallback().
  _verify_methods_fallback: _verify_methods_fallback().
  _verify_fields_fallback: _verify_fields_fallback().
  _verify_annotations_fallback: _verify_annotations_fallback().
  _assert_package_schema: _assert_package_schema().
  _assert_import_schema: _assert_import_schema().
  _assert_class_schema: _assert_class_schema().
  _assert_method_schema: _assert_method_schema().
  _assert_field_schema: _assert_field_schema().
  _assert_annotation_schema: _assert_annotation_schema().
  sample_java_path: sample_java_path().
  simple_java_code: simple_java_code().
  test_analyze_structure_method_unit_test: test_analyze_structure_method_unit_test().
  test_empty_java_file: test_empty_java_file().
  test_nonexistent_file_handling: test_nonexistent_file_handling().
---
# Module: [`tests/unit/languages/test_java_structure_analyzer.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_structure_analyzer.py)

## Functions
- `_assert_annotation_schema(ann: dict)` — [`L567`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_structure_analyzer.py#L567)
- `_assert_class_schema(cls: dict)` — [`L492`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_structure_analyzer.py#L492)
- `_assert_field_schema(field: dict)` — [`L548`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_structure_analyzer.py#L548)
- `_assert_import_schema(imp: dict)` — [`L483`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_structure_analyzer.py#L483)
- `_assert_method_schema(method: dict)` — [`L516`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_structure_analyzer.py#L516)
- `_assert_package_schema(package: dict)` — [`L476`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_structure_analyzer.py#L476)
- `_extract_json_from_cli_output(output)` — [`L80`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_structure_analyzer.py#L80) — CLI出力からJSON部分を抽出するヘルパーメソッド
- `_verify_annotations_fallback(annotations: list, code: str)` — [`L353`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_structure_analyzer.py#L353)
- `_verify_classes_fallback(classes: list, code: str)` — [`L296`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_structure_analyzer.py#L296)
- `_verify_fields_fallback(fields: list, code: str)` — [`L341`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_structure_analyzer.py#L341)
- `_verify_imports_fallback(imports: list, code: str)` — [`L280`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_structure_analyzer.py#L280)
- `_verify_methods_fallback(methods: list, code: str)` — [`L323`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_structure_analyzer.py#L323)
- `_verify_package_fallback(package_info: dict | None, code: str)` — [`L269`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_structure_analyzer.py#L269)
- `analyzer()` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_structure_analyzer.py#L29) — テスト用のAnalyzerインスタンスを提供するfixture
- `sample_java_path()` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_structure_analyzer.py#L35) — サンプルJavaファイルのパスを提供するfixture
- `simple_java_code()` — [`L41`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_structure_analyzer.py#L41) — テスト用の簡単なJavaコードを提供するfixture
- `test_analyze_structure_method_unit_test(analyzer, simple_java_code)` — [`L177`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_structure_analyzer.py#L177) — analyze_structureメソッドの単体テスト
- `test_cli_structure_option_json_format(mocker, simple_java_code)` — [`L127`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_structure_analyzer.py#L127) — CLIの--structureオプションでJSON形式出力をテスト
- `test_cli_structure_option_text_format(mocker, simple_java_code)` — [`L613`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_structure_analyzer.py#L613) — CLIの--structureオプションでテキスト形式出力をテスト
- `test_cli_structure_option_with_sample_file(mocker, sample_java_path)` — [`L102`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_structure_analyzer.py#L102) — CLIの--structureオプションでSample.javaを解析するテスト
- `test_complex_structure_analysis(analyzer)` — [`L368`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_structure_analyzer.py#L368) — Test complex Java file structure analysis
- `test_empty_java_file(analyzer)` — [`L241`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_structure_analyzer.py#L241) — 空のJavaファイルのテスト
- `test_nonexistent_file_handling(analyzer)` — [`L604`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_structure_analyzer.py#L604) — 存在しないファイルの処理テスト
- `test_output_schema_validation(analyzer, simple_java_code)` — [`L575`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_structure_analyzer.py#L575) — 出力スキーマの詳細検証

