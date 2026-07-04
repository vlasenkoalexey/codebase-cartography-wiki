---
title: 'Module: tests/unit/mcp/test_analyze_code_structure_helpers.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_analyze_code_structure_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_analyze_code_structure_helpers`/Test
symbols:
  TestConvertClass._make_cls: ConvertClass#_make_cls().
  TestConvertClass.test_converts_public_visibility: ConvertClass#test_converts_public_visibility().
  TestConvertClass.test_converts_package_private_visibility: ConvertClass#test_converts_package_private_visibility().
  TestConvertClass.test_converts_protected_visibility: ConvertClass#test_converts_protected_visibility().
  TestConvertClass.test_converts_private_visibility: ConvertClass#test_converts_private_visibility().
  TestConvertClass.test_convert_class_superclass_field_surfaces_as_extends: ConvertClass#test_convert_class_superclass_field_surfaces_as_extends().
  TestConvertClass.test_convert_class_interfaces_field_surfaces_as_implements: ConvertClass#test_convert_class_interfaces_field_surfaces_as_implements().
  TestConvertClass.test_convert_class_both_non_java_fields_surface: ConvertClass#test_convert_class_both_non_java_fields_surface().
  TestConvertClass.test_convert_class_java_spelling_extends_class_takes_priority: ConvertClass#test_convert_class_java_spelling_extends_class_takes_priority().
  TestResolverMockLeakGuard.test_bare_mock_outline_resolvers_safe: ResolverMockLeakGuard#test_bare_mock_outline_resolvers_safe().
  TestConvertClass._make_cls_non_java: ConvertClass#_make_cls_non_java().
  TestAnalyzeCodeStructureHelpers.test_extract_metadata_coerces_non_int_statistics_to_zero: AnalyzeCodeStructureHelpers#test_extract_metadata_coerces_non_int_statistics_to_zero().
  TestAnalyzeCodeStructureHelpers.test_extract_metadata_defaults_missing_statistics_to_zero: AnalyzeCodeStructureHelpers#test_extract_metadata_defaults_missing_statistics_to_zero().
  TestAnalyzeCodeStructureFormatting.test_format_table_uses_language_formatter_and_normalizes_newlines: AnalyzeCodeStructureFormatting#test_format_table_uses_language_formatter_and_normalizes_newlines().
  TestAnalyzeCodeStructureFormatting.test_format_table_raises_for_unsupported_format: AnalyzeCodeStructureFormatting#test_format_table_raises_for_unsupported_format().
  TestAnalyzeCodeStructureNextSteps.test_build_next_steps_prefers_complex_method: AnalyzeCodeStructureNextSteps#test_build_next_steps_prefers_complex_method().
  TestAnalyzeCodeStructureNextSteps.test_build_next_steps_handles_invalid_collections: AnalyzeCodeStructureNextSteps#test_build_next_steps_handles_invalid_collections().
  TestAnalyzeCodeStructureNextSteps.test_build_next_steps_adds_query_navigation_steps: AnalyzeCodeStructureNextSteps#test_build_next_steps_adds_query_navigation_steps().
  TestAnalyzeCodeStructureNextSteps.test_build_next_steps_uses_large_file_fallback: AnalyzeCodeStructureNextSteps#test_build_next_steps_uses_large_file_fallback().
  TestAnalyzeCodeStructureNextSteps.test_build_next_steps_caps_to_three_suggestions: AnalyzeCodeStructureNextSteps#test_build_next_steps_caps_to_three_suggestions().
  TestConvertClass.test_defaults_to_public_when_no_visibility_attr: ConvertClass#test_defaults_to_public_when_no_visibility_attr().
  TestResolverMockLeakGuard.test_bare_mock_extends_resolves_to_none: ResolverMockLeakGuard#test_bare_mock_extends_resolves_to_none().
  TestResolverMockLeakGuard.test_bare_mock_implements_resolves_to_empty: ResolverMockLeakGuard#test_bare_mock_implements_resolves_to_empty().
  TestAnalyzeCodeStructureHelpers: AnalyzeCodeStructureHelpers#
  TestAnalyzeCodeStructureFormatting: AnalyzeCodeStructureFormatting#
  TestAnalyzeCodeStructureNextSteps: AnalyzeCodeStructureNextSteps#
  TestConvertClass: ConvertClass#
  TestResolverMockLeakGuard: ResolverMockLeakGuard#
---
# Module: [`tests/unit/mcp/test_analyze_code_structure_helpers.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_helpers.py)

## Classes
### `TestAnalyzeCodeStructureFormatting`
- def: [`tests/unit/mcp/test_analyze_code_structure_helpers.py:51`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_helpers.py#L51)
- doc: Tests for module-level structure table formatting.
- signature: `class TestAnalyzeCodeStructureFormatting:`
- members:
  - `test_format_table_raises_for_unsupported_format(self)` — [`L68`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_helpers.py#L68) — Unsupported formats should fail before formatter lookup.
  - `test_format_table_uses_language_formatter_and_normalizes_newlines(self)` — [`L54`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_helpers.py#L54) — Language-backed formats should return stable LF-only text.
- uses (calls/refs, reference-scoped): [`_format_table`](../../../tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.md#_format_table)

### `TestAnalyzeCodeStructureHelpers`
- def: [`tests/unit/mcp/test_analyze_code_structure_helpers.py:18`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_helpers.py#L18)
- doc: Tests for module-level analyze_code_structure helpers.
- signature: `class TestAnalyzeCodeStructureHelpers:`
- members:
  - `test_extract_metadata_coerces_non_int_statistics_to_zero(self)` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_helpers.py#L21) — Non-integer statistics should not leak into response metadata.
  - `test_extract_metadata_defaults_missing_statistics_to_zero(self)` — [`L41`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_helpers.py#L41) — Missing statistics should produce stable zero counts.
- uses (calls/refs, reference-scoped): [`extract_metadata`](../../../tree_sitter_analyzer/mcp/tools/analyze_code_structure_helpers.md#extract_metadata)

### `TestAnalyzeCodeStructureNextSteps`
- def: [`tests/unit/mcp/test_analyze_code_structure_helpers.py:78`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_helpers.py#L78)
- doc: Tests for next-step suggestions exposed to agents.
- signature: `class TestAnalyzeCodeStructureNextSteps:`
- members:
  - `test_build_next_steps_adds_query_navigation_steps(self)` — [`L120`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_helpers.py#L120) — Larger method and class sets should route agents to query tools.
  - `test_build_next_steps_caps_to_three_suggestions(self)` — [`L158`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_helpers.py#L158) — The agent-facing response should stay compact even for busy files.
  - `test_build_next_steps_handles_invalid_collections(self)` — [`L107`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_helpers.py#L107) — Invalid structure shapes should not produce noisy suggestions.
  - `test_build_next_steps_prefers_complex_method(self)` — [`L81`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_helpers.py#L81) — Complex methods should route agents to focused section extraction.
  - `test_build_next_steps_uses_large_file_fallback(self)` — [`L138`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_helpers.py#L138) — Large files without complex methods should suggest a first read slice.
- uses (calls/refs, reference-scoped): [`_build_next_steps`](../../../tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.md#_build_next_steps)

### `TestConvertClass`
- def: [`tests/unit/mcp/test_analyze_code_structure_helpers.py:180`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_helpers.py#L180)
- doc: Tests for _convert_class — ensures class attributes are passed through.
- signature: `class TestConvertClass:`
- members:
  - `_make_cls_non_java(self, **kwargs)` — [`L221`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_helpers.py#L221) — Build a Class mock using superclass/interfaces (non-Java spellings).
  - `test_convert_class_both_non_java_fields_surface(self)` — [`L251`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_helpers.py#L251) — Both superclass= and interfaces= surface when set together.
  - `test_convert_class_interfaces_field_surfaces_as_implements(self)` — [`L245`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_helpers.py#L245) — interfaces= (non-Java spelling) must surface as implements in output.
  - `test_convert_class_java_spelling_extends_class_takes_priority(self)` — [`L258`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_helpers.py#L258) — extends_class= (Java spelling) surfaces when set, even if superclass= is also set.
  - `test_convert_class_superclass_field_surfaces_as_extends(self)` — [`L239`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_helpers.py#L239) — superclass= (non-Java spelling) must surface as extends in output.
  - `test_converts_package_private_visibility(self)` — [`L200`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_helpers.py#L200) — Package-private classes must not be reported as 'public'.
  - `test_converts_private_visibility(self)` — [`L211`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_helpers.py#L211)
  - `test_converts_protected_visibility(self)` — [`L206`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_helpers.py#L206)
  - `test_converts_public_visibility(self)` — [`L195`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_helpers.py#L195)
  - `test_defaults_to_public_when_no_visibility_attr(self)` — [`L216`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_helpers.py#L216)
- protocol/private: `_make_cls`[`L183`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_helpers.py#L183)
- uses (calls/refs, reference-scoped): [`_convert_class`](../../../tree_sitter_analyzer/mcp/tools/analyze_code_structure_helpers.md#_convert_class)

### `TestResolverMockLeakGuard`
- def: [`tests/unit/mcp/test_analyze_code_structure_helpers.py:266`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_helpers.py#L266)
- doc: A bare MagicMock (auto-generated attributes) must NOT leak its repr
- signature: `class TestResolverMockLeakGuard:`
- members:
  - `test_bare_mock_extends_resolves_to_none(self)` — [`L271`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_helpers.py#L271)
  - `test_bare_mock_implements_resolves_to_empty(self)` — [`L282`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_helpers.py#L282)
  - `test_bare_mock_outline_resolvers_safe(self)` — [`L293`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_helpers.py#L293)
- uses (calls/refs, reference-scoped): [`_resolve_class_extends`](../../../tree_sitter_analyzer/mcp/tools/analyze_code_structure_helpers.md#_resolve_class_extends), [`_resolve_class_implements`](../../../tree_sitter_analyzer/mcp/tools/analyze_code_structure_helpers.md#_resolve_class_implements), [`_resolve_extends`](../../../tree_sitter_analyzer/mcp/tools/get_code_outline_tool.md#_resolve_extends), [`_resolve_implements`](../../../tree_sitter_analyzer/mcp/tools/get_code_outline_tool.md#_resolve_implements)

