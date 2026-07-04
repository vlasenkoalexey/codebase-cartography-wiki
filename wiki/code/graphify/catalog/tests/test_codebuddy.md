---
title: 'Module: tests/test_codebuddy.py'
type: catalog
provenance: extracted
module: tests/test_codebuddy.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_codebuddy`/
symbols:
  _codebuddy_md_path: _codebuddy_md_path().
  test_codebuddy_installation_roundtrip: test_codebuddy_installation_roundtrip().
  test_codebuddy_install_upgrades_stale_section: test_codebuddy_install_upgrades_stale_section().
  test_codebuddy_uninstall_removes_section: test_codebuddy_uninstall_removes_section().
  test_codebuddy_uninstall_removes_hook: test_codebuddy_uninstall_removes_hook().
  test_codebuddy_uninstall_preserves_other_content: test_codebuddy_uninstall_preserves_other_content().
  _settings_path: _settings_path().
  _codebuddy_install_user: _codebuddy_install_user().
  test_codebuddy_install_user_creates_skill_file: test_codebuddy_install_user_creates_skill_file().
  test_codebuddy_skill_file_contains_frontmatter: test_codebuddy_skill_file_contains_frontmatter().
  test_codebuddy_skill_file_references_graphify_query: test_codebuddy_skill_file_references_graphify_query().
  test_codebuddy_install_project_writes_codebuddy_md: test_codebuddy_install_project_writes_codebuddy_md().
  test_codebuddy_install_project_writes_hook: test_codebuddy_install_project_writes_hook().
  test_codebuddy_install_hook_has_bash_matcher: test_codebuddy_install_hook_has_bash_matcher().
  test_codebuddy_install_hook_has_read_glob_matcher: test_codebuddy_install_hook_has_read_glob_matcher().
  test_codebuddy_install_idempotent: test_codebuddy_install_idempotent().
  test_codebuddy_install_merges_existing_codebuddy_md: test_codebuddy_install_merges_existing_codebuddy_md().
  test_codebuddy_uninstall_noop_if_no_section: test_codebuddy_uninstall_noop_if_no_section().
  test_uninstall_all_removes_codebuddy_md: test_uninstall_all_removes_codebuddy_md().
  test_uninstall_all_removes_codebuddy_hook: test_uninstall_all_removes_codebuddy_hook().
  _skill_path_user: _skill_path_user().
  test_codebuddy_install_prints_no_change_on_second_run: test_codebuddy_install_prints_no_change_on_second_run().
  test_codebuddy_install_hint_git_add: test_codebuddy_install_hint_git_add().
  test_codebuddy_uninstall_noop_if_not_installed: test_codebuddy_uninstall_noop_if_not_installed().
  test_codebuddy_in_platform_config: test_codebuddy_in_platform_config().
  test_codebuddy_platform_skill_destination_user_scope: test_codebuddy_platform_skill_destination_user_scope().
  test_codebuddy_platform_skill_destination_project_scope: test_codebuddy_platform_skill_destination_project_scope().
  test_codebuddy_in_main_help_text: test_codebuddy_in_main_help_text().
  _skill_path_project: _skill_path_project().
  test_codebuddy_skill_file_exists_in_package: test_codebuddy_skill_file_exists_in_package().
---
# Module: [`tests/test_codebuddy.py`](../../../../../raw/code/graphify/tests/test_codebuddy.py)

## Functions
- `_codebuddy_install_user(tmp_path)` — [`L14`](../../../../../raw/code/graphify/tests/test_codebuddy.py#L14)
- `_codebuddy_md_path(project_dir)` — [`L35`](../../../../../raw/code/graphify/tests/test_codebuddy.py#L35)
- `_settings_path(project_dir)` — [`L39`](../../../../../raw/code/graphify/tests/test_codebuddy.py#L39)
- `_skill_path_project(project_dir)` — [`L31`](../../../../../raw/code/graphify/tests/test_codebuddy.py#L31)
- `_skill_path_user(tmp_path)` — [`L27`](../../../../../raw/code/graphify/tests/test_codebuddy.py#L27)
- `test_codebuddy_in_main_help_text(capsys, monkeypatch)` — [`L300`](../../../../../raw/code/graphify/tests/test_codebuddy.py#L300) — `graphify --help` must list codebuddy in the platform list and per-platform section.
- `test_codebuddy_in_platform_config()` — [`L277`](../../../../../raw/code/graphify/tests/test_codebuddy.py#L277) — codebuddy must be registered in _PLATFORM_CONFIG.
- `test_codebuddy_install_hint_git_add(tmp_path, capsys)` — [`L160`](../../../../../raw/code/graphify/tests/test_codebuddy.py#L160) — Project-scoped install via CLI prints a git add hint.
- `test_codebuddy_install_hook_has_bash_matcher(tmp_path)` — [`L95`](../../../../../raw/code/graphify/tests/test_codebuddy.py#L95) — The installed hook must include Bash matcher for code search interception.
- `test_codebuddy_install_hook_has_read_glob_matcher(tmp_path)` — [`L105`](../../../../../raw/code/graphify/tests/test_codebuddy.py#L105) — The installed hook must include Read|Glob matcher for file-read interception.
- `test_codebuddy_install_idempotent(tmp_path)` — [`L115`](../../../../../raw/code/graphify/tests/test_codebuddy.py#L115) — Re-install does not duplicate ## graphify sections.
- `test_codebuddy_install_merges_existing_codebuddy_md(tmp_path)` — [`L139`](../../../../../raw/code/graphify/tests/test_codebuddy.py#L139) — Install appends to an existing CODEBUDDY.md, preserving other content.
- `test_codebuddy_install_prints_no_change_on_second_run(tmp_path, capsys)` — [`L150`](../../../../../raw/code/graphify/tests/test_codebuddy.py#L150) — Second install prints '(no change)' when content is identical.
- `test_codebuddy_install_project_writes_codebuddy_md(tmp_path)` — [`L73`](../../../../../raw/code/graphify/tests/test_codebuddy.py#L73) — Project-scope install writes CODEBUDDY.md with graphify section.
- `test_codebuddy_install_project_writes_hook(tmp_path)` — [`L84`](../../../../../raw/code/graphify/tests/test_codebuddy.py#L84) — Project-scope install registers PreToolUse hook in .codebuddy/settings.json.
- `test_codebuddy_install_upgrades_stale_section(tmp_path)` — [`L124`](../../../../../raw/code/graphify/tests/test_codebuddy.py#L124) — Re-install replaces an old graphify section with the current template.
- `test_codebuddy_install_user_creates_skill_file(tmp_path)` — [`L47`](../../../../../raw/code/graphify/tests/test_codebuddy.py#L47) — User-scope install copies skill to ~/.codebuddy/skills/graphify/SKILL.md.
- `test_codebuddy_installation_roundtrip(tmp_path)` — [`L322`](../../../../../raw/code/graphify/tests/test_codebuddy.py#L322) — Install then uninstall leaves no trace of graphify CODEBUDDY.md or hook.
- `test_codebuddy_platform_skill_destination_project_scope(tmp_path)` — [`L293`](../../../../../raw/code/graphify/tests/test_codebuddy.py#L293) — Project-scope destination must be <project>/.codebuddy/skills/graphify/SKILL.md.
- `test_codebuddy_platform_skill_destination_user_scope(tmp_path)` — [`L285`](../../../../../raw/code/graphify/tests/test_codebuddy.py#L285) — User-scope destination must be ~/.codebuddy/skills/graphify/SKILL.md.
- `test_codebuddy_skill_file_contains_frontmatter(tmp_path)` — [`L54`](../../../../../raw/code/graphify/tests/test_codebuddy.py#L54) — Installed skill file must include graphify YAML frontmatter.
- `test_codebuddy_skill_file_exists_in_package()` — [`L315`](../../../../../raw/code/graphify/tests/test_codebuddy.py#L315) — skill.md must be present in the installed package (shared with claude).
- `test_codebuddy_skill_file_references_graphify_query(tmp_path)` — [`L62`](../../../../../raw/code/graphify/tests/test_codebuddy.py#L62) — /graphify skill must mention graphify query (query-first policy).
- `test_codebuddy_uninstall_noop_if_no_section(tmp_path)` — [`L211`](../../../../../raw/code/graphify/tests/test_codebuddy.py#L211) — Uninstall should not error when CODEBUDDY.md exists but no graphify section.
- `test_codebuddy_uninstall_noop_if_not_installed(tmp_path)` — [`L205`](../../../../../raw/code/graphify/tests/test_codebuddy.py#L205) — Uninstall should not raise when CODEBUDDY.md doesn't exist.
- `test_codebuddy_uninstall_preserves_other_content(tmp_path)` — [`L220`](../../../../../raw/code/graphify/tests/test_codebuddy.py#L220) — Uninstall preserves non-graphify content in CODEBUDDY.md.
- `test_codebuddy_uninstall_removes_hook(tmp_path)` — [`L193`](../../../../../raw/code/graphify/tests/test_codebuddy.py#L193) — Uninstall removes the PreToolUse hook from .codebuddy/settings.json.
- `test_codebuddy_uninstall_removes_section(tmp_path)` — [`L184`](../../../../../raw/code/graphify/tests/test_codebuddy.py#L184) — Uninstall removes the ## graphify section from CODEBUDDY.md.
- `test_uninstall_all_removes_codebuddy_hook(tmp_path, monkeypatch)` — [`L254`](../../../../../raw/code/graphify/tests/test_codebuddy.py#L254) — graphify uninstall must clean up .codebuddy/settings.json hooks.
- `test_uninstall_all_removes_codebuddy_md(tmp_path, monkeypatch)` — [`L237`](../../../../../raw/code/graphify/tests/test_codebuddy.py#L237) — graphify uninstall must clean up CODEBUDDY.md.

