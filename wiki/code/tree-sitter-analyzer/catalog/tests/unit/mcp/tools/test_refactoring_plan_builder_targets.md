---
title: 'Module: tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.tools.test_refactoring_plan_builder_targets`/Test
symbols:
  TestBuildExtractionTarget.test_target_fields: BuildExtractionTarget#test_target_fields().
  TestExtractionTargetContext.test_creation: ExtractionTargetContext#test_creation().
  TestExtractionTargetContext.test_frozen: ExtractionTargetContext#test_frozen().
  TestExtractionTargetContext.test_equality: ExtractionTargetContext#test_equality().
  TestBuildPrecisePlans.test_none_analysis_returns_early: BuildPrecisePlans#test_none_analysis_returns_early().
  TestBuildPrecisePlans.test_no_matching_function: BuildPrecisePlans#test_no_matching_function().
  TestBuildPrecisePlans.test_skips_non_long_function_suggestions: BuildPrecisePlans#test_skips_non_long_function_suggestions().
  TestBuildPrecisePlans.test_skips_suggestions_without_line_range: BuildPrecisePlans#test_skips_suggestions_without_line_range().
  TestBuildPlanForFunc.test_returns_none_for_no_blocks: BuildPlanForFunc#test_returns_none_for_no_blocks().
  TestBuildPlanForFunc.test_returns_plan_for_extractable_function: BuildPlanForFunc#test_returns_plan_for_extractable_function().
  TestBuildPlanForFunc.test_helper_module_in_plan: BuildPlanForFunc#test_helper_module_in_plan().
  TestBuildExtractionTargets.test_builds_targets_for_blocks: BuildExtractionTargets#test_builds_targets_for_blocks().
  TestBuildExtractionTargets.test_limits_to_three_targets: BuildExtractionTargets#test_limits_to_three_targets().
  TestHelperModuleStem.test_simple_file: HelperModuleStem#test_simple_file().
  TestHelperModuleStem.test_private_file: HelperModuleStem#test_private_file().
  TestHelperModuleStem.test_deeply_nested: HelperModuleStem#test_deeply_nested().
  TestHelperModuleStem.test_all_underscores: HelperModuleStem#test_all_underscores().
  TestHelperModulePath.test_current_dir: HelperModulePath#test_current_dir().
  TestHelperModulePath.test_nested_dir: HelperModulePath#test_nested_dir().
  TestHelperModulePath.test_deep_nested: HelperModulePath#test_deep_nested().
  TestHelperImportStatement.test_without_init: HelperImportStatement#test_without_init().
  TestHelperImportStatement.test_with_init: HelperImportStatement#test_with_init().
  TestFindExtractableBlocks.test_empty_lines: FindExtractableBlocks#test_empty_lines().
  TestFindExtractableBlocks.test_no_indented_body: FindExtractableBlocks#test_no_indented_body().
  TestFindExtractableBlocks.test_finds_loop_block: FindExtractableBlocks#test_finds_loop_block().
  TestFindExtractableBlocks.test_finds_conditional_block: FindExtractableBlocks#test_finds_conditional_block().
  TestFindExtractableBlocks.test_finds_computation_block_with_continuation: FindExtractableBlocks#test_finds_computation_block_with_continuation().
  TestFindExtractableBlocks.test_blocks_sorted_by_size_descending: FindExtractableBlocks#test_blocks_sorted_by_size_descending().
  TestFindExtractableBlocks.test_short_blocks_excluded: FindExtractableBlocks#test_short_blocks_excluded().
  TestFindExtractableBlocks.test_absolute_start_offset: FindExtractableBlocks#test_absolute_start_offset().
  TestNextExtractableBlock.test_empty_line_skipped: NextExtractableBlock#test_empty_line_skipped().
  TestNextExtractableBlock.test_comment_line_skipped: NextExtractableBlock#test_comment_line_skipped().
  TestNextExtractableBlock.test_wrong_indent_skipped: NextExtractableBlock#test_wrong_indent_skipped().
  TestNextExtractableBlock.test_valid_block_returned: NextExtractableBlock#test_valid_block_returned().
  TestScanBlockEnd.test_stops_at_lower_indent: ScanBlockEnd#test_stops_at_lower_indent().
  TestScanBlockEnd.test_stops_at_same_indent_non_continuation: ScanBlockEnd#test_stops_at_same_indent_non_continuation().
  TestScanBlockEnd.test_continues_through_blank_lines: ScanBlockEnd#test_continues_through_blank_lines().
  TestScanBlockEnd.test_all_lines_consumed: ScanBlockEnd#test_all_lines_consumed().
  TestBodyIndent.test_first_indented_line: BodyIndent#test_first_indented_line().
  TestBodyIndent.test_skips_blank_lines: BodyIndent#test_skips_blank_lines().
  TestBodyIndent.test_skips_comments: BodyIndent#test_skips_comments().
  TestBodyIndent.test_no_body: BodyIndent#test_no_body().
  TestClassifyLine.test_classifications: ClassifyLine#test_classifications().
  TestIsBlockContinuation.test_resource_except: IsBlockContinuation#test_resource_except().
  TestIsBlockContinuation.test_resource_else: IsBlockContinuation#test_resource_else().
  TestIsBlockContinuation.test_resource_finally: IsBlockContinuation#test_resource_finally().
  TestIsBlockContinuation.test_conditional_elif: IsBlockContinuation#test_conditional_elif().
  TestIsBlockContinuation.test_conditional_else: IsBlockContinuation#test_conditional_else().
  TestIsBlockContinuation.test_unrelated_hint: IsBlockContinuation#test_unrelated_hint().
  TestIsBlockContinuation.test_unrelated_line: IsBlockContinuation#test_unrelated_line().
  TestExtractionTargetContext: ExtractionTargetContext#
  TestBuildPrecisePlans: BuildPrecisePlans#
  TestBuildPlanForFunc: BuildPlanForFunc#
  TestBuildExtractionTargets: BuildExtractionTargets#
  TestBuildExtractionTarget: BuildExtractionTarget#
  TestHelperModuleStem: HelperModuleStem#
  TestHelperModulePath: HelperModulePath#
  TestHelperImportStatement: HelperImportStatement#
  TestFindExtractableBlocks: FindExtractableBlocks#
  TestNextExtractableBlock: NextExtractableBlock#
  TestScanBlockEnd: ScanBlockEnd#
  TestBodyIndent: BodyIndent#
  TestClassifyLine: ClassifyLine#
  TestIsBlockContinuation: IsBlockContinuation#
---
# Module: [`tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py)

## Classes
### `TestBodyIndent`
- def: [`tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py:406`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py#L406)
- signature: `class TestBodyIndent:`
- members:
  - `test_first_indented_line(self)` — [`L407`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py#L407)
  - `test_no_body(self)` — [`L419`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py#L419)
  - `test_skips_blank_lines(self)` — [`L411`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py#L411)
  - `test_skips_comments(self)` — [`L415`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py#L415)
- uses (calls/refs, reference-scoped): [`_body_indent`](../../../../tree_sitter_analyzer/mcp/tools/_refactoring_plan_builder.md#_body_indent)

### `TestBuildExtractionTarget`
- def: [`tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py:164`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py#L164)
- signature: `class TestBuildExtractionTarget:`
- members:
  - `test_target_fields(self)` — [`L165`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py#L165)
- uses (calls/refs, reference-scoped): [`_build_extraction_target`](../../../../tree_sitter_analyzer/mcp/tools/_refactoring_plan_builder.md#_build_extraction_target), [`ExtractionTargetContext`](../../../../tree_sitter_analyzer/mcp/tools/_refactoring_plan_builder.md#ExtractionTargetContext), [`func_name`](../../../../tree_sitter_analyzer/mcp/tools/_refactoring_plan_builder.md#ExtractionTargetContext.func_name), [`ext`](../../../../tree_sitter_analyzer/mcp/tools/_refactoring_plan_builder.md#ExtractionTargetContext.ext), [`func_assigned`](../../../../tree_sitter_analyzer/mcp/tools/_refactoring_plan_builder.md#ExtractionTargetContext.func_assigned), [`lines`](../../../../tree_sitter_analyzer/mcp/tools/_refactoring_plan_builder.md#ExtractionTargetContext.lines)

### `TestBuildExtractionTargets`
- def: [`tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py:132`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py#L132)
- signature: `class TestBuildExtractionTargets:`
- members:
  - `test_builds_targets_for_blocks(self)` — [`L133`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py#L133)
  - `test_limits_to_three_targets(self)` — [`L152`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py#L152)
- uses (calls/refs, reference-scoped): [`_build_extraction_targets`](../../../../tree_sitter_analyzer/mcp/tools/_refactoring_plan_builder.md#_build_extraction_targets)

### `TestBuildPlanForFunc`
- def: [`tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py:79`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py#L79)
- signature: `class TestBuildPlanForFunc:`
- members:
  - `test_helper_module_in_plan(self)` — [`L112`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py#L112)
  - `test_returns_none_for_no_blocks(self)` — [`L80`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py#L80)
  - `test_returns_plan_for_extractable_function(self)` — [`L87`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py#L87)
- uses (calls/refs, reference-scoped): [`_build_plan_for_func`](../../../../tree_sitter_analyzer/mcp/tools/_refactoring_plan_builder.md#_build_plan_for_func)

### `TestBuildPrecisePlans`
- def: [`tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py:51`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py#L51)
- signature: `class TestBuildPrecisePlans:`
- members:
  - `test_no_matching_function(self)` — [`L57`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py#L57)
  - `test_none_analysis_returns_early(self)` — [`L52`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py#L52)
  - `test_skips_non_long_function_suggestions(self)` — [`L68`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py#L68)
  - `test_skips_suggestions_without_line_range(self)` — [`L73`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py#L73)
- uses (calls/refs, reference-scoped): [`build_precise_plans`](../../../../tree_sitter_analyzer/mcp/tools/_refactoring_plan_builder.md#build_precise_plans)

### `TestClassifyLine`
- def: [`tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py:424`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py#L424)
- signature: `class TestClassifyLine:`
- members:
  - `test_classifications(self, line, expected)` — [`L444`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py#L444)
- uses (calls/refs, reference-scoped): [`_classify_line`](../../../../tree_sitter_analyzer/mcp/tools/_refactoring_plan_builder.md#_classify_line)

### `TestExtractionTargetContext`
- def: [`tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py:24`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py#L24)
- signature: `class TestExtractionTargetContext:`
- members:
  - `test_creation(self)` — [`L25`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py#L25)
  - `test_equality(self)` — [`L41`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py#L41)
  - `test_frozen(self)` — [`L34`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py#L34)
- uses (calls/refs, reference-scoped): [`ExtractionTargetContext`](../../../../tree_sitter_analyzer/mcp/tools/_refactoring_plan_builder.md#ExtractionTargetContext), [`func_name`](../../../../tree_sitter_analyzer/mcp/tools/_refactoring_plan_builder.md#ExtractionTargetContext.func_name), [`ext`](../../../../tree_sitter_analyzer/mcp/tools/_refactoring_plan_builder.md#ExtractionTargetContext.ext), [`func_assigned`](../../../../tree_sitter_analyzer/mcp/tools/_refactoring_plan_builder.md#ExtractionTargetContext.func_assigned), [`lines`](../../../../tree_sitter_analyzer/mcp/tools/_refactoring_plan_builder.md#ExtractionTargetContext.lines)

### `TestFindExtractableBlocks`
- def: [`tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py:234`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py#L234)
- signature: `class TestFindExtractableBlocks:`
- members:
  - `test_absolute_start_offset(self)` — [`L315`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py#L315)
  - `test_blocks_sorted_by_size_descending(self)` — [`L286`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py#L286)
  - `test_empty_lines(self)` — [`L235`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py#L235)
  - `test_finds_computation_block_with_continuation(self)` — [`L272`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py#L272)
  - `test_finds_conditional_block(self)` — [`L257`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py#L257)
  - `test_finds_loop_block(self)` — [`L242`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py#L242)
  - `test_no_indented_body(self)` — [`L238`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py#L238)
  - `test_short_blocks_excluded(self)` — [`L306`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py#L306)
- uses (calls/refs, reference-scoped): [`_find_extractable_blocks`](../../../../tree_sitter_analyzer/mcp/tools/_refactoring_plan_builder.md#_find_extractable_blocks)

### `TestHelperImportStatement`
- def: [`tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py:215`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py#L215)
- signature: `class TestHelperImportStatement:`
- members:
  - `test_with_init(self, tmp_path)` — [`L224`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py#L224)
  - `test_without_init(self, tmp_path)` — [`L216`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py#L216)
- uses (calls/refs, reference-scoped): [`_helper_import_statement`](../../../../tree_sitter_analyzer/mcp/tools/_refactoring_plan_builder.md#_helper_import_statement)

### `TestHelperModulePath`
- def: [`tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py:198`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py#L198)
- signature: `class TestHelperModulePath:`
- members:
  - `test_current_dir(self)` — [`L199`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py#L199)
  - `test_deep_nested(self)` — [`L210`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py#L210)
  - `test_nested_dir(self)` — [`L203`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py#L203)
- uses (calls/refs, reference-scoped): [`_helper_module_path`](../../../../tree_sitter_analyzer/mcp/tools/_refactoring_plan_builder.md#_helper_module_path)

### `TestHelperModuleStem`
- def: [`tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py:184`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py#L184)
- signature: `class TestHelperModuleStem:`
- members:
  - `test_all_underscores(self)` — [`L194`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py#L194)
  - `test_deeply_nested(self)` — [`L191`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py#L191)
  - `test_private_file(self)` — [`L188`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py#L188)
  - `test_simple_file(self)` — [`L185`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py#L185)
- uses (calls/refs, reference-scoped): [`_helper_module_stem`](../../../../tree_sitter_analyzer/mcp/tools/_refactoring_plan_builder.md#_helper_module_stem)

### `TestIsBlockContinuation`
- def: [`tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py:448`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py#L448)
- signature: `class TestIsBlockContinuation:`
- members:
  - `test_conditional_elif(self)` — [`L458`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py#L458)
  - `test_conditional_else(self)` — [`L461`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py#L461)
  - `test_resource_else(self)` — [`L452`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py#L452)
  - `test_resource_except(self)` — [`L449`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py#L449)
  - `test_resource_finally(self)` — [`L455`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py#L455)
  - `test_unrelated_hint(self)` — [`L464`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py#L464)
  - `test_unrelated_line(self)` — [`L467`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py#L467)
- uses (calls/refs, reference-scoped): [`_is_block_continuation`](../../../../tree_sitter_analyzer/mcp/tools/_refactoring_plan_builder.md#_is_block_continuation)

### `TestNextExtractableBlock`
- def: [`tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py:330`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py#L330)
- signature: `class TestNextExtractableBlock:`
- members:
  - `test_comment_line_skipped(self)` — [`L337`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py#L337)
  - `test_empty_line_skipped(self)` — [`L331`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py#L331)
  - `test_valid_block_returned(self)` — [`L348`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py#L348)
  - `test_wrong_indent_skipped(self)` — [`L343`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py#L343)
- uses (calls/refs, reference-scoped): [`_next_extractable_block`](../../../../tree_sitter_analyzer/mcp/tools/_refactoring_plan_builder.md#_next_extractable_block)

### `TestScanBlockEnd`
- def: [`tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py:363`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py#L363)
- signature: `class TestScanBlockEnd:`
- members:
  - `test_all_lines_consumed(self)` — [`L395`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py#L395)
  - `test_continues_through_blank_lines(self)` — [`L384`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py#L384)
  - `test_stops_at_lower_indent(self)` — [`L364`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py#L364)
  - `test_stops_at_same_indent_non_continuation(self)` — [`L374`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_refactoring_plan_builder_targets.py#L374)
- uses (calls/refs, reference-scoped): [`_scan_block_end`](../../../../tree_sitter_analyzer/mcp/tools/_refactoring_plan_builder.md#_scan_block_end)

