---
title: 'Module: tests/unit/languages/_test_c_comment_include_helpers.py'
type: catalog
provenance: extracted
module: tests/unit/languages/_test_c_comment_include_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages._test_c_comment_include_helpers`/
symbols:
  TestExtractIncludeInfo.test_system_include: TestExtractIncludeInfo#test_system_include().
  TestExtractIncludeInfo.test_local_include: TestExtractIncludeInfo#test_local_include().
  TestExtractIncludeInfo.test_line_number: TestExtractIncludeInfo#test_line_number().
  TestExtractIncludeInfo.test_path_with_subdirectory: TestExtractIncludeInfo#test_path_with_subdirectory().
  FakeNode: FakeNode#
  TestExtractIncludeInfo.test_no_match: TestExtractIncludeInfo#test_no_match().
  TestExtractIncludeInfo.test_exception_returns_none: TestExtractIncludeInfo#test_exception_returns_none().
  _get_node_text: _get_node_text().
  FakeNode.text: FakeNode#text.
  FakeNode.start_point: FakeNode#start_point.
  FakeNode.child_by_field_name: FakeNode#child_by_field_name().
  TestIncludeFromLine.test_system_include_line: TestIncludeFromLine#test_system_include_line().
  TestIncludeFromLine.test_local_include_line: TestIncludeFromLine#test_local_include_line().
  TestExtractIncludesFallback.test_single_system_include: TestExtractIncludesFallback#test_single_system_include().
  TestExtractIncludesFallback.test_mixed_includes: TestExtractIncludesFallback#test_mixed_includes().
  TestExtractIncludesFallback.test_line_numbers_correct: TestExtractIncludesFallback#test_line_numbers_correct().
  FakeNode.fields: FakeNode#fields.
  FakeNode.children: FakeNode#children.
  FakeNode.parent: FakeNode#parent.
  TestIsBlockCommentStart.test_double_slash_star: TestIsBlockCommentStart#test_double_slash_star().
  TestIsBlockCommentStart.test_single_slash_star: TestIsBlockCommentStart#test_single_slash_star().
  TestIsBlockCommentStart.test_triple_slash: TestIsBlockCommentStart#test_triple_slash().
  TestIsBlockCommentStart.test_no_comment: TestIsBlockCommentStart#test_no_comment().
  TestIsBlockCommentStart.test_empty_string: TestIsBlockCommentStart#test_empty_string().
  TestIsBlockCommentStart.test_indented_block_comment: TestIsBlockCommentStart#test_indented_block_comment().
  TestIsBlockCommentStart.test_code_line: TestIsBlockCommentStart#test_code_line().
  TestCollectBlockComment.test_single_line_block: TestCollectBlockComment#test_single_line_block().
  TestCollectBlockComment.test_multi_line_block: TestCollectBlockComment#test_multi_line_block().
  TestCollectBlockComment.test_stops_at_end_marker: TestCollectBlockComment#test_stops_at_end_marker().
  TestCollectBlockComment.test_single_line_content: TestCollectBlockComment#test_single_line_content().
  TestExtractCommentForLine.test_triple_slash_comment: TestExtractCommentForLine#test_triple_slash_comment().
  TestExtractCommentForLine.test_block_comment_above: TestExtractCommentForLine#test_block_comment_above().
  TestExtractCommentForLine.test_no_comment: TestExtractCommentForLine#test_no_comment().
  TestExtractCommentForLine.test_line_out_of_range: TestExtractCommentForLine#test_line_out_of_range().
  TestExtractCommentForLine.test_empty_lines: TestExtractCommentForLine#test_empty_lines().
  TestExtractCommentForLine.test_comment_too_far_above: TestExtractCommentForLine#test_comment_too_far_above().
  TestExtractCommentForLine.test_multi_line_block_comment: TestExtractCommentForLine#test_multi_line_block_comment().
  TestExtractCommentForLine.test_comment_within_range: TestExtractCommentForLine#test_comment_within_range().
  TestIncludePathMatch.test_angle_bracket: TestIncludePathMatch#test_angle_bracket().
  TestIncludePathMatch.test_quoted: TestIncludePathMatch#test_quoted().
  TestIncludePathMatch.test_no_match: TestIncludePathMatch#test_no_match().
  TestIncludeFromLine.test_non_include_line: TestIncludeFromLine#test_non_include_line().
  TestIncludeFromLine.test_whitespace_include: TestIncludeFromLine#test_whitespace_include().
  TestExtractIncludesFallback.test_multiple_includes: TestExtractIncludesFallback#test_multiple_includes().
  TestExtractIncludesFallback.test_no_includes: TestExtractIncludesFallback#test_no_includes().
  TestExtractIncludesFallback.test_empty_source: TestExtractIncludesFallback#test_empty_source().
  FakeNode.end_point: FakeNode#end_point.
  FakeNode.start_byte: FakeNode#start_byte.
  FakeNode.end_byte: FakeNode#end_byte.
  TestIsBlockCommentStart: TestIsBlockCommentStart#
  TestCollectBlockComment: TestCollectBlockComment#
  TestExtractCommentForLine: TestExtractCommentForLine#
  TestExtractIncludeInfo: TestExtractIncludeInfo#
  TestIncludePathMatch: TestIncludePathMatch#
  TestIncludeFromLine: TestIncludeFromLine#
  TestExtractIncludesFallback: TestExtractIncludesFallback#
---
# Module: [`tests/unit/languages/_test_c_comment_include_helpers.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_comment_include_helpers.py)

## Classes
### `FakeNode`
- def: [`tests/unit/languages/_test_c_comment_include_helpers.py:22`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_comment_include_helpers.py#L22)
- signature: `class FakeNode:`
- members:
  - `child_by_field_name(self, name: str)` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_comment_include_helpers.py#L33)
  - `children` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_comment_include_helpers.py#L25)
  - `end_byte` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_comment_include_helpers.py#L30)
  - `end_point` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_comment_include_helpers.py#L28)
  - `fields` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_comment_include_helpers.py#L26)
  - `parent` — [`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_comment_include_helpers.py#L31)
  - `start_byte` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_comment_include_helpers.py#L29)
  - `start_point` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_comment_include_helpers.py#L27)
  - `text` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_comment_include_helpers.py#L24)
- used by: (6 test-only callers)

### `TestCollectBlockComment`
- def: [`tests/unit/languages/_test_c_comment_include_helpers.py:64`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_comment_include_helpers.py#L64)
- signature: `class TestCollectBlockComment:`
- members:
  - `test_multi_line_block(self)` — [`L70`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_comment_include_helpers.py#L70)
  - `test_single_line_block(self)` — [`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_comment_include_helpers.py#L65)
  - `test_single_line_content(self)` — [`L81`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_comment_include_helpers.py#L81)
  - `test_stops_at_end_marker(self)` — [`L76`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_comment_include_helpers.py#L76)
- uses (calls/refs, reference-scoped): [`_collect_block_comment`](../../../tree_sitter_analyzer/languages/_c_comment_helpers.md#_collect_block_comment)

### `TestExtractCommentForLine`
- def: [`tests/unit/languages/_test_c_comment_include_helpers.py:87`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_comment_include_helpers.py#L87)
- signature: `class TestExtractCommentForLine:`
- members:
  - `test_block_comment_above(self)` — [`L93`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_comment_include_helpers.py#L93)
  - `test_comment_too_far_above(self)` — [`L112`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_comment_include_helpers.py#L112)
  - `test_comment_within_range(self)` — [`L122`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_comment_include_helpers.py#L122)
  - `test_empty_lines(self)` — [`L108`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_comment_include_helpers.py#L108)
  - `test_line_out_of_range(self)` — [`L103`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_comment_include_helpers.py#L103)
  - `test_multi_line_block_comment(self)` — [`L117`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_comment_include_helpers.py#L117)
  - `test_no_comment(self)` — [`L98`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_comment_include_helpers.py#L98)
  - `test_triple_slash_comment(self)` — [`L88`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_comment_include_helpers.py#L88)
- uses (calls/refs, reference-scoped): [`extract_comment_for_line`](../../../tree_sitter_analyzer/languages/_c_comment_helpers.md#extract_comment_for_line)

### `TestExtractIncludeInfo`
- def: [`tests/unit/languages/_test_c_comment_include_helpers.py:128`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_comment_include_helpers.py#L128)
- signature: `class TestExtractIncludeInfo:`
- members:
  - `test_exception_returns_none(self)` — [`L175`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_comment_include_helpers.py#L175)
  - `test_line_number(self)` — [`L155`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_comment_include_helpers.py#L155)
  - `test_local_include(self)` — [`L140`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_comment_include_helpers.py#L140)
  - `test_no_match(self)` — [`L150`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_comment_include_helpers.py#L150)
  - `test_path_with_subdirectory(self)` — [`L165`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_comment_include_helpers.py#L165)
  - `test_system_include(self)` — [`L129`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_comment_include_helpers.py#L129)
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`start_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`module_name`](../../../tree_sitter_analyzer/models/base.md#Import.module_name), [`extract_include_info`](../../../tree_sitter_analyzer/languages/_c_include_helpers.md#extract_include_info)  (4 test-only)

### `TestExtractIncludesFallback`
- def: [`tests/unit/languages/_test_c_comment_include_helpers.py:218`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_comment_include_helpers.py#L218)
- signature: `class TestExtractIncludesFallback:`
- members:
  - `test_empty_source(self)` — [`L235`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_comment_include_helpers.py#L235)
  - `test_line_numbers_correct(self)` — [`L247`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_comment_include_helpers.py#L247)
  - `test_mixed_includes(self)` — [`L239`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_comment_include_helpers.py#L239)
  - `test_multiple_includes(self)` — [`L225`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_comment_include_helpers.py#L225)
  - `test_no_includes(self)` — [`L230`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_comment_include_helpers.py#L230)
  - `test_single_system_include(self)` — [`L219`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_comment_include_helpers.py#L219)
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`start_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`extract_includes_fallback`](../../../tree_sitter_analyzer/languages/_c_include_helpers.md#extract_includes_fallback)

### `TestIncludeFromLine`
- def: [`tests/unit/languages/_test_c_comment_include_helpers.py:198`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_comment_include_helpers.py#L198)
- signature: `class TestIncludeFromLine:`
- members:
  - `test_local_include_line(self)` — [`L204`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_comment_include_helpers.py#L204)
  - `test_non_include_line(self)` — [`L209`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_comment_include_helpers.py#L209)
  - `test_system_include_line(self)` — [`L199`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_comment_include_helpers.py#L199)
  - `test_whitespace_include(self)` — [`L213`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_comment_include_helpers.py#L213)
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`_include_from_line`](../../../tree_sitter_analyzer/languages/_c_include_helpers.md#_include_from_line)

### `TestIncludePathMatch`
- def: [`tests/unit/languages/_test_c_comment_include_helpers.py:182`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_comment_include_helpers.py#L182)
- signature: `class TestIncludePathMatch:`
- members:
  - `test_angle_bracket(self)` — [`L183`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_comment_include_helpers.py#L183)
  - `test_no_match(self)` — [`L193`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_comment_include_helpers.py#L193)
  - `test_quoted(self)` — [`L188`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_comment_include_helpers.py#L188)
- uses (calls/refs, reference-scoped): [`_include_path_match`](../../../tree_sitter_analyzer/languages/_c_include_helpers.md#_include_path_match)

### `TestIsBlockCommentStart`
- def: [`tests/unit/languages/_test_c_comment_include_helpers.py:41`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_comment_include_helpers.py#L41)
- signature: `class TestIsBlockCommentStart:`
- members:
  - `test_code_line(self)` — [`L60`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_comment_include_helpers.py#L60)
  - `test_double_slash_star(self)` — [`L42`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_comment_include_helpers.py#L42)
  - `test_empty_string(self)` — [`L54`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_comment_include_helpers.py#L54)
  - `test_indented_block_comment(self)` — [`L57`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_comment_include_helpers.py#L57)
  - `test_no_comment(self)` — [`L51`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_comment_include_helpers.py#L51)
  - `test_single_slash_star(self)` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_comment_include_helpers.py#L45)
  - `test_triple_slash(self)` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_comment_include_helpers.py#L48)
- uses (calls/refs, reference-scoped): [`_is_block_comment_start`](../../../tree_sitter_analyzer/languages/_c_comment_helpers.md#_is_block_comment_start)

## Functions
- `_get_node_text(node: Any)` — [`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_comment_include_helpers.py#L37)

