---
title: 'Module: tests/unit/cli/test_registry_command.py'
type: catalog
provenance: extracted
module: tests/unit/cli/test_registry_command.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `tests.unit.cli.test_registry_command`/
symbols:
  runner: runner.
  test_registry_no_subcommand_exits_zero: test_registry_no_subcommand_exits_zero().
  test_registry_no_subcommand_shows_help: test_registry_no_subcommand_shows_help().
  test_registry_help_flag_exits_zero: test_registry_help_flag_exits_zero().
  test_registry_help_flag_shows_help: test_registry_help_flag_shows_help().
  test_registry_list_still_works: test_registry_list_still_works().
  test_registry_download_accepts_cgc_suffix: test_registry_download_accepts_cgc_suffix().
  test_registry_no_subcommand_no_error_message: test_registry_no_subcommand_no_error_message().
  test_registry_download_accepts_cgc_suffix.DummyResponse: test_registry_download_accepts_cgc_suffix().DummyResponse#
  test_registry_download_accepts_cgc_suffix.DummyResponse.status_code: test_registry_download_accepts_cgc_suffix().DummyResponse#status_code.
  test_registry_download_accepts_cgc_suffix.DummyResponse.headers: test_registry_download_accepts_cgc_suffix().DummyResponse#headers.
  test_registry_download_accepts_cgc_suffix.DummyResponse.content: test_registry_download_accepts_cgc_suffix().DummyResponse#content.
  test_registry_download_accepts_cgc_suffix.DummyResponse.raise_for_status: test_registry_download_accepts_cgc_suffix().DummyResponse#raise_for_status().
  test_registry_download_accepts_cgc_suffix.DummyResponse.iter_content: test_registry_download_accepts_cgc_suffix().DummyResponse#iter_content().
---
# Module: [`tests/unit/cli/test_registry_command.py`](../../../../../../../raw/code/codegraphcontext/tests/unit/cli/test_registry_command.py)

## Classes
### `DummyResponse`
- def: [`tests/unit/cli/test_registry_command.py:84`](../../../../../../../raw/code/codegraphcontext/tests/unit/cli/test_registry_command.py#L84)
- signature: `class DummyResponse:`
- members:
  - `iter_content(self, chunk_size=8192)` — [`L92`](../../../../../../../raw/code/codegraphcontext/tests/unit/cli/test_registry_command.py#L92)
  - `raise_for_status(self)` — [`L89`](../../../../../../../raw/code/codegraphcontext/tests/unit/cli/test_registry_command.py#L89)
  - `content` — [`L87`](../../../../../../../raw/code/codegraphcontext/tests/unit/cli/test_registry_command.py#L87)
  - `headers` — [`L86`](../../../../../../../raw/code/codegraphcontext/tests/unit/cli/test_registry_command.py#L86)
  - `status_code` — [`L85`](../../../../../../../raw/code/codegraphcontext/tests/unit/cli/test_registry_command.py#L85)
- used by: (1 test-only callers)

## Functions
- `test_registry_download_accepts_cgc_suffix(bundle_name, tmp_path)` — [`L77`](../../../../../../../raw/code/codegraphcontext/tests/unit/cli/test_registry_command.py#L77) — Running `cgc registry download` should accept names with an optional .cgc suffix.
- `test_registry_help_flag_exits_zero()` — [`L39`](../../../../../../../raw/code/codegraphcontext/tests/unit/cli/test_registry_command.py#L39) — Running `cgc registry --help` should exit with code 0.
- `test_registry_help_flag_shows_help()` — [`L47`](../../../../../../../raw/code/codegraphcontext/tests/unit/cli/test_registry_command.py#L47) — Running `cgc registry --help` should print help text.
- `test_registry_list_still_works()` — [`L57`](../../../../../../../raw/code/codegraphcontext/tests/unit/cli/test_registry_command.py#L57) — Running `cgc registry list` should still call list_bundles.
- `test_registry_no_subcommand_exits_zero()` — [`L20`](../../../../../../../raw/code/codegraphcontext/tests/unit/cli/test_registry_command.py#L20) — Running `cgc registry` without a subcommand should exit with code 0.
- `test_registry_no_subcommand_no_error_message()` — [`L117`](../../../../../../../raw/code/codegraphcontext/tests/unit/cli/test_registry_command.py#L117) — Running `cgc registry` should NOT produce an error about a missing command.
- `test_registry_no_subcommand_shows_help()` — [`L28`](../../../../../../../raw/code/codegraphcontext/tests/unit/cli/test_registry_command.py#L28) — Running `cgc registry` without a subcommand should print help text.

## Module values
- `runner` — [`L17`](../../../../../../../raw/code/codegraphcontext/tests/unit/cli/test_registry_command.py#L17)

