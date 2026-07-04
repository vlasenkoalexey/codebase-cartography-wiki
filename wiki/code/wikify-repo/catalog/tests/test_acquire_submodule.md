---
title: 'Module: tests/test_acquire_submodule.py'
type: catalog
provenance: extracted
module: tests/test_acquire_submodule.py
status: fresh
symbol_base: scip-python python wikify-repo 0.0.0 `tests.test_acquire_submodule`/
symbols:
  _git: _git().
  test_wiki_subdir_defaults_to_code_and_is_configurable: test_wiki_subdir_defaults_to_code_and_is_configurable().
  test_submodule_mode_adds_gitlink: test_submodule_mode_adds_gitlink().
  test_clone_mode_is_default: test_clone_mode_is_default().
  test_local_source_under_raw_code_makes_no_symlink: test_local_source_under_raw_code_makes_no_symlink().
  test_config_parses_acquire_field: test_config_parses_acquire_field().
  test_local_source_outside_raw_code_makes_relative_symlink: test_local_source_outside_raw_code_makes_relative_symlink().
  _make_source_repo: _make_source_repo().
---
# Module: [`tests/test_acquire_submodule.py`](../../../../../raw/code/wikify-repo/tests/test_acquire_submodule.py)

## Functions
- `_git(args, cwd)` — [`L16`](../../../../../raw/code/wikify-repo/tests/test_acquire_submodule.py#L16)
- `_make_source_repo(path: Path)` — [`L21`](../../../../../raw/code/wikify-repo/tests/test_acquire_submodule.py#L21)
- `test_clone_mode_is_default(tmp_path)` — [`L82`](../../../../../raw/code/wikify-repo/tests/test_acquire_submodule.py#L82) — documented in [wikify-acquire](../../concepts/wikify-acquire.md)
- `test_config_parses_acquire_field(tmp_path)` — [`L32`](../../../../../raw/code/wikify-repo/tests/test_acquire_submodule.py#L32) — documented in [wikify-config](../../concepts/wikify-config.md)
- `test_local_source_outside_raw_code_makes_relative_symlink(tmp_path)` — [`L108`](../../../../../raw/code/wikify-repo/tests/test_acquire_submodule.py#L108) — documented in [wikify-acquire](../../concepts/wikify-acquire.md)
- `test_local_source_under_raw_code_makes_no_symlink(tmp_path)` — [`L92`](../../../../../raw/code/wikify-repo/tests/test_acquire_submodule.py#L92) — documented in [wikify-acquire](../../concepts/wikify-acquire.md)
- `test_submodule_mode_adds_gitlink(tmp_path, monkeypatch)` — [`L57`](../../../../../raw/code/wikify-repo/tests/test_acquire_submodule.py#L57) — documented in [wikify-acquire](../../concepts/wikify-acquire.md)
- `test_wiki_subdir_defaults_to_code_and_is_configurable(tmp_path)` — [`L40`](../../../../../raw/code/wikify-repo/tests/test_acquire_submodule.py#L40) — documented in [wikify-config](../../concepts/wikify-config.md)

