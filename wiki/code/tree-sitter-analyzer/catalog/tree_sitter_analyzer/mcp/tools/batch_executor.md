---
title: 'Module: tree_sitter_analyzer/mcp/tools/batch_executor.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/batch_executor.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.batch_executor`/
symbols:
  execute_batch: execute_batch().
  BATCH_LIMITS: BATCH_LIMITS.
  _resolve_file: _resolve_file().
  _process_file_request: _process_file_request().
  _build_batch_response: _build_batch_response().
  _validate_file_request: _validate_file_request().
  _process_one_section: _process_one_section().
  _enforce_bytes_lines_limit: _enforce_bytes_lines_limit().
  _validate_batch_top_level: _validate_batch_top_level().
  _make_error_result: _make_error_result().
  _enforce_section_count_limit: _enforce_section_count_limit().
  _clamp_requests: _clamp_requests().
  _BatchAccumulator.error_count: _BatchAccumulator#error_count.
  _BatchAccumulator: _BatchAccumulator#
  _BatchAccumulator.truncated: _BatchAccumulator#truncated.
  _BatchAccumulator.ok_sections: _BatchAccumulator#ok_sections.
  _BatchAccumulator.total_bytes: _BatchAccumulator#total_bytes.
  _BatchAccumulator.total_lines: _BatchAccumulator#total_lines.
  _BatchAccumulator.sections_seen_total: _BatchAccumulator#sections_seen_total.
  _validate_section_range: _validate_section_range().
---
# Module: [`tree_sitter_analyzer/mcp/tools/batch_executor.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/batch_executor.py)

## Classes
### `_BatchAccumulator`
- def: [`tree_sitter_analyzer/mcp/tools/batch_executor.py:172`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/batch_executor.py#L172)
- doc: Running counters threaded through the batch loop.
- signature: `class _BatchAccumulator:`
- members:
  - `error_count` — [`L185`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/batch_executor.py#L185)
  - `ok_sections` — [`L183`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/batch_executor.py#L183)
  - `sections_seen_total` — [`L184`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/batch_executor.py#L184)
  - `total_bytes` — [`L181`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/batch_executor.py#L181)
  - `total_lines` — [`L182`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/batch_executor.py#L182)
  - `truncated` — [`L186`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/batch_executor.py#L186)
- used by: [`execute_batch`](batch_executor.md#execute_batch), [`_build_batch_response`](batch_executor.md#_build_batch_response), [`_process_file_request`](batch_executor.md#_process_file_request), [`_process_one_section`](batch_executor.md#_process_one_section), [`_enforce_bytes_lines_limit`](batch_executor.md#_enforce_bytes_lines_limit), [`_enforce_section_count_limit`](batch_executor.md#_enforce_section_count_limit)

## Functions
- `_build_batch_response(results: list[dict[str, Any]], acc: _BatchAccumulator, output_format: str, *, fail_fast: bool)` — [`L411`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/batch_executor.py#L411) — Compose the canonical batch envelope + apply TOON formatting.
- `_clamp_requests(requests: list[Any], allow_truncate: bool)` — [`L42`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/batch_executor.py#L42) — Truncate request list to max_files limit if allow_truncate is set.
- `_enforce_bytes_lines_limit(acc: _BatchAccumulator, content_bytes: int, content_lines: int, allow_truncate: bool)` — [`L293`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/batch_executor.py#L293) — Check ``max_total_bytes`` / ``max_total_lines`` ceilings.
- `_enforce_section_count_limit(acc: _BatchAccumulator, allow_truncate: bool)` — [`L274`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/batch_executor.py#L274) — K7: check the ``max_sections_total`` ceiling.
- `_make_error_result(file_path: str, resolved_path: str, error: str)` — [`L58`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/batch_executor.py#L58) — Build a standard error result dict for a file request.
- `_process_file_request(*, file_req: Any, tool: BaseMCPTool, acc: _BatchAccumulator, fail_fast: bool, allow_truncate: bool, content_format: str, read_file_partial_fn: Callable[..., str | None])` — [`L227`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/batch_executor.py#L227) — Validate one file request, resolve its path, then process every section.
- `_process_one_section(*, section: Any, resolved: str | None, file_result: dict[str, Any], acc: _BatchAccumulator, fail_fast: bool, allow_truncate: bool, content_format: str, read_file_partial_fn: Callable[..., str | None])` — [`L324`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/batch_executor.py#L324) — Process one section. Return True when the caller should ``break``.
- `_resolve_file(tool: BaseMCPTool, file_path: str, fail_fast: bool)` — [`L129`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/batch_executor.py#L129) — Resolve file path. Returns (resolved_path, error_result).
- `_validate_batch_top_level(arguments: dict[str, Any])` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/batch_executor.py#L24) — Validate top-level batch arguments for mutual exclusivity.
- `_validate_file_request(file_req: Any, fail_fast: bool, allow_truncate: bool)` — [`L71`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/batch_executor.py#L71) — Validate a single file request. Returns (file_path, sections, error_result, truncated).
- `_validate_section_range(label: Any, start_line: Any, end_line: Any)` — [`L398`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/batch_executor.py#L398) — Return an error dict on bad start/end_line, else ``None``.
- `execute_batch(tool: BaseMCPTool, arguments: dict[str, Any], read_file_partial_fn: Callable[..., str | None])` — [`L189`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/batch_executor.py#L189) — Batch mode for extracting multiple ranges from multiple files. — documented in [tree_sitter_analyzer-mcp-tools-read_partial_tool](../../../../concepts/tree_sitter_analyzer-mcp-tools-read_partial_tool.md)

## Module values
- `BATCH_LIMITS` — [`L13`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/batch_executor.py#L13)

