---
title: 'Module: tests/test_install.py'
type: catalog
provenance: extracted
module: tests/test_install.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_install`/
symbols:
  _agents_install: _agents_install().
  _install: _install().
  _agents_uninstall: _agents_uninstall().
  test_codebuddy_uninstall_removes_section: test_codebuddy_uninstall_removes_section().
  test_codebuddy_uninstall_removes_hook: test_codebuddy_uninstall_removes_hook().
  test_agents_uninstall_removes_section: test_agents_uninstall_removes_section().
  test_agents_uninstall_preserves_other_content: test_agents_uninstall_preserves_other_content().
  test_opencode_agents_uninstall_removes_plugin: test_opencode_agents_uninstall_removes_plugin().
  test_kilo_agents_uninstall_preserves_existing_jsonc_config: test_kilo_agents_uninstall_preserves_existing_jsonc_config().
  test_kilo_uninstall_removes_plugin_registration_and_command: test_kilo_uninstall_removes_plugin_registration_and_command().
  test_cursor_uninstall_removes_rule: test_cursor_uninstall_removes_rule().
  test_gemini_uninstall_removes_section: test_gemini_uninstall_removes_section().
  test_gemini_uninstall_removes_hook: test_gemini_uninstall_removes_hook().
  _kilo_install: _kilo_install().
  _kilo_uninstall: _kilo_uninstall().
  test_install_default_claude: test_install_default_claude().
  test_install_codebuddy: test_install_codebuddy().
  test_install_codex: test_install_codex().
  test_install_opencode: test_install_opencode().
  test_install_positional_platform_opencode: test_install_positional_platform_opencode().
  test_install_project_claude_writes_project_scope: test_install_project_claude_writes_project_scope().
  test_install_project_codex_writes_skill_and_agents: test_install_project_codex_writes_skill_and_agents().
  test_claude_subcommand_project_install_and_uninstall_are_project_scoped: test_claude_subcommand_project_install_and_uninstall_are_project_scoped().
  test_codex_subcommand_project_install_and_uninstall_are_project_scoped: test_codex_subcommand_project_install_and_uninstall_are_project_scoped().
  test_antigravity_install_project_writes_project_skill: test_antigravity_install_project_writes_project_skill().
  test_install_help_does_not_install_default: test_install_help_does_not_install_default().
  test_install_claw: test_install_claw().
  test_install_droid: test_install_droid().
  test_install_trae: test_install_trae().
  test_install_trae_cn: test_install_trae_cn().
  test_install_windows: test_install_windows().
  test_install_unknown_platform_exits: test_install_unknown_platform_exits().
  test_codex_agents_install_mentions_dirty_graph_output: test_codex_agents_install_mentions_dirty_graph_output().
  test_claude_install_registers_claude_md: test_claude_install_registers_claude_md().
  test_codex_install_does_not_write_claude_md: test_codex_install_does_not_write_claude_md().
  test_codebuddy_install_writes_codebuddy_md: test_codebuddy_install_writes_codebuddy_md().
  test_codebuddy_install_writes_hook: test_codebuddy_install_writes_hook().
  test_codebuddy_install_idempotent: test_codebuddy_install_idempotent().
  test_codebuddy_install_merges_existing_codebuddy_md: test_codebuddy_install_merges_existing_codebuddy_md().
  test_codebuddy_uninstall_noop_if_not_installed: test_codebuddy_uninstall_noop_if_not_installed().
  test_uninstall_project_removes_project_skill_only: test_uninstall_project_removes_project_skill_only().
  test_uninstall_project_without_platform_removes_project_installs: test_uninstall_project_without_platform_removes_project_installs().
  test_antigravity_uninstall_project_removes_project_skill_only: test_antigravity_uninstall_project_removes_project_skill_only().
  test_antigravity_global_install_writes_gemini_config_skills: test_antigravity_global_install_writes_gemini_config_skills().
  test_antigravity_global_uninstall_removes_gemini_config_skill: test_antigravity_global_uninstall_removes_gemini_config_skill().
  test_codex_agents_install_writes_agents_md: test_codex_agents_install_writes_agents_md().
  test_opencode_agents_install_writes_agents_md: test_opencode_agents_install_writes_agents_md().
  test_claw_agents_install_writes_agents_md: test_claw_agents_install_writes_agents_md().
  test_agents_install_idempotent: test_agents_install_idempotent().
  test_agents_install_appends_to_existing: test_agents_install_appends_to_existing().
  test_agents_uninstall_no_op_when_not_installed: test_agents_uninstall_no_op_when_not_installed().
  test_opencode_agents_install_writes_plugin: test_opencode_agents_install_writes_plugin().
  test_opencode_plugin_reminder_has_no_backticks: test_opencode_plugin_reminder_has_no_backticks().
  test_opencode_agents_install_registers_plugin_in_config: test_opencode_agents_install_registers_plugin_in_config().
  test_opencode_agents_install_merges_existing_config: test_opencode_agents_install_merges_existing_config().
  test_kilo_agents_install_writes_agents_md: test_kilo_agents_install_writes_agents_md().
  test_kilo_agents_install_writes_plugin: test_kilo_agents_install_writes_plugin().
  test_kilo_agents_install_registers_plugin_in_config: test_kilo_agents_install_registers_plugin_in_config().
  test_kilo_agents_install_merges_existing_config: test_kilo_agents_install_merges_existing_config().
  test_kilo_agents_install_preserves_existing_jsonc_config: test_kilo_agents_install_preserves_existing_jsonc_config().
  test_kilo_agents_install_idempotent: test_kilo_agents_install_idempotent().
  test_kilo_install_writes_global_and_project_artifacts: test_kilo_install_writes_global_and_project_artifacts().
  test_cursor_install_writes_rule: test_cursor_install_writes_rule().
  test_cursor_install_idempotent: test_cursor_install_idempotent().
  test_cursor_uninstall_noop_if_not_installed: test_cursor_uninstall_noop_if_not_installed().
  test_gemini_install_writes_gemini_md: test_gemini_install_writes_gemini_md().
  test_gemini_install_writes_hook: test_gemini_install_writes_hook().
  test_gemini_install_idempotent: test_gemini_install_idempotent().
  test_gemini_install_merges_existing_gemini_md: test_gemini_install_merges_existing_gemini_md().
  test_gemini_uninstall_noop_if_not_installed: test_gemini_uninstall_noop_if_not_installed().
  test_amp_user_install_lands_in_config_agents: test_amp_user_install_lands_in_config_agents().
  test_amp_install_cleans_legacy_amp_skills_dir: test_amp_install_cleans_legacy_amp_skills_dir().
  test_amp_user_uninstall_removes_skill_and_agents: test_amp_user_uninstall_removes_skill_and_agents().
  test_amp_project_install_lands_in_dot_agents: test_amp_project_install_lands_in_dot_agents().
  test_uninstall_all_removes_amp_user_skill: test_uninstall_all_removes_amp_user_skill().
  test_hermes_skill_destination_windows_uses_localappdata: test_hermes_skill_destination_windows_uses_localappdata().
  test_hermes_skill_destination_posix_uses_home: test_hermes_skill_destination_posix_uses_home().
  PLATFORMS: PLATFORMS.
  test_codex_skill_contains_spawn_agent: test_codex_skill_contains_spawn_agent().
  test_codex_skill_uses_graphify_with_existing_graph: test_codex_skill_uses_graphify_with_existing_graph().
  test_opencode_skill_contains_mention: test_opencode_skill_contains_mention().
  test_opencode_skill_uses_opencode_agent_guidance: test_opencode_skill_uses_opencode_agent_guidance().
  test_kilo_skill_mentions_task_tool: test_kilo_skill_mentions_task_tool().
  test_kilo_skill_avoids_double_quoted_python_c_fstring_dict_keys: test_kilo_skill_avoids_double_quoted_python_c_fstring_dict_keys().
  test_claw_skill_uses_agent_tool_dispatch: test_claw_skill_uses_agent_tool_dispatch().
  test_all_skill_files_exist_in_package: test_all_skill_files_exist_in_package().
  test_kilo_command_file_exists_in_package: test_kilo_command_file_exists_in_package().
---
# Module: [`tests/test_install.py`](../../../../../raw/code/graphify/tests/test_install.py)

## Functions
- `_agents_install(tmp_path, platform)` — [`L503`](../../../../../raw/code/graphify/tests/test_install.py#L503)
- `_agents_uninstall(tmp_path, platform="")` — [`L509`](../../../../../raw/code/graphify/tests/test_install.py#L509)
- `_install(tmp_path, platform)` — [`L26`](../../../../../raw/code/graphify/tests/test_install.py#L26)
- `_kilo_install(project_dir, home_dir)` — [`L515`](../../../../../raw/code/graphify/tests/test_install.py#L515)
- `_kilo_uninstall(project_dir, home_dir)` — [`L522`](../../../../../raw/code/graphify/tests/test_install.py#L522)
- `test_agents_install_appends_to_existing(tmp_path)` — [`L555`](../../../../../raw/code/graphify/tests/test_install.py#L555) — Installs into an existing AGENTS.md without overwriting other content.
- `test_agents_install_idempotent(tmp_path)` — [`L547`](../../../../../raw/code/graphify/tests/test_install.py#L547) — Installing twice does not duplicate the section.
- `test_agents_uninstall_no_op_when_not_installed(tmp_path, capsys)` — [`L585`](../../../../../raw/code/graphify/tests/test_install.py#L585)
- `test_agents_uninstall_preserves_other_content(tmp_path)` — [`L573`](../../../../../raw/code/graphify/tests/test_install.py#L573) — Uninstall keeps pre-existing content.
- `test_agents_uninstall_removes_section(tmp_path)` — [`L565`](../../../../../raw/code/graphify/tests/test_install.py#L565)
- `test_all_skill_files_exist_in_package()` — [`L306`](../../../../../raw/code/graphify/tests/test_install.py#L306) — All installable platform skill files must be present in the installed package.
- `test_amp_install_cleans_legacy_amp_skills_dir(tmp_path, monkeypatch)` — [`L917`](../../../../../raw/code/graphify/tests/test_install.py#L917) — A pre-fix ~/.amp/skills/graphify install is removed on the next install.
- `test_amp_project_install_lands_in_dot_agents(tmp_path, monkeypatch)` — [`L958`](../../../../../raw/code/graphify/tests/test_install.py#L958) — Project-scope amp install lands in .agents/skills, an Amp project search root.
- `test_amp_user_install_lands_in_config_agents(tmp_path, monkeypatch)` — [`L896`](../../../../../raw/code/graphify/tests/test_install.py#L896) — `graphify amp install` (user scope) must drop the skill into an Amp search
- `test_amp_user_uninstall_removes_skill_and_agents(tmp_path, monkeypatch)` — [`L936`](../../../../../raw/code/graphify/tests/test_install.py#L936) — `graphify amp uninstall` removes the user-scope skill and AGENTS.md section.
- `test_antigravity_global_install_writes_gemini_config_skills(tmp_path, monkeypatch)` — [`L461`](../../../../../raw/code/graphify/tests/test_install.py#L461) — Global `graphify antigravity install` must write to ~/.gemini/config/skills/ (#1079).
- `test_antigravity_global_uninstall_removes_gemini_config_skill(tmp_path, monkeypatch)` — [`L480`](../../../../../raw/code/graphify/tests/test_install.py#L480) — Global `graphify antigravity uninstall` must remove from ~/.gemini/config/skills/ (#1079).
- `test_antigravity_install_project_writes_project_skill(tmp_path, monkeypatch)` — [`L156`](../../../../../raw/code/graphify/tests/test_install.py#L156)
- `test_antigravity_uninstall_project_removes_project_skill_only(tmp_path, monkeypatch)` — [`L442`](../../../../../raw/code/graphify/tests/test_install.py#L442)
- `test_claude_install_registers_claude_md(tmp_path)` — [`L332`](../../../../../raw/code/graphify/tests/test_install.py#L332) — Claude platform install writes CLAUDE.md; others do not.
- `test_claude_subcommand_project_install_and_uninstall_are_project_scoped(tmp_path, monkeypatch)` — [`L102`](../../../../../raw/code/graphify/tests/test_install.py#L102)
- `test_claw_agents_install_writes_agents_md(tmp_path)` — [`L542`](../../../../../raw/code/graphify/tests/test_install.py#L542)
- `test_claw_skill_uses_agent_tool_dispatch()` — [`L290`](../../../../../raw/code/graphify/tests/test_install.py#L290) — OpenClaw rides the shared Agent-tool disk-collect dispatch.
- `test_codebuddy_install_idempotent(tmp_path)` — [`L362`](../../../../../raw/code/graphify/tests/test_install.py#L362)
- `test_codebuddy_install_merges_existing_codebuddy_md(tmp_path)` — [`L370`](../../../../../raw/code/graphify/tests/test_install.py#L370)
- `test_codebuddy_install_writes_codebuddy_md(tmp_path)` — [`L345`](../../../../../raw/code/graphify/tests/test_install.py#L345)
- `test_codebuddy_install_writes_hook(tmp_path)` — [`L353`](../../../../../raw/code/graphify/tests/test_install.py#L353)
- `test_codebuddy_uninstall_noop_if_not_installed(tmp_path)` — [`L399`](../../../../../raw/code/graphify/tests/test_install.py#L399)
- `test_codebuddy_uninstall_removes_hook(tmp_path)` — [`L387`](../../../../../raw/code/graphify/tests/test_install.py#L387)
- `test_codebuddy_uninstall_removes_section(tmp_path)` — [`L379`](../../../../../raw/code/graphify/tests/test_install.py#L379)
- `test_codex_agents_install_mentions_dirty_graph_output(tmp_path)` — [`L236`](../../../../../raw/code/graphify/tests/test_install.py#L236)
- `test_codex_agents_install_writes_agents_md(tmp_path)` — [`L529`](../../../../../raw/code/graphify/tests/test_install.py#L529)
- `test_codex_install_does_not_write_claude_md(tmp_path)` — [`L338`](../../../../../raw/code/graphify/tests/test_install.py#L338)
- `test_codex_skill_contains_spawn_agent()` — [`L212`](../../../../../raw/code/graphify/tests/test_install.py#L212) — Codex skill file must reference spawn_agent.
- `test_codex_skill_uses_graphify_with_existing_graph()` — [`L220`](../../../../../raw/code/graphify/tests/test_install.py#L220) — Codex skill must keep graph-first orientation in the lean-core split.
- `test_codex_subcommand_project_install_and_uninstall_are_project_scoped(tmp_path, monkeypatch)` — [`L128`](../../../../../raw/code/graphify/tests/test_install.py#L128)
- `test_cursor_install_idempotent(tmp_path)` — [`L799`](../../../../../raw/code/graphify/tests/test_install.py#L799) — cursor install does not overwrite an existing rule file.
- `test_cursor_install_writes_rule(tmp_path)` — [`L787`](../../../../../raw/code/graphify/tests/test_install.py#L787) — cursor install writes .cursor/rules/graphify.mdc.
- `test_cursor_uninstall_noop_if_not_installed(tmp_path)` — [`L820`](../../../../../raw/code/graphify/tests/test_install.py#L820) — cursor uninstall does nothing if rule was never written.
- `test_cursor_uninstall_removes_rule(tmp_path)` — [`L810`](../../../../../raw/code/graphify/tests/test_install.py#L810) — cursor uninstall removes the rule file.
- `test_gemini_install_idempotent(tmp_path)` — [`L849`](../../../../../raw/code/graphify/tests/test_install.py#L849)
- `test_gemini_install_merges_existing_gemini_md(tmp_path)` — [`L858`](../../../../../raw/code/graphify/tests/test_install.py#L858)
- `test_gemini_install_writes_gemini_md(tmp_path)` — [`L830`](../../../../../raw/code/graphify/tests/test_install.py#L830)
- `test_gemini_install_writes_hook(tmp_path)` — [`L839`](../../../../../raw/code/graphify/tests/test_install.py#L839)
- `test_gemini_uninstall_noop_if_not_installed(tmp_path)` — [`L890`](../../../../../raw/code/graphify/tests/test_install.py#L890)
- `test_gemini_uninstall_removes_hook(tmp_path)` — [`L877`](../../../../../raw/code/graphify/tests/test_install.py#L877)
- `test_gemini_uninstall_removes_section(tmp_path)` — [`L868`](../../../../../raw/code/graphify/tests/test_install.py#L868)
- `test_hermes_skill_destination_posix_uses_home()` — [`L1007`](../../../../../raw/code/graphify/tests/test_install.py#L1007) — Non-Windows hermes destination is unchanged (~/.hermes/skills).
- `test_hermes_skill_destination_windows_uses_localappdata()` — [`L997`](../../../../../raw/code/graphify/tests/test_install.py#L997) — #1403: on Windows, Hermes scans %LOCALAPPDATA%\hermes\skills, so the global
- `test_install_claw(tmp_path)` — [`L182`](../../../../../raw/code/graphify/tests/test_install.py#L182)
- `test_install_codebuddy(tmp_path)` — [`L43`](../../../../../raw/code/graphify/tests/test_install.py#L43)
- `test_install_codex(tmp_path)` — [`L48`](../../../../../raw/code/graphify/tests/test_install.py#L48)
- `test_install_default_claude(tmp_path)` — [`L38`](../../../../../raw/code/graphify/tests/test_install.py#L38)
- `test_install_droid(tmp_path)` — [`L187`](../../../../../raw/code/graphify/tests/test_install.py#L187)
- `test_install_help_does_not_install_default(tmp_path, monkeypatch, capsys)` — [`L169`](../../../../../raw/code/graphify/tests/test_install.py#L169)
- `test_install_opencode(tmp_path)` — [`L53`](../../../../../raw/code/graphify/tests/test_install.py#L53)
- `test_install_positional_platform_opencode(tmp_path, monkeypatch)` — [`L60`](../../../../../raw/code/graphify/tests/test_install.py#L60)
- `test_install_project_claude_writes_project_scope(tmp_path, monkeypatch, capsys)` — [`L70`](../../../../../raw/code/graphify/tests/test_install.py#L70)
- `test_install_project_codex_writes_skill_and_agents(tmp_path, monkeypatch)` — [`L87`](../../../../../raw/code/graphify/tests/test_install.py#L87)
- `test_install_trae(tmp_path)` — [`L192`](../../../../../raw/code/graphify/tests/test_install.py#L192)
- `test_install_trae_cn(tmp_path)` — [`L197`](../../../../../raw/code/graphify/tests/test_install.py#L197)
- `test_install_unknown_platform_exits(tmp_path)` — [`L207`](../../../../../raw/code/graphify/tests/test_install.py#L207)
- `test_install_windows(tmp_path)` — [`L202`](../../../../../raw/code/graphify/tests/test_install.py#L202)
- `test_kilo_agents_install_idempotent(tmp_path)` — [`L738`](../../../../../raw/code/graphify/tests/test_install.py#L738)
- `test_kilo_agents_install_merges_existing_config(tmp_path)` — [`L686`](../../../../../raw/code/graphify/tests/test_install.py#L686)
- `test_kilo_agents_install_preserves_existing_jsonc_config(tmp_path)` — [`L702`](../../../../../raw/code/graphify/tests/test_install.py#L702)
- `test_kilo_agents_install_registers_plugin_in_config(tmp_path)` — [`L674`](../../../../../raw/code/graphify/tests/test_install.py#L674)
- `test_kilo_agents_install_writes_agents_md(tmp_path)` — [`L662`](../../../../../raw/code/graphify/tests/test_install.py#L662)
- `test_kilo_agents_install_writes_plugin(tmp_path)` — [`L667`](../../../../../raw/code/graphify/tests/test_install.py#L667)
- `test_kilo_agents_uninstall_preserves_existing_jsonc_config(tmp_path)` — [`L719`](../../../../../raw/code/graphify/tests/test_install.py#L719)
- `test_kilo_command_file_exists_in_package()` — [`L325`](../../../../../raw/code/graphify/tests/test_install.py#L325)
- `test_kilo_install_writes_global_and_project_artifacts(tmp_path)` — [`L750`](../../../../../raw/code/graphify/tests/test_install.py#L750)
- `test_kilo_skill_avoids_double_quoted_python_c_fstring_dict_keys()` — [`L281`](../../../../../raw/code/graphify/tests/test_install.py#L281) — Kilo runs snippets through double-quoted python -c strings.
- `test_kilo_skill_mentions_task_tool()` — [`L273`](../../../../../raw/code/graphify/tests/test_install.py#L273) — Kilo skill file should use the native Task tool flow.
- `test_kilo_uninstall_removes_plugin_registration_and_command(tmp_path)` — [`L762`](../../../../../raw/code/graphify/tests/test_install.py#L762)
- `test_opencode_agents_install_merges_existing_config(tmp_path)` — [`L635`](../../../../../raw/code/graphify/tests/test_install.py#L635) — opencode install preserves existing .opencode/opencode.json keys.
- `test_opencode_agents_install_registers_plugin_in_config(tmp_path)` — [`L624`](../../../../../raw/code/graphify/tests/test_install.py#L624) — opencode install registers the plugin in .opencode/opencode.json.
- `test_opencode_agents_install_writes_agents_md(tmp_path)` — [`L537`](../../../../../raw/code/graphify/tests/test_install.py#L537)
- `test_opencode_agents_install_writes_plugin(tmp_path)` — [`L594`](../../../../../raw/code/graphify/tests/test_install.py#L594) — opencode install writes .opencode/plugins/graphify.js.
- `test_opencode_agents_uninstall_removes_plugin(tmp_path)` — [`L648`](../../../../../raw/code/graphify/tests/test_install.py#L648) — opencode uninstall removes the plugin file and deregisters from opencode.json.
- `test_opencode_plugin_reminder_has_no_backticks(tmp_path)` — [`L602`](../../../../../raw/code/graphify/tests/test_install.py#L602) — The bash reminder string must not contain backticks or $(...) (regression test for #1413).
- `test_opencode_skill_contains_mention()` — [`L243`](../../../../../raw/code/graphify/tests/test_install.py#L243) — OpenCode skill file must reference @mention.
- `test_opencode_skill_uses_opencode_agent_guidance()` — [`L251`](../../../../../raw/code/graphify/tests/test_install.py#L251) — OpenCode's dispatch slot uses @mention, not the Claude Agent-tool example.
- `test_uninstall_all_removes_amp_user_skill(tmp_path, monkeypatch)` — [`L977`](../../../../../raw/code/graphify/tests/test_install.py#L977) — The user-scope `graphify uninstall` enumeration removes the amp skill.
- `test_uninstall_project_removes_project_skill_only(tmp_path, monkeypatch)` — [`L404`](../../../../../raw/code/graphify/tests/test_install.py#L404)
- `test_uninstall_project_without_platform_removes_project_installs(tmp_path, monkeypatch)` — [`L423`](../../../../../raw/code/graphify/tests/test_install.py#L423)

## Module values
- `PLATFORMS` — [`L9`](../../../../../raw/code/graphify/tests/test_install.py#L9)

