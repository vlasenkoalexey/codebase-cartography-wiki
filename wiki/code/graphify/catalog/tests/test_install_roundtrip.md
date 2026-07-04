---
title: 'Module: tests/test_install_roundtrip.py'
type: catalog
provenance: extracted
module: tests/test_install_roundtrip.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_install_roundtrip`/
symbols:
  test_skill_roundtrip_at_real_destination: test_skill_roundtrip_at_real_destination().
  test_vscode_install_uninstall_roundtrip: test_vscode_install_uninstall_roundtrip().
  test_install_entrypoint_roundtrip_for_progressive_and_monolith: test_install_entrypoint_roundtrip_for_progressive_and_monolith().
  _has_real_bundle: _has_real_bundle().
  _copy_in_tmp: _copy_in_tmp().
  test_amp_user_install_at_corrected_agents_path: test_amp_user_install_at_corrected_agents_path().
  test_amp_project_install_at_agents_path: test_amp_project_install_at_agents_path().
  fake_progressive_bundle: fake_progressive_bundle().
  test_monolith_to_progressive_upgrade: test_monolith_to_progressive_upgrade().
  test_failed_copytree_leaves_no_partial_references: test_failed_copytree_leaves_no_partial_references().
  ALL_CONFIG_PLATFORMS: ALL_CONFIG_PLATFORMS.
  _install_via_entrypoint: _install_via_entrypoint().
  PKG_DIR: PKG_DIR.
  test_progressive_to_monolith_downgrade_clears_references: test_progressive_to_monolith_downgrade_clears_references().
  test_interrupted_references_staging_self_heals: test_interrupted_references_staging_self_heals().
---
# Module: [`tests/test_install_roundtrip.py`](../../../../../raw/code/graphify/tests/test_install_roundtrip.py)

## Functions
- `_copy_in_tmp(tmp_path, platform)` — [`L161`](../../../../../raw/code/graphify/tests/test_install_roundtrip.py#L161) — Run _copy_skill_file with home + cwd redirected into tmp_path, restoring cwd.
- `_has_real_bundle(platform: str)` — [`L38`](../../../../../raw/code/graphify/tests/test_install_roundtrip.py#L38) — True if this platform's references bundle ships in the package right now.
- `_install_via_entrypoint(tmp_path, platform)` — [`L150`](../../../../../raw/code/graphify/tests/test_install_roundtrip.py#L150) — Drive the high-level install() entry point with home + cwd in tmp_path.
- `fake_progressive_bundle()` — [`L199`](../../../../../raw/code/graphify/tests/test_install_roundtrip.py#L199) — Stage a controllable references bundle in claude's slot.
- `test_amp_project_install_at_agents_path(tmp_path, monkeypatch)` — [`L112`](../../../../../raw/code/graphify/tests/test_install_roundtrip.py#L112) — amp's project-scope skill lands under .agents/skills, an Amp search root.
- `test_amp_user_install_at_corrected_agents_path(tmp_path, monkeypatch)` — [`L97`](../../../../../raw/code/graphify/tests/test_install_roundtrip.py#L97) — amp's user-scope skill lands under ~/.config/agents/skills (the fix), not ~/.amp.
- `test_failed_copytree_leaves_no_partial_references(tmp_path, fake_progressive_bundle)` — [`L296`](../../../../../raw/code/graphify/tests/test_install_roundtrip.py#L296) — If copytree blows up mid-stage, no half-written references/ is left visible.
- `test_install_entrypoint_roundtrip_for_progressive_and_monolith(tmp_path)` — [`L172`](../../../../../raw/code/graphify/tests/test_install_roundtrip.py#L172) — The public install() entry point round-trips a progressive and a monolith host.
- `test_interrupted_references_staging_self_heals(tmp_path, fake_progressive_bundle)` — [`L274`](../../../../../raw/code/graphify/tests/test_install_roundtrip.py#L274) — A leftover references.tmp from a crashed install is cleared on the next install.
- `test_monolith_to_progressive_upgrade(tmp_path, fake_progressive_bundle)` — [`L233`](../../../../../raw/code/graphify/tests/test_install_roundtrip.py#L233) — A pre-progressive install (SKILL.md, no references/) gains references/ on upgrade.
- `test_progressive_to_monolith_downgrade_clears_references(tmp_path, fake_progressive_bundle)` — [`L254`](../../../../../raw/code/graphify/tests/test_install_roundtrip.py#L254) — If a host loses its bundle, the next install clears the orphan references/.
- `test_skill_roundtrip_at_real_destination(platform, project, tmp_path, monkeypatch)` — [`L48`](../../../../../raw/code/graphify/tests/test_install_roundtrip.py#L48) — Install then uninstall every platform's SKILL.md at its real destination.
- `test_vscode_install_uninstall_roundtrip(tmp_path, monkeypatch)` — [`L125`](../../../../../raw/code/graphify/tests/test_install_roundtrip.py#L125) — VS Code Copilot Chat round trip at ~/.copilot/skills/graphify + instructions file.

## Module values
- `ALL_CONFIG_PLATFORMS` — [`L35`](../../../../../raw/code/graphify/tests/test_install_roundtrip.py#L35)
- `PKG_DIR` — [`L30`](../../../../../raw/code/graphify/tests/test_install_roundtrip.py#L30)

