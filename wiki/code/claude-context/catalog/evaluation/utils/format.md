---
title: 'Module: evaluation/utils/format.py'
type: catalog
provenance: extracted
module: evaluation/utils/format.py
status: fresh
symbol_base: scip-python python claude-context 0.0.0 `evaluation.utils.format`/
symbols:
  create_unified_diff_file: create_unified_diff_file().
  extract_conversation_summary: extract_conversation_summary().
  extract_file_paths_from_edits: extract_file_paths_from_edits().
  generate_unified_diff: generate_unified_diff().
  calculate_total_tokens: calculate_total_tokens().
  print_token_usage: print_token_usage().
  print_conversation_summary: print_conversation_summary().
  _normalize_to_relative_path: _normalize_to_relative_path().
  extract_oracle_files_from_patch: extract_oracle_files_from_patch().
  extract_edit_calls_from_conversation_log: extract_edit_calls_from_conversation_log().
  find_line_number_for_old_string: find_line_number_for_old_string().
  truncate_long_content: truncate_long_content().
  extract_final_answer: extract_final_answer().
---
# Module: [`evaluation/utils/format.py`](../../../../../../raw/code/claude-context/evaluation/utils/format.py)

## Functions
- `_normalize_to_relative_path(file_path, codebase_path)` — [`L77`](../../../../../../raw/code/claude-context/evaluation/utils/format.py#L77) — Convert a file path to relative path based on codebase_path
- `calculate_total_tokens(response)` — [`L262`](../../../../../../raw/code/claude-context/evaluation/utils/format.py#L262) — Calculate total token usage from the response
- `create_unified_diff_file(instance_dir: str, conversation_summary: str)` — [`L231`](../../../../../../raw/code/claude-context/evaluation/utils/format.py#L231) — Create a unified diff file from conversation log content
- `extract_conversation_summary(response)` — [`L349`](../../../../../../raw/code/claude-context/evaluation/utils/format.py#L349) — Extract conversation summary and return as (summary_string, tool_stats_dict)
- `extract_edit_calls_from_conversation_log(log_content: str)` — [`L108`](../../../../../../raw/code/claude-context/evaluation/utils/format.py#L108) — Extract all edit tool calls from conversation log content
- `extract_file_paths_from_edits(response, codebase_path)` — [`L25`](../../../../../../raw/code/claude-context/evaluation/utils/format.py#L25) — Extract file paths from edit tool responses and convert to relative paths
- `extract_final_answer(response)` — [`L6`](../../../../../../raw/code/claude-context/evaluation/utils/format.py#L6) — Extract the final answer from the agent response
- `extract_oracle_files_from_patch(patch)` — [`L94`](../../../../../../raw/code/claude-context/evaluation/utils/format.py#L94) — Extract the list of oracle files from the patch field
- `find_line_number_for_old_string(file_path: str, old_string: str)` — [`L177`](../../../../../../raw/code/claude-context/evaluation/utils/format.py#L177) — Find the line number where old_string starts in the file
- `generate_unified_diff(file_path: str, old_string: str, new_string: str)` — [`L195`](../../../../../../raw/code/claude-context/evaluation/utils/format.py#L195) — Generate unified diff format for a single edit
- `print_conversation_summary(response)` — [`L443`](../../../../../../raw/code/claude-context/evaluation/utils/format.py#L443) — Print a clean summary of the conversation
- `print_token_usage(response)` — [`L325`](../../../../../../raw/code/claude-context/evaluation/utils/format.py#L325) — Print simple token usage statistics
- `truncate_long_content(content, max_lines=30)` — [`L335`](../../../../../../raw/code/claude-context/evaluation/utils/format.py#L335) — Truncate content if it exceeds max_lines

