---
title: 'Module: tests/integration/formatters/specification_compliance_tests.py'
type: catalog
provenance: extracted
module: tests/integration/formatters/specification_compliance_tests.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.formatters.specification_compliance_tests`/
symbols:
  FormatSpecificationValidator.errors: FormatSpecificationValidator#errors.
  FormatSpecificationValidator.validate_full_format_specification: FormatSpecificationValidator#validate_full_format_specification().
  FormatSpecificationValidator.validate_compact_format_specification: FormatSpecificationValidator#validate_compact_format_specification().
  FormatSpecificationValidator.validate_csv_format_specification: FormatSpecificationValidator#validate_csv_format_specification().
  FormatSpecificationValidator.warnings: FormatSpecificationValidator#warnings.
  FormatSpecificationValidator._validate_csv_row: FormatSpecificationValidator#_validate_csv_row().
  FormatSpecificationValidator._validate_common_formatting: FormatSpecificationValidator#_validate_common_formatting().
  FormatSpecificationValidator._validate_full_format_header: FormatSpecificationValidator#_validate_full_format_header().
  FormatSpecificationValidator._validate_full_format_sections: FormatSpecificationValidator#_validate_full_format_sections().
  FormatSpecificationValidator._validate_full_format_tables: FormatSpecificationValidator#_validate_full_format_tables().
  FormatSpecificationValidator._validate_compact_format_header: FormatSpecificationValidator#_validate_compact_format_header().
  FormatSpecificationValidator._validate_compact_format_tables: FormatSpecificationValidator#_validate_compact_format_tables().
  FormatSpecificationValidator._validate_csv_structure: FormatSpecificationValidator#_validate_csv_structure().
  FormatSpecificationValidator._validate_csv_data_rows: FormatSpecificationValidator#_validate_csv_data_rows().
  FormatSpecificationValidator._validate_markdown_table: FormatSpecificationValidator#_validate_markdown_table().
  FormatSpecificationValidator.get_validation_report: FormatSpecificationValidator#get_validation_report().
  TestFormatSpecificationCompliance.test_full_format_specification_compliance: TestFormatSpecificationCompliance#test_full_format_specification_compliance().
  TestFormatSpecificationCompliance.test_compact_format_specification_compliance: TestFormatSpecificationCompliance#test_compact_format_specification_compliance().
  TestFormatSpecificationCompliance.test_csv_format_specification_compliance: TestFormatSpecificationCompliance#test_csv_format_specification_compliance().
  TestFormatSpecificationCompliance.test_specification_compliance_across_formats: TestFormatSpecificationCompliance#test_specification_compliance_across_formats().
  FormatSpecificationValidator._validate_compact_format_sections: FormatSpecificationValidator#_validate_compact_format_sections().
  FormatSpecificationValidator._append_inconsistent_csv_row_errors: FormatSpecificationValidator#_append_inconsistent_csv_row_errors().
  FormatSpecificationValidator._validate_csv_header: FormatSpecificationValidator#_validate_csv_header().
  FormatSpecificationValidator._append_line_number_error: FormatSpecificationValidator#_append_line_number_error().
  TestFormatSpecificationCompliance.test_java_file: TestFormatSpecificationCompliance#test_java_file().
  TestFormatSpecificationCompliance.validator: TestFormatSpecificationCompliance#validator().
  ANALYTICS_SERVICE_JAVA: ANALYTICS_SERVICE_JAVA.
  FormatSpecificationValidator: FormatSpecificationValidator#
  FormatSpecificationValidator._validate_parameters_format: FormatSpecificationValidator#_validate_parameters_format().
  assert_specification_compliance_across_formats: assert_specification_compliance_across_formats().
  FormatSpecificationValidator.__init__: FormatSpecificationValidator#__init__().
  TestFormatSpecificationCompliance: TestFormatSpecificationCompliance#
  TestFormatSpecificationCompliance.test_specification_error_handling: TestFormatSpecificationCompliance#test_specification_error_handling().
  TestFormatSpecificationCompliance.test_specification_edge_cases: TestFormatSpecificationCompliance#test_specification_edge_cases().
---
# Module: [`tests/integration/formatters/specification_compliance_tests.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/specification_compliance_tests.py)

## Classes
### `FormatSpecificationValidator`
- def: [`tests/integration/formatters/specification_compliance_tests.py:153`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/specification_compliance_tests.py#L153)
- doc: Validator for format specification compliance
- signature: `class FormatSpecificationValidator:`
- members:
  - `_validate_common_formatting(self, output: str)` — [`L567`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/specification_compliance_tests.py#L567) — Validate common formatting requirements
  - `_validate_compact_format_header(self, lines: list[str], class_name: str)` — [`L282`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/specification_compliance_tests.py#L282) — Validate Compact Format header: # {ClassName}
  - `_validate_compact_format_sections(self, lines: list[str])` — [`L315`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/specification_compliance_tests.py#L315) — Validate required sections for Compact Format
  - `_validate_compact_format_tables(self, lines: list[str])` — [`L327`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/specification_compliance_tests.py#L327) — Validate table structures for Compact Format
  - `_validate_csv_data_rows(self, output: str)` — [`L437`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/specification_compliance_tests.py#L437) — Validate CSV data rows
  - `_validate_csv_header(self, output: str)` — [`L408`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/specification_compliance_tests.py#L408) — Validate CSV header compliance
  - `_validate_csv_row(self, row: list[str], row_num: int)` — [`L453`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/specification_compliance_tests.py#L453) — Validate individual CSV row
  - `_validate_csv_structure(self, output: str)` — [`L378`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/specification_compliance_tests.py#L378) — Validate CSV structure
  - `_validate_full_format_header(self, lines: list[str], class_name: str)` — [`L181`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/specification_compliance_tests.py#L181) — Validate Full Format header: # {package}.{ClassName}
  - `_validate_full_format_sections(self, lines: list[str])` — [`L211`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/specification_compliance_tests.py#L211) — Validate required sections for Full Format
  - `_validate_full_format_tables(self, lines: list[str])` — [`L226`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/specification_compliance_tests.py#L226) — Validate table structures for Full Format
  - `_validate_markdown_table(self, table_content: str, expected_headers: list[str])` — [`L528`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/specification_compliance_tests.py#L528) — Validate Markdown table structure
  - `_validate_parameters_format(self, parameters: str)` — [`L506`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/specification_compliance_tests.py#L506) — Validate parameters format: param1:type1;param2:type2
  - `get_validation_report(self)` — [`L594`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/specification_compliance_tests.py#L594) — Get validation report
  - `validate_compact_format_specification(self, output: str, class_name: str)` — [`L255`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/specification_compliance_tests.py#L255) — Validate Compact Format specification compliance
  - `validate_csv_format_specification(self, output: str)` — [`L359`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/specification_compliance_tests.py#L359) — Validate CSV Format specification compliance
  - `validate_full_format_specification(self, output: str, class_name: str)` — [`L160`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/specification_compliance_tests.py#L160) — Validate Full Format specification compliance
  - `errors` — [`L157`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/specification_compliance_tests.py#L157)
  - `warnings` — [`L158`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/specification_compliance_tests.py#L158)
- protocol/private: `__init__`[`L156`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/specification_compliance_tests.py#L156), `_append_inconsistent_csv_row_errors`[`L397`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/specification_compliance_tests.py#L397), `_append_line_number_error`[`L494`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/specification_compliance_tests.py#L494)
- used by: (1 test-only callers)

### `TestFormatSpecificationCompliance`
- def: [`tests/integration/formatters/specification_compliance_tests.py:643`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/specification_compliance_tests.py#L643)
- doc: Test format specification compliance
- signature: `class TestFormatSpecificationCompliance:`
- members:
  - `test_compact_format_specification_compliance(self, test_java_file, validator)` — [`L709`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/specification_compliance_tests.py#L709) — Test Compact Format specification compliance
  - `test_csv_format_specification_compliance(self, test_java_file, validator)` — [`L749`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/specification_compliance_tests.py#L749) — Test CSV Format specification compliance
  - `test_full_format_specification_compliance(self, test_java_file, validator)` — [`L669`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/specification_compliance_tests.py#L669) — Test Full Format specification compliance
  - `test_java_file(self)` — [`L647`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/specification_compliance_tests.py#L647) — Create a comprehensive Java test file
  - `test_specification_compliance_across_formats(self, test_java_file, validator)` — [`L798`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/specification_compliance_tests.py#L798) — Test specification compliance across all formats
  - `test_specification_edge_cases(self, validator)` — [`L840`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/specification_compliance_tests.py#L840) — Test specification validation with edge cases
  - `test_specification_error_handling(self, validator)` — [`L810`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/specification_compliance_tests.py#L810) — Test specification validation error handling
  - `validator(self)` — [`L661`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/specification_compliance_tests.py#L661) — Create specification validator
- uses (calls/refs, reference-scoped): [`AnalyzeCodeStructureTool`](../../../tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.md#AnalyzeCodeStructureTool), [`execute`](../../../tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.md#AnalyzeCodeStructureTool.execute)  (3 test-only)

## Functions
- `assert_specification_compliance_across_formats(tool: Any, file_path: Path, class_name: str, validator: Any)` — [`L605`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/specification_compliance_tests.py#L605) — Run all format specification compliance checks.

## Module values
- `ANALYTICS_SERVICE_JAVA` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/specification_compliance_tests.py#L21)

