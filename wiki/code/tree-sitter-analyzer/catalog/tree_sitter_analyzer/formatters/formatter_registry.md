---
title: 'Module: tree_sitter_analyzer/formatters/formatter_registry.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/formatters/formatter_registry.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.formatters.formatter_registry`/
symbols:
  FormatterRegistry: FormatterRegistry#
  _register_language_formatters_safe: _register_language_formatters_safe().
  FormatterRegistry.get_formatter_for_language: FormatterRegistry#get_formatter_for_language().
  JsonFormatter: JsonFormatter#
  CsvFormatter.format: CsvFormatter#format().
  JsonFormatter.format: JsonFormatter#format().
  FormatterRegistry.register_formatter: FormatterRegistry#register_formatter().
  register_builtin_formatters: register_builtin_formatters().
  CsvFormatter: CsvFormatter#
  FormatterRegistry.get_formatter: FormatterRegistry#get_formatter().
  CompactFormatter.format: CompactFormatter#format().
  FullFormatter: FullFormatter#
  CompactFormatter: CompactFormatter#
  FormatterRegistry.clear_registry: FormatterRegistry#clear_registry().
  _append_full_element_lines: _append_full_element_lines().
  FormatterRegistry._formatters: FormatterRegistry#_formatters.
  FullFormatter.format: FullFormatter#format().
  FormatterRegistry.get_available_formats: FormatterRegistry#get_available_formats().
  FormatterRegistry.is_format_supported: FormatterRegistry#is_format_supported().
  logger: logger.
  FormatterRegistry._language_formatters: FormatterRegistry#_language_formatters.
  FormatterRegistry.get_supported_languages: FormatterRegistry#get_supported_languages().
  FormatterRegistry.unregister_formatter: FormatterRegistry#unregister_formatter().
  FormatterRegistry.register_language_formatter: FormatterRegistry#register_language_formatter().
  FormatterRegistry.set_default_language_formatter: FormatterRegistry#set_default_language_formatter().
  FormatterRegistry.is_language_supported: FormatterRegistry#is_language_supported().
  FormatterRegistry._create_formatter_instance: FormatterRegistry#_create_formatter_instance().
  FormatterRegistry._default_language_formatter: FormatterRegistry#_default_language_formatter.
  FormatterRegistry._try_format_type_or_bare: FormatterRegistry#_try_format_type_or_bare().
  JsonFormatter.get_format_name: JsonFormatter#get_format_name().
  JsonFormatter._element_to_dict: JsonFormatter#_element_to_dict().
  CsvFormatter.get_format_name: CsvFormatter#get_format_name().
  FullFormatter.get_format_name: FullFormatter#get_format_name().
  CompactFormatter.get_format_name: CompactFormatter#get_format_name().
  CompactFormatter._get_visibility_symbol: CompactFormatter#_get_visibility_symbol().
---
# Module: [`tree_sitter_analyzer/formatters/formatter_registry.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/formatter_registry.py)

## Classes
### `CompactFormatter`  ·  implements/extends IFormatter
- def: [`tree_sitter_analyzer/formatters/formatter_registry.py:478`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/formatter_registry.py#L478)
- doc: Compact formatter for CodeElement lists
- signature: `class CompactFormatter(IFormatter):`
- members:
  - `_get_visibility_symbol(self, visibility: str)` — [`L506`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/formatter_registry.py#L506) — Get symbol for visibility
  - `format(self, elements: list[CodeElement])` — [`L487`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/formatter_registry.py#L487) — Format elements in compact format
  - `get_format_name()` — [`L483`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/formatter_registry.py#L483)
- uses (calls/refs, reference-scoped): [`name`](../models/base.md#CodeElement.name), [`start_line`](../models/base.md#CodeElement.start_line), [`end_line`](../models/base.md#CodeElement.end_line), [`CodeElement`](../models/base.md#CodeElement), [`IFormatter`](_formatter_interface.md#IFormatter)
- used by: [`IFormatter`](_formatter_interface.md#IFormatter), [`format`](_formatter_interface.md#IFormatter.format), [`get_format_name`](_formatter_interface.md#IFormatter.get_format_name), [`register_builtin_formatters`](formatter_registry.md#register_builtin_formatters)  (9 test-only)

### `CsvFormatter`  ·  implements/extends IFormatter
- def: [`tree_sitter_analyzer/formatters/formatter_registry.py:348`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/formatter_registry.py#L348)
- doc: CSV formatter for CodeElement lists
- signature: `class CsvFormatter(IFormatter):`
- members:
  - `format(self, elements: list[CodeElement])` — [`L357`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/formatter_registry.py#L357) — Format elements as CSV
  - `get_format_name()` — [`L353`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/formatter_registry.py#L353)
- uses (calls/refs, reference-scoped): [`name`](../models/base.md#CodeElement.name), [`start_line`](../models/base.md#CodeElement.start_line), [`end_line`](../models/base.md#CodeElement.end_line), [`language`](../models/base.md#CodeElement.language), [`CodeElement`](../models/base.md#CodeElement), [`IFormatter`](_formatter_interface.md#IFormatter), [`csv_safe_row`](_csv_safety.md#csv_safe_row)
- used by: [`IFormatter`](_formatter_interface.md#IFormatter), [`format`](_formatter_interface.md#IFormatter.format), [`get_format_name`](_formatter_interface.md#IFormatter.get_format_name), [`register_builtin_formatters`](formatter_registry.md#register_builtin_formatters)  (15 test-only)

### `FormatterRegistry`
- def: [`tree_sitter_analyzer/formatters/formatter_registry.py:20`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/formatter_registry.py#L20)
- doc: Unified registry for managing and providing formatter instances.
- signature: `class FormatterRegistry:`
- members:
  - `_create_formatter_instance(cls, formatter_class: type[Any], format_type: str, language: str, **kwargs: Any)` — [`L243`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/formatter_registry.py#L243) — Create a formatter instance with appropriate constructor arguments.
  - `_try_format_type_or_bare(cls, formatter_class: type[Any], format_type: str)` — [`L268`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/formatter_registry.py#L268) — Fallback: try format_type-only constructor, then bare constructor.
  - `clear_registry(cls)` — [`L131`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/formatter_registry.py#L131) — Clear all registered formatters.
  - `get_available_formats(cls)` — [`L88`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/formatter_registry.py#L88) — Get list of all available format names.
  - `get_formatter(cls, format_name: str)` — [`L64`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/formatter_registry.py#L64) — Get a formatter instance for the specified format.
  - `get_formatter_for_language(cls, language: str, format_type: str = "full", **kwargs: Any)` — [`L188`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/formatter_registry.py#L188) — Get a formatter instance for the specified language and format type.
  - `get_supported_languages(cls)` — [`L278`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/formatter_registry.py#L278) — Get list of all languages with registered formatters.
  - `is_format_supported(cls, format_name: str)` — [`L99`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/formatter_registry.py#L99) — Check if a format is supported.
  - `is_language_supported(cls, language: str)` — [`L288`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/formatter_registry.py#L288) — Check if a language has specific formatters registered.
  - `register_formatter(cls, formatter_class: type[IFormatter])` — [`L38`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/formatter_registry.py#L38) — Register a formatter class in the registry.
  - `register_language_formatter(cls, language: str, format_type: str, formatter_class: type[Any])` — [`L144`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/formatter_registry.py#L144) — Register a language-specific formatter.
  - `set_default_language_formatter(cls, formatter_class: type[Any])` — [`L176`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/formatter_registry.py#L176) — Set the default formatter class for languages without specific formatters.
  - `unregister_formatter(cls, format_name: str)` — [`L113`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/formatter_registry.py#L113) — Unregister a formatter for the specified format.
- protocol/private: `_default_language_formatter`[`L34`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/formatter_registry.py#L34), `_formatters`[`L32`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/formatter_registry.py#L32), `_language_formatters`[`L33`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/formatter_registry.py#L33)
- uses (calls/refs, reference-scoped): [`IFormatter`](_formatter_interface.md#IFormatter), [`get_format_name`](_formatter_interface.md#IFormatter.get_format_name), [`logger`](formatter_registry.md#logger)
- used by: [`_register_language_formatters_safe`](formatter_registry.md#_register_language_formatters_safe), [`register_builtin_formatters`](formatter_registry.md#register_builtin_formatters), [`_format_table`](../mcp/tools/analyze_code_structure_tool.md#_format_table), [`_render_table_output`](../cli/commands/table_command.md#TableCommand._render_table_output)  (57 test-only)

### `FullFormatter`  ·  implements/extends IFormatter
- def: [`tree_sitter_analyzer/formatters/formatter_registry.py:436`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/formatter_registry.py#L436)
- doc: Full table formatter for CodeElement lists
- signature: `class FullFormatter(IFormatter):`
- members:
  - `format(self, elements: list[CodeElement])` — [`L445`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/formatter_registry.py#L445) — Format elements as full table
  - `get_format_name()` — [`L441`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/formatter_registry.py#L441)
- uses (calls/refs, reference-scoped): [`CodeElement`](../models/base.md#CodeElement), [`IFormatter`](_formatter_interface.md#IFormatter), [`_append_full_element_lines`](formatter_registry.md#_append_full_element_lines)
- used by: [`IFormatter`](_formatter_interface.md#IFormatter), [`format`](_formatter_interface.md#IFormatter.format), [`get_format_name`](_formatter_interface.md#IFormatter.get_format_name), [`register_builtin_formatters`](formatter_registry.md#register_builtin_formatters)  (9 test-only)

### `JsonFormatter`  ·  implements/extends IFormatter
- def: [`tree_sitter_analyzer/formatters/formatter_registry.py:304`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/formatter_registry.py#L304)
- doc: JSON formatter for CodeElement lists
- signature: `class JsonFormatter(IFormatter):`
- members:
  - `_element_to_dict(element: Any)` — [`L313`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/formatter_registry.py#L313) — Convert one element to a JSON-serialisable dict.
  - `format(self, elements: list[CodeElement])` — [`L340`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/formatter_registry.py#L340) — Format elements as JSON
  - `get_format_name()` — [`L309`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/formatter_registry.py#L309)
- uses (calls/refs, reference-scoped): [`CodeElement`](../models/base.md#CodeElement), [`IFormatter`](_formatter_interface.md#IFormatter)
- used by: [`IFormatter`](_formatter_interface.md#IFormatter), [`format`](_formatter_interface.md#IFormatter.format), [`get_format_name`](_formatter_interface.md#IFormatter.get_format_name), [`register_builtin_formatters`](formatter_registry.md#register_builtin_formatters)  (21 test-only)

## Functions
- `_append_full_element_lines(lines: list[str], element: CodeElement)` — [`L412`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/formatter_registry.py#L412) — Append the per-element block lines used by ``FullFormatter.format``.
- `_register_language_formatters_safe()` — [`L527`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/formatter_registry.py#L527) — Register language-specific formatters safely to avoid circular imports
- `register_builtin_formatters()` — [`L513`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/formatter_registry.py#L513) — Register all built-in formatters

## Module values
- `logger` — [`L17`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/formatter_registry.py#L17)

