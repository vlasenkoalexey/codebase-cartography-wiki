---
title: 'Module: tests/test_hooks.py'
type: catalog
provenance: extracted
module: tests/test_hooks.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_hooks`/
symbols:
  _make_git_repo: _make_git_repo().
  _HOOK_SCRIPTS: _HOOK_SCRIPTS.
  test_install_creates_hook: test_install_creates_hook().
  test_install_idempotent: test_install_idempotent().
  test_install_appends_to_existing_hook: test_install_appends_to_existing_hook().
  test_uninstall_removes_hook: test_uninstall_removes_hook().
  test_status_installed: test_status_installed().
  test_install_creates_post_checkout_hook: test_install_creates_post_checkout_hook().
  test_uninstall_removes_post_checkout_hook: test_uninstall_removes_post_checkout_hook().
  test_status_shows_both_hooks: test_status_shows_both_hooks().
  test_hooks_dir_resolves_relative_git_hooks_path: test_hooks_dir_resolves_relative_git_hooks_path().
  test_hooks_dir_rejects_multiline_git_output: test_hooks_dir_rejects_multiline_git_output().
  test_hooks_dir_accepts_absolute_git_hooks_path: test_hooks_dir_accepts_absolute_git_hooks_path().
  test_windows_hookspath_rejected_no_junk_dir_on_posix: test_windows_hookspath_rejected_no_junk_dir_on_posix().
  test_posix_custom_hookspath_still_works: test_posix_custom_hookspath_still_works().
  test_install_is_executable: test_install_is_executable().
  test_uninstall_no_hook: test_uninstall_no_hook().
  test_status_not_installed: test_status_not_installed().
  test_install_post_checkout_is_executable: test_install_post_checkout_is_executable().
  test_install_embeds_pinned_interpreter: test_install_embeds_pinned_interpreter().
  test_launcher_payload_is_shell_quote_safe: test_launcher_payload_is_shell_quote_safe().
  test_launcher_and_rebuild_body_are_valid_python: test_launcher_and_rebuild_body_are_valid_python().
  test_rebuild_bodies_are_shell_quote_safe: test_rebuild_bodies_are_shell_quote_safe().
  test_rebuild_bodies_read_graphify_root: test_rebuild_bodies_read_graphify_root().
  test_rebuild_bodies_with_graphify_root_are_valid_python: test_rebuild_bodies_with_graphify_root_are_valid_python().
  test_detached_launch_targets_graphify_python: test_detached_launch_targets_graphify_python().
  test_installed_hooks_contain_no_nohup: test_installed_hooks_contain_no_nohup().
  test_default_hooks_dir_unaffected: test_default_hooks_dir_unaffected().
  test_no_git_repo_raises: test_no_git_repo_raises().
  test_hook_skips_head_on_exe: test_hook_skips_head_on_exe().
  test_install_fallback_is_loud_not_silent: test_install_fallback_is_loud_not_silent().
  test_hooks_use_cross_platform_detach: test_hooks_use_cross_platform_detach().
  test_hooks_limit_windows_workers_by_default: test_hooks_limit_windows_workers_by_default().
  test_probes_use_find_spec_not_full_import: test_probes_use_find_spec_not_full_import().
  test_shebang_read_is_null_byte_safe: test_shebang_read_is_null_byte_safe().
  test_probe_prefers_sibling_python_exe_on_windows_layouts: test_probe_prefers_sibling_python_exe_on_windows_layouts().
  test_hooks_reuse_git_dir_from_env: test_hooks_reuse_git_dir_from_env().
  _launcher_payload: _launcher_payload().
  _set_hookspath: _set_hookspath().
  test_hooks_dir_resolves_relative_git_hooks_path.fake_run: test_hooks_dir_resolves_relative_git_hooks_path().fake_run().
  test_hooks_dir_rejects_multiline_git_output.fake_run: test_hooks_dir_rejects_multiline_git_output().fake_run().
  test_hooks_dir_accepts_absolute_git_hooks_path.fake_run: test_hooks_dir_accepts_absolute_git_hooks_path().fake_run().
  test_hook_check_no_additionalContext: test_hook_check_no_additionalContext().
  test_hooks_do_not_use_nohup: test_hooks_do_not_use_nohup().
---
# Module: [`tests/test_hooks.py`](../../../../../raw/code/graphify/tests/test_hooks.py)

## Functions
- `_launcher_payload(script: str)` — [`L266`](../../../../../raw/code/graphify/tests/test_hooks.py#L266) — Extract the `python -c "<payload>"` the hook hands to GRAPHIFY_PYTHON.
- `_make_git_repo(tmp_path: Path)` — [`L10`](../../../../../raw/code/graphify/tests/test_hooks.py#L10)
- `_set_hookspath(repo: Path, value: str)` — [`L352`](../../../../../raw/code/graphify/tests/test_hooks.py#L352)
- `fake_run(*args, **kwargs)` — [`L127`](../../../../../raw/code/graphify/tests/test_hooks.py#L127)
- `fake_run(*args, **kwargs)` — [`L138`](../../../../../raw/code/graphify/tests/test_hooks.py#L138)
- `fake_run(*args, **kwargs)` — [`L151`](../../../../../raw/code/graphify/tests/test_hooks.py#L151)
- `test_default_hooks_dir_unaffected(tmp_path)` — [`L385`](../../../../../raw/code/graphify/tests/test_hooks.py#L385) — No core.hooksPath -> normal .git/hooks install, no rejection.
- `test_detached_launch_targets_graphify_python()` — [`L332`](../../../../../raw/code/graphify/tests/test_hooks.py#L332) — The launcher must run via the resolved $GRAPHIFY_PYTHON, not a bare
- `test_hook_check_no_additionalContext(tmp_path)` — [`L202`](../../../../../raw/code/graphify/tests/test_hooks.py#L202) — graphify hook-check must not emit additionalContext — Codex Desktop rejects it.
- `test_hook_skips_head_on_exe()` — [`L158`](../../../../../raw/code/graphify/tests/test_hooks.py#L158) — Hook script must skip shebang extraction for .exe binaries (Windows).
- `test_hooks_dir_accepts_absolute_git_hooks_path(tmp_path, monkeypatch)` — [`L147`](../../../../../raw/code/graphify/tests/test_hooks.py#L147)
- `test_hooks_dir_rejects_multiline_git_output(tmp_path, monkeypatch)` — [`L135`](../../../../../raw/code/graphify/tests/test_hooks.py#L135)
- `test_hooks_dir_resolves_relative_git_hooks_path(tmp_path, monkeypatch)` — [`L124`](../../../../../raw/code/graphify/tests/test_hooks.py#L124)
- `test_hooks_do_not_use_nohup(name, script)` — [`L238`](../../../../../raw/code/graphify/tests/test_hooks.py#L238) — Git for Windows' bundled shell ships no `nohup`/`setsid`, so the old
- `test_hooks_limit_windows_workers_by_default(name, script)` — [`L258`](../../../../../raw/code/graphify/tests/test_hooks.py#L258) — Git for Windows/MSYS hooks can expose fragile pipe handles to spawned
- `test_hooks_reuse_git_dir_from_env(name, script)` — [`L428`](../../../../../raw/code/graphify/tests/test_hooks.py#L428) — git exports GIT_DIR to hooks, so the rev-parse fallback should only run
- `test_hooks_use_cross_platform_detach(name, script)` — [`L248`](../../../../../raw/code/graphify/tests/test_hooks.py#L248) — The replacement detaches via Python: start_new_session on POSIX and
- `test_install_appends_to_existing_hook(tmp_path)` — [`L44`](../../../../../raw/code/graphify/tests/test_hooks.py#L44)
- `test_install_creates_hook(tmp_path)` — [`L15`](../../../../../raw/code/graphify/tests/test_hooks.py#L15)
- `test_install_creates_post_checkout_hook(tmp_path)` — [`L88`](../../../../../raw/code/graphify/tests/test_hooks.py#L88)
- `test_install_embeds_pinned_interpreter(tmp_path)` — [`L164`](../../../../../raw/code/graphify/tests/test_hooks.py#L164) — Hook scripts must embed sys.executable so the hook works without the
- `test_install_fallback_is_loud_not_silent(tmp_path)` — [`L190`](../../../../../raw/code/graphify/tests/test_hooks.py#L190) — The detection fallback must emit a message to stderr rather than bare exit 0.
- `test_install_idempotent(tmp_path)` — [`L34`](../../../../../raw/code/graphify/tests/test_hooks.py#L34)
- `test_install_is_executable(tmp_path)` — [`L24`](../../../../../raw/code/graphify/tests/test_hooks.py#L24)
- `test_install_post_checkout_is_executable(tmp_path)` — [`L96`](../../../../../raw/code/graphify/tests/test_hooks.py#L96)
- `test_installed_hooks_contain_no_nohup(tmp_path)` — [`L340`](../../../../../raw/code/graphify/tests/test_hooks.py#L340) — End-to-end: the files written to .git/hooks must be nohup-free (#1161).
- `test_launcher_and_rebuild_body_are_valid_python(name, script)` — [`L288`](../../../../../raw/code/graphify/tests/test_hooks.py#L288) — Both the launcher and the rebuild body it re-executes must parse, so a
- `test_launcher_payload_is_shell_quote_safe(name, script)` — [`L278`](../../../../../raw/code/graphify/tests/test_hooks.py#L278) — The launcher is carried inside a shell double-quoted `-c "..."` argument,
- `test_no_git_repo_raises(tmp_path)` — [`L83`](../../../../../raw/code/graphify/tests/test_hooks.py#L83)
- `test_posix_custom_hookspath_still_works(tmp_path)` — [`L376`](../../../../../raw/code/graphify/tests/test_hooks.py#L376) — A legitimate POSIX core.hooksPath (Husky-style) must still install.
- `test_probe_prefers_sibling_python_exe_on_windows_layouts()` — [`L418`](../../../../../raw/code/graphify/tests/test_hooks.py#L418) — pip on Windows puts Scripts/graphify(.exe) beside ..\python.exe (or
- `test_probes_use_find_spec_not_full_import()` — [`L394`](../../../../../raw/code/graphify/tests/test_hooks.py#L394) — `python -c "import graphify"` executes the FULL package import — 10s+ on a
- `test_rebuild_bodies_are_shell_quote_safe()` — [`L298`](../../../../../raw/code/graphify/tests/test_hooks.py#L298) — The shared rebuild bodies are embedded verbatim into the launcher, so they
- `test_rebuild_bodies_read_graphify_root(name, body)` — [`L311`](../../../../../raw/code/graphify/tests/test_hooks.py#L311) — The rebuild must honour the persisted scan root rather than hardcoding the
- `test_rebuild_bodies_with_graphify_root_are_valid_python()` — [`L325`](../../../../../raw/code/graphify/tests/test_hooks.py#L325) — The .graphify_root snippet must parse so a quoting slip can't ship a hook
- `test_shebang_read_is_null_byte_safe()` — [`L408`](../../../../../raw/code/graphify/tests/test_hooks.py#L408) — On Windows, `command -v graphify` can return the launcher path WITHOUT its
- `test_status_installed(tmp_path)` — [`L70`](../../../../../raw/code/graphify/tests/test_hooks.py#L70)
- `test_status_not_installed(tmp_path)` — [`L77`](../../../../../raw/code/graphify/tests/test_hooks.py#L77)
- `test_status_shows_both_hooks(tmp_path)` — [`L114`](../../../../../raw/code/graphify/tests/test_hooks.py#L114)
- `test_uninstall_no_hook(tmp_path)` — [`L64`](../../../../../raw/code/graphify/tests/test_hooks.py#L64)
- `test_uninstall_removes_hook(tmp_path)` — [`L55`](../../../../../raw/code/graphify/tests/test_hooks.py#L55)
- `test_uninstall_removes_post_checkout_hook(tmp_path)` — [`L106`](../../../../../raw/code/graphify/tests/test_hooks.py#L106)
- `test_windows_hookspath_rejected_no_junk_dir_on_posix(tmp_path, monkeypatch, winpath)` — [`L363`](../../../../../raw/code/graphify/tests/test_hooks.py#L363) — A Windows-style core.hooksPath must raise (loud failure), not silently

## Module values
- `_HOOK_SCRIPTS` — [`L234`](../../../../../raw/code/graphify/tests/test_hooks.py#L234)

