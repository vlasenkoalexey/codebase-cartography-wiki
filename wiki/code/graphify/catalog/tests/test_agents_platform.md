---
title: 'Module: tests/test_agents_platform.py'
type: catalog
provenance: extracted
module: tests/test_agents_platform.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_agents_platform`/
symbols:
  _run: _run().
  test_install_platform_agents_writes_user_global_skill_only: test_install_platform_agents_writes_user_global_skill_only().
  test_agents_user_destination_is_user_global_dot_agents: test_agents_user_destination_is_user_global_dot_agents().
  test_agents_project_destination_is_dot_agents: test_agents_project_destination_is_dot_agents().
  test_skills_alias_resolves_to_agents: test_skills_alias_resolves_to_agents().
  test_uninstall_platform_agents_removes_user_global_skill: test_uninstall_platform_agents_removes_user_global_skill().
  test_uninstall_platform_flag_global_removes_skill: test_uninstall_platform_flag_global_removes_skill().
  test_project_uninstall_all_removes_agents_skill: test_project_uninstall_all_removes_agents_skill().
  test_install_platform_agents_project_writes_dot_agents: test_install_platform_agents_project_writes_dot_agents().
  test_agents_subcommand_install_also_wires_agents_md: test_agents_subcommand_install_also_wires_agents_md().
  test_agents_subcommand_install_is_idempotent: test_agents_subcommand_install_is_idempotent().
  test_skills_subcommand_is_the_agents_subcommand: test_skills_subcommand_is_the_agents_subcommand().
  test_bare_install_does_not_touch_dot_agents: test_bare_install_does_not_touch_dot_agents().
---
# Module: [`tests/test_agents_platform.py`](../../../../../raw/code/graphify/tests/test_agents_platform.py)

## Functions
- `_run(tmp_path, argv, home)` — [`L52`](../../../../../raw/code/graphify/tests/test_agents_platform.py#L52) — Drive main() with argv, cwd at tmp_path, and Path.home redirected.
- `test_agents_project_destination_is_dot_agents(tmp_path)` — [`L33`](../../../../../raw/code/graphify/tests/test_agents_platform.py#L33) — Project agents skill lands at ./.agents/skills.
- `test_agents_subcommand_install_also_wires_agents_md(tmp_path)` — [`L163`](../../../../../raw/code/graphify/tests/test_agents_platform.py#L163) — `graphify agents install` is the amp-twin: skill at ~/.agents/skills PLUS a
- `test_agents_subcommand_install_is_idempotent(tmp_path)` — [`L187`](../../../../../raw/code/graphify/tests/test_agents_platform.py#L187) — Running `graphify agents install` twice leaves a single AGENTS.md section.
- `test_agents_user_destination_is_user_global_dot_agents(tmp_path)` — [`L25`](../../../../../raw/code/graphify/tests/test_agents_platform.py#L25) — Global agents skill lands at ~/.agents/skills (the spec's user-global dir),
- `test_bare_install_does_not_touch_dot_agents(tmp_path)` — [`L226`](../../../../../raw/code/graphify/tests/test_agents_platform.py#L226) — `graphify install` (no platform) stays single-platform claude/windows and
- `test_install_platform_agents_project_writes_dot_agents(tmp_path)` — [`L140`](../../../../../raw/code/graphify/tests/test_agents_platform.py#L140) — `graphify install --project --platform agents` writes ./.agents/skills and
- `test_install_platform_agents_writes_user_global_skill_only(tmp_path, platform_arg)` — [`L65`](../../../../../raw/code/graphify/tests/test_agents_platform.py#L65) — `graphify install --platform agents|skills` writes ~/.agents/skills/...
- `test_project_uninstall_all_removes_agents_skill(tmp_path)` — [`L123`](../../../../../raw/code/graphify/tests/test_agents_platform.py#L123) — `graphify uninstall --project` (no platform) removes the agents project skill
- `test_skills_alias_resolves_to_agents()` — [`L42`](../../../../../raw/code/graphify/tests/test_agents_platform.py#L42)
- `test_skills_subcommand_is_the_agents_subcommand(tmp_path)` — [`L201`](../../../../../raw/code/graphify/tests/test_agents_platform.py#L201) — `graphify skills install`/`uninstall` behaves exactly like the agents form:
- `test_uninstall_platform_agents_removes_user_global_skill(tmp_path)` — [`L84`](../../../../../raw/code/graphify/tests/test_agents_platform.py#L84) — Bare `graphify uninstall` clears the ~/.agents/skills skill the AGENTS.md and
- `test_uninstall_platform_flag_global_removes_skill(tmp_path, platform_arg)` — [`L103`](../../../../../raw/code/graphify/tests/test_agents_platform.py#L103) — `graphify uninstall --platform agents|skills` (global) clears ~/.agents/skills.

