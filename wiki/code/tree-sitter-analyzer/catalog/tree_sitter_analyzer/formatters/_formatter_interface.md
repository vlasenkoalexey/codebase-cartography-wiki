---
title: 'Module: tree_sitter_analyzer/formatters/_formatter_interface.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/formatters/_formatter_interface.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.formatters._formatter_interface`/I
symbols:
  IFormatter: Formatter#
  IFormatter.format: Formatter#format().
  IFormatter.get_format_name: Formatter#get_format_name().
  IStructureFormatter: StructureFormatter#
  IStructureFormatter.format_structure: StructureFormatter#format_structure().
---
# Module: [`tree_sitter_analyzer/formatters/_formatter_interface.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_formatter_interface.py)

## Classes
### `IFormatter`  ·  implements/extends ABC
- def: [`tree_sitter_analyzer/formatters/_formatter_interface.py:11`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_formatter_interface.py#L11)
- doc: Interface for code element formatters.
- signature: `class IFormatter(ABC):`
- members:
  - `format(self, elements: list[CodeElement])` — [`L20`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_formatter_interface.py#L20) — Format a list of CodeElements into a string representation.
  - `get_format_name()` — [`L16`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_formatter_interface.py#L16) — Return the format name this formatter supports.
- uses (calls/refs, reference-scoped): [`CodeElement`](../models/base.md#CodeElement), [`HtmlFormatter`](html_formatter.md#HtmlFormatter), [`format`](html_formatter.md#HtmlJsonFormatter.format), [`JsonFormatter`](formatter_registry.md#JsonFormatter), [`format`](formatter_registry.md#CsvFormatter.format), [`format`](formatter_registry.md#JsonFormatter.format), [`format`](html_formatter.md#HtmlCompactFormatter.format), [`CsvFormatter`](formatter_registry.md#CsvFormatter), [`format`](html_formatter.md#HtmlCsvFormatter.format), [`format`](formatter_registry.md#CompactFormatter.format), [`CompactFormatter`](formatter_registry.md#CompactFormatter), [`FullFormatter`](formatter_registry.md#FullFormatter), [`format`](formatter_registry.md#FullFormatter.format), [`get_format_name`](formatter_registry.md#CompactFormatter.get_format_name), [`get_format_name`](formatter_registry.md#CsvFormatter.get_format_name), [`get_format_name`](formatter_registry.md#FullFormatter.get_format_name), [`get_format_name`](formatter_registry.md#JsonFormatter.get_format_name), [`get_format_name`](html_formatter.md#HtmlCompactFormatter.get_format_name), [`get_format_name`](html_formatter.md#HtmlCsvFormatter.get_format_name), [`get_format_name`](html_formatter.md#HtmlFormatter.get_format_name), [`get_format_name`](html_formatter.md#HtmlJsonFormatter.get_format_name)  (34 test-only)
- used by: [`HtmlFormatter`](html_formatter.md#HtmlFormatter), [`JsonFormatter`](formatter_registry.md#JsonFormatter), [`format_analysis_result`](html_formatter.md#HtmlFormatter.format_analysis_result), [`register_formatter`](formatter_registry.md#FormatterRegistry.register_formatter), [`CsvFormatter`](formatter_registry.md#CsvFormatter), [`HtmlCompactFormatter`](html_formatter.md#HtmlCompactFormatter), [`_format_table`](../mcp/tools/analyze_code_structure_tool.md#_format_table), [`get_formatter`](formatter_registry.md#FormatterRegistry.get_formatter), [`HtmlJsonFormatter`](html_formatter.md#HtmlJsonFormatter), [`CompactFormatter`](formatter_registry.md#CompactFormatter), [`FullFormatter`](formatter_registry.md#FullFormatter), [`_formatters`](formatter_registry.md#FormatterRegistry._formatters), [`HtmlCsvFormatter`](html_formatter.md#HtmlCsvFormatter)  (19 test-only)

### `IStructureFormatter`  ·  implements/extends ABC
- def: [`tree_sitter_analyzer/formatters/_formatter_interface.py:24`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_formatter_interface.py#L24)
- doc: Interface for structure-based formatters (legacy compatibility).
- signature: `class IStructureFormatter(ABC):`
- members:
  - `format_structure(self, structure_data: dict[str, Any])` — [`L28`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_formatter_interface.py#L28) — Format structure data dictionary into a string representation.

