---
title: 'Module: tests/integration/formatters/schema_validation.py'
type: catalog
provenance: extracted
module: tests/integration/formatters/schema_validation.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.formatters.schema_validation`/
symbols:
  validate_format: validate_format().
  ValidationResult.is_valid: ValidationResult#is_valid.
  ValidationResult.errors: ValidationResult#errors.
  ValidationResult.add_error: ValidationResult#add_error().
  ValidationResult: ValidationResult#
  MarkdownTableValidator.validate: MarkdownTableValidator#validate().
  CSVFormatValidator.validate: CSVFormatValidator#validate().
  MarkdownTableValidator._validate_table_syntax: MarkdownTableValidator#_validate_table_syntax().
  MarkdownTableValidator: MarkdownTableValidator#
  CSVFormatValidator: CSVFormatValidator#
  JSONFormatValidator.validate: JSONFormatValidator#validate().
  FormatValidator: FormatValidator#
  FormatValidator.validate: FormatValidator#validate().
  MarkdownTableValidator._validate_overall_structure: MarkdownTableValidator#_validate_overall_structure().
  MarkdownTableValidator._validate_table_alignment: MarkdownTableValidator#_validate_table_alignment().
  FormatValidatorFactory._validators: FormatValidatorFactory#_validators.
  ValidationResult.merge: ValidationResult#merge().
  MarkdownTableValidator._validate_section_headers: MarkdownTableValidator#_validate_section_headers().
  CSVFormatValidator._validate_csv_data_consistency: CSVFormatValidator#_validate_csv_data_consistency().
  CSVFormatValidator._validate_csv_required_columns: CSVFormatValidator#_validate_csv_required_columns().
  JSONFormatValidator._validate_json_schema: JSONFormatValidator#_validate_json_schema().
  ValidationResult.add_warning: ValidationResult#add_warning().
  CSVFormatValidator._validate_csv_header: CSVFormatValidator#_validate_csv_header().
  FormatValidatorFactory.create_validator: FormatValidatorFactory#create_validator().
  ValidationResult.success: ValidationResult#success().
  JSONFormatValidator: JSONFormatValidator#
  ValidationResult.warnings: ValidationResult#warnings.
  MarkdownTableValidator._extract_table_groups: MarkdownTableValidator#_extract_table_groups().
  MarkdownTableValidator._is_table_line: MarkdownTableValidator#_is_table_line().
  JSONFormatValidator.schema: JSONFormatValidator#schema.
  ValidationResult.error: ValidationResult#error().
  ValidationResult.warning: ValidationResult#warning().
  FormatValidatorFactory.get_supported_formats: FormatValidatorFactory#get_supported_formats().
  MarkdownTableValidator.TABLE_SEPARATOR_PATTERN: MarkdownTableValidator#TABLE_SEPARATOR_PATTERN.
  MarkdownTableValidator._count_table_columns: MarkdownTableValidator#_count_table_columns().
  MarkdownTableValidator.TABLE_HEADER_PATTERN: MarkdownTableValidator#TABLE_HEADER_PATTERN.
  MarkdownTableValidator.SECTION_HEADER_PATTERN: MarkdownTableValidator#SECTION_HEADER_PATTERN.
  FormatValidatorFactory: FormatValidatorFactory#
  MarkdownTableValidator.TABLE_ROW_PATTERN: MarkdownTableValidator#TABLE_ROW_PATTERN.
  JSONFormatValidator.__init__: JSONFormatValidator#__init__().
---
# Module: [`tests/integration/formatters/schema_validation.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/schema_validation.py)

## Classes
### `CSVFormatValidator`  ·  implements/extends FormatValidator
- def: [`tests/integration/formatters/schema_validation.py:244`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/schema_validation.py#L244)
- doc: Validator for CSV format compliance
- signature: `class CSVFormatValidator(FormatValidator):`
- members:
  - `_validate_csv_data_consistency(self, rows: list[list[str]], result: ValidationResult)` — [`L304`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/schema_validation.py#L304) — Validate CSV data consistency
  - `_validate_csv_header(self, header: list[str], result: ValidationResult)` — [`L286`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/schema_validation.py#L286) — Validate CSV header row
  - `_validate_csv_required_columns(self, header: list[str], result: ValidationResult)` — [`L320`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/schema_validation.py#L320) — Validate presence of required columns
  - `validate(self, content: str)` — [`L247`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/schema_validation.py#L247) — Validate CSV format compliance
- uses (calls/refs, reference-scoped): (5 test-only callers)
- used by: (9 test-only callers)

### `FormatValidator`  ·  implements/extends ABC
- def: [`tests/integration/formatters/schema_validation.py:62`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/schema_validation.py#L62)
- doc: Abstract base class for format validators
- signature: `class FormatValidator(ABC):`
- members:
  - `validate(self, content: str)` — [`L66`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/schema_validation.py#L66) — Validate format content
- uses (calls/refs, reference-scoped): (7 test-only callers)
- used by: (5 test-only callers)

### `FormatValidatorFactory`
- def: [`tests/integration/formatters/schema_validation.py:437`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/schema_validation.py#L437)
- doc: Factory for creating format validators
- signature: `class FormatValidatorFactory:`
- members:
  - `create_validator(self, format_type: str, **kwargs)` — [`L447`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/schema_validation.py#L447) — Create format validator for specified type
  - `get_supported_formats(cls)` — [`L468`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/schema_validation.py#L468) — Get list of supported format types
- protocol/private: `_validators`[`L440`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/schema_validation.py#L440)
- uses (calls/refs, reference-scoped): (4 test-only callers)
- used by: (1 test-only callers)

### `JSONFormatValidator`  ·  implements/extends FormatValidator
- def: [`tests/integration/formatters/schema_validation.py:382`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/schema_validation.py#L382)
- doc: Validator for JSON format compliance
- signature: `class JSONFormatValidator(FormatValidator):`
- members:
  - `__init__(self, schema: dict[str, Any] | None = None)` — [`L385`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/schema_validation.py#L385) — Initialize JSON validator
  - `_validate_json_schema(self, data: Any, result: ValidationResult)` — [`L423`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/schema_validation.py#L423) — Validate JSON data against schema
  - `validate(self, content: str)` — [`L394`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/schema_validation.py#L394) — Validate JSON format compliance
  - `schema` — [`L392`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/schema_validation.py#L392)
- uses (calls/refs, reference-scoped): (4 test-only callers)
- used by: (4 test-only callers)

### `MarkdownTableValidator`  ·  implements/extends FormatValidator
- def: [`tests/integration/formatters/schema_validation.py:71`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/schema_validation.py#L71)
- doc: Validator for Markdown table structure and syntax
- signature: `class MarkdownTableValidator(FormatValidator):`
- members:
  - `_count_table_columns(self, line: str)` — [`L216`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/schema_validation.py#L216) — Count number of columns in table line
  - `_extract_table_groups(self, lines: list[str])` — [`L221`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/schema_validation.py#L221) — Extract groups of consecutive table lines
  - `_is_table_line(self, line: str)` — [`L211`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/schema_validation.py#L211) — Check if line is part of a table
  - `_validate_overall_structure(self, lines: list[str], result: ValidationResult)` — [`L107`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/schema_validation.py#L107) — Validate overall markdown structure
  - `_validate_section_headers(self, lines: list[str], result: ValidationResult)` — [`L168`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/schema_validation.py#L168) — Validate section headers
  - `_validate_table_alignment(self, lines: list[str], result: ValidationResult)` — [`L191`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/schema_validation.py#L191) — Validate table column alignment
  - `_validate_table_syntax(self, lines: list[str], result: ValidationResult)` — [`L124`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/schema_validation.py#L124) — Validate table syntax
  - `validate(self, content: str)` — [`L80`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/schema_validation.py#L80) — Validate markdown table structure and syntax
  - `SECTION_HEADER_PATTERN` — [`L78`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/schema_validation.py#L78)
  - `TABLE_HEADER_PATTERN` — [`L75`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/schema_validation.py#L75)
  - `TABLE_ROW_PATTERN` — [`L77`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/schema_validation.py#L77)
  - `TABLE_SEPARATOR_PATTERN` — [`L76`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/schema_validation.py#L76)
- uses (calls/refs, reference-scoped): (5 test-only callers)
- used by: (9 test-only callers)

### `ValidationResult`
- def: [`tests/integration/formatters/schema_validation.py:22`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/schema_validation.py#L22)
- doc: Result of format validation
- signature: `class ValidationResult:`
- members:
  - `add_error(self, message: str)` — [`L44`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/schema_validation.py#L44) — Add error message
  - `add_warning(self, message: str)` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/schema_validation.py#L49) — Add warning message
  - `error(cls, message: str)` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/schema_validation.py#L35) — Create error validation result
  - `merge(self, other: ValidationResult)` — [`L53`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/schema_validation.py#L53) — Merge with another validation result
  - `success(cls)` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/schema_validation.py#L30) — Create successful validation result
  - `warning(cls, message: str)` — [`L40`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/schema_validation.py#L40) — Create warning validation result
  - `errors` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/schema_validation.py#L26)
  - `is_valid` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/schema_validation.py#L25)
  - `warnings` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/schema_validation.py#L27)
- used by: [`_validate_format_output`](../../../scripts/pre_commit_format_validation.md#PreCommitFormatValidator._validate_format_output), [`_validate_format_compliance`](../../../scripts/format_monitoring_tool.md#FormatMonitor._validate_format_compliance)  (26 test-only)

## Functions
- `validate_format(content: str, format_type: str, **kwargs)` — [`L473`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/schema_validation.py#L473) — Convenience function to validate format content

