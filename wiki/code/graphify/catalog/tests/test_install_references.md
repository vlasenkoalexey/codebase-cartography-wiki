---
title: 'Module: tests/test_install_references.py'
type: catalog
provenance: extracted
module: tests/test_install_references.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_install_references`/
symbols:
  test_built_wheel_ships_the_full_skill_payload: test_built_wheel_ships_the_full_skill_payload().
  _install: _install().
  test_unbuilt_bundle_host_falls_back_to_monolith: test_unbuilt_bundle_host_falls_back_to_monolith().
  PKG_DIR: PKG_DIR.
  test_check_skill_version_ignores_permission_error: test_check_skill_version_ignores_permission_error().
  test_hard_fail_when_bundle_dir_present_but_references_missing: test_hard_fail_when_bundle_dir_present_but_references_missing().
  test_claude_install_ships_lean_core_and_references: test_claude_install_ships_lean_core_and_references().
  _first_unbuilt_progressive_host: _first_unbuilt_progressive_host().
  fake_bundle: fake_bundle().
  test_single_version_stamp_covers_skill_and_references: test_single_version_stamp_covers_skill_and_references().
  test_uninstall_removes_references_then_walks_dirs: test_uninstall_removes_references_then_walks_dirs().
  test_check_skill_version_warns_on_missing_references: test_check_skill_version_warns_on_missing_references().
  test_claude_twins_ride_the_claude_bundle: test_claude_twins_ride_the_claude_bundle().
  test_amp_user_install_carries_references: test_amp_user_install_carries_references().
  test_install_stages_references_sidecar: test_install_stages_references_sidecar().
  test_reinstall_replaces_references_atomically: test_reinstall_replaces_references_atomically().
  test_gemini_install_references_all_resolve: test_gemini_install_references_all_resolve().
  test_pyproject_declares_references_globs: test_pyproject_declares_references_globs().
  test_monolith_install_clears_orphan_references: test_monolith_install_clears_orphan_references().
  _EXPECTED_SKILL_BODIES: _EXPECTED_SKILL_BODIES.
  _SPLIT_HOSTS: _SPLIT_HOSTS.
  _REFERENCE_NAMES: _REFERENCE_NAMES.
  _ALWAYS_ON_NAMES: _ALWAYS_ON_NAMES.
  test_check_skill_version_ignores_permission_error.guarded_exists: test_check_skill_version_ignores_permission_error().guarded_exists().
  _build_wheel_names: _build_wheel_names().
---
# Module: [`tests/test_install_references.py`](../../../../../raw/code/graphify/tests/test_install_references.py)

## Functions
- `_build_wheel_names(repo_root)` — [`L388`](../../../../../raw/code/graphify/tests/test_install_references.py#L388) — Build the wheel and return the set of arcnames inside it.
- `_first_unbuilt_progressive_host()` — [`L217`](../../../../../raw/code/graphify/tests/test_install_references.py#L217) — Find a progressive host whose bundle dir has not shipped in this build.
- `_install(tmp_path, platform)` — [`L67`](../../../../../raw/code/graphify/tests/test_install_references.py#L67)
- `fake_bundle()` — [`L32`](../../../../../raw/code/graphify/tests/test_install_references.py#L32) — Stage a fake references/ bundle in claude's slot, then restore the real one.
- `guarded_exists(self)` — [`L166`](../../../../../raw/code/graphify/tests/test_install_references.py#L166)
- `test_amp_user_install_carries_references(tmp_path, monkeypatch)` — [`L487`](../../../../../raw/code/graphify/tests/test_install_references.py#L487) — amp is progressive: its corrected user dir also gets the references/ sidecar.
- `test_built_wheel_ships_the_full_skill_payload()` — [`L425`](../../../../../raw/code/graphify/tests/test_install_references.py#L425) — The built wheel must carry every skill body, reference, and always-on block.
- `test_check_skill_version_ignores_permission_error(tmp_path, fake_bundle, monkeypatch, capsys)` — [`L153`](../../../../../raw/code/graphify/tests/test_install_references.py#L153) — Unreadable version probes should not crash startup.
- `test_check_skill_version_warns_on_missing_references(tmp_path, fake_bundle, capsys)` — [`L137`](../../../../../raw/code/graphify/tests/test_install_references.py#L137) — If SKILL.md links references/ but the dir is gone, warn to repair.
- `test_claude_install_ships_lean_core_and_references(tmp_path)` — [`L262`](../../../../../raw/code/graphify/tests/test_install_references.py#L262) — claude's real bundle ships: a lean SKILL.md plus the references/ sidecar.
- `test_claude_twins_ride_the_claude_bundle(tmp_path)` — [`L317`](../../../../../raw/code/graphify/tests/test_install_references.py#L317) — antigravity and kimi reuse claude's split bundle, so they go progressive too.
- `test_gemini_install_references_all_resolve(tmp_path)` — [`L298`](../../../../../raw/code/graphify/tests/test_install_references.py#L298) — End-to-end: every references/ pointer in gemini's installed SKILL.md resolves.
- `test_hard_fail_when_bundle_dir_present_but_references_missing(tmp_path, monkeypatch)` — [`L180`](../../../../../raw/code/graphify/tests/test_install_references.py#L180) — A bundle dir that exists but has no references/ subdir is a malformed
- `test_install_stages_references_sidecar(tmp_path, fake_bundle)` — [`L77`](../../../../../raw/code/graphify/tests/test_install_references.py#L77) — A progressive platform install drops references/ alongside SKILL.md.
- `test_monolith_install_clears_orphan_references(tmp_path, fake_bundle)` — [`L474`](../../../../../raw/code/graphify/tests/test_install_references.py#L474) — A monolith platform install removes any orphan references/ left behind.
- `test_pyproject_declares_references_globs()` — [`L330`](../../../../../raw/code/graphify/tests/test_install_references.py#L330) — package-data must declare the references + always-on globs that ship the bundles.
- `test_reinstall_replaces_references_atomically(tmp_path, fake_bundle)` — [`L102`](../../../../../raw/code/graphify/tests/test_install_references.py#L102) — Reinstall swaps references/ in place, dropping a stale fragment.
- `test_single_version_stamp_covers_skill_and_references(tmp_path, fake_bundle)` — [`L91`](../../../../../raw/code/graphify/tests/test_install_references.py#L91) — One .graphify_version stamp versions SKILL.md + references/ together.
- `test_unbuilt_bundle_host_falls_back_to_monolith(tmp_path)` — [`L240`](../../../../../raw/code/graphify/tests/test_install_references.py#L240) — A progressive host whose bundle has not shipped installs the monolith.
- `test_uninstall_removes_references_then_walks_dirs(tmp_path, fake_bundle)` — [`L121`](../../../../../raw/code/graphify/tests/test_install_references.py#L121) — Uninstall rmtrees references/ before the dir walk so the tree is cleared.

## Module values
- `PKG_DIR` — [`L28`](../../../../../raw/code/graphify/tests/test_install_references.py#L28)
- `_ALWAYS_ON_NAMES` — [`L382`](../../../../../raw/code/graphify/tests/test_install_references.py#L382)
- `_EXPECTED_SKILL_BODIES` — [`L357`](../../../../../raw/code/graphify/tests/test_install_references.py#L357)
- `_REFERENCE_NAMES` — [`L378`](../../../../../raw/code/graphify/tests/test_install_references.py#L378)
- `_SPLIT_HOSTS` — [`L374`](../../../../../raw/code/graphify/tests/test_install_references.py#L374)

