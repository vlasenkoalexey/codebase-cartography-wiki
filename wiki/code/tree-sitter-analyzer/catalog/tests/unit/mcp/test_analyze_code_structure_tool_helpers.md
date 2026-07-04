---
title: 'Module: tests/unit/mcp/test_analyze_code_structure_tool_helpers.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_analyze_code_structure_tool_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_analyze_code_structure_tool_helpers`/
symbols:
  test_attach_agent_summary_emits_canonical_info_verdict: test_attach_agent_summary_emits_canonical_info_verdict().
  tool: tool().
  tool_with_project_root: tool_with_project_root().
  TestAnalyzeCodeStructureHelpers.test_extract_metadata_coerces_non_int_statistics_to_zero: TestAnalyzeCodeStructureHelpers#test_extract_metadata_coerces_non_int_statistics_to_zero().
  TestAnalyzeCodeStructureHelpers.test_extract_metadata_defaults_missing_statistics_to_zero: TestAnalyzeCodeStructureHelpers#test_extract_metadata_defaults_missing_statistics_to_zero().
  TestAnalyzeCodeStructureFormatting.test_format_table_uses_language_formatter_and_normalizes_newlines: TestAnalyzeCodeStructureFormatting#test_format_table_uses_language_formatter_and_normalizes_newlines().
  TestAnalyzeCodeStructureFormatting.test_format_table_raises_for_unsupported_format: TestAnalyzeCodeStructureFormatting#test_format_table_raises_for_unsupported_format().
  TestAnalyzeCodeStructureNextSteps.test_build_next_steps_prefers_complex_method: TestAnalyzeCodeStructureNextSteps#test_build_next_steps_prefers_complex_method().
  TestAnalyzeCodeStructureNextSteps.test_build_next_steps_handles_invalid_collections: TestAnalyzeCodeStructureNextSteps#test_build_next_steps_handles_invalid_collections().
  TestAnalyzeCodeStructureNextSteps.test_build_next_steps_adds_query_navigation_steps: TestAnalyzeCodeStructureNextSteps#test_build_next_steps_adds_query_navigation_steps().
  TestAnalyzeCodeStructureNextSteps.test_build_next_steps_uses_large_file_fallback: TestAnalyzeCodeStructureNextSteps#test_build_next_steps_uses_large_file_fallback().
  TestAnalyzeCodeStructureNextSteps.test_build_next_steps_caps_to_three_suggestions: TestAnalyzeCodeStructureNextSteps#test_build_next_steps_caps_to_three_suggestions().
  TestAnalyzeCodeStructureToolConvertParameters.test_convert_parameters_empty: TestAnalyzeCodeStructureToolConvertParameters#test_convert_parameters_empty().
  TestAnalyzeCodeStructureToolConvertParameters.test_convert_parameters_dict: TestAnalyzeCodeStructureToolConvertParameters#test_convert_parameters_dict().
  TestAnalyzeCodeStructureToolConvertParameters.test_convert_parameters_object: TestAnalyzeCodeStructureToolConvertParameters#test_convert_parameters_object().
  TestAnalyzeCodeStructureToolGetMethodModifiers.test_get_method_modifiers_none: TestAnalyzeCodeStructureToolGetMethodModifiers#test_get_method_modifiers_none().
  TestAnalyzeCodeStructureToolGetMethodModifiers.test_get_method_modifiers_static: TestAnalyzeCodeStructureToolGetMethodModifiers#test_get_method_modifiers_static().
  TestAnalyzeCodeStructureToolGetMethodModifiers.test_get_method_modifiers_final: TestAnalyzeCodeStructureToolGetMethodModifiers#test_get_method_modifiers_final().
  TestAnalyzeCodeStructureToolGetMethodModifiers.test_get_method_modifiers_abstract: TestAnalyzeCodeStructureToolGetMethodModifiers#test_get_method_modifiers_abstract().
  TestAnalyzeCodeStructureToolGetMethodModifiers.test_get_method_modifiers_multiple: TestAnalyzeCodeStructureToolGetMethodModifiers#test_get_method_modifiers_multiple().
  TestAnalyzeCodeStructureToolGetFieldModifiers.test_get_field_modifiers_none: TestAnalyzeCodeStructureToolGetFieldModifiers#test_get_field_modifiers_none().
  TestAnalyzeCodeStructureToolGetFieldModifiers.test_get_field_modifiers_private: TestAnalyzeCodeStructureToolGetFieldModifiers#test_get_field_modifiers_private().
  TestAnalyzeCodeStructureToolGetFieldModifiers.test_get_field_modifiers_static: TestAnalyzeCodeStructureToolGetFieldModifiers#test_get_field_modifiers_static().
  TestAnalyzeCodeStructureToolGetFieldModifiers.test_get_field_modifiers_multiple: TestAnalyzeCodeStructureToolGetFieldModifiers#test_get_field_modifiers_multiple().
  TestAnalyzeCodeStructureToolGetMethodParameters.test_get_method_parameters_empty: TestAnalyzeCodeStructureToolGetMethodParameters#test_get_method_parameters_empty().
  TestAnalyzeCodeStructureToolGetMethodParameters.test_get_method_parameters_list_of_strings: TestAnalyzeCodeStructureToolGetMethodParameters#test_get_method_parameters_list_of_strings().
  TestAnalyzeCodeStructureToolGetMethodParameters.test_get_method_parameters_list_of_dicts: TestAnalyzeCodeStructureToolGetMethodParameters#test_get_method_parameters_list_of_dicts().
  TestAnalyzeCodeStructureToolGetMethodParameters.test_get_method_parameters_mixed: TestAnalyzeCodeStructureToolGetMethodParameters#test_get_method_parameters_mixed().
  TestAnalyzeCodeStructureToolGetMethodParameters.test_get_method_parameters_compound_generic_types: TestAnalyzeCodeStructureToolGetMethodParameters#test_get_method_parameters_compound_generic_types().
  TestAnalyzeCodeStructureHelpers: TestAnalyzeCodeStructureHelpers#
  TestAnalyzeCodeStructureFormatting: TestAnalyzeCodeStructureFormatting#
  TestAnalyzeCodeStructureNextSteps: TestAnalyzeCodeStructureNextSteps#
  TestAnalyzeCodeStructureToolConvertParameters: TestAnalyzeCodeStructureToolConvertParameters#
  TestAnalyzeCodeStructureToolGetMethodModifiers: TestAnalyzeCodeStructureToolGetMethodModifiers#
  TestAnalyzeCodeStructureToolGetFieldModifiers: TestAnalyzeCodeStructureToolGetFieldModifiers#
  TestAnalyzeCodeStructureToolGetMethodParameters: TestAnalyzeCodeStructureToolGetMethodParameters#
---
# Module: [`tests/unit/mcp/test_analyze_code_structure_tool_helpers.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_helpers.py)

## Classes
### `TestAnalyzeCodeStructureFormatting`
- def: [`tests/unit/mcp/test_analyze_code_structure_tool_helpers.py:90`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_helpers.py#L90)
- doc: Tests for module-level structure table formatting.
- signature: `class TestAnalyzeCodeStructureFormatting:`
- members:
  - `test_format_table_raises_for_unsupported_format(self)` — [`L107`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_helpers.py#L107) — Unsupported formats should fail before formatter lookup.
  - `test_format_table_uses_language_formatter_and_normalizes_newlines(self)` — [`L93`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_helpers.py#L93) — Language-backed formats should return stable LF-only text.
- uses (calls/refs, reference-scoped): [`_format_table`](../../../tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.md#_format_table)

### `TestAnalyzeCodeStructureHelpers`
- def: [`tests/unit/mcp/test_analyze_code_structure_tool_helpers.py:57`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_helpers.py#L57)
- doc: Tests for module-level analyze_code_structure helpers.
- signature: `class TestAnalyzeCodeStructureHelpers:`
- members:
  - `test_extract_metadata_coerces_non_int_statistics_to_zero(self)` — [`L60`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_helpers.py#L60) — Non-integer statistics should not leak into response metadata.
  - `test_extract_metadata_defaults_missing_statistics_to_zero(self)` — [`L80`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_helpers.py#L80) — Missing statistics should produce stable zero counts.
- uses (calls/refs, reference-scoped): [`extract_metadata`](../../../tree_sitter_analyzer/mcp/tools/analyze_code_structure_helpers.md#extract_metadata)

### `TestAnalyzeCodeStructureNextSteps`
- def: [`tests/unit/mcp/test_analyze_code_structure_tool_helpers.py:117`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_helpers.py#L117)
- doc: Tests for next-step suggestions exposed to agents.
- signature: `class TestAnalyzeCodeStructureNextSteps:`
- members:
  - `test_build_next_steps_adds_query_navigation_steps(self)` — [`L159`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_helpers.py#L159) — Larger method and class sets should route agents to query tools.
  - `test_build_next_steps_caps_to_three_suggestions(self)` — [`L197`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_helpers.py#L197) — The agent-facing response should stay compact even for busy files.
  - `test_build_next_steps_handles_invalid_collections(self)` — [`L146`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_helpers.py#L146) — Invalid structure shapes should not produce noisy suggestions.
  - `test_build_next_steps_prefers_complex_method(self)` — [`L120`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_helpers.py#L120) — Complex methods should route agents to focused section extraction.
  - `test_build_next_steps_uses_large_file_fallback(self)` — [`L177`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_helpers.py#L177) — Large files without complex methods should suggest a first read slice.
- uses (calls/refs, reference-scoped): [`_build_next_steps`](../../../tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.md#_build_next_steps)

### `TestAnalyzeCodeStructureToolConvertParameters`
- def: [`tests/unit/mcp/test_analyze_code_structure_tool_helpers.py:219`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_helpers.py#L219)
- doc: Tests for _convert_parameters helper.
- signature: `class TestAnalyzeCodeStructureToolConvertParameters:`
- members:
  - `test_convert_parameters_dict(self)` — [`L227`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_helpers.py#L227) — Test converting dict parameters.
  - `test_convert_parameters_empty(self)` — [`L222`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_helpers.py#L222) — Test converting empty parameters.
  - `test_convert_parameters_object(self)` — [`L235`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_helpers.py#L235) — Test converting object parameters.
- uses (calls/refs, reference-scoped): [`_convert_parameters`](../../../tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.md#_convert_parameters)

### `TestAnalyzeCodeStructureToolGetFieldModifiers`
- def: [`tests/unit/mcp/test_analyze_code_structure_tool_helpers.py:304`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_helpers.py#L304)
- doc: Tests for _get_field_modifiers helper.
- signature: `class TestAnalyzeCodeStructureToolGetFieldModifiers:`
- members:
  - `test_get_field_modifiers_multiple(self)` — [`L339`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_helpers.py#L339) — Test getting multiple modifiers.
  - `test_get_field_modifiers_none(self)` — [`L307`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_helpers.py#L307) — Test getting modifiers with no modifiers.
  - `test_get_field_modifiers_private(self)` — [`L318`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_helpers.py#L318) — Test getting private visibility.
  - `test_get_field_modifiers_static(self)` — [`L328`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_helpers.py#L328) — Test getting static modifier.
- uses (calls/refs, reference-scoped): [`_get_field_modifiers`](../../../tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.md#_get_field_modifiers)

### `TestAnalyzeCodeStructureToolGetMethodModifiers`
- def: [`tests/unit/mcp/test_analyze_code_structure_tool_helpers.py:247`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_helpers.py#L247)
- doc: Tests for _get_method_modifiers helper.
- signature: `class TestAnalyzeCodeStructureToolGetMethodModifiers:`
- members:
  - `test_get_method_modifiers_abstract(self)` — [`L280`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_helpers.py#L280) — Test getting abstract modifier.
  - `test_get_method_modifiers_final(self)` — [`L270`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_helpers.py#L270) — Test getting final modifier.
  - `test_get_method_modifiers_multiple(self)` — [`L290`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_helpers.py#L290) — Test getting multiple modifiers.
  - `test_get_method_modifiers_none(self)` — [`L250`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_helpers.py#L250) — Test getting modifiers with no modifiers.
  - `test_get_method_modifiers_static(self)` — [`L260`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_helpers.py#L260) — Test getting static modifier.
- uses (calls/refs, reference-scoped): [`_get_method_modifiers`](../../../tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.md#_get_method_modifiers)

### `TestAnalyzeCodeStructureToolGetMethodParameters`
- def: [`tests/unit/mcp/test_analyze_code_structure_tool_helpers.py:353`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_helpers.py#L353)
- doc: Tests for _get_method_parameters helper.
- signature: `class TestAnalyzeCodeStructureToolGetMethodParameters:`
- members:
  - `test_get_method_parameters_compound_generic_types(self)` — [`L399`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_helpers.py#L399) — #576: ``name: <generic with spaces>`` must split on the FIRST ':',
  - `test_get_method_parameters_empty(self)` — [`L356`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_helpers.py#L356) — Test getting empty parameters.
  - `test_get_method_parameters_list_of_dicts(self)` — [`L376`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_helpers.py#L376) — Test getting parameters as list of dicts.
  - `test_get_method_parameters_list_of_strings(self)` — [`L364`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_helpers.py#L364) — Test getting parameters as list of strings.
  - `test_get_method_parameters_mixed(self)` — [`L386`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_helpers.py#L386) — Test getting mixed parameters.
- uses (calls/refs, reference-scoped): [`_get_method_parameters`](../../../tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.md#_get_method_parameters)

## Functions
- `test_attach_agent_summary_emits_canonical_info_verdict()` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_helpers.py#L35) — Wave 1b (audit structure-07): a successful structural analysis must emit
- `tool()` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_helpers.py#L30) — Create an AnalyzeCodeStructureTool instance for testing.
- `tool_with_project_root()` — [`L52`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_helpers.py#L52) — Create an AnalyzeCodeStructureTool instance with a project root.

