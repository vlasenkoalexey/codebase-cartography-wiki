---
title: 'Module: tree_sitter_analyzer/file_handler.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/file_handler.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.file_handler`/
symbols:
  read_file_partial: read_file_partial().
  detect_language_from_extension: detect_language_from_extension().
  read_file_with_fallback: read_file_with_fallback().
  read_file_lines_range: read_file_lines_range().
  log_error: log_error().
  log_info: log_info().
  log_warning: log_warning().
  _slice_streaming_lines: _slice_streaming_lines().
  _apply_column_range: _apply_column_range().
  logger: logger.
  _read_file_partial_validate: _read_file_partial_validate().
  _log_partial_read_success: _log_partial_read_success().
  _clip_end_column: _clip_end_column().
  _trailing_newline: _trailing_newline().
---
# Module: [`tree_sitter_analyzer/file_handler.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/file_handler.py)

## Functions
- `_apply_column_range(selected_lines: list[str], start_column: int | None, end_column: int | None)` — [`L184`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/file_handler.py#L184) — Clip each line by ``start_column`` / ``end_column`` and rejoin.
- `_clip_end_column(line_content: str, start_column: int | None, end_column: int)` — [`L211`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/file_handler.py#L211) — Apply ``end_column`` to the final (possibly only) line of the slice.
- `_log_partial_read_success(file_path: str, start_line: int, end_line: int | None, start_column: int | None, end_column: int | None, selected_lines: list[str])` — [`L237`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/file_handler.py#L237) — Emit the success log line shared by both column-range and full-line paths.
- `_read_file_partial_validate(file_path: str, start_line: int, end_line: int | None)` — [`L139`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/file_handler.py#L139) — Return False (after logging) when the caller's args are unusable.
- `_slice_streaming_lines(file_path: str, start_line: int, end_line: int | None)` — [`L155`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/file_handler.py#L155) — Stream-read just the requested 1-indexed line range.
- `_trailing_newline(original_line: str)` — [`L226`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/file_handler.py#L226) — Return the original newline characters (handles \r\n / \n / \r).
- `detect_language_from_extension(file_path: str)` — [`L33`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/file_handler.py#L33) — Detect programming language from file extension
- `log_error(message: str, *args: object, **kwargs: object)` — [`L18`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/file_handler.py#L18) — Log error message
- `log_info(message: str, *args: object, **kwargs: object)` — [`L23`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/file_handler.py#L23) — Log info message
- `log_warning(message: str, *args: object, **kwargs: object)` — [`L28`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/file_handler.py#L28) — Log warning message
- `read_file_lines_range(file_path: str, start_line: int, end_line: int | None = None)` — [`L259`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/file_handler.py#L259) — 指定した行番号範囲でファイルの一部を読み込み（列指定なし）
- `read_file_partial(file_path: str, start_line: int, end_line: int | None = None, start_column: int | None = None, end_column: int | None = None)` — [`L99`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/file_handler.py#L99) — Read partial file content by line/column range using streaming for memory efficiency. — documented in [tree_sitter_analyzer-mcp-tools-read_partial_tool](../../concepts/tree_sitter_analyzer-mcp-tools-read_partial_tool.md)
- `read_file_with_fallback(file_path: str)` — [`L71`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/file_handler.py#L71) — Read file with encoding fallback using unified encoding utilities

## Module values
- `logger` — [`L15`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/file_handler.py#L15)

