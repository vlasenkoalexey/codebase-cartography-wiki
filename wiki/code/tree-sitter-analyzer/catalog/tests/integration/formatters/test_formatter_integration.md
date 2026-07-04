---
title: 'Module: tests/integration/formatters/test_formatter_integration.py'
type: catalog
provenance: extracted
module: tests/integration/formatters/test_formatter_integration.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.formatters.test_formatter_integration`/Test
symbols:
  TestRealImplementationValidation.test_format_validation_with_real_output: RealImplementationValidation#test_format_validation_with_real_output().
  TestRealImplementationValidation.test_legacy_formatters_produce_valid_output: RealImplementationValidation#test_legacy_formatters_produce_valid_output().
  TestFormatConsistency.test_formatter_registry_vs_legacy_formatter: FormatConsistency#test_formatter_registry_vs_legacy_formatter().
  TestFormatConsistency.sample_java_elements: FormatConsistency#sample_java_elements().
  TestFormatConsistency.test_mcp_vs_cli_format_consistency: FormatConsistency#test_mcp_vs_cli_format_consistency().
  TestTableFormatToolIntegration.real_tool: TableFormatToolIntegration#real_tool().
  TestTableFormatToolIntegration.golden_master_manager: TableFormatToolIntegration#golden_master_manager().
  TestTableFormatToolIntegration: TableFormatToolIntegration#
  TestFormatConsistency: FormatConsistency#
  TestRealImplementationValidation: RealImplementationValidation#
  TestTableFormatToolIntegration.temp_project_with_java_file: TableFormatToolIntegration#temp_project_with_java_file().
  TestTableFormatToolIntegration.test_full_format_end_to_end: TableFormatToolIntegration#test_full_format_end_to_end().
  TestTableFormatToolIntegration.test_compact_format_end_to_end: TableFormatToolIntegration#test_compact_format_end_to_end().
  TestTableFormatToolIntegration.test_csv_format_end_to_end: TableFormatToolIntegration#test_csv_format_end_to_end().
  TestTableFormatToolIntegration.test_format_consistency_across_all_types: TableFormatToolIntegration#test_format_consistency_across_all_types().
  TestFormatConsistency.temp_project_with_java_file: FormatConsistency#temp_project_with_java_file().
---
# Module: [`tests/integration/formatters/test_formatter_integration.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_formatter_integration.py)

## Classes
### `TestFormatConsistency`
- def: [`tests/integration/formatters/test_formatter_integration.py:293`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_formatter_integration.py#L293)
- doc: Test format consistency across different code paths
- signature: `class TestFormatConsistency:`
- members:
  - `sample_java_elements(self)` — [`L297`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_formatter_integration.py#L297) — Create sample Java CodeElements for testing
  - `temp_project_with_java_file(self)` — [`L481`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_formatter_integration.py#L481) — Create temporary project with Java test file
  - `test_formatter_registry_vs_legacy_formatter(self, sample_java_elements)` — [`L388`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_formatter_integration.py#L388) — Ensure FormatterRegistry and legacy formatters produce identical output
  - `test_mcp_vs_cli_format_consistency(self, temp_project_with_java_file)` — [`L428`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_formatter_integration.py#L428) — Ensure MCP and CLI interfaces produce consistent format output
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`start_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`end_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.end_line), [`language`](../../../tree_sitter_analyzer/models/base.md#CodeElement.language), [`CodeElement`](../../../tree_sitter_analyzer/models/base.md#CodeElement), [`AnalyzeCodeStructureTool`](../../../tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.md#AnalyzeCodeStructureTool), [`FormatterRegistry`](../../../tree_sitter_analyzer/formatters/formatter_registry.md#FormatterRegistry), [`element_type`](../../../tree_sitter_analyzer/models/base.md#CodeElement.element_type), [`execute`](../../../tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.md#AnalyzeCodeStructureTool.execute), [`format`](../../../tree_sitter_analyzer/formatters/_formatter_interface.md#IFormatter.format), [`CsvFormatter`](../../../tree_sitter_analyzer/formatters/formatter_registry.md#CsvFormatter), [`get_formatter`](../../../tree_sitter_analyzer/formatters/formatter_registry.md#FormatterRegistry.get_formatter), [`CompactFormatter`](../../../tree_sitter_analyzer/formatters/formatter_registry.md#CompactFormatter), [`FullFormatter`](../../../tree_sitter_analyzer/formatters/formatter_registry.md#FullFormatter), [`is_format_supported`](../../../tree_sitter_analyzer/formatters/formatter_registry.md#FormatterRegistry.is_format_supported)
- used by: (1 test-only callers)

### `TestRealImplementationValidation`
- def: [`tests/integration/formatters/test_formatter_integration.py:520`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_formatter_integration.py#L520)
- doc: Test real implementation behavior without mocks
- signature: `class TestRealImplementationValidation:`
- members:
  - `test_format_validation_with_real_output(self)` — [`L563`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_formatter_integration.py#L563) — Test format validation utilities with real formatter output
  - `test_legacy_formatters_produce_valid_output(self)` — [`L523`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_formatter_integration.py#L523) — Test that legacy formatters produce valid, compliant output
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`start_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`end_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.end_line), [`language`](../../../tree_sitter_analyzer/models/base.md#CodeElement.language), [`CodeElement`](../../../tree_sitter_analyzer/models/base.md#CodeElement), [`element_type`](../../../tree_sitter_analyzer/models/base.md#CodeElement.element_type), [`format`](../../../tree_sitter_analyzer/formatters/formatter_registry.md#CsvFormatter.format), [`CsvFormatter`](../../../tree_sitter_analyzer/formatters/formatter_registry.md#CsvFormatter), [`CompactFormatter`](../../../tree_sitter_analyzer/formatters/formatter_registry.md#CompactFormatter), [`FullFormatter`](../../../tree_sitter_analyzer/formatters/formatter_registry.md#FullFormatter), [`format`](../../../tree_sitter_analyzer/formatters/formatter_registry.md#FullFormatter.format)  (3 test-only)
- used by: (1 test-only callers)

### `TestTableFormatToolIntegration`
- def: [`tests/integration/formatters/test_formatter_integration.py:27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_formatter_integration.py#L27)
- doc: Integration tests using real implementations, minimal mocking
- signature: `class TestTableFormatToolIntegration:`
- members:
  - `golden_master_manager(self)` — [`L88`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_formatter_integration.py#L88) — Provide golden master manager for testing
  - `real_tool(self, temp_project_with_java_file)` — [`L82`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_formatter_integration.py#L82) — Create TableFormatTool with real dependencies
  - `temp_project_with_java_file(self)` — [`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_formatter_integration.py#L31) — Create temporary project with Java test file
  - `test_compact_format_end_to_end(self, real_tool, temp_project_with_java_file, golden_master_manager)` — [`L134`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_formatter_integration.py#L134) — Test complete flow with real formatting - compact format
  - `test_csv_format_end_to_end(self, real_tool, temp_project_with_java_file, golden_master_manager)` — [`L172`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_formatter_integration.py#L172) — Test complete flow with real formatting - CSV format
  - `test_format_consistency_across_all_types(self, real_tool, temp_project_with_java_file)` — [`L222`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_formatter_integration.py#L222) — Test format consistency across different output types
  - `test_full_format_end_to_end(self, real_tool, temp_project_with_java_file, golden_master_manager)` — [`L93`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_formatter_integration.py#L93) — Test complete flow with real formatting - full format
- uses (calls/refs, reference-scoped): [`AnalyzeCodeStructureTool`](../../../tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.md#AnalyzeCodeStructureTool)  (1 test-only)
- used by: (1 test-only callers)

