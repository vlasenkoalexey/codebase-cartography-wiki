---
title: 'Module: tests/unit/mcp/test_fd_rg_utils_p1.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_fd_rg_utils_p1.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_fd_rg_utils_p1`/Test
symbols:
  TestCheckExternalCommand.test_check_command_caching: CheckExternalCommand#test_check_command_caching().
  TestRunCommandCapture.test_run_command_timeout: RunCommandCapture#test_run_command_timeout().
  TestCheckExternalCommand.test_check_existing_command: CheckExternalCommand#test_check_existing_command().
  TestCheckExternalCommand.test_check_nonexistent_command: CheckExternalCommand#test_check_nonexistent_command().
  TestGetMissingCommands.test_all_commands_present: GetMissingCommands#test_all_commands_present().
  TestGetMissingCommands.test_fd_missing: GetMissingCommands#test_fd_missing().
  TestGetMissingCommands.test_rg_missing: GetMissingCommands#test_rg_missing().
  TestGetMissingCommands.test_both_missing: GetMissingCommands#test_both_missing().
  TestClampInt.test_clamp_with_value: ClampInt#test_clamp_with_value().
  TestClampInt.test_clamp_below_min: ClampInt#test_clamp_below_min().
  TestClampInt.test_clamp_above_max: ClampInt#test_clamp_above_max().
  TestClampInt.test_clamp_none_value: ClampInt#test_clamp_none_value().
  TestClampInt.test_clamp_invalid_string: ClampInt#test_clamp_invalid_string().
  TestParseSizeToBytes.test_parse_kb: ParseSizeToBytes#test_parse_kb().
  TestParseSizeToBytes.test_parse_mb: ParseSizeToBytes#test_parse_mb().
  TestParseSizeToBytes.test_parse_gb: ParseSizeToBytes#test_parse_gb().
  TestParseSizeToBytes.test_parse_bytes: ParseSizeToBytes#test_parse_bytes().
  TestParseSizeToBytes.test_parse_lowercase: ParseSizeToBytes#test_parse_lowercase().
  TestParseSizeToBytes.test_parse_none: ParseSizeToBytes#test_parse_none().
  TestParseSizeToBytes.test_parse_empty_string: ParseSizeToBytes#test_parse_empty_string().
  TestParseSizeToBytes.test_parse_invalid_format: ParseSizeToBytes#test_parse_invalid_format().
  TestRunCommandCapture.test_run_command_success: RunCommandCapture#test_run_command_success().
  TestRunCommandCapture.test_run_command_failure: RunCommandCapture#test_run_command_failure().
  TestRunCommandCapture.test_run_command_not_found: RunCommandCapture#test_run_command_not_found().
  TestRunCommandCapture.test_run_command_with_input: RunCommandCapture#test_run_command_with_input().
  TestBuildFdCommand.test_build_basic_command: BuildFdCommand#test_build_basic_command().
  TestBuildFdCommand.test_build_with_glob: BuildFdCommand#test_build_with_glob().
  TestBuildFdCommand.test_build_with_full_path_match: BuildFdCommand#test_build_with_full_path_match().
  TestBuildFdCommand.test_build_with_absolute: BuildFdCommand#test_build_with_absolute().
  TestBuildFdCommand.test_build_with_follow_symlinks: BuildFdCommand#test_build_with_follow_symlinks().
  TestBuildFdCommand.test_build_with_hidden: BuildFdCommand#test_build_with_hidden().
  TestBuildFdCommand.test_build_with_no_ignore: BuildFdCommand#test_build_with_no_ignore().
  TestBuildFdCommand.test_build_with_depth: BuildFdCommand#test_build_with_depth().
  TestBuildFdCommand.test_build_with_types: BuildFdCommand#test_build_with_types().
  TestBuildFdCommand.test_build_with_extensions: BuildFdCommand#test_build_with_extensions().
  TestBuildFdCommand.test_build_with_exclude: BuildFdCommand#test_build_with_exclude().
  TestBuildFdCommand.test_build_with_size: BuildFdCommand#test_build_with_size().
  TestBuildFdCommand.test_build_with_limit: BuildFdCommand#test_build_with_limit().
  TestBuildFdCommand.test_build_without_pattern: BuildFdCommand#test_build_without_pattern().
  TestRunCommandCapture.fake_wait_for: RunCommandCapture#fake_wait_for().
  TestCheckExternalCommand: CheckExternalCommand#
  TestGetMissingCommands: GetMissingCommands#
  TestClampInt: ClampInt#
  TestParseSizeToBytes: ParseSizeToBytes#
  TestRunCommandCapture: RunCommandCapture#
  TestBuildFdCommand: BuildFdCommand#
---
# Module: [`tests/unit/mcp/test_fd_rg_utils_p1.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p1.py)

## Classes
### `TestBuildFdCommand`
- def: [`tests/unit/mcp/test_fd_rg_utils_p1.py:251`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p1.py#L251)
- doc: Tests for build_fd_command function.
- signature: `class TestBuildFdCommand:`
- members:
  - `test_build_basic_command(self)` — [`L254`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p1.py#L254) — Test building basic fd command.
  - `test_build_with_absolute(self)` — [`L324`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p1.py#L324) — Test building fd command with absolute paths.
  - `test_build_with_depth(self)` — [`L412`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p1.py#L412) — Test building fd command with depth.
  - `test_build_with_exclude(self)` — [`L483`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p1.py#L483) — Test building fd command with exclude patterns.
  - `test_build_with_extensions(self)` — [`L459`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p1.py#L459) — Test building fd command with extensions.
  - `test_build_with_follow_symlinks(self)` — [`L346`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p1.py#L346) — Test building fd command with follow symlinks.
  - `test_build_with_full_path_match(self)` — [`L302`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p1.py#L302) — Test building fd command with full path match.
  - `test_build_with_glob(self)` — [`L280`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p1.py#L280) — Test building fd command with glob.
  - `test_build_with_hidden(self)` — [`L368`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p1.py#L368) — Test building fd command with hidden files.
  - `test_build_with_limit(self)` — [`L531`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p1.py#L531) — Test building fd command with limit.
  - `test_build_with_no_ignore(self)` — [`L390`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p1.py#L390) — Test building fd command with no ignore.
  - `test_build_with_size(self)` — [`L507`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p1.py#L507) — Test building fd command with size filters.
  - `test_build_with_types(self)` — [`L435`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p1.py#L435) — Test building fd command with types.
  - `test_build_without_pattern(self)` — [`L554`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p1.py#L554) — Test building fd command without pattern.
- uses (calls/refs, reference-scoped): [`build_fd_command`](../../../tree_sitter_analyzer/mcp/tools/fd_rg_utils.md#build_fd_command)

### `TestCheckExternalCommand`
- def: [`tests/unit/mcp/test_fd_rg_utils_p1.py:17`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p1.py#L17)
- doc: Tests for check_external_command function.
- signature: `class TestCheckExternalCommand:`
- members:
  - `test_check_command_caching(self)` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p1.py#L32) — Test that command existence is cached.
  - `test_check_existing_command(self)` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p1.py#L20) — Test checking for an existing command.
  - `test_check_nonexistent_command(self)` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p1.py#L26) — Test checking for a nonexistent command.
- uses (calls/refs, reference-scoped): [`check_external_command`](../../../tree_sitter_analyzer/mcp/tools/fd_rg_utils.md#check_external_command), [`_COMMAND_EXISTS_CACHE`](../../../tree_sitter_analyzer/mcp/tools/fd_rg_utils.md#_COMMAND_EXISTS_CACHE._COMMAND_EXISTS_CACHE)

### `TestClampInt`
- def: [`tests/unit/mcp/test_fd_rg_utils_p1.py:82`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p1.py#L82)
- doc: Tests for clamp_int function.
- signature: `class TestClampInt:`
- members:
  - `test_clamp_above_max(self)` — [`L95`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p1.py#L95) — Test clamping when value is above maximum.
  - `test_clamp_below_min(self)` — [`L90`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p1.py#L90) — Test clamping when value is below minimum.
  - `test_clamp_invalid_string(self)` — [`L105`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p1.py#L105) — Test clamping with invalid string value.
  - `test_clamp_none_value(self)` — [`L100`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p1.py#L100) — Test clamping with None value.
  - `test_clamp_with_value(self)` — [`L85`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p1.py#L85) — Test clamping with a valid value.
- uses (calls/refs, reference-scoped): [`clamp_int`](../../../tree_sitter_analyzer/mcp/tools/fd_rg_utils.md#clamp_int)

### `TestGetMissingCommands`
- def: [`tests/unit/mcp/test_fd_rg_utils_p1.py:47`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p1.py#L47)
- doc: Tests for get_missing_commands function.
- signature: `class TestGetMissingCommands:`
- members:
  - `test_all_commands_present(self)` — [`L50`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p1.py#L50) — Test when all commands are present.
  - `test_both_missing(self)` — [`L74`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p1.py#L74) — Test when both commands are missing.
  - `test_fd_missing(self)` — [`L56`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p1.py#L56) — Test when fd is missing.
  - `test_rg_missing(self)` — [`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p1.py#L65) — Test when rg is missing.
- uses (calls/refs, reference-scoped): [`get_missing_commands`](../../../tree_sitter_analyzer/mcp/tools/fd_rg_utils.md#get_missing_commands)

### `TestParseSizeToBytes`
- def: [`tests/unit/mcp/test_fd_rg_utils_p1.py:111`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p1.py#L111)
- doc: Tests for parse_size_to_bytes function.
- signature: `class TestParseSizeToBytes:`
- members:
  - `test_parse_bytes(self)` — [`L129`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p1.py#L129) — Test parsing bytes.
  - `test_parse_empty_string(self)` — [`L144`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p1.py#L144) — Test parsing empty string.
  - `test_parse_gb(self)` — [`L124`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p1.py#L124) — Test parsing gigabytes.
  - `test_parse_invalid_format(self)` — [`L149`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p1.py#L149) — Test parsing invalid format.
  - `test_parse_kb(self)` — [`L114`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p1.py#L114) — Test parsing kilobytes.
  - `test_parse_lowercase(self)` — [`L134`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p1.py#L134) — Test parsing lowercase units.
  - `test_parse_mb(self)` — [`L119`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p1.py#L119) — Test parsing megabytes.
  - `test_parse_none(self)` — [`L139`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p1.py#L139) — Test parsing None.
- uses (calls/refs, reference-scoped): [`parse_size_to_bytes`](../../../tree_sitter_analyzer/mcp/tools/fd_rg_utils.md#parse_size_to_bytes)

### `TestRunCommandCapture`
- def: [`tests/unit/mcp/test_fd_rg_utils_p1.py:155`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p1.py#L155)
- doc: Tests for run_command_capture function.
- signature: `class TestRunCommandCapture:`
- members:
  - `fake_wait_for(awaitable, timeout=None)` — [`L205`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p1.py#L205)
  - `test_run_command_failure(self)` — [`L177`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p1.py#L177) — Test command execution with non-zero return code.
  - `test_run_command_not_found(self)` — [`L218`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p1.py#L218) — Test command execution when command not found.
  - `test_run_command_success(self)` — [`L159`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p1.py#L159) — Test successful command execution.
  - `test_run_command_timeout(self)` — [`L193`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p1.py#L193) — Test command execution with timeout.
  - `test_run_command_with_input(self)` — [`L232`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p1.py#L232) — Test command execution with input data.
- uses (calls/refs, reference-scoped): [`run_command_capture`](../../../tree_sitter_analyzer/mcp/tools/fd_rg_utils.md#run_command_capture)

