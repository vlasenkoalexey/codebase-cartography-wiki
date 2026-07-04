---
title: 'Module: tests/unit/mcp/test_utils/test_file_metrics.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_utils/test_file_metrics.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_utils.test_file_metrics`/Test
symbols:
  TestFileMetrics.test_file_metrics_as_dict: FileMetrics#test_file_metrics_as_dict().
  TestFileMetrics.test_file_metrics_creation: FileMetrics#test_file_metrics_creation().
  TestFileMetrics.test_file_metrics_frozen: FileMetrics#test_file_metrics_frozen().
  TestEstimateTokens.test_estimate_tokens_simple: EstimateTokens#test_estimate_tokens_simple().
  TestEstimateTokens.test_estimate_tokens_empty: EstimateTokens#test_estimate_tokens_empty().
  TestEstimateTokens.test_estimate_tokens_whitespace_only: EstimateTokens#test_estimate_tokens_whitespace_only().
  TestEstimateTokens.test_estimate_tokens_with_keywords: EstimateTokens#test_estimate_tokens_with_keywords().
  TestEstimateTokens.test_estimate_tokens_with_operators: EstimateTokens#test_estimate_tokens_with_operators().
  TestEstimateTokens.test_estimate_tokens_with_identifiers: EstimateTokens#test_estimate_tokens_with_identifiers().
  TestEstimateTokens.test_estimate_tokens_with_numbers: EstimateTokens#test_estimate_tokens_with_numbers().
  TestComputeLineMetrics.test_compute_line_metrics_simple_code: ComputeLineMetrics#test_compute_line_metrics_simple_code().
  TestComputeLineMetrics.test_compute_line_metrics_with_blank_lines: ComputeLineMetrics#test_compute_line_metrics_with_blank_lines().
  TestComputeLineMetrics.test_compute_line_metrics_with_single_line_comments: ComputeLineMetrics#test_compute_line_metrics_with_single_line_comments().
  TestComputeLineMetrics.test_compute_line_metrics_python_comments: ComputeLineMetrics#test_compute_line_metrics_python_comments().
  TestComputeLineMetrics.test_compute_line_metrics_sql_comments: ComputeLineMetrics#test_compute_line_metrics_sql_comments().
  TestComputeLineMetrics.test_compute_line_metrics_c_style_comments: ComputeLineMetrics#test_compute_line_metrics_c_style_comments().
  TestComputeLineMetrics.test_compute_line_metrics_multiline_comment: ComputeLineMetrics#test_compute_line_metrics_multiline_comment().
  TestComputeLineMetrics.test_compute_line_metrics_multiline_comment_single_line: ComputeLineMetrics#test_compute_line_metrics_multiline_comment_single_line().
  TestComputeLineMetrics.test_compute_line_metrics_javadoc_comment: ComputeLineMetrics#test_compute_line_metrics_javadoc_comment().
  TestComputeLineMetrics.test_compute_line_metrics_javadoc_continuation: ComputeLineMetrics#test_compute_line_metrics_javadoc_continuation().
  TestComputeLineMetrics.test_compute_line_metrics_html_comment: ComputeLineMetrics#test_compute_line_metrics_html_comment().
  TestComputeLineMetrics.test_compute_line_metrics_html_multiline_comment: ComputeLineMetrics#test_compute_line_metrics_html_multiline_comment().
  TestComputeLineMetrics.test_compute_line_metrics_xml_comment: ComputeLineMetrics#test_compute_line_metrics_xml_comment().
  TestComputeLineMetrics.test_compute_line_metrics_empty_content: ComputeLineMetrics#test_compute_line_metrics_empty_content().
  TestComputeLineMetrics.test_compute_line_metrics_trailing_newline: ComputeLineMetrics#test_compute_line_metrics_trailing_newline().
  TestComputeLineMetrics.test_compute_line_metrics_mixed_content: ComputeLineMetrics#test_compute_line_metrics_mixed_content().
  TestComputeMaxNestingDepth.test_flat_module_has_zero_depth: ComputeMaxNestingDepth#test_flat_module_has_zero_depth().
  TestComputeMaxNestingDepth.test_five_level_nest_pins_exactly: ComputeMaxNestingDepth#test_five_level_nest_pins_exactly().
  TestComputeMaxNestingDepth.test_empty_content_has_zero_depth: ComputeMaxNestingDepth#test_empty_content_has_zero_depth().
  TestComputeFileMetrics.test_compute_file_metrics_max_nesting_depth: ComputeFileMetrics#test_compute_file_metrics_max_nesting_depth().
  TestComputeFileMetrics.test_compute_file_metrics_success: ComputeFileMetrics#test_compute_file_metrics_success().
  TestComputeFileMetrics.test_compute_file_metrics_cached: ComputeFileMetrics#test_compute_file_metrics_cached().
  TestComputeFileMetrics.test_compute_file_metrics_cache_miss: ComputeFileMetrics#test_compute_file_metrics_cache_miss().
  TestComputeFileMetrics.test_compute_file_metrics_file_not_found: ComputeFileMetrics#test_compute_file_metrics_file_not_found().
  TestComputeFileMetrics.test_compute_file_metrics_os_error: ComputeFileMetrics#test_compute_file_metrics_os_error().
  TestComputeFileMetrics.test_compute_file_metrics_content_hash: ComputeFileMetrics#test_compute_file_metrics_content_hash().
  TestComputeFileMetrics.test_compute_file_metrics_file_size: ComputeFileMetrics#test_compute_file_metrics_file_size().
  TestComputeFileMetrics.test_compute_file_metrics_with_language: ComputeFileMetrics#test_compute_file_metrics_with_language().
  TestComputeFileMetrics.test_compute_file_metrics_without_language: ComputeFileMetrics#test_compute_file_metrics_without_language().
  TestComputeFileMetrics.test_compute_file_metrics_with_project_root: ComputeFileMetrics#test_compute_file_metrics_with_project_root().
  TestComputeFileMetrics.test_compute_file_metrics_unicode_content: ComputeFileMetrics#test_compute_file_metrics_unicode_content().
  TestComputeFileMetrics.test_compute_file_metrics_estimated_tokens: ComputeFileMetrics#test_compute_file_metrics_estimated_tokens().
  TestIntegration.test_full_metrics_workflow: Integration#test_full_metrics_workflow().
  TestIntegration.test_cache_key_includes_content_hash: Integration#test_cache_key_includes_content_hash().
  TestIntegration.test_different_content_different_hash: Integration#test_different_content_different_hash().
  TestFileMetrics: FileMetrics#
  TestEstimateTokens: EstimateTokens#
  TestComputeLineMetrics: ComputeLineMetrics#
  TestComputeMaxNestingDepth: ComputeMaxNestingDepth#
  TestComputeFileMetrics: ComputeFileMetrics#
  TestIntegration: Integration#
---
# Module: [`tests/unit/mcp/test_utils/test_file_metrics.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_metrics.py)

## Classes
### `TestComputeFileMetrics`
- def: [`tests/unit/mcp/test_utils/test_file_metrics.py:320`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_metrics.py#L320)
- doc: Tests for compute_file_metrics function.
- signature: `class TestComputeFileMetrics:`
- members:
  - `test_compute_file_metrics_cache_miss(self, mock_get_cache, mock_read_file)` — [`L394`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_metrics.py#L394) — Test compute_file_metrics with cache miss.
  - `test_compute_file_metrics_cached(self, mock_get_cache, mock_read_file)` — [`L370`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_metrics.py#L370) — Test compute_file_metrics with cached result.
  - `test_compute_file_metrics_content_hash(self, mock_get_cache, mock_read_file)` — [`L445`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_metrics.py#L445) — Test compute_file_metrics computes content hash correctly.
  - `test_compute_file_metrics_estimated_tokens(self, mock_get_cache, mock_read_file)` — [`L549`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_metrics.py#L549) — Test compute_file_metrics estimates tokens.
  - `test_compute_file_metrics_file_not_found(self, mock_read_file)` — [`L412`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_metrics.py#L412) — Test compute_file_metrics with FileNotFoundError.
  - `test_compute_file_metrics_file_size(self, mock_get_cache, mock_read_file)` — [`L460`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_metrics.py#L460) — Test compute_file_metrics computes file size correctly.
  - `test_compute_file_metrics_max_nesting_depth(self, mock_get_cache, mock_read_file)` — [`L325`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_metrics.py#L325) — file_metrics carries max_nesting_depth pinned to the hand count (#580).
  - `test_compute_file_metrics_os_error(self, mock_read_file)` — [`L428`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_metrics.py#L428) — Test compute_file_metrics with OSError.
  - `test_compute_file_metrics_success(self, mock_get_cache, mock_read_file)` — [`L348`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_metrics.py#L348) — Test compute_file_metrics with successful file read.
  - `test_compute_file_metrics_unicode_content(self, mock_get_cache, mock_read_file)` — [`L530`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_metrics.py#L530) — Test compute_file_metrics with Unicode content.
  - `test_compute_file_metrics_with_language(self, mock_get_cache, mock_read_file)` — [`L475`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_metrics.py#L475) — Test compute_file_metrics with language parameter.
  - `test_compute_file_metrics_with_project_root(self, mock_get_cache, mock_read_file)` — [`L509`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_metrics.py#L509) — Test compute_file_metrics with project_root parameter.
  - `test_compute_file_metrics_without_language(self, mock_get_cache, mock_read_file)` — [`L491`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_metrics.py#L491) — Test compute_file_metrics without language parameter.
- uses (calls/refs, reference-scoped): [`compute_file_metrics`](../../../../tree_sitter_analyzer/mcp/utils/file_metrics.md#compute_file_metrics)

### `TestComputeLineMetrics`
- def: [`tests/unit/mcp/test_utils/test_file_metrics.py:128`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_metrics.py#L128)
- doc: Tests for _compute_line_metrics function.
- signature: `class TestComputeLineMetrics:`
- members:
  - `test_compute_line_metrics_c_style_comments(self)` — [`L178`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_metrics.py#L178) — Test line metrics with C-style comments.
  - `test_compute_line_metrics_empty_content(self)` — [`L250`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_metrics.py#L250) — Test line metrics with empty content.
  - `test_compute_line_metrics_html_comment(self)` — [`L223`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_metrics.py#L223) — Test line metrics with HTML comment.
  - `test_compute_line_metrics_html_multiline_comment(self)` — [`L232`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_metrics.py#L232) — Test line metrics with HTML multi-line comment.
  - `test_compute_line_metrics_javadoc_comment(self)` — [`L205`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_metrics.py#L205) — Test line metrics with JavaDoc comment.
  - `test_compute_line_metrics_javadoc_continuation(self)` — [`L214`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_metrics.py#L214) — Test line metrics with JavaDoc continuation lines.
  - `test_compute_line_metrics_mixed_content(self)` — [`L268`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_metrics.py#L268) — Test line metrics with mixed content.
  - `test_compute_line_metrics_multiline_comment(self)` — [`L187`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_metrics.py#L187) — Test line metrics with multi-line comment.
  - `test_compute_line_metrics_multiline_comment_single_line(self)` — [`L196`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_metrics.py#L196) — Test line metrics with multi-line comment on single line.
  - `test_compute_line_metrics_python_comments(self)` — [`L159`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_metrics.py#L159) — Test line metrics with Python comments.
  - `test_compute_line_metrics_simple_code(self)` — [`L131`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_metrics.py#L131) — Test line metrics with simple code.
  - `test_compute_line_metrics_sql_comments(self)` — [`L169`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_metrics.py#L169) — Test line metrics with SQL comments.
  - `test_compute_line_metrics_trailing_newline(self)` — [`L259`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_metrics.py#L259) — Test line metrics with trailing newline.
  - `test_compute_line_metrics_with_blank_lines(self)` — [`L140`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_metrics.py#L140) — Test line metrics with blank lines.
  - `test_compute_line_metrics_with_single_line_comments(self)` — [`L149`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_metrics.py#L149) — Test line metrics with single-line comments.
  - `test_compute_line_metrics_xml_comment(self)` — [`L241`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_metrics.py#L241) — Test line metrics with XML comment.
- uses (calls/refs, reference-scoped): [`_compute_line_metrics`](../../../../tree_sitter_analyzer/mcp/utils/file_metrics.md#_compute_line_metrics)

### `TestComputeMaxNestingDepth`
- def: [`tests/unit/mcp/test_utils/test_file_metrics.py:279`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_metrics.py#L279)
- doc: Tests for _compute_max_nesting_depth (feature #580).
- signature: `class TestComputeMaxNestingDepth:`
- members:
  - `test_empty_content_has_zero_depth(self)` — [`L315`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_metrics.py#L315) — Empty content has nesting depth 0.
  - `test_five_level_nest_pins_exactly(self)` — [`L293`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_metrics.py#L293) — A hand-built 5-level nest (def→if→if→while→for body) == 5.
  - `test_flat_module_has_zero_depth(self)` — [`L288`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_metrics.py#L288) — Top-level-only code has nesting depth 0.
- uses (calls/refs, reference-scoped): [`_compute_max_nesting_depth`](../../../../tree_sitter_analyzer/mcp/utils/file_metrics.md#_compute_max_nesting_depth)

### `TestEstimateTokens`
- def: [`tests/unit/mcp/test_utils/test_file_metrics.py:80`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_metrics.py#L80)
- doc: Tests for _estimate_tokens function.
- signature: `class TestEstimateTokens:`
- members:
  - `test_estimate_tokens_empty(self)` — [`L90`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_metrics.py#L90) — Test token estimation with empty content.
  - `test_estimate_tokens_simple(self)` — [`L83`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_metrics.py#L83) — Test token estimation with simple code.
  - `test_estimate_tokens_whitespace_only(self)` — [`L96`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_metrics.py#L96) — Test token estimation with whitespace only.
  - `test_estimate_tokens_with_identifiers(self)` — [`L115`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_metrics.py#L115) — Test token estimation with identifiers.
  - `test_estimate_tokens_with_keywords(self)` — [`L102`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_metrics.py#L102) — Test token estimation with keywords.
  - `test_estimate_tokens_with_numbers(self)` — [`L121`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_metrics.py#L121) — Test token estimation with numbers.
  - `test_estimate_tokens_with_operators(self)` — [`L109`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_metrics.py#L109) — Test token estimation with operators.
- uses (calls/refs, reference-scoped): [`_estimate_tokens`](../../../../tree_sitter_analyzer/mcp/utils/file_metrics.md#_estimate_tokens)

### `TestFileMetrics`
- def: [`tests/unit/mcp/test_utils/test_file_metrics.py:22`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_metrics.py#L22)
- doc: Tests for FileMetrics dataclass.
- signature: `class TestFileMetrics:`
- members:
  - `test_file_metrics_as_dict(self)` — [`L44`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_metrics.py#L44) — Test FileMetrics.as_dict() method.
  - `test_file_metrics_creation(self)` — [`L25`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_metrics.py#L25) — Test FileMetrics dataclass creation.
  - `test_file_metrics_frozen(self)` — [`L65`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_metrics.py#L65) — Test FileMetrics is frozen (immutable).
- uses (calls/refs, reference-scoped): [`as_dict`](../../../../tree_sitter_analyzer/mcp/utils/file_metrics.md#FileMetrics.as_dict), [`total_lines`](../../../../tree_sitter_analyzer/mcp/utils/file_metrics.md#FileMetrics.total_lines), [`blank_lines`](../../../../tree_sitter_analyzer/mcp/utils/file_metrics.md#FileMetrics.blank_lines), [`code_lines`](../../../../tree_sitter_analyzer/mcp/utils/file_metrics.md#FileMetrics.code_lines), [`comment_lines`](../../../../tree_sitter_analyzer/mcp/utils/file_metrics.md#FileMetrics.comment_lines), [`content_hash`](../../../../tree_sitter_analyzer/mcp/utils/file_metrics.md#FileMetrics.content_hash), [`estimated_tokens`](../../../../tree_sitter_analyzer/mcp/utils/file_metrics.md#FileMetrics.estimated_tokens), [`file_size_bytes`](../../../../tree_sitter_analyzer/mcp/utils/file_metrics.md#FileMetrics.file_size_bytes), [`FileMetrics`](../../../../tree_sitter_analyzer/mcp/utils/file_metrics.md#FileMetrics)

### `TestIntegration`
- def: [`tests/unit/mcp/test_utils/test_file_metrics.py:565`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_metrics.py#L565)
- doc: Integration tests for file_metrics module.
- signature: `class TestIntegration:`
- members:
  - `test_cache_key_includes_content_hash(self, mock_get_cache, mock_read_file)` — [`L608`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_metrics.py#L608) — Test cache key includes content hash.
  - `test_different_content_different_hash(self, mock_get_cache, mock_read_file)` — [`L625`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_metrics.py#L625) — Test different content produces different hash.
  - `test_full_metrics_workflow(self, mock_get_cache, mock_read_file)` — [`L570`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_metrics.py#L570) — Test complete metrics computation workflow.
- uses (calls/refs, reference-scoped): [`compute_file_metrics`](../../../../tree_sitter_analyzer/mcp/utils/file_metrics.md#compute_file_metrics)

