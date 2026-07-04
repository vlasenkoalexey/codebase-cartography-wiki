---
title: 'Module: tests/integration/formatters/enhanced_assertions.py'
type: catalog
provenance: extracted
module: tests/integration/formatters/enhanced_assertions.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.formatters.enhanced_assertions`/
symbols:
  _invalid_naming_result: _invalid_naming_result().
  _invalid_return_type_result: _invalid_return_type_result().
  _invalid_access_modifier_result: _invalid_access_modifier_result().
  _orphan_constructor_result: _orphan_constructor_result().
  _undefined_class_result: _undefined_class_result().
  _missing_constructor_result: _missing_constructor_result().
  build_assertion_report: build_assertion_report().
  parse_csv_elements: parse_csv_elements().
  EnhancedAssertions.validate_format_output: EnhancedAssertions#validate_format_output().
  StructuralFormatValidator._validate_csv_structure: StructuralFormatValidator#_validate_csv_structure().
  _validate_markdown_row: _validate_markdown_row().
  _validate_markdown_separator: _validate_markdown_separator().
  _csv_row_element: _csv_row_element().
  _markdown_section_element: _markdown_section_element().
  _markdown_table_row: _markdown_table_row().
  ContentAwareValidator._compare_elements: ContentAwareValidator#_compare_elements().
  _count_mismatch_result: _count_mismatch_result().
  SemanticFormatValidator.validate_semantic_consistency: SemanticFormatValidator#validate_semantic_consistency().
  validate_element_relationships: validate_element_relationships().
  _validate_class_method_relationships: _validate_class_method_relationships().
  _compare_one_format_count: _compare_one_format_count().
  validate_inheritance_relationships: validate_inheritance_relationships().
  _undefined_class_results_for_context: _undefined_class_results_for_context().
  parse_markdown_elements: parse_markdown_elements().
  validate_naming_conventions: validate_naming_conventions().
  validate_type_consistency: validate_type_consistency().
  validate_access_modifiers: validate_access_modifiers().
  _validate_constructor_relationships: _validate_constructor_relationships().
  _undefined_class_results: _undefined_class_results().
  ContentAwareValidator.validate_content_accuracy: ContentAwareValidator#validate_content_accuracy().
  StructuralFormatValidator.validate_table_structure: StructuralFormatValidator#validate_table_structure().
  StructuralFormatValidator._validate_markdown_table_structure: StructuralFormatValidator#_validate_markdown_table_structure().
  parse_format_elements: parse_format_elements().
  EnhancedFormatAssertionsAssertMixin.assert_format_completeness: EnhancedFormatAssertionsAssertMixin#assert_format_completeness().
  EnhancedFormatAssertionsAssertMixin.assert_format_consistency: EnhancedFormatAssertionsAssertMixin#assert_format_consistency().
  ContentAwareValidator._parse_source_code: ContentAwareValidator#_parse_source_code().
  _count_mismatch_results: _count_mismatch_results().
  _count_mismatch_result_for_expected: _count_mismatch_result_for_expected().
  _group_elements_by_type: _group_elements_by_type().
  _class_missing_constructor: _class_missing_constructor().
  _matching_constructor_class: _matching_constructor_class().
  _referenced_type_contexts: _referenced_type_contexts().
  compare_format_counts: compare_format_counts().
  _group_by_severity: _group_by_severity().
  _group_by_message_type: _group_by_message_type().
  EnhancedFormatAssertionsAssertMixin.assert_semantic_correctness: EnhancedFormatAssertionsAssertMixin#assert_semantic_correctness().
  EnhancedFormatAssertionsAssertMixin.generate_assertion_report: EnhancedFormatAssertionsAssertMixin#generate_assertion_report().
  EnhancedFormatAssertions: EnhancedFormatAssertions#
  _content_accuracy_results: _content_accuracy_results().
  EnhancedAssertions: EnhancedAssertions#
  EnhancedFormatAssertionsAssertMixin: EnhancedFormatAssertionsAssertMixin#
  EnhancedAssertions.semantic_validator: EnhancedAssertions#semantic_validator.
  EnhancedAssertions.structural_validator: EnhancedAssertions#structural_validator.
  EnhancedAssertions.content_validator: EnhancedAssertions#content_validator.
  _is_method_in_class: _is_method_in_class().
  _is_known_class_reference: _is_known_class_reference().
  EnhancedFormatAssertions.semantic_validator: EnhancedFormatAssertions#semantic_validator.
  EnhancedFormatAssertions.structural_validator: EnhancedFormatAssertions#structural_validator.
  EnhancedFormatAssertions.content_validator: EnhancedFormatAssertions#content_validator.
  SemanticFormatValidator.__init__: SemanticFormatValidator#__init__().
  count_format_elements: count_format_elements().
  TYPE_MAPPINGS: TYPE_MAPPINGS.
  VALID_MODIFIERS: VALID_MODIFIERS.
  ContentAwareValidator: ContentAwareValidator#
  StructuralFormatValidator: StructuralFormatValidator#
  SemanticFormatValidator: SemanticFormatValidator#
  ContentAwareValidator._parse_python_code: ContentAwareValidator#_parse_python_code().
  ContentAwareValidator._parse_java_code: ContentAwareValidator#_parse_java_code().
  ContentAwareValidator._parse_format_output: ContentAwareValidator#_parse_format_output().
  _is_markdown_table_row: _is_markdown_table_row().
  _potential_class_names: _potential_class_names().
  LANGUAGE_KEYWORDS: LANGUAGE_KEYWORDS.
  NAMING_RULES: NAMING_RULES.
  BUILTIN_CLASS_REFERENCES: BUILTIN_CLASS_REFERENCES.
  __all__: __all__.
  EnhancedFormatAssertions.__init__: EnhancedFormatAssertions#__init__().
  EnhancedAssertions.__init__: EnhancedAssertions#__init__().
  SemanticFormatValidator.language_keywords: SemanticFormatValidator#language_keywords.
---
# Module: [`tests/integration/formatters/enhanced_assertions.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py)

## Classes
### `ContentAwareValidator`
- def: [`tests/integration/formatters/enhanced_assertions.py:141`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L141)
- members:
  - `_compare_elements(self, actual: dict[str, list[dict[str, Any]]], reported: dict[str, list[dict[str, Any]]])` — [`L238`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L238) — Compare actual vs reported elements
  - `_parse_format_output(self, format_output: str)` — [`L231`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L231) — Parse format output to extract reported elements
  - `_parse_java_code(self, source_code: str)` — [`L204`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L204) — Parse Java source code using regex patterns
  - `_parse_python_code(self, source_code: str)` — [`L165`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L165) — Parse Python source code using AST
  - `_parse_source_code(self, source_code: str, language: str)` — [`L152`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L152) — Parse source code to extract actual elements
  - `validate_content_accuracy(self, format_output: str, source_code: str, language: str)` — [`L144`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L144) — Validate that format output accurately represents source code
- uses (calls/refs, reference-scoped): (6 test-only callers)
- used by: (2 test-only callers)

### `EnhancedAssertions`
- def: [`tests/integration/formatters/enhanced_assertions.py:95`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L95)
- doc: Main enhanced assertions class that integrates all validation components
- signature: `class EnhancedAssertions:`
- members:
  - `validate_format_output(self, output: str, format_type: str, language: str = "python")` — [`L103`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L103) — Comprehensive format output validation
  - `content_validator` — [`L101`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L101)
  - `semantic_validator` — [`L99`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L99)
  - `structural_validator` — [`L100`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L100)
- protocol/private: `__init__`[`L98`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L98)
- uses (calls/refs, reference-scoped): (7 test-only callers)
- used by: (2 test-only callers)

### `EnhancedFormatAssertions`  ·  implements/extends EnhancedFormatAssertionsAssertMixin, FormatComplianceAssertions
- def: [`tests/integration/formatters/enhanced_assertions.py:83`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L83)
- doc: Enhanced format assertions with semantic and structural validation
- signature: `class EnhancedFormatAssertions(EnhancedFormatAssertionsAssertMixin, FormatComplianceAssertions):`
- members:
  - `content_validator` — [`L92`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L92)
  - `semantic_validator` — [`L90`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L90)
  - `structural_validator` — [`L91`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L91)
- protocol/private: `__init__`[`L88`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L88)
- uses (calls/refs, reference-scoped): (5 test-only callers)
- used by: (2 test-only callers)

### `EnhancedFormatAssertionsAssertMixin`
- def: [`tests/integration/formatters/enhanced_assertions.py:28`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L28)
- doc: Assertion helpers used by EnhancedFormatAssertions.
- signature: `class EnhancedFormatAssertionsAssertMixin:`
- members:
  - `assert_format_completeness(self, format_output: str, expected_elements: dict[str, int])` — [`L59`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L59) — Assert format completeness
  - `assert_format_consistency(self, outputs: dict[str, str])` — [`L66`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L66) — Assert consistency across different format types
  - `assert_semantic_correctness(self, format_output: str, format_type: str, language: str, source_code: str | None = None)` — [`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L31) — Assert semantic correctness of format output
  - `generate_assertion_report(self, results: list[AssertionResult])` — [`L76`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L76) — Generate comprehensive assertion report
- uses (calls/refs, reference-scoped): (7 test-only callers)
- used by: (1 test-only callers)

### `SemanticFormatValidator`
- def: [`tests/integration/formatters/enhanced_assertions.py:528`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L528)
- members:
  - `validate_semantic_consistency(self, format_output: str, format_type: str, language: str)` — [`L534`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L534) — Validate semantic consistency of format output
  - `language_keywords` — [`L532`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L532)
- protocol/private: `__init__`[`L531`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L531)
- uses (calls/refs, reference-scoped): (7 test-only callers)
- used by: (3 test-only callers)

### `StructuralFormatValidator`
- def: [`tests/integration/formatters/enhanced_assertions.py:285`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L285)
- members:
  - `_validate_csv_structure(self, output: str)` — [`L301`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L301) — Validate CSV structure
  - `_validate_markdown_table_structure(self, output: str)` — [`L383`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L383) — Validate Markdown table structure
  - `validate_table_structure(self, output: str, format_type: str)` — [`L288`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L288) — Validate table structure consistency
- uses (calls/refs, reference-scoped): (9 test-only callers)
- used by: (3 test-only callers)

## Functions
- `_class_missing_constructor(class_name: str, class_methods: list[FormatElement], language: str)` — [`L861`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L861)
- `_compare_one_format_count(base_format: str, base_counts: dict[str, int], other_format: str, other_counts: dict[str, int])` — [`L1115`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L1115)
- `_content_accuracy_results(content_validator: Any, format_output: str, source_code: str | None, language: str)` — [`L495`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L495)
- `_count_mismatch_result(element_type: str, expected_count: int, actual_count: int, actual_counts: dict[str, int])` — [`L508`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L508)
- `_count_mismatch_result_for_expected(element_type: str, expected_count: int, actual_counts: dict[str, int])` — [`L482`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L482)
- `_count_mismatch_results(actual_counts: dict[str, int], expected_elements: dict[str, int])` — [`L466`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L466)
- `_csv_row_element(row: dict[str, str | None], line_num: int)` — [`L576`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L576)
- `_group_by_message_type(results: list[AssertionResult])` — [`L1155`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L1155)
- `_group_by_severity(results: list[AssertionResult])` — [`L1143`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L1143)
- `_group_elements_by_type(elements: list[FormatElement])` — [`L825`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L825)
- `_invalid_access_modifier_result(element: FormatElement, language: str, valid_set: set[str])` — [`L776`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L776)
- `_invalid_naming_result(element: FormatElement, language: str, rules: dict[str, str])` — [`L687`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L687)
- `_invalid_return_type_result(element: FormatElement, language: str, valid_types: set[str])` — [`L732`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L732)
- `_is_known_class_reference(potential_class: str, class_names: set[str])` — [`L1003`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L1003)
- `_is_markdown_table_row(line: str)` — [`L645`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L645)
- `_is_method_in_class(method: FormatElement, class_name: str)` — [`L856`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L856) — Check if method belongs to class (simplified heuristic).
- `_markdown_section_element(current_section: str, line: str, line_num: int)` — [`L632`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L632)
- `_markdown_table_row(line: str, line_num: int, current_section: str | None, current_table: list[FormatElement])` — [`L649`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L649)
- `_matching_constructor_class(constructor: FormatElement, classes: list[FormatElement], language: str)` — [`L909`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L909)
- `_missing_constructor_result(class_elem: FormatElement, class_name: str, language: str)` — [`L874`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L874)
- `_orphan_constructor_result(constructor: FormatElement, classes: list[FormatElement])` — [`L925`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L925)
- `_potential_class_names(text: str)` — [`L999`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L999)
- `_referenced_type_contexts(element: FormatElement)` — [`L988`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L988)
- `_undefined_class_result(element: FormatElement, potential_class: str, text: str, class_names: set[str])` — [`L1007`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L1007)
- `_undefined_class_results(element: FormatElement, class_names: set[str])` — [`L959`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L959)
- `_undefined_class_results_for_context(element: FormatElement, text: str, class_names: set[str])` — [`L971`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L971)
- `_validate_class_method_relationships(classes: list[FormatElement], methods: list[FormatElement], language: str)` — [`L836`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L836)
- `_validate_constructor_relationships(classes: list[FormatElement], constructors: list[FormatElement], language: str)` — [`L894`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L894)
- `_validate_markdown_row(line: str, line_num: int, table_start_line: int, table_headers: list[str])` — [`L418`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L418)
- `_validate_markdown_separator(line: str, line_num: int, table_headers: list[str])` — [`L445`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L445)
- `build_assertion_report(results: list[AssertionResult])` — [`L1028`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L1028) — Build a grouped assertion report with summary and detail sections.
- `compare_format_counts(format_counts: dict[str, dict[str, int]])` — [`L1093`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L1093) — Compare element counts across format outputs.
- `count_format_elements(output: str)` — [`L1071`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L1071) — Count table rows and section headings in format output.
- `parse_csv_elements(output: str)` — [`L553`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L553) — Parse CSV format elements.
- `parse_format_elements(output: str, format_type: str)` — [`L546`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L546) — Parse format output into structured elements.
- `parse_markdown_elements(output: str)` — [`L594`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L594) — Parse Markdown format elements.
- `validate_access_modifiers(elements: list[FormatElement], language: str)` — [`L758`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L758) — Validate access modifiers.
- `validate_element_relationships(elements: list[FormatElement], language: str)` — [`L800`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L800) — Validate relationships between parsed format elements.
- `validate_inheritance_relationships(elements: list[FormatElement], language: str)` — [`L943`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L943) — Validate inheritance relationships.
- `validate_naming_conventions(elements: list[FormatElement], language: str)` — [`L672`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L672) — Validate naming conventions.
- `validate_type_consistency(elements: list[FormatElement], language: str)` — [`L714`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L714) — Validate type consistency.

## Module values
- `BUILTIN_CLASS_REFERENCES` — [`L1262`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L1262)
- `LANGUAGE_KEYWORDS` — [`L1171`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L1171)
- `NAMING_RULES` — [`L1217`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L1217)
- `TYPE_MAPPINGS` — [`L1240`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L1240)
- `VALID_MODIFIERS` — [`L1255`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L1255)
- `__all__` — [`L17`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/enhanced_assertions.py#L17)

