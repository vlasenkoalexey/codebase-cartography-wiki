---
title: 'Module: tests/unit/languages/test_go_class_method_association.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_go_class_method_association.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_go_class_method_association`/
symbols:
  _make_element: _make_element().
  TestGoSampleIntegration._build_outline_for_go_sample: TestGoSampleIntegration#_build_outline_for_go_sample().
  TestRustImplMethodAssociation._build_outline: TestRustImplMethodAssociation#_build_outline().
  TestBuildOutlineGoReceiverAssociation.test_go_method_with_pointer_receiver_nested_under_struct: TestBuildOutlineGoReceiverAssociation#test_go_method_with_pointer_receiver_nested_under_struct().
  TestBuildOutlineGoReceiverAssociation.test_go_value_receiver_nested_under_struct: TestBuildOutlineGoReceiverAssociation#test_go_value_receiver_nested_under_struct().
  TestBuildOutlineGoReceiverAssociation.test_multiple_structs_each_get_correct_methods: TestBuildOutlineGoReceiverAssociation#test_multiple_structs_each_get_correct_methods().
  TestBuildOutlineGoReceiverAssociation.test_free_function_stays_top_level: TestBuildOutlineGoReceiverAssociation#test_free_function_stays_top_level().
  TestSingleOwnershipInvariant.test_method_inside_class_range_takes_precedence_over_receiver_type: TestSingleOwnershipInvariant#test_method_inside_class_range_takes_precedence_over_receiver_type().
  TestSingleOwnershipInvariant.test_multiple_methods_never_double_counted: TestSingleOwnershipInvariant#test_multiple_methods_never_double_counted().
  TestCrossFileScopes.test_method_with_unknown_receiver_type_stays_top_level: TestCrossFileScopes#test_method_with_unknown_receiver_type_stays_top_level().
  _patch_is_elem: _patch_is_elem().
  _make_result: _make_result().
  TestBuildOutlineGoReceiverAssociation.tool: TestBuildOutlineGoReceiverAssociation#tool.
  TestMethodOwnedByClass.test_line_range_containment: TestMethodOwnedByClass#test_line_range_containment().
  TestMethodOwnedByClass.test_line_range_miss_no_receiver: TestMethodOwnedByClass#test_line_range_miss_no_receiver().
  TestMethodOwnedByClass.test_receiver_type_match_pointer: TestMethodOwnedByClass#test_receiver_type_match_pointer().
  TestMethodOwnedByClass.test_receiver_type_match_no_pointer: TestMethodOwnedByClass#test_receiver_type_match_no_pointer().
  TestMethodOwnedByClass.test_receiver_type_mismatch: TestMethodOwnedByClass#test_receiver_type_mismatch().
  TestInClassRanges.test_old_signature_still_works: TestInClassRanges#test_old_signature_still_works().
  TestInClassRanges.test_receiver_type_detected_with_class_names: TestInClassRanges#test_receiver_type_detected_with_class_names().
  TestInClassRanges.test_no_match_with_class_names: TestInClassRanges#test_no_match_with_class_names().
  TestSingleOwnershipInvariant.tool: TestSingleOwnershipInvariant#tool.
  TestRustImplMethodAssociation.RUST_SRC: TestRustImplMethodAssociation#RUST_SRC.
  TestNormalizeReceiverType.test_strips_pointer_prefix: TestNormalizeReceiverType#test_strips_pointer_prefix().
  TestNormalizeReceiverType.test_no_star_unchanged: TestNormalizeReceiverType#test_no_star_unchanged().
  TestNormalizeReceiverType.test_none_returns_none: TestNormalizeReceiverType#test_none_returns_none().
  TestBuildOutlineGoReceiverAssociation.setup_method: TestBuildOutlineGoReceiverAssociation#setup_method().
  TestSingleOwnershipInvariant.setup_method: TestSingleOwnershipInvariant#setup_method().
  TestGoSampleIntegration.test_service_struct_has_correct_method_count: TestGoSampleIntegration#test_service_struct_has_correct_method_count().
  TestGoSampleIntegration.test_worker_pool_struct_has_correct_method_count: TestGoSampleIntegration#test_worker_pool_struct_has_correct_method_count().
  TestGoSampleIntegration.test_top_level_functions_are_free_functions_only: TestGoSampleIntegration#test_top_level_functions_are_free_functions_only().
  TestGoSampleIntegration.test_total_method_count_unchanged: TestGoSampleIntegration#test_total_method_count_unchanged().
  TestGoSampleIntegration.test_interface_method_signatures_nested_under_interface: TestGoSampleIntegration#test_interface_method_signatures_nested_under_interface().
  TestRustImplMethodAssociation.test_rust_impl_method_nested_under_struct: TestRustImplMethodAssociation#test_rust_impl_method_nested_under_struct().
  TestRustImplMethodAssociation.test_rust_free_function_stays_top_level: TestRustImplMethodAssociation#test_rust_free_function_stays_top_level().
  _patch_is_elem._mock: _patch_is_elem()._mock().
  TestNormalizeReceiverType: TestNormalizeReceiverType#
  TestMethodOwnedByClass: TestMethodOwnedByClass#
  TestInClassRanges: TestInClassRanges#
  TestBuildOutlineGoReceiverAssociation: TestBuildOutlineGoReceiverAssociation#
  TestSingleOwnershipInvariant: TestSingleOwnershipInvariant#
  TestGoSampleIntegration: TestGoSampleIntegration#
  TestGoSampleIntegration._check_deps: TestGoSampleIntegration#_check_deps().
  TestCrossFileScopes: TestCrossFileScopes#
  TestRustImplMethodAssociation: TestRustImplMethodAssociation#
  TestRustImplMethodAssociation._check_deps: TestRustImplMethodAssociation#_check_deps().
---
# Module: [`tests/unit/languages/test_go_class_method_association.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_class_method_association.py)

## Classes
### `TestBuildOutlineGoReceiverAssociation`
- def: [`tests/unit/languages/test_go_class_method_association.py:195`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_class_method_association.py#L195)
- doc: End-to-end outline builder with mock Go elements.
- signature: `class TestBuildOutlineGoReceiverAssociation:`
- members:
  - `setup_method(self)` — [`L198`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_class_method_association.py#L198)
  - `test_free_function_stays_top_level(self)` — [`L279`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_class_method_association.py#L279) — NewService (no receiver) stays at top_level_functions.
  - `test_go_method_with_pointer_receiver_nested_under_struct(self)` — [`L205`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_class_method_association.py#L205) — func (s *Service) Name() should appear in Service.methods, NOT top_level_functions.
  - `test_go_value_receiver_nested_under_struct(self)` — [`L235`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_class_method_association.py#L235) — func (s Service) Get() — value receiver (no *) also associates.
  - `test_multiple_structs_each_get_correct_methods(self)` — [`L254`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_class_method_association.py#L254) — Service.methods and WorkerPool.methods stay separate.
  - `tool` — [`L203`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_class_method_association.py#L203)
- uses (calls/refs, reference-scoped): [`GetCodeOutlineTool`](../../../tree_sitter_analyzer/mcp/tools/get_code_outline_tool.md#GetCodeOutlineTool), [`_build_outline`](../../../tree_sitter_analyzer/mcp/tools/get_code_outline_tool.md#GetCodeOutlineTool._build_outline)  (3 test-only)

### `TestCrossFileScopes`
- def: [`tests/unit/languages/test_go_class_method_association.py:474`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_class_method_association.py#L474)
- doc: Known limitation: receiver_type matching is per-file only.
- signature: `class TestCrossFileScopes:`
- members:
  - `test_method_with_unknown_receiver_type_stays_top_level(self)` — [`L486`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_class_method_association.py#L486) — Method with receiver_type='Service' but NO Service class in result.
- uses (calls/refs, reference-scoped): [`GetCodeOutlineTool`](../../../tree_sitter_analyzer/mcp/tools/get_code_outline_tool.md#GetCodeOutlineTool), [`_build_outline`](../../../tree_sitter_analyzer/mcp/tools/get_code_outline_tool.md#GetCodeOutlineTool._build_outline)  (3 test-only)

### `TestGoSampleIntegration`
- def: [`tests/unit/languages/test_go_class_method_association.py:369`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_class_method_association.py#L369)
- doc: Parse examples/sample.go end-to-end and verify exact association counts.
- signature: `class TestGoSampleIntegration:`
- members:
  - `test_interface_method_signatures_nested_under_interface(self)` — [`L459`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_class_method_association.py#L459) — #588: Reader/Writer interfaces own their method signatures.
  - `test_service_struct_has_correct_method_count(self)` — [`L408`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_class_method_association.py#L408) — Service should have exactly 7 receiver methods nested under it.
  - `test_top_level_functions_are_free_functions_only(self)` — [`L434`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_class_method_association.py#L434) — top_level_functions must contain only non-receiver functions.
  - `test_total_method_count_unchanged(self)` — [`L453`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_class_method_association.py#L453) — statistics.method_count == 20: 18 receiver methods + Reader.Read and
  - `test_worker_pool_struct_has_correct_method_count(self)` — [`L422`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_class_method_association.py#L422) — WorkerPool should have exactly 4 receiver methods.
- protocol/private: `_build_outline_for_go_sample`[`L376`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_class_method_association.py#L376), `_check_deps`[`L373`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_class_method_association.py#L373)
- uses (calls/refs, reference-scoped): [`AnalysisRequest`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest), [`file_path`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest.file_path), [`GetCodeOutlineTool`](../../../tree_sitter_analyzer/mcp/tools/get_code_outline_tool.md#GetCodeOutlineTool), [`language`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest.language), [`get_analysis_engine`](../../../tree_sitter_analyzer/core/analysis_engine.md#get_analysis_engine), [`_build_outline`](../../../tree_sitter_analyzer/mcp/tools/get_code_outline_tool.md#GetCodeOutlineTool._build_outline), [`analyze`](../../../tree_sitter_analyzer/core/_analysis_engine_analysis_mixin.md#UnifiedAnalysisEngineAnalysisMixin.analyze), [`include_complexity`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest.include_complexity), [`include_details`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest.include_details)

### `TestInClassRanges`
- def: [`tests/unit/languages/test_go_class_method_association.py:157`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_class_method_association.py#L157)
- doc: _in_class_ranges helper — backward-compat and new class_names path.
- signature: `class TestInClassRanges:`
- members:
  - `test_no_match_with_class_names(self)` — [`L179`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_class_method_association.py#L179)
  - `test_old_signature_still_works(self)` — [`L160`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_class_method_association.py#L160) — No class_names → pure line-range check (backward compat).
  - `test_receiver_type_detected_with_class_names(self)` — [`L170`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_class_method_association.py#L170)
- uses (calls/refs, reference-scoped): [`_in_class_ranges`](../../../tree_sitter_analyzer/mcp/tools/get_code_outline_tool.md#_in_class_ranges)  (1 test-only)

### `TestMethodOwnedByClass`
- def: [`tests/unit/languages/test_go_class_method_association.py:109`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_class_method_association.py#L109)
- doc: _method_owned_by_class helper.
- signature: `class TestMethodOwnedByClass:`
- members:
  - `test_line_range_containment(self)` — [`L112`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_class_method_association.py#L112)
  - `test_line_range_miss_no_receiver(self)` — [`L120`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_class_method_association.py#L120)
  - `test_receiver_type_match_no_pointer(self)` — [`L138`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_class_method_association.py#L138) — Go value receiver: receiver_type='Service' → matches.
  - `test_receiver_type_match_pointer(self)` — [`L128`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_class_method_association.py#L128) — Go pointer receiver: receiver_type='*Service' → normalized 'Service' matches.
  - `test_receiver_type_mismatch(self)` — [`L147`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_class_method_association.py#L147)
- uses (calls/refs, reference-scoped): [`_method_owned_by_class`](../../../tree_sitter_analyzer/mcp/tools/get_code_outline_tool.md#_method_owned_by_class)  (1 test-only)

### `TestNormalizeReceiverType`
- def: [`tests/unit/languages/test_go_class_method_association.py:82`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_class_method_association.py#L82)
- doc: _normalize_receiver_type helper.
- signature: `class TestNormalizeReceiverType:`
- members:
  - `test_no_star_unchanged(self)` — [`L93`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_class_method_association.py#L93)
  - `test_none_returns_none(self)` — [`L100`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_class_method_association.py#L100)
  - `test_strips_pointer_prefix(self)` — [`L85`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_class_method_association.py#L85)
- uses (calls/refs, reference-scoped): [`_normalize_receiver_type`](../../../tree_sitter_analyzer/mcp/tools/get_code_outline_tool.md#_normalize_receiver_type)

### `TestRustImplMethodAssociation`
- def: [`tests/unit/languages/test_go_class_method_association.py:519`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_class_method_association.py#L519)
- doc: Rust impl-block methods should nest under their struct via receiver_type.
- signature: `class TestRustImplMethodAssociation:`
- members:
  - `test_rust_free_function_stays_top_level(self)` — [`L577`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_class_method_association.py#L577)
  - `test_rust_impl_method_nested_under_struct(self)` — [`L567`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_class_method_association.py#L567) — inc and get should appear in Counter.methods, not top_level_functions.
  - `RUST_SRC` — [`L526`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_class_method_association.py#L526)
- protocol/private: `_build_outline`[`L537`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_class_method_association.py#L537), `_check_deps`[`L523`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_class_method_association.py#L523)
- uses (calls/refs, reference-scoped): [`GetCodeOutlineTool`](../../../tree_sitter_analyzer/mcp/tools/get_code_outline_tool.md#GetCodeOutlineTool), [`_build_outline`](../../../tree_sitter_analyzer/mcp/tools/get_code_outline_tool.md#GetCodeOutlineTool._build_outline), [`RustElementExtractor`](../../../tree_sitter_analyzer/languages/rust_plugin.md#RustElementExtractor), [`extract_classes`](../../../tree_sitter_analyzer/languages/rust_plugin.md#RustElementExtractor.extract_classes), [`extract_functions`](../../../tree_sitter_analyzer/languages/rust_plugin.md#RustElementExtractor.extract_functions)

### `TestSingleOwnershipInvariant`
- def: [`tests/unit/languages/test_go_class_method_association.py:303`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_class_method_association.py#L303)
- doc: P2: Each method is assigned to exactly one class (or zero).
- signature: `class TestSingleOwnershipInvariant:`
- members:
  - `setup_method(self)` — [`L310`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_class_method_association.py#L310)
  - `test_method_inside_class_range_takes_precedence_over_receiver_type(self)` — [`L317`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_class_method_association.py#L317) — Method in A's range with receiver_type=B → goes to A, not B.
  - `test_multiple_methods_never_double_counted(self)` — [`L347`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_class_method_association.py#L347) — Three methods: two in A's range, one with A's receiver_type outside range.
  - `tool` — [`L315`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_class_method_association.py#L315)
- uses (calls/refs, reference-scoped): [`GetCodeOutlineTool`](../../../tree_sitter_analyzer/mcp/tools/get_code_outline_tool.md#GetCodeOutlineTool), [`_build_outline`](../../../tree_sitter_analyzer/mcp/tools/get_code_outline_tool.md#GetCodeOutlineTool._build_outline)  (3 test-only)

## Functions
- `_make_element(element_type: str, name: str, start: int, end: int, **kw)` — [`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_class_method_association.py#L31)
- `_make_result(elements: list, file_path: str = "/p/foo.go", language: str = "go")` — [`L53`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_class_method_association.py#L53)
- `_mock(elem, type_const)` — [`L68`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_class_method_association.py#L68)
- `_patch_is_elem()` — [`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_class_method_association.py#L65) — Patch is_element_of_type to compare element_type strings directly.

