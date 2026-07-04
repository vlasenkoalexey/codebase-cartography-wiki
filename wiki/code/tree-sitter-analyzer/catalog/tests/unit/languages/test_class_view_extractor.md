---
title: 'Module: tests/unit/languages/test_class_view_extractor.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_class_view_extractor.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_class_view_extractor`/Test
symbols:
  TestAppendClassView.test_appends_valid_view: AppendClassView#test_appends_valid_view().
  TestExtractClassViews.test_extracts_create_view_nodes: ExtractClassViews#test_extracts_create_view_nodes().
  TestExtractClassViews.test_skips_non_view_nodes: ExtractClassViews#test_skips_non_view_nodes().
  TestExtractClassViews.test_view_with_invalid_name_skipped: ExtractClassViews#test_view_with_invalid_name_skipped().
  TestAppendClassView.test_no_valid_name_returns_early: AppendClassView#test_no_valid_name_returns_early().
  TestAppendClassView.test_exception_handled: AppendClassView#test_exception_handled().
  TestExtractClassViews.fake_traverse: ExtractClassViews#fake_traverse().
  TestViewNameFromText.test_simple_create_view: ViewNameFromText#test_simple_create_view().
  TestViewNameFromText.test_create_view_if_not_exists: ViewNameFromText#test_create_view_if_not_exists().
  TestViewNameFromText.test_empty_text: ViewNameFromText#test_empty_text().
  TestViewNameFromText.test_no_view_keyword: ViewNameFromText#test_no_view_keyword().
  TestViewNameFromText.test_invalid_identifier: ViewNameFromText#test_invalid_identifier().
  TestViewNameFromText.test_case_insensitive: ViewNameFromText#test_case_insensitive().
  TestIsValidViewIdentifier.test_valid_identifier: IsValidViewIdentifier#test_valid_identifier().
  TestIsValidViewIdentifier.test_empty_string: IsValidViewIdentifier#test_empty_string().
  TestIsValidViewIdentifier.test_invalid_identifier: IsValidViewIdentifier#test_invalid_identifier().
  TestIsValidViewIdentifier.test_reserved_keyword: IsValidViewIdentifier#test_reserved_keyword().
  TestIsValidViewIdentifier.test_reserved_keyword_lowercase: IsValidViewIdentifier#test_reserved_keyword_lowercase().
  TestViewNameFromChildren.test_object_reference_with_identifier: ViewNameFromChildren#test_object_reference_with_identifier().
  TestViewNameFromChildren.test_no_object_reference: ViewNameFromChildren#test_no_object_reference().
  TestViewNameFromChildren.test_object_reference_without_identifier: ViewNameFromChildren#test_object_reference_without_identifier().
  TestViewNameFromChildren.test_empty_children: ViewNameFromChildren#test_empty_children().
  TestViewNameFromChildren.test_reserved_identifier_rejected: ViewNameFromChildren#test_reserved_identifier_rejected().
  TestViewName.test_from_text_succeeds: ViewName#test_from_text_succeeds().
  TestViewName.test_fallback_to_children: ViewName#test_fallback_to_children().
  TestViewName.test_no_name_found: ViewName#test_no_name_found().
  TestFindViewStatementEnd.test_finds_semicolon: FindViewStatementEnd#test_finds_semicolon().
  TestFindViewStatementEnd.test_falls_back_to_create_keyword: FindViewStatementEnd#test_falls_back_to_create_keyword().
  TestFindViewStatementEnd.test_empty_line_fallback: FindViewStatementEnd#test_empty_line_fallback().
  TestFindViewStatementEnd.test_beyond_50_lines_returns_none: FindViewStatementEnd#test_beyond_50_lines_returns_none().
  TestFindViewStatementEnd.test_no_terminator: FindViewStatementEnd#test_no_terminator().
  TestRecoverSingleLineViewSpan.test_same_start_end_no_source: RecoverSingleLineViewSpan#test_same_start_end_no_source().
  TestRecoverSingleLineViewSpan.test_multiline_already: RecoverSingleLineViewSpan#test_multiline_already().
  TestRecoverSingleLineViewSpan.test_recovery_finds_semicolon: RecoverSingleLineViewSpan#test_recovery_finds_semicolon().
  TestRecoverSingleLineViewSpan.test_recovery_not_found_returns_original: RecoverSingleLineViewSpan#test_recovery_not_found_returns_original().
  TestViewNameFromText: ViewNameFromText#
  TestIsValidViewIdentifier: IsValidViewIdentifier#
  TestViewNameFromChildren: ViewNameFromChildren#
  TestViewName: ViewName#
  TestFindViewStatementEnd: FindViewStatementEnd#
  TestRecoverSingleLineViewSpan: RecoverSingleLineViewSpan#
  TestAppendClassView: AppendClassView#
  TestExtractClassViews: ExtractClassViews#
---
# Module: [`tests/unit/languages/test_class_view_extractor.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_class_view_extractor.py)

## Classes
### `TestAppendClassView`
- def: [`tests/unit/languages/test_class_view_extractor.py:274`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_class_view_extractor.py#L274)
- signature: `class TestAppendClassView:`
- members:
  - `test_appends_valid_view(self)` — [`L275`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_class_view_extractor.py#L275)
  - `test_exception_handled(self)` — [`L304`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_class_view_extractor.py#L304) — When start_point raises, exception is caught and logged.
  - `test_no_valid_name_returns_early(self)` — [`L295`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_class_view_extractor.py#L295)
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`start_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`language`](../../../tree_sitter_analyzer/models/base.md#CodeElement.language), [`Class`](../../../tree_sitter_analyzer/models/base.md#Class), [`_append_class_view`](../../../tree_sitter_analyzer/languages/sql_plugin/_class_view_extractor.md#_append_class_view)

### `TestExtractClassViews`
- def: [`tests/unit/languages/test_class_view_extractor.py:323`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_class_view_extractor.py#L323)
- signature: `class TestExtractClassViews:`
- members:
  - `fake_traverse(r)` — [`L331`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_class_view_extractor.py#L331)
  - `test_extracts_create_view_nodes(self)` — [`L324`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_class_view_extractor.py#L324)
  - `test_skips_non_view_nodes(self)` — [`L347`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_class_view_extractor.py#L347)
  - `test_view_with_invalid_name_skipped(self)` — [`L367`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_class_view_extractor.py#L367)
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`Class`](../../../tree_sitter_analyzer/models/base.md#Class), [`extract_class_views`](../../../tree_sitter_analyzer/languages/sql_plugin/_class_view_extractor.md#extract_class_views)

### `TestFindViewStatementEnd`
- def: [`tests/unit/languages/test_class_view_extractor.py:192`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_class_view_extractor.py#L192)
- signature: `class TestFindViewStatementEnd:`
- members:
  - `test_beyond_50_lines_returns_none(self)` — [`L216`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_class_view_extractor.py#L216)
  - `test_empty_line_fallback(self)` — [`L205`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_class_view_extractor.py#L205)
  - `test_falls_back_to_create_keyword(self)` — [`L197`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_class_view_extractor.py#L197)
  - `test_finds_semicolon(self)` — [`L193`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_class_view_extractor.py#L193)
  - `test_no_terminator(self)` — [`L220`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_class_view_extractor.py#L220) — Only one line, no semicolon, no next CREATE statement.
- uses (calls/refs, reference-scoped): [`_find_view_statement_end`](../../../tree_sitter_analyzer/languages/sql_plugin/_class_view_extractor.md#_find_view_statement_end)

### `TestIsValidViewIdentifier`
- def: [`tests/unit/languages/test_class_view_extractor.py:56`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_class_view_extractor.py#L56)
- signature: `class TestIsValidViewIdentifier:`
- members:
  - `test_empty_string(self)` — [`L60`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_class_view_extractor.py#L60)
  - `test_invalid_identifier(self)` — [`L63`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_class_view_extractor.py#L63)
  - `test_reserved_keyword(self)` — [`L66`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_class_view_extractor.py#L66)
  - `test_reserved_keyword_lowercase(self)` — [`L74`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_class_view_extractor.py#L74) — Reserved check is case-insensitive (upper() comparison).
  - `test_valid_identifier(self)` — [`L57`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_class_view_extractor.py#L57)
- uses (calls/refs, reference-scoped): [`_is_valid_view_identifier`](../../../tree_sitter_analyzer/languages/sql_plugin/_class_view_extractor.md#_is_valid_view_identifier)

### `TestRecoverSingleLineViewSpan`
- def: [`tests/unit/languages/test_class_view_extractor.py:228`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_class_view_extractor.py#L228)
- signature: `class TestRecoverSingleLineViewSpan:`
- members:
  - `test_multiline_already(self)` — [`L236`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_class_view_extractor.py#L236) — When start_line != end_line, no recovery needed.
  - `test_recovery_finds_semicolon(self)` — [`L244`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_class_view_extractor.py#L244)
  - `test_recovery_not_found_returns_original(self)` — [`L259`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_class_view_extractor.py#L259)
  - `test_same_start_end_no_source(self)` — [`L229`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_class_view_extractor.py#L229)
- uses (calls/refs, reference-scoped): [`_recover_single_line_view_span`](../../../tree_sitter_analyzer/languages/sql_plugin/_class_view_extractor.md#_recover_single_line_view_span)

### `TestViewName`
- def: [`tests/unit/languages/test_class_view_extractor.py:150`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_class_view_extractor.py#L150)
- signature: `class TestViewName:`
- members:
  - `test_fallback_to_children(self)` — [`L161`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_class_view_extractor.py#L161)
  - `test_from_text_succeeds(self)` — [`L151`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_class_view_extractor.py#L151)
  - `test_no_name_found(self)` — [`L178`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_class_view_extractor.py#L178)
- uses (calls/refs, reference-scoped): [`_view_name`](../../../tree_sitter_analyzer/languages/sql_plugin/_class_view_extractor.md#_view_name)

### `TestViewNameFromChildren`
- def: [`tests/unit/languages/test_class_view_extractor.py:81`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_class_view_extractor.py#L81)
- signature: `class TestViewNameFromChildren:`
- members:
  - `test_empty_children(self)` — [`L123`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_class_view_extractor.py#L123)
  - `test_no_object_reference(self)` — [`L98`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_class_view_extractor.py#L98)
  - `test_object_reference_with_identifier(self)` — [`L82`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_class_view_extractor.py#L82)
  - `test_object_reference_without_identifier(self)` — [`L109`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_class_view_extractor.py#L109)
  - `test_reserved_identifier_rejected(self)` — [`L131`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_class_view_extractor.py#L131)
- uses (calls/refs, reference-scoped): [`_view_name_from_children`](../../../tree_sitter_analyzer/languages/sql_plugin/_class_view_extractor.md#_view_name_from_children)

### `TestViewNameFromText`
- def: [`tests/unit/languages/test_class_view_extractor.py:19`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_class_view_extractor.py#L19)
- signature: `class TestViewNameFromText:`
- members:
  - `test_case_insensitive(self)` — [`L47`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_class_view_extractor.py#L47)
  - `test_create_view_if_not_exists(self)` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_class_view_extractor.py#L26)
  - `test_empty_text(self)` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_class_view_extractor.py#L32)
  - `test_invalid_identifier(self)` — [`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_class_view_extractor.py#L38)
  - `test_no_view_keyword(self)` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_class_view_extractor.py#L35)
  - `test_simple_create_view(self)` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_class_view_extractor.py#L20)
- uses (calls/refs, reference-scoped): [`_view_name_from_text`](../../../tree_sitter_analyzer/languages/sql_plugin/_class_view_extractor.md#_view_name_from_text)

