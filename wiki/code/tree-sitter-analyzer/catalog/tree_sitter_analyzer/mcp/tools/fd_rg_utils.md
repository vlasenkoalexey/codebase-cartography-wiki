---
title: 'Module: tree_sitter_analyzer/mcp/tools/fd_rg_utils.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/fd_rg_utils.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.fd_rg_utils`/
symbols:
  build_rg_command: build_rg_command().
  build_fd_command: build_fd_command().
  run_command_capture: run_command_capture().
  parse_size_to_bytes: parse_size_to_bytes().
  normalize_max_filesize: normalize_max_filesize().
  MAX_RESULTS_HARD_CAP: MAX_RESULTS_HARD_CAP.
  parse_rg_count_output: parse_rg_count_output().
  clamp_int: clamp_int().
  check_external_command: check_external_command().
  merge_rg_results: merge_rg_results().
  get_missing_commands: get_missing_commands().
  TempFileList.__exit__: TempFileList#__exit__().
  run_parallel_rg_searches: run_parallel_rg_searches().
  split_roots_for_parallel_processing: split_roots_for_parallel_processing().
  _kill_proc: _kill_proc().
  _merge_count_results: _merge_count_results().
  write_files_to_temp: write_files_to_temp().
  DEFAULT_RESULTS_LIMIT: DEFAULT_RESULTS_LIMIT.
  _apply_size_suffix: _apply_size_suffix().
  run_parallel_rg_searches.run_single_command: run_parallel_rg_searches().run_single_command().
  _merge_json_results: _merge_json_results().
  DEFAULT_RG_MAX_FILESIZE: DEFAULT_RG_MAX_FILESIZE.
  _SUBPROC_PIPE: _SUBPROC_PIPE.
  TempFileList: TempFileList#
  _COMMAND_EXISTS_CACHE._COMMAND_EXISTS_CACHE: _COMMAND_EXISTS_CACHE._COMMAND_EXISTS_CACHE.
  TempFileList.__enter__: TempFileList#__enter__().
  contextlib.suppress.__exit__: contextlib#suppress#__exit__().
  RG_MAX_FILESIZE_HARD_CAP_BYTES: RG_MAX_FILESIZE_HARD_CAP_BYTES.
  DEFAULT_RG_TIMEOUT_MS: DEFAULT_RG_TIMEOUT_MS.
  contextlib: contextlib#
  contextlib.suppress: contextlib#suppress#
  RG_TIMEOUT_HARD_CAP_MS: RG_TIMEOUT_HARD_CAP_MS.
  _glob_with_negation: _glob_with_negation().
  TempFileList.path: TempFileList#path.
  suppress.exceptions: suppress#exceptions.
  _merge_single_count: _merge_single_count().
  _collect_result_lines: _collect_result_lines().
  _SUFFIX_MULTIPLIERS._SUFFIX_MULTIPLIERS: _SUFFIX_MULTIPLIERS._SUFFIX_MULTIPLIERS.
  TempFileList.__init__: TempFileList#__init__().
  contextlib.suppress.__init__: contextlib#suppress#__init__().
  contextlib.suppress.__enter__: contextlib#suppress#__enter__().
---
# Module: [`tree_sitter_analyzer/mcp/tools/fd_rg_utils.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/fd_rg_utils.py)

## Classes
### `TempFileList`
- def: [`tree_sitter_analyzer/mcp/tools/fd_rg_utils.py:441`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/fd_rg_utils.py#L441)
- doc: Context manager that deletes a temporary file on exit.
- signature: `class TempFileList:`
- members:
  - `__enter__(self)` — [`L447`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/fd_rg_utils.py#L447) — Context manager for temporary file cleanup.
  - `__exit__(self, exc_type: type[BaseException] | None, exc: BaseException | None, tb: Any)` — [`L451`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/fd_rg_utils.py#L451) — Clean up temporary file on context exit.
  - `path` — [`L445`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/fd_rg_utils.py#L445)
- protocol/private: `__init__`[`L444`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/fd_rg_utils.py#L444)
- uses (calls/refs, reference-scoped): [`contextlib`](fd_rg_utils.md#contextlib), [`suppress`](fd_rg_utils.md#contextlib.suppress)
- used by: [`write_files_to_temp`](fd_rg_utils.md#write_files_to_temp)

### `contextlib`
- def: [`tree_sitter_analyzer/mcp/tools/fd_rg_utils.py:460`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/fd_rg_utils.py#L460)
- used by: [`__exit__`](fd_rg_utils.md#TempFileList.__exit__), [`_kill_proc`](fd_rg_utils.md#_kill_proc)

### `suppress`
- def: [`tree_sitter_analyzer/mcp/tools/fd_rg_utils.py:461`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/fd_rg_utils.py#L461)
- members:
  - `__exit__(self, exc_type: type | None, exc: BaseException | None, tb: Any)` — [`L470`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/fd_rg_utils.py#L470) — Suppress exc if it matches one of the registered exception types.
  - `__init__(self, *exceptions: type[BaseException])` — [`L463`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/fd_rg_utils.py#L463) — Initialize temporary file writer.
  - `exceptions` — [`L465`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/fd_rg_utils.py#L465)
- protocol/private: `__enter__`[`L467`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/fd_rg_utils.py#L467)
- used by: [`__exit__`](fd_rg_utils.md#TempFileList.__exit__), [`_kill_proc`](fd_rg_utils.md#_kill_proc)

## Functions
- `_apply_size_suffix(s: str)` — [`L81`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/fd_rg_utils.py#L81) — Apply K/M/G multiplier to a normalised size string; return None on error.
- `_collect_result_lines(rc: int, stdout: bytes)` — [`L582`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/fd_rg_utils.py#L582) — Extract JSON lines from one rg result; return (lines, had_matches).
- `_glob_with_negation(g: str)` — [`L262`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/fd_rg_utils.py#L262) — Prefix g with '!' if it is not already a negation pattern.
- `_kill_proc(proc: Any)` — [`L107`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/fd_rg_utils.py#L107) — Kill a subprocess and wait for it to exit, suppressing errors.
- `_merge_count_results(results: list[tuple[int, bytes, bytes]])` — [`L561`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/fd_rg_utils.py#L561) — Merge count-only results from multiple ripgrep executions.
- `_merge_json_results(results: list[tuple[int, bytes, bytes]])` — [`L589`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/fd_rg_utils.py#L589) — Merge JSON results from multiple ripgrep executions.
- `_merge_single_count(merged: dict[str, int], file_counts: dict[str, int])` — [`L551`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/fd_rg_utils.py#L551) — Accumulate file_counts into merged; return the number of new matches.
- `build_fd_command(*, pattern: str | None, glob: bool, types: list[str] | None, extensions: list[str] | None, exclude: list[str] | None, depth: int | None, follow_symlinks: bool, hidden: bool, no_ignore: bool, size: list[str] | None, changed_within: str | None, changed_before: str | None, full_path_match: bool, absolute: bool, limit: int | None, roots: list[str], min_depth: int | None = None, prune: bool = False, threads: int | None = None, strip_cwd_prefix: bool = False, one_file_system: bool = False, show_errors: bool = False)` — [`L152`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/fd_rg_utils.py#L152) — Build an fd command with appropriate flags.
- `build_rg_command(*, query: str, case: str | None, fixed_strings: bool, word: bool, multiline: bool, include_globs: list[str] | None, exclude_globs: list[str] | None, follow_symlinks: bool, hidden: bool, no_ignore: bool, max_filesize: str | None, context_before: int | None, context_after: int | None, encoding: str | None, max_count: int | None, timeout_ms: int | None, roots: list[str] | None, files_from: str | None, count_only_matches: bool = False, file_types: list[str] | None = None, exclude_types: list[str] | None = None, files_with_matches: bool = False, only_matching: bool = False, context: int | None = None, pcre2: bool = False, max_depth: int | None = None, sort: str | None = None, invert_match: bool = False, include_stats: bool = False)` — [`L267`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/fd_rg_utils.py#L267) — Build ripgrep command with JSON output and options.
- `check_external_command(command: str)` — [`L40`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/fd_rg_utils.py#L40) — Check if an external command is available in the system PATH.
- `clamp_int(value: int | None, default_value: int, hard_cap: int)` — [`L63`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/fd_rg_utils.py#L63) — Clamp an integer value to a safe range.
- `get_missing_commands()` — [`L53`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/fd_rg_utils.py#L53) — Get list of missing external commands required by fd/rg tools.
- `merge_rg_results(results: list[tuple[int, bytes, bytes]], count_only_mode: bool = False)` — [`L525`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/fd_rg_utils.py#L525) — Merge results from multiple ripgrep executions.
- `normalize_max_filesize(user_value: str | None)` — [`L249`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/fd_rg_utils.py#L249) — Normalize max_filesize string (e.g., '1M') to bytes.
- `parse_rg_count_output(stdout_bytes: bytes)` — [`L418`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/fd_rg_utils.py#L418) — Parse ripgrep --count-matches output and return file->count mapping.
- `parse_size_to_bytes(size_str: str)` — [`L97`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/fd_rg_utils.py#L97) — Parse ripgrep --max-filesize strings like '10M', '200K' to bytes.
- `run_command_capture(cmd: list[str], input_data: bytes | None = None, timeout_ms: int | None = None)` — [`L116`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/fd_rg_utils.py#L116) — Run a subprocess and capture output.
- `run_parallel_rg_searches(commands: list[list[str]], timeout_ms: int | None = None, max_concurrent: int = 4)` — [`L491`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/fd_rg_utils.py#L491) — Run multiple ripgrep commands in parallel with concurrency control.
- `run_single_command(cmd: list[str])` — [`L502`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/fd_rg_utils.py#L502) — Run a single command synchronously and capture output.
- `split_roots_for_parallel_processing(roots: list[str], max_chunks: int = 4)` — [`L608`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/fd_rg_utils.py#L608) — Split roots into chunks for parallel processing.
- `write_files_to_temp(files: list[str])` — [`L480`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/fd_rg_utils.py#L480) — Write file list to a temporary file for --files-from option.

## Module values
- `DEFAULT_RESULTS_LIMIT` — [`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/fd_rg_utils.py#L31)
- `DEFAULT_RG_MAX_FILESIZE` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/fd_rg_utils.py#L33)
- `DEFAULT_RG_TIMEOUT_MS` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/fd_rg_utils.py#L36)
- `MAX_RESULTS_HARD_CAP` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/fd_rg_utils.py#L30)
- `RG_MAX_FILESIZE_HARD_CAP_BYTES` — [`L34`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/fd_rg_utils.py#L34)
- `RG_TIMEOUT_HARD_CAP_MS` — [`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/fd_rg_utils.py#L37)
- `_COMMAND_EXISTS_CACHE` — [`L50`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/fd_rg_utils.py#L50)
- `_SUBPROC_PIPE` — [`L104`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/fd_rg_utils.py#L104)
- `_SUFFIX_MULTIPLIERS` — [`L74`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/fd_rg_utils.py#L74)

