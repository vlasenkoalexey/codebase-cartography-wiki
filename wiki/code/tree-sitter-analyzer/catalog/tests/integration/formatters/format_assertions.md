---
title: 'Module: tests/integration/formatters/format_assertions.py'
type: catalog
provenance: extracted
module: tests/integration/formatters/format_assertions.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.formatters.format_assertions`/
symbols:
  MarkdownTableAssertions: MarkdownTableAssertions#
  assert_full_format_compliance: assert_full_format_compliance().
  assert_csv_format_compliance: assert_csv_format_compliance().
  MarkdownTableAssertions.assert_markdown_table_structure: MarkdownTableAssertions#assert_markdown_table_structure().
  assert_compact_format_compliance: assert_compact_format_compliance().
  CSVFormatAssertions.assert_csv_format_compliance: CSVFormatAssertions#assert_csv_format_compliance().
  FormatComplianceAssertions.assert_format_consistency: FormatComplianceAssertions#assert_format_consistency().
  FormatAssertions: FormatAssertions#
  FormatComplianceAssertions: FormatComplianceAssertions#
  CSVFormatAssertions: CSVFormatAssertions#
  MarkdownTableAssertions.assert_table_column_headers: MarkdownTableAssertions#assert_table_column_headers().
  MarkdownTableAssertions._extract_section_headers: MarkdownTableAssertions#_extract_section_headers().
  MarkdownTableAssertions._validate_table_in_section: MarkdownTableAssertions#_validate_table_in_section().
  FullFormatAssertions.assert_full_format_sections: FullFormatAssertions#assert_full_format_sections().
  FullFormatAssertions.assert_full_format_class_info_table: FullFormatAssertions#assert_full_format_class_info_table().
  FullFormatAssertions.assert_full_format_detailed_sections: FullFormatAssertions#assert_full_format_detailed_sections().
  CompactFormatAssertions: CompactFormatAssertions#
  FullFormatAssertions: FullFormatAssertions#
  MarkdownTableAssertions.assert_table_row_count: MarkdownTableAssertions#assert_table_row_count().
  MarkdownTableAssertions.assert_code_block_language: MarkdownTableAssertions#assert_code_block_language().
  MarkdownTableAssertions._extract_section_content: MarkdownTableAssertions#_extract_section_content().
  FormatAssertions.assert_not_empty: FormatAssertions#assert_not_empty().
  FormatAssertions.assert_valid_markdown_table: FormatAssertions#assert_valid_markdown_table().
  FormatAssertions.assert_valid_csv_format: FormatAssertions#assert_valid_csv_format().
  MarkdownTableAssertions.HEADER_PATTERN: MarkdownTableAssertions#HEADER_PATTERN.
  MarkdownTableAssertions.TABLE_SEPARATOR_PATTERN: MarkdownTableAssertions#TABLE_SEPARATOR_PATTERN.
  MarkdownTableAssertions.CODE_BLOCK_PATTERN: MarkdownTableAssertions#CODE_BLOCK_PATTERN.
  CompactFormatAssertions.assert_compact_format_includes_complexity: CompactFormatAssertions#assert_compact_format_includes_complexity().
  CompactFormatAssertions.assert_compact_visibility_symbols: CompactFormatAssertions#assert_compact_visibility_symbols().
  CompactFormatAssertions.assert_compact_abbreviated_signatures: CompactFormatAssertions#assert_compact_abbreviated_signatures().
  CSVFormatAssertions.assert_csv_required_columns: CSVFormatAssertions#assert_csv_required_columns().
  CSVFormatAssertions.assert_csv_complexity_scores: CSVFormatAssertions#assert_csv_complexity_scores().
  CSVFormatAssertions._assert_csv_header_compliance: CSVFormatAssertions#_assert_csv_header_compliance().
  FormatComplianceAssertions._assert_element_count_consistency: FormatComplianceAssertions#_assert_element_count_consistency().
  FormatAssertions.assert_contains_all: FormatAssertions#assert_contains_all().
  FormatAssertions.assert_line_count_range: FormatAssertions#assert_line_count_range().
  MarkdownTableAssertions.TABLE_HEADER_PATTERN: MarkdownTableAssertions#TABLE_HEADER_PATTERN.
  MarkdownTableAssertions.assert_main_header_format: MarkdownTableAssertions#assert_main_header_format().
  CSVFormatAssertions.assert_csv_row_format: CSVFormatAssertions#assert_csv_row_format().
  FormatComplianceAssertions.assert_no_format_regression: FormatComplianceAssertions#assert_no_format_regression().
---
# Module: [`tests/integration/formatters/format_assertions.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/format_assertions.py)

## Classes
### `CSVFormatAssertions`  ·  implements/extends FormatAssertions
- def: [`tests/integration/formatters/format_assertions.py:268`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/format_assertions.py#L268)
- doc: Assertions for CSV format validation
- signature: `class CSVFormatAssertions(FormatAssertions):`
- members:
  - `_assert_csv_header_compliance(header: list[str])` — [`L334`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/format_assertions.py#L334) — Assert CSV header follows specification
  - `assert_csv_complexity_scores(content: str)` — [`L314`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/format_assertions.py#L314) — Assert CSV includes complexity scores for methods
  - `assert_csv_format_compliance(content: str)` — [`L272`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/format_assertions.py#L272) — Assert CSV format follows specification
  - `assert_csv_required_columns(content: str, required_columns: list[str])` — [`L288`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/format_assertions.py#L288) — Assert CSV has all required columns
  - `assert_csv_row_format(content: str, row_type: str, expected_pattern: Pattern)` — [`L299`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/format_assertions.py#L299) — Assert CSV rows of specific type match expected pattern
- uses (calls/refs, reference-scoped): (4 test-only callers)
- used by: (2 test-only callers)

### `CompactFormatAssertions`  ·  implements/extends MarkdownTableAssertions
- def: [`tests/integration/formatters/format_assertions.py:236`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/format_assertions.py#L236)
- doc: Assertions specific to compact format
- signature: `class CompactFormatAssertions(MarkdownTableAssertions):`
- members:
  - `assert_compact_abbreviated_signatures(content: str)` — [`L257`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/format_assertions.py#L257) — Assert compact format uses simplified structure
  - `assert_compact_format_includes_complexity(content: str)` — [`L241`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/format_assertions.py#L241) — Assert compact format includes complexity scores
  - `assert_compact_visibility_symbols(content: str)` — [`L248`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/format_assertions.py#L248) — Assert compact format includes visibility information
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (2 test-only callers)

### `FormatAssertions`
- def: [`tests/integration/formatters/format_assertions.py:14`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/format_assertions.py#L14)
- doc: Base class for format-specific assertions
- signature: `class FormatAssertions:`
- members:
  - `assert_contains_all(content: str, required_items: list[str])` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/format_assertions.py#L25) — Assert content contains all required items
  - `assert_line_count_range(content: str, min_lines: int, max_lines: int | None = None)` — [`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/format_assertions.py#L31) — Assert content has line count within specified range
  - `assert_not_empty(content: str, message: str = "Content should not be empty")` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/format_assertions.py#L18) — Assert content is not empty
  - `assert_valid_csv_format(content: str)` — [`L70`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/format_assertions.py#L70) — Assert content contains valid CSV format
  - `assert_valid_markdown_table(content: str)` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/format_assertions.py#L48) — Assert content contains valid markdown table structure
- uses (calls/refs, reference-scoped): (2 test-only callers)
- used by: (4 test-only callers)

### `FormatComplianceAssertions`
- def: [`tests/integration/formatters/format_assertions.py:406`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/format_assertions.py#L406)
- doc: Cross-format validation assertions
- signature: `class FormatComplianceAssertions:`
- members:
  - `_assert_element_count_consistency(outputs: dict[str, str], expected_counts: dict[str, int])` — [`L449`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/format_assertions.py#L449) — Assert element counts are consistent across formats
  - `assert_format_consistency(outputs: dict[str, str], element_counts: dict[str, int])` — [`L410`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/format_assertions.py#L410) — Assert consistency across different format outputs
  - `assert_no_format_regression(current_output: str, reference_output: str, format_type: str, allow_additions: bool = False)` — [`L426`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/format_assertions.py#L426) — Assert current output doesn't regress from reference
- uses (calls/refs, reference-scoped): (3 test-only callers)
- used by: (2 test-only callers)

### `FullFormatAssertions`  ·  implements/extends MarkdownTableAssertions
- def: [`tests/integration/formatters/format_assertions.py:344`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/format_assertions.py#L344)
- doc: Assertions specific to full format
- signature: `class FullFormatAssertions(MarkdownTableAssertions):`
- members:
  - `assert_full_format_class_info_table(content: str)` — [`L362`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/format_assertions.py#L362) — Assert full format has proper Class Info table
  - `assert_full_format_detailed_sections(content: str)` — [`L382`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/format_assertions.py#L382) — Assert full format has detailed method/field sections
  - `assert_full_format_sections(content: str, class_name: str)` — [`L348`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/format_assertions.py#L348) — Assert full format has all required sections
- uses (calls/refs, reference-scoped): (4 test-only callers)
- used by: (2 test-only callers)

### `MarkdownTableAssertions`  ·  implements/extends FormatAssertions
- def: [`tests/integration/formatters/format_assertions.py:88`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/format_assertions.py#L88)
- doc: Assertions for Markdown table format validation
- signature: `class MarkdownTableAssertions(FormatAssertions):`
- members:
  - `_extract_section_content(content: str, section_name: str)` — [`L212`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/format_assertions.py#L212) — Extract content of specific section
  - `_extract_section_headers(content: str)` — [`L206`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/format_assertions.py#L206) — Extract section header names from content
  - `_validate_table_in_section(section_content: str)` — [`L221`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/format_assertions.py#L221) — Validate table structure within a section
  - `assert_code_block_language(content: str, expected_language: str)` — [`L195`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/format_assertions.py#L195) — Assert code blocks use expected language
  - `assert_main_header_format(content: str, expected_class_name: str)` — [`L131`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/format_assertions.py#L131) — Assert main header follows expected format
  - `assert_markdown_table_structure(content: str, expected_sections: list[str], require_all_sections: bool = True)` — [`L98`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/format_assertions.py#L98) — Assert markdown table has required sections and structure
  - `assert_table_column_headers(content: str, section_name: str, expected_columns: list[str])` — [`L144`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/format_assertions.py#L144) — Assert table in section has expected column headers
  - `assert_table_row_count(content: str, section_name: str, min_rows: int, max_rows: int | None = None)` — [`L170`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/format_assertions.py#L170) — Assert table in section has expected number of rows
  - `CODE_BLOCK_PATTERN` — [`L95`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/format_assertions.py#L95)
  - `HEADER_PATTERN` — [`L92`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/format_assertions.py#L92)
  - `TABLE_HEADER_PATTERN` — [`L93`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/format_assertions.py#L93)
  - `TABLE_SEPARATOR_PATTERN` — [`L94`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/format_assertions.py#L94)
- uses (calls/refs, reference-scoped): (6 test-only callers)
- used by: (6 test-only callers)

## Functions
- `assert_compact_format_compliance(content: str)` — [`L492`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/format_assertions.py#L492) — Assert content complies with compact format specification
- `assert_csv_format_compliance(content: str)` — [`L499`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/format_assertions.py#L499) — Assert content complies with CSV format specification
- `assert_full_format_compliance(content: str, class_name: str)` — [`L485`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/format_assertions.py#L485) — Assert content complies with full format specification

