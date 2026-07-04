---
title: 'Module: tree_sitter_analyzer/formatters/language_formatter_factory.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/formatters/language_formatter_factory.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.formatters.language_formatter_factory`/
symbols:
  LanguageFormatterFactory._formatters: LanguageFormatterFactory#_formatters.
  LanguageFormatterFactory: LanguageFormatterFactory#
  LanguageFormatterFactory.create_formatter: LanguageFormatterFactory#create_formatter().
  create_language_formatter: create_language_formatter().
  LanguageFormatterFactory.supports_language: LanguageFormatterFactory#supports_language().
  LanguageFormatterFactory.register_formatter: LanguageFormatterFactory#register_formatter().
  LanguageFormatterFactory.get_supported_languages: LanguageFormatterFactory#get_supported_languages().
---
# Module: [`tree_sitter_analyzer/formatters/language_formatter_factory.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/language_formatter_factory.py)

## Classes
### `LanguageFormatterFactory`
- def: [`tree_sitter_analyzer/formatters/language_formatter_factory.py:25`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/language_formatter_factory.py#L25)
- doc: Factory for creating language-specific formatters
- signature: `class LanguageFormatterFactory:`
- members:
  - `create_formatter(cls, language: str)` — [`L66`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/language_formatter_factory.py#L66) — Create formatter for specified language
  - `get_supported_languages(cls)` — [`L97`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/language_formatter_factory.py#L97) — Get list of supported languages
  - `register_formatter(cls, language: str, formatter_class: type[BaseFormatter])` — [`L84`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/language_formatter_factory.py#L84) — Register new language formatter
  - `supports_language(cls, language: str)` — [`L107`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/language_formatter_factory.py#L107) — Check if language is supported
- protocol/private: `_formatters`[`L28`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/language_formatter_factory.py#L28)
- uses (calls/refs, reference-scoped): [`JavaTableFormatter`](java_formatter.md#JavaTableFormatter), [`MarkdownFormatter`](markdown_formatter.md#MarkdownFormatter), [`PythonTableFormatter`](python_formatter.md#PythonTableFormatter), [`BaseFormatter`](base_formatter.md#BaseFormatter), [`GoTableFormatter`](go_formatter.md#GoTableFormatter), [`JavaScriptTableFormatter`](javascript_formatter.md#JavaScriptTableFormatter), [`RustTableFormatter`](rust_formatter.md#RustTableFormatter), [`YAMLFormatter`](yaml_formatter.md#YAMLFormatter), [`KotlinTableFormatter`](kotlin_formatter.md#KotlinTableFormatter), [`CSharpTableFormatter`](csharp_formatter.md#CSharpTableFormatter), [`PHPTableFormatter`](php_formatter.md#PHPTableFormatter), [`RubyTableFormatter`](ruby_formatter.md#RubyTableFormatter), [`TypeScriptTableFormatter`](typescript_formatter.md#TypeScriptTableFormatter), [`HtmlFormatter`](html_formatter.md#HtmlFormatter), [`CppTableFormatter`](cpp_formatter.md#CppTableFormatter), [`SQLFormatterWrapper`](sql_formatter_wrapper.md#SQLFormatterWrapper), [`CSSFormatter`](css_formatter.md#CSSFormatter)
- used by: [`create_language_formatter`](language_formatter_factory.md#create_language_formatter)  (33 test-only)

## Functions
- `create_language_formatter(language: str)` — [`L120`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/language_formatter_factory.py#L120) — Create language formatter (function for compatibility)

