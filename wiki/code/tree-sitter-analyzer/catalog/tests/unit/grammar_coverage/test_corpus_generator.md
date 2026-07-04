---
title: 'Module: tests/unit/grammar_coverage/test_corpus_generator.py'
type: catalog
provenance: extracted
module: tests/unit/grammar_coverage/test_corpus_generator.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.grammar_coverage.test_corpus_generator`/Test
symbols:
  TestCorpusValidation.test_all_python_templates_valid: CorpusValidation#test_all_python_templates_valid().
  TestCorpusValidation.test_all_javascript_templates_valid: CorpusValidation#test_all_javascript_templates_valid().
  TestCorpusValidation.test_all_java_templates_valid: CorpusValidation#test_all_java_templates_valid().
  TestGenerateMinimalCode.test_python_function_definition: GenerateMinimalCode#test_python_function_definition().
  TestGenerateMinimalCode.test_python_class_definition: GenerateMinimalCode#test_python_class_definition().
  TestGenerateMinimalCode.test_python_if_statement: GenerateMinimalCode#test_python_if_statement().
  TestGenerateMinimalCode.test_javascript_function_declaration: GenerateMinimalCode#test_javascript_function_declaration().
  TestGenerateMinimalCode.test_javascript_arrow_function: GenerateMinimalCode#test_javascript_arrow_function().
  TestGenerateMinimalCode.test_java_class_declaration: GenerateMinimalCode#test_java_class_declaration().
  TestGenerateMinimalCode.test_java_method_declaration: GenerateMinimalCode#test_java_method_declaration().
  TestGenerateMinimalCode.test_unsupported_language: GenerateMinimalCode#test_unsupported_language().
  TestGenerateMinimalCode.test_unsupported_node_type: GenerateMinimalCode#test_unsupported_node_type().
  TestValidateGeneratedCode.test_valid_python_code: ValidateGeneratedCode#test_valid_python_code().
  TestValidateGeneratedCode.test_valid_javascript_code: ValidateGeneratedCode#test_valid_javascript_code().
  TestValidateGeneratedCode.test_valid_java_code: ValidateGeneratedCode#test_valid_java_code().
  TestValidateGeneratedCode.test_invalid_python_code: ValidateGeneratedCode#test_invalid_python_code().
  TestValidateGeneratedCode.test_invalid_javascript_code: ValidateGeneratedCode#test_invalid_javascript_code().
  TestValidateGeneratedCode.test_unsupported_language_validation: ValidateGeneratedCode#test_unsupported_language_validation().
  TestGenerateCorpusByCategory.test_python_corpus_structure: GenerateCorpusByCategory#test_python_corpus_structure().
  TestGenerateCorpusByCategory.test_python_corpus_file_extensions: GenerateCorpusByCategory#test_python_corpus_file_extensions().
  TestGenerateCorpusByCategory.test_python_corpus_content: GenerateCorpusByCategory#test_python_corpus_content().
  TestGenerateCorpusByCategory.test_javascript_corpus_structure: GenerateCorpusByCategory#test_javascript_corpus_structure().
  TestGenerateCorpusByCategory.test_javascript_corpus_file_extensions: GenerateCorpusByCategory#test_javascript_corpus_file_extensions().
  TestGenerateCorpusByCategory.test_java_corpus_structure: GenerateCorpusByCategory#test_java_corpus_structure().
  TestGenerateCorpusByCategory.test_java_corpus_file_extensions: GenerateCorpusByCategory#test_java_corpus_file_extensions().
  TestGenerateCorpusByCategory.test_unsupported_language_corpus: GenerateCorpusByCategory#test_unsupported_language_corpus().
  TestSaveCorpusFiles.test_save_python_corpus: SaveCorpusFiles#test_save_python_corpus().
  TestSaveCorpusFiles.test_save_multiple_files: SaveCorpusFiles#test_save_multiple_files().
  TestSaveCorpusFiles.test_create_nested_directories: SaveCorpusFiles#test_create_nested_directories().
  TestSaveCorpusFiles.test_utf8_encoding: SaveCorpusFiles#test_utf8_encoding().
  TestGenerateAndSaveCorpus.test_python_end_to_end: GenerateAndSaveCorpus#test_python_end_to_end().
  TestGenerateAndSaveCorpus.test_javascript_end_to_end: GenerateAndSaveCorpus#test_javascript_end_to_end().
  TestGenerateAndSaveCorpus.test_java_end_to_end: GenerateAndSaveCorpus#test_java_end_to_end().
  TestGenerateAndSaveCorpus.test_without_validation: GenerateAndSaveCorpus#test_without_validation().
  TestGenerateAndSaveCorpus.test_unsupported_language_end_to_end: GenerateAndSaveCorpus#test_unsupported_language_end_to_end().
  TestGenerateMinimalCode: GenerateMinimalCode#
  TestValidateGeneratedCode: ValidateGeneratedCode#
  TestGenerateCorpusByCategory: GenerateCorpusByCategory#
  TestSaveCorpusFiles: SaveCorpusFiles#
  TestGenerateAndSaveCorpus: GenerateAndSaveCorpus#
  TestCorpusValidation: CorpusValidation#
---
# Module: [`tests/unit/grammar_coverage/test_corpus_generator.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_corpus_generator.py)

## Classes
### `TestCorpusValidation`
- def: [`tests/unit/grammar_coverage/test_corpus_generator.py:281`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_corpus_generator.py#L281)
- doc: 测试生成的语料库可被 tree-sitter 成功解析
- signature: `class TestCorpusValidation:`
- members:
  - `test_all_java_templates_valid(self)` — [`L311`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_corpus_generator.py#L311) — 测试所有 Java 模板都是有效的
  - `test_all_javascript_templates_valid(self)` — [`L298`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_corpus_generator.py#L298) — 测试所有 JavaScript 模板都是有效的
  - `test_all_python_templates_valid(self)` — [`L284`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_corpus_generator.py#L284) — 测试所有 Python 模板都是有效的
- uses (calls/refs, reference-scoped): [`generate_corpus_by_category`](../../../tree_sitter_analyzer/grammar_coverage/corpus_generator.md#generate_corpus_by_category), [`validate_generated_code`](../../../tree_sitter_analyzer/grammar_coverage/corpus_generator.md#validate_generated_code)

### `TestGenerateAndSaveCorpus`
- def: [`tests/unit/grammar_coverage/test_corpus_generator.py:224`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_corpus_generator.py#L224)
- doc: 测试完整的生成和保存流程
- signature: `class TestGenerateAndSaveCorpus:`
- members:
  - `test_java_end_to_end(self)` — [`L249`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_corpus_generator.py#L249) — 测试 Java 端到端流程
  - `test_javascript_end_to_end(self)` — [`L238`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_corpus_generator.py#L238) — 测试 JavaScript 端到端流程
  - `test_python_end_to_end(self)` — [`L227`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_corpus_generator.py#L227) — 测试 Python 端到端流程
  - `test_unsupported_language_end_to_end(self)` — [`L270`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_corpus_generator.py#L270) — 测试不支持的语言端到端流程
  - `test_without_validation(self)` — [`L260`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_corpus_generator.py#L260) — 测试跳过验证的情况
- uses (calls/refs, reference-scoped): [`generate_and_save_corpus`](../../../tree_sitter_analyzer/grammar_coverage/corpus_generator.md#generate_and_save_corpus)

### `TestGenerateCorpusByCategory`
- def: [`tests/unit/grammar_coverage/test_corpus_generator.py:120`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_corpus_generator.py#L120)
- doc: 测试按分类生成语料库
- signature: `class TestGenerateCorpusByCategory:`
- members:
  - `test_java_corpus_file_extensions(self)` — [`L166`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_corpus_generator.py#L166) — 测试 Java 语料库文件扩展名
  - `test_java_corpus_structure(self)` — [`L160`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_corpus_generator.py#L160) — 测试 Java 语料库结构
  - `test_javascript_corpus_file_extensions(self)` — [`L154`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_corpus_generator.py#L154) — 测试 JavaScript 语料库文件扩展名
  - `test_javascript_corpus_structure(self)` — [`L147`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_corpus_generator.py#L147) — 测试 JavaScript 语料库结构
  - `test_python_corpus_content(self)` — [`L138`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_corpus_generator.py#L138) — 测试 Python 语料库内容包含节点类型注释
  - `test_python_corpus_file_extensions(self)` — [`L132`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_corpus_generator.py#L132) — 测试 Python 语料库文件扩展名
  - `test_python_corpus_structure(self)` — [`L123`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_corpus_generator.py#L123) — 测试 Python 语料库结构
  - `test_unsupported_language_corpus(self)` — [`L172`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_corpus_generator.py#L172) — 测试不支持的语言返回空字典
- uses (calls/refs, reference-scoped): [`generate_corpus_by_category`](../../../tree_sitter_analyzer/grammar_coverage/corpus_generator.md#generate_corpus_by_category)

### `TestGenerateMinimalCode`
- def: [`tests/unit/grammar_coverage/test_corpus_generator.py:21`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_corpus_generator.py#L21)
- doc: 测试最小化代码生成
- signature: `class TestGenerateMinimalCode:`
- members:
  - `test_java_class_declaration(self)` — [`L61`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_corpus_generator.py#L61) — 测试 Java class_declaration 生成
  - `test_java_method_declaration(self)` — [`L68`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_corpus_generator.py#L68) — 测试 Java method_declaration 生成
  - `test_javascript_arrow_function(self)` — [`L54`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_corpus_generator.py#L54) — 测试 JavaScript arrow_function 生成
  - `test_javascript_function_declaration(self)` — [`L47`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_corpus_generator.py#L47) — 测试 JavaScript function_declaration 生成
  - `test_python_class_definition(self)` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_corpus_generator.py#L32) — 测试 Python class_definition 生成
  - `test_python_function_definition(self)` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_corpus_generator.py#L24) — 测试 Python function_definition 生成
  - `test_python_if_statement(self)` — [`L40`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_corpus_generator.py#L40) — 测试 Python if_statement 生成
  - `test_unsupported_language(self)` — [`L75`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_corpus_generator.py#L75) — 测试不支持的语言返回空字符串
  - `test_unsupported_node_type(self)` — [`L80`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_corpus_generator.py#L80) — 测试不支持的节点类型返回空字符串
- uses (calls/refs, reference-scoped): [`generate_minimal_code_for_node_type`](../../../tree_sitter_analyzer/grammar_coverage/corpus_generator.md#generate_minimal_code_for_node_type)

### `TestSaveCorpusFiles`
- def: [`tests/unit/grammar_coverage/test_corpus_generator.py:178`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_corpus_generator.py#L178)
- doc: 测试语料库文件保存
- signature: `class TestSaveCorpusFiles:`
- members:
  - `test_create_nested_directories(self)` — [`L204`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_corpus_generator.py#L204) — 测试创建嵌套目录
  - `test_save_multiple_files(self)` — [`L193`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_corpus_generator.py#L193) — 测试保存多个文件
  - `test_save_python_corpus(self)` — [`L181`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_corpus_generator.py#L181) — 测试保存 Python 语料库
  - `test_utf8_encoding(self)` — [`L214`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_corpus_generator.py#L214) — 测试 UTF-8 编码支持
- uses (calls/refs, reference-scoped): [`save_corpus_files`](../../../tree_sitter_analyzer/grammar_coverage/corpus_generator.md#save_corpus_files)

### `TestValidateGeneratedCode`
- def: [`tests/unit/grammar_coverage/test_corpus_generator.py:86`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_corpus_generator.py#L86)
- doc: 测试代码验证功能
- signature: `class TestValidateGeneratedCode:`
- members:
  - `test_invalid_javascript_code(self)` — [`L109`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_corpus_generator.py#L109) — 测试无效的 JavaScript 代码
  - `test_invalid_python_code(self)` — [`L104`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_corpus_generator.py#L104) — 测试无效的 Python 代码
  - `test_unsupported_language_validation(self)` — [`L114`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_corpus_generator.py#L114) — 测试不支持的语言验证返回 False
  - `test_valid_java_code(self)` — [`L99`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_corpus_generator.py#L99) — 测试有效的 Java 代码
  - `test_valid_javascript_code(self)` — [`L94`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_corpus_generator.py#L94) — 测试有效的 JavaScript 代码
  - `test_valid_python_code(self)` — [`L89`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/grammar_coverage/test_corpus_generator.py#L89) — 测试有效的 Python 代码
- uses (calls/refs, reference-scoped): [`validate_generated_code`](../../../tree_sitter_analyzer/grammar_coverage/corpus_generator.md#validate_generated_code)

