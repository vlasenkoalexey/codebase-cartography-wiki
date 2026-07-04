---
title: 'Module: tests/unit/languages/test_bash_bugs_776_777_778.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_bash_bugs_776_777_778.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_bash_bugs_776_777_778`/
symbols:
  _parse: _parse().
  TestVariableExtractionWired.test_variables_key_present_in_extract_elements: TestVariableExtractionWired#test_variables_key_present_in_extract_elements().
  TestVariableExtractionWired.test_simple_assignment_is_extracted: TestVariableExtractionWired#test_simple_assignment_is_extracted().
  TestVariableExtractionWired.test_variable_has_name_attribute: TestVariableExtractionWired#test_variable_has_name_attribute().
  TestNoPhantomElements.test_shebang_not_in_expressions: TestNoPhantomElements#test_shebang_not_in_expressions().
  TestNoPhantomElements.test_bare_exit_not_a_function: TestNoPhantomElements#test_bare_exit_not_a_function().
  TestNoPhantomElements.test_real_functions_still_extracted: TestNoPhantomElements#test_real_functions_still_extracted().
  TestCompactTableHeaderNoUnknown.test_compact_table_output_no_unknown_for_bash_data: TestCompactTableHeaderNoUnknown#test_compact_table_output_no_unknown_for_bash_data().
  TestCompactTableHeaderNoUnknown.test_no_unknown_when_classes_empty: TestCompactTableHeaderNoUnknown#test_no_unknown_when_classes_empty().
  TestCompactTableHeaderNoUnknown.test_uses_filename_stem_when_no_classes: TestCompactTableHeaderNoUnknown#test_uses_filename_stem_when_no_classes().
  TestCompactTableHeaderNoUnknown.test_class_name_still_used_when_classes_present: TestCompactTableHeaderNoUnknown#test_class_name_still_used_when_classes_present().
  TestCompactTableHeaderNoUnknown.test_package_plus_class_unchanged: TestCompactTableHeaderNoUnknown#test_package_plus_class_unchanged().
  TestVariableExtractionWired: TestVariableExtractionWired#
  TestNoPhantomElements: TestNoPhantomElements#
  TestCompactTableHeaderNoUnknown: TestCompactTableHeaderNoUnknown#
---
# Module: [`tests/unit/languages/test_bash_bugs_776_777_778.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_bash_bugs_776_777_778.py)

## Classes
### `TestCompactTableHeaderNoUnknown`
- def: [`tests/unit/languages/test_bash_bugs_776_777_778.py:94`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_bash_bugs_776_777_778.py#L94)
- doc: Bug #778: compact_table_header must not render '# Unknown' for class-less
- signature: `class TestCompactTableHeaderNoUnknown:`
- members:
  - `test_class_name_still_used_when_classes_present(self)` — [`L121`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_bash_bugs_776_777_778.py#L121) — When classes are present the class name must still be used (not filename).
  - `test_compact_table_output_no_unknown_for_bash_data(self)` — [`L147`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_bash_bugs_776_777_778.py#L147) — The full compact table output for a Bash-like structure dict must not
  - `test_no_unknown_when_classes_empty(self)` — [`L98`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_bash_bugs_776_777_778.py#L98) — compact_table_header must not return 'Unknown' when classes is [].
  - `test_package_plus_class_unchanged(self)` — [`L134`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_bash_bugs_776_777_778.py#L134) — Package.ClassName format must be preserved when both are present.
  - `test_uses_filename_stem_when_no_classes(self)` — [`L110`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_bash_bugs_776_777_778.py#L110) — When classes is empty, the header must use the filename without extension.
- uses (calls/refs, reference-scoped): [`LegacyTableFormatter`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter), [`format_structure`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter.format_structure), [`compact_table_header`](../../../tree_sitter_analyzer/_legacy_table_formatter_compact.md#compact_table_header)

### `TestNoPhantomElements`
- def: [`tests/unit/languages/test_bash_bugs_776_777_778.py:59`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_bash_bugs_776_777_778.py#L59)
- doc: Bug #777: shebang must not be a 'comment'; bare commands must not be
- signature: `class TestNoPhantomElements:`
- members:
  - `test_bare_exit_not_a_function(self)` — [`L73`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_bash_bugs_776_777_778.py#L73) — A bare 'exit 0' at top-level must not be classified as a function.
  - `test_real_functions_still_extracted(self)` — [`L83`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_bash_bugs_776_777_778.py#L83) — Real function definitions must still be extracted after the fix.
  - `test_shebang_not_in_expressions(self)` — [`L63`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_bash_bugs_776_777_778.py#L63) — #!/usr/bin/env bash shebang must not appear as a comment expression.
- uses (calls/refs, reference-scoped): [`extract_elements`](../../../tree_sitter_analyzer/plugins/base.md#ElementExtractor.extract_elements), [`create_extractor`](../../../tree_sitter_analyzer/languages/bash_plugin.md#BashPlugin.create_extractor), [`extract_expressions`](../../../tree_sitter_analyzer/plugins/base.md#ElementExtractor.extract_expressions)  (1 test-only)

### `TestVariableExtractionWired`
- def: [`tests/unit/languages/test_bash_bugs_776_777_778.py:29`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_bash_bugs_776_777_778.py#L29)
- doc: Bug #776: extract_variables() must be called by the pipeline.
- signature: `class TestVariableExtractionWired:`
- members:
  - `test_simple_assignment_is_extracted(self)` — [`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_bash_bugs_776_777_778.py#L39) — A plain variable assignment must yield at least one variable entry.
  - `test_variable_has_name_attribute(self)` — [`L47`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_bash_bugs_776_777_778.py#L47) — Each extracted variable must carry the variable name.
  - `test_variables_key_present_in_extract_elements(self)` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_bash_bugs_776_777_778.py#L32) — extract_elements() must return a 'variables' key.
- uses (calls/refs, reference-scoped): [`extract_elements`](../../../tree_sitter_analyzer/plugins/base.md#ElementExtractor.extract_elements), [`create_extractor`](../../../tree_sitter_analyzer/languages/bash_plugin.md#BashPlugin.create_extractor)  (1 test-only)

## Functions
- `_parse(code: str)` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_bash_bugs_776_777_778.py#L18)

