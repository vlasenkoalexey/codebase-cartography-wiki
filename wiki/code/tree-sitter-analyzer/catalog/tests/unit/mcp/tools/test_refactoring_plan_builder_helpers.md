---
title: 'Module: tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.tools.test_refactoring_plan_builder_helpers`/Test
symbols:
  TestSuggestHelperName.test_conditional_suffix: SuggestHelperName#test_conditional_suffix().
  TestSuggestHelperName.test_loop_suffix: SuggestHelperName#test_loop_suffix().
  TestSuggestHelperName.test_resource_suffix: SuggestHelperName#test_resource_suffix().
  TestSuggestHelperName.test_computation_suffix: SuggestHelperName#test_computation_suffix().
  TestSuggestHelperName.test_result_building_suffix: SuggestHelperName#test_result_building_suffix().
  TestSuggestHelperName.test_logic_suffix: SuggestHelperName#test_logic_suffix().
  TestSuggestHelperName.test_index_zero_no_suffix_number: SuggestHelperName#test_index_zero_no_suffix_number().
  TestSuggestHelperName.test_index_nonzero_adds_number: SuggestHelperName#test_index_nonzero_adds_number().
  TestSuggestHelperName.test_private_func_stripped: SuggestHelperName#test_private_func_stripped().
  TestCollectAssignedNames.test_simple_assignment: CollectAssignedNames#test_simple_assignment().
  TestCollectAssignedNames.test_multiple_assignments: CollectAssignedNames#test_multiple_assignments().
  TestCollectAssignedNames.test_function_args: CollectAssignedNames#test_function_args().
  TestCollectAssignedNames.test_syntax_error_returns_empty: CollectAssignedNames#test_syntax_error_returns_empty().
  TestCollectAssignedNames.test_augmented_assignment: CollectAssignedNames#test_augmented_assignment().
  TestInferParamsForBlock.test_uses_outer_dep: InferParamsForBlock#test_uses_outer_dep().
  TestInferParamsForBlock.test_no_params_for_self_contained: InferParamsForBlock#test_no_params_for_self_contained().
  TestInferParamsForBlock.test_limits_to_six: InferParamsForBlock#test_limits_to_six().
  TestInferParamsForBlock.test_syntax_error_returns_empty: InferParamsForBlock#test_syntax_error_returns_empty().
  TestInferParamsForBlock.test_excludes_builtins: InferParamsForBlock#test_excludes_builtins().
  TestInferParamsForBlock.test_attribute_access: InferParamsForBlock#test_attribute_access().
  TestInferReturns.test_simple_assignment: InferReturns#test_simple_assignment().
  TestInferReturns.test_empty_source: InferReturns#test_empty_source().
  TestInferReturns.test_syntax_error: InferReturns#test_syntax_error().
  TestInferReturns.test_tuple_unpacking: InferReturns#test_tuple_unpacking().
  TestInferReturns.test_ann_assign: InferReturns#test_ann_assign().
  TestInferReturns.test_limits_to_four: InferReturns#test_limits_to_four().
  TestAssignedNamesFromStatement.test_assign: AssignedNamesFromStatement#test_assign().
  TestAssignedNamesFromStatement.test_ann_assign: AssignedNamesFromStatement#test_ann_assign().
  TestAssignedNamesFromStatement.test_aug_assign: AssignedNamesFromStatement#test_aug_assign().
  TestAssignedNamesFromStatement.test_non_assignment: AssignedNamesFromStatement#test_non_assignment().
  TestAssignedNamesFromTarget.test_name_target: AssignedNamesFromTarget#test_name_target().
  TestAssignedNamesFromTarget.test_tuple_target: AssignedNamesFromTarget#test_tuple_target().
  TestAssignedNamesFromTarget.test_subscript_target: AssignedNamesFromTarget#test_subscript_target().
  TestAssignedNamesFromTargets.test_multiple_targets: AssignedNamesFromTargets#test_multiple_targets().
  TestAssignedNamesFromStatements.test_multiple_statements: AssignedNamesFromStatements#test_multiple_statements().
  TestAssignedNamesFromStatementAndBody.test_try_body: AssignedNamesFromStatementAndBody#test_try_body().
  TestAssignedNamesFromStatementAndBody.test_with_body: AssignedNamesFromStatementAndBody#test_with_body().
  TestAssignedNamesFromStatementAndBody.test_if_body: AssignedNamesFromStatementAndBody#test_if_body().
  TestAssignedNamesFromStatementAndBody.test_regular_statement: AssignedNamesFromStatementAndBody#test_regular_statement().
  TestNestedBodiesForReturnInference.test_try: NestedBodiesForReturnInference#test_try().
  TestNestedBodiesForReturnInference.test_with: NestedBodiesForReturnInference#test_with().
  TestNestedBodiesForReturnInference.test_async_with: NestedBodiesForReturnInference#test_async_with().
  TestNestedBodiesForReturnInference.test_if: NestedBodiesForReturnInference#test_if().
  TestNestedBodiesForReturnInference.test_for_loop: NestedBodiesForReturnInference#test_for_loop().
  TestUniqueNames.test_deduplicates: UniqueNames#test_deduplicates().
  TestUniqueNames.test_preserves_order: UniqueNames#test_preserves_order().
  TestUniqueNames.test_empty: UniqueNames#test_empty().
  TestUniqueNames.test_single: UniqueNames#test_single().
  TestMakeSkeleton.test_python_skeleton: MakeSkeleton#test_python_skeleton().
  TestMakeSkeleton.test_python_skeleton_no_returns: MakeSkeleton#test_python_skeleton_no_returns().
  TestMakeSkeleton.test_non_python_skeleton: MakeSkeleton#test_non_python_skeleton().
  TestMakeSkeleton.test_python_skeleton_dedents: MakeSkeleton#test_python_skeleton_dedents().
  TestMakeSkeleton.test_non_python_various_extensions: MakeSkeleton#test_non_python_various_extensions().
  TestIntegration.test_full_pipeline_long_function: Integration#test_full_pipeline_long_function().
  TestIntegration.test_full_pipeline_tiny_function_returns_none: Integration#test_full_pipeline_tiny_function_returns_none().
  TestIntegration.test_full_pipeline_nested_conditionals: Integration#test_full_pipeline_nested_conditionals().
  TestSuggestHelperName: SuggestHelperName#
  TestCollectAssignedNames: CollectAssignedNames#
  TestInferParamsForBlock: InferParamsForBlock#
  TestInferReturns: InferReturns#
  TestAssignedNamesFromStatement: AssignedNamesFromStatement#
  TestAssignedNamesFromTarget: AssignedNamesFromTarget#
  TestAssignedNamesFromTargets: AssignedNamesFromTargets#
  TestAssignedNamesFromStatements: AssignedNamesFromStatements#
  TestAssignedNamesFromStatementAndBody: AssignedNamesFromStatementAndBody#
  TestNestedBodiesForReturnInference: NestedBodiesForReturnInference#
  TestUniqueNames: UniqueNames#
  TestMakeSkeleton: MakeSkeleton#
  TestIntegration: Integration#
---
# Module: [`tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py)

## Classes
### `TestAssignedNamesFromStatement`
- def: [`tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py:130`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py#L130)
- signature: `class TestAssignedNamesFromStatement:`
- members:
  - `test_ann_assign(self)` — [`L137`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py#L137)
  - `test_assign(self)` — [`L131`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py#L131)
  - `test_aug_assign(self)` — [`L143`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py#L143)
  - `test_non_assignment(self)` — [`L149`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py#L149)
- uses (calls/refs, reference-scoped): [`_assigned_names_from_statement`](../../../../tree_sitter_analyzer/mcp/tools/_refactoring_plan_builder.md#_assigned_names_from_statement)

### `TestAssignedNamesFromStatementAndBody`
- def: [`tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py:198`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py#L198)
- signature: `class TestAssignedNamesFromStatementAndBody:`
- members:
  - `test_if_body(self)` — [`L215`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py#L215)
  - `test_regular_statement(self)` — [`L223`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py#L223)
  - `test_try_body(self)` — [`L199`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py#L199)
  - `test_with_body(self)` — [`L207`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py#L207)
- uses (calls/refs, reference-scoped): [`_assigned_names_from_statement_and_body`](../../../../tree_sitter_analyzer/mcp/tools/_refactoring_plan_builder.md#_assigned_names_from_statement_and_body)

### `TestAssignedNamesFromStatements`
- def: [`tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py:188`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py#L188)
- signature: `class TestAssignedNamesFromStatements:`
- members:
  - `test_multiple_statements(self)` — [`L189`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py#L189)
- uses (calls/refs, reference-scoped): [`_assigned_names_from_statements`](../../../../tree_sitter_analyzer/mcp/tools/_refactoring_plan_builder.md#_assigned_names_from_statements)

### `TestAssignedNamesFromTarget`
- def: [`tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py:156`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py#L156)
- signature: `class TestAssignedNamesFromTarget:`
- members:
  - `test_name_target(self)` — [`L157`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py#L157)
  - `test_subscript_target(self)` — [`L171`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py#L171)
  - `test_tuple_target(self)` — [`L163`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py#L163)
- uses (calls/refs, reference-scoped): [`_assigned_names_from_target`](../../../../tree_sitter_analyzer/mcp/tools/_refactoring_plan_builder.md#_assigned_names_from_target)

### `TestAssignedNamesFromTargets`
- def: [`tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py:178`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py#L178)
- signature: `class TestAssignedNamesFromTargets:`
- members:
  - `test_multiple_targets(self)` — [`L179`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py#L179)
- uses (calls/refs, reference-scoped): [`_assigned_names_from_targets`](../../../../tree_sitter_analyzer/mcp/tools/_refactoring_plan_builder.md#_assigned_names_from_targets)

### `TestCollectAssignedNames`
- def: [`tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py:53`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py#L53)
- signature: `class TestCollectAssignedNames:`
- members:
  - `test_augmented_assignment(self)` — [`L71`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py#L71)
  - `test_function_args(self)` — [`L63`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py#L63)
  - `test_multiple_assignments(self)` — [`L57`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py#L57)
  - `test_simple_assignment(self)` — [`L54`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py#L54)
  - `test_syntax_error_returns_empty(self)` — [`L68`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py#L68)
- uses (calls/refs, reference-scoped): [`_collect_assigned_names`](../../../../tree_sitter_analyzer/mcp/tools/_refactoring_plan_builder.md#_collect_assigned_names)

### `TestInferParamsForBlock`
- def: [`tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py:75`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py#L75)
- signature: `class TestInferParamsForBlock:`
- members:
  - `test_attribute_access(self)` — [`L100`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py#L100)
  - `test_excludes_builtins(self)` — [`L94`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py#L94)
  - `test_limits_to_six(self)` — [`L86`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py#L86)
  - `test_no_params_for_self_contained(self)` — [`L81`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py#L81)
  - `test_syntax_error_returns_empty(self)` — [`L91`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py#L91)
  - `test_uses_outer_dep(self)` — [`L76`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py#L76)
- uses (calls/refs, reference-scoped): [`_infer_params_for_block`](../../../../tree_sitter_analyzer/mcp/tools/_refactoring_plan_builder.md#_infer_params_for_block)

### `TestInferReturns`
- def: [`tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py:106`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py#L106)
- signature: `class TestInferReturns:`
- members:
  - `test_ann_assign(self)` — [`L121`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py#L121)
  - `test_empty_source(self)` — [`L110`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py#L110)
  - `test_limits_to_four(self)` — [`L125`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py#L125)
  - `test_simple_assignment(self)` — [`L107`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py#L107)
  - `test_syntax_error(self)` — [`L113`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py#L113)
  - `test_tuple_unpacking(self)` — [`L116`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py#L116)
- uses (calls/refs, reference-scoped): [`_infer_returns`](../../../../tree_sitter_analyzer/mcp/tools/_refactoring_plan_builder.md#_infer_returns)

### `TestIntegration`
- def: [`tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py:317`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py#L317)
- signature: `class TestIntegration:`
- members:
  - `test_full_pipeline_long_function(self)` — [`L318`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py#L318)
  - `test_full_pipeline_nested_conditionals(self)` — [`L352`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py#L352)
  - `test_full_pipeline_tiny_function_returns_none(self)` — [`L346`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py#L346)
- uses (calls/refs, reference-scoped): [`_build_plan_for_func`](../../../../tree_sitter_analyzer/mcp/tools/_refactoring_plan_builder.md#_build_plan_for_func)

### `TestMakeSkeleton`
- def: [`tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py:283`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py#L283)
- signature: `class TestMakeSkeleton:`
- members:
  - `test_non_python_skeleton(self)` — [`L300`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py#L300)
  - `test_non_python_various_extensions(self)` — [`L311`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py#L311)
  - `test_python_skeleton(self)` — [`L284`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py#L284)
  - `test_python_skeleton_dedents(self)` — [`L304`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py#L304)
  - `test_python_skeleton_no_returns(self)` — [`L295`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py#L295)
- uses (calls/refs, reference-scoped): [`_make_skeleton`](../../../../tree_sitter_analyzer/mcp/tools/_refactoring_plan_builder.md#_make_skeleton)

### `TestNestedBodiesForReturnInference`
- def: [`tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py:232`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py#L232)
- signature: `class TestNestedBodiesForReturnInference:`
- members:
  - `test_async_with(self)` — [`L247`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py#L247)
  - `test_for_loop(self)` — [`L261`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py#L261)
  - `test_if(self)` — [`L254`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py#L254)
  - `test_try(self)` — [`L233`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py#L233)
  - `test_with(self)` — [`L240`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py#L240)
- uses (calls/refs, reference-scoped): [`_nested_bodies_for_return_inference`](../../../../tree_sitter_analyzer/mcp/tools/_refactoring_plan_builder.md#_nested_bodies_for_return_inference)

### `TestSuggestHelperName`
- def: [`tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py:22`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py#L22)
- signature: `class TestSuggestHelperName:`
- members:
  - `test_computation_suffix(self)` — [`L32`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py#L32)
  - `test_conditional_suffix(self)` — [`L23`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py#L23)
  - `test_index_nonzero_adds_number(self)` — [`L45`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py#L45)
  - `test_index_zero_no_suffix_number(self)` — [`L41`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py#L41)
  - `test_logic_suffix(self)` — [`L38`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py#L38)
  - `test_loop_suffix(self)` — [`L26`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py#L26)
  - `test_private_func_stripped(self)` — [`L49`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py#L49)
  - `test_resource_suffix(self)` — [`L29`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py#L29)
  - `test_result_building_suffix(self)` — [`L35`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py#L35)
- uses (calls/refs, reference-scoped): [`_suggest_helper_name`](../../../../tree_sitter_analyzer/mcp/tools/_refactoring_plan_builder.md#_suggest_helper_name)

### `TestUniqueNames`
- def: [`tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py:269`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py#L269)
- signature: `class TestUniqueNames:`
- members:
  - `test_deduplicates(self)` — [`L270`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py#L270)
  - `test_empty(self)` — [`L276`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py#L276)
  - `test_preserves_order(self)` — [`L273`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py#L273)
  - `test_single(self)` — [`L279`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_helpers.py#L279)
- uses (calls/refs, reference-scoped): [`_unique_names`](../../../../tree_sitter_analyzer/mcp/tools/_refactoring_plan_builder.md#_unique_names)

