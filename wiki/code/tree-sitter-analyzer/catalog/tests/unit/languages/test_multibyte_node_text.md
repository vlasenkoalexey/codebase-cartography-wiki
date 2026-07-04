---
title: 'Module: tests/unit/languages/test_multibyte_node_text.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_multibyte_node_text.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_multibyte_node_text`/
symbols:
  test_python_function_signature_after_multibyte: test_python_function_signature_after_multibyte().
  test_python_class_name_after_multibyte_docstring: test_python_class_name_after_multibyte_docstring().
  test_ruby_class_name_after_multibyte_comment: test_ruby_class_name_after_multibyte_comment().
  test_ruby_function_name_after_multibyte_comment: test_ruby_function_name_after_multibyte_comment().
  test_csharp_class_name_after_multibyte_comment: test_csharp_class_name_after_multibyte_comment().
  test_csharp_method_name_after_multibyte_comment: test_csharp_method_name_after_multibyte_comment().
  test_php_class_name_after_multibyte_comment: test_php_class_name_after_multibyte_comment().
  test_php_function_name_after_multibyte_comment: test_php_function_name_after_multibyte_comment().
  _parse: _parse().
  MULTIBYTE_SAMPLES: MULTIBYTE_SAMPLES.
  _has_simple_name: _has_simple_name().
  _build_parser: _build_parser().
---
# Module: [`tests/unit/languages/test_multibyte_node_text.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_multibyte_node_text.py)

## Functions
- `_build_parser(language: tree_sitter.Language)` — [`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_multibyte_node_text.py#L39) — Construct a parser working with old + new tree_sitter binding APIs.
- `_has_simple_name(names: list[str], expected: str)` — [`L61`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_multibyte_node_text.py#L61) — Return True if any extracted name contains ``expected`` as a whole
- `_parse(source: str, plugin: object)` — [`L53`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_multibyte_node_text.py#L53) — Parse ``source`` using ``plugin``'s tree-sitter language.
- `test_csharp_class_name_after_multibyte_comment(mb: str)` — [`L204`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_multibyte_node_text.py#L204) — C# class extraction stays aligned past a multibyte XML doc comment.
- `test_csharp_method_name_after_multibyte_comment(mb: str)` — [`L230`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_multibyte_node_text.py#L230) — C# method extraction stays aligned past a multibyte comment.
- `test_php_class_name_after_multibyte_comment(mb: str)` — [`L261`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_multibyte_node_text.py#L261) — PHP class extraction stays aligned past a multibyte PHPDoc comment.
- `test_php_function_name_after_multibyte_comment(mb: str)` — [`L288`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_multibyte_node_text.py#L288) — PHP method extraction stays aligned past a multibyte comment.
- `test_python_class_name_after_multibyte_docstring(mb: str)` — [`L88`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_multibyte_node_text.py#L88) — Python class extraction stays aligned past a multibyte docstring.
- `test_python_function_signature_after_multibyte(mb: str)` — [`L118`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_multibyte_node_text.py#L118) — Function name + parameter extraction stays aligned past multibyte.
- `test_ruby_class_name_after_multibyte_comment(mb: str)` — [`L155`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_multibyte_node_text.py#L155) — Ruby class extraction stays aligned past a multibyte comment.
- `test_ruby_function_name_after_multibyte_comment(mb: str)` — [`L177`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_multibyte_node_text.py#L177) — Ruby method extraction stays aligned past a multibyte comment.

## Module values
- `MULTIBYTE_SAMPLES` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_multibyte_node_text.py#L36)

