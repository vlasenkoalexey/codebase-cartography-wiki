---
title: 'Module: tests/test_devin.py'
type: catalog
provenance: extracted
module: tests/test_devin.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_devin`/
symbols:
  _devin_install_user: _devin_install_user().
  test_devin_install_project_creates_skill_file: test_devin_install_project_creates_skill_file().
  test_devin_uninstall_user_removes_skill_file: test_devin_uninstall_user_removes_skill_file().
  _skill_path_user: _skill_path_user().
  _rules_path: _rules_path().
  test_devin_install_user_creates_skill_file: test_devin_install_user_creates_skill_file().
  test_devin_skill_file_contains_frontmatter: test_devin_skill_file_contains_frontmatter().
  test_devin_skill_file_references_graphify_query: test_devin_skill_file_references_graphify_query().
  test_devin_install_user_does_not_write_rules: test_devin_install_user_does_not_write_rules().
  test_devin_install_project_creates_rules_file: test_devin_install_project_creates_rules_file().
  test_devin_rules_content_recommends_graphify_query: test_devin_rules_content_recommends_graphify_query().
  test_devin_rules_install_idempotent: test_devin_rules_install_idempotent().
  test_devin_uninstall_project_removes_skill_file: test_devin_uninstall_project_removes_skill_file().
  test_devin_uninstall_project_removes_rules_file: test_devin_uninstall_project_removes_rules_file().
  test_devin_uninstall_project_does_not_touch_user_scope: test_devin_uninstall_project_does_not_touch_user_scope().
  test_devin_install_project_hints_git_add: test_devin_install_project_hints_git_add().
  test_devin_uninstall_user_noop_when_not_installed: test_devin_uninstall_user_noop_when_not_installed().
  test_devin_rules_uninstall_noop_when_not_installed: test_devin_rules_uninstall_noop_when_not_installed().
  test_devin_in_platform_config: test_devin_in_platform_config().
  test_devin_platform_skill_destination_user_scope: test_devin_platform_skill_destination_user_scope().
  test_devin_in_main_help_text: test_devin_in_main_help_text().
  test_devin_platform_skill_destination_project_scope: test_devin_platform_skill_destination_project_scope().
  _skill_path_project: _skill_path_project().
  test_devin_skill_file_exists_in_package: test_devin_skill_file_exists_in_package().
  test_devin_skill_file_uses_python_c_syntax: test_devin_skill_file_uses_python_c_syntax().
  test_devin_skill_file_frontmatter_has_triggers: test_devin_skill_file_frontmatter_has_triggers().
---
# Module: [`tests/test_devin.py`](../../../../../raw/code/graphify/tests/test_devin.py)

## Functions
- `_devin_install_user(tmp_path)` — [`L12`](../../../../../raw/code/graphify/tests/test_devin.py#L12)
- `_rules_path(project_dir)` — [`L33`](../../../../../raw/code/graphify/tests/test_devin.py#L33)
- `_skill_path_project(project_dir)` — [`L29`](../../../../../raw/code/graphify/tests/test_devin.py#L29)
- `_skill_path_user(tmp_path)` — [`L25`](../../../../../raw/code/graphify/tests/test_devin.py#L25)
- `test_devin_in_main_help_text(capsys, monkeypatch)` — [`L283`](../../../../../raw/code/graphify/tests/test_devin.py#L283) — `graphify --help` must list devin in the platform list and in the per-platform section.
- `test_devin_in_platform_config()` — [`L267`](../../../../../raw/code/graphify/tests/test_devin.py#L267) — devin must be registered in _PLATFORM_CONFIG.
- `test_devin_install_project_creates_rules_file(tmp_path, monkeypatch)` — [`L88`](../../../../../raw/code/graphify/tests/test_devin.py#L88) — Project-scope install writes .windsurf/rules/graphify.md.
- `test_devin_install_project_creates_skill_file(tmp_path, monkeypatch)` — [`L74`](../../../../../raw/code/graphify/tests/test_devin.py#L74) — Project-scope install copies skill to .devin/skills/graphify/SKILL.md.
- `test_devin_install_project_hints_git_add(tmp_path, monkeypatch, capsys)` — [`L123`](../../../../../raw/code/graphify/tests/test_devin.py#L123) — Project-scope install prints a git add hint covering .devin/ and .windsurf/.
- `test_devin_install_user_creates_skill_file(tmp_path)` — [`L41`](../../../../../raw/code/graphify/tests/test_devin.py#L41) — User-scope install copies skill to ~/.config/devin/skills/graphify/SKILL.md.
- `test_devin_install_user_does_not_write_rules(tmp_path)` — [`L64`](../../../../../raw/code/graphify/tests/test_devin.py#L64) — User-scope install does NOT write .windsurf/rules/ — that's project-only.
- `test_devin_platform_skill_destination_project_scope(tmp_path)` — [`L305`](../../../../../raw/code/graphify/tests/test_devin.py#L305) — Project-scope destination must be <project>/.devin/skills/graphify/SKILL.md.
- `test_devin_platform_skill_destination_user_scope(tmp_path)` — [`L275`](../../../../../raw/code/graphify/tests/test_devin.py#L275) — User-scope destination must be ~/.config/devin/skills/graphify/SKILL.md.
- `test_devin_rules_content_recommends_graphify_query(tmp_path)` — [`L104`](../../../../../raw/code/graphify/tests/test_devin.py#L104) — The rules file installed by devin must use query-first policy.
- `test_devin_rules_install_idempotent(tmp_path, capsys)` — [`L112`](../../../../../raw/code/graphify/tests/test_devin.py#L112) — Installing rules twice does not change content and prints 'no change'.
- `test_devin_rules_uninstall_noop_when_not_installed(tmp_path)` — [`L222`](../../../../../raw/code/graphify/tests/test_devin.py#L222) — _devin_rules_uninstall does nothing if the rules file was never written.
- `test_devin_skill_file_contains_frontmatter(tmp_path)` — [`L48`](../../../../../raw/code/graphify/tests/test_devin.py#L48) — Installed skill file must include Devin-specific YAML frontmatter.
- `test_devin_skill_file_exists_in_package()` — [`L232`](../../../../../raw/code/graphify/tests/test_devin.py#L232) — skill-devin.md must be present in the installed package.
- `test_devin_skill_file_frontmatter_has_triggers()` — [`L255`](../../../../../raw/code/graphify/tests/test_devin.py#L255) — Devin skill frontmatter must list triggers for model-invocable activation.
- `test_devin_skill_file_references_graphify_query(tmp_path)` — [`L57`](../../../../../raw/code/graphify/tests/test_devin.py#L57) — /graphify skill must mention graphify query (query-first policy).
- `test_devin_skill_file_uses_python_c_syntax()` — [`L239`](../../../../../raw/code/graphify/tests/test_devin.py#L239) — Devin skill must use inline python -c syntax (cross-platform, no bash heredocs).
- `test_devin_uninstall_project_does_not_touch_user_scope(tmp_path, monkeypatch)` — [`L203`](../../../../../raw/code/graphify/tests/test_devin.py#L203) — Project-scope uninstall must not remove the user-scope skill file.
- `test_devin_uninstall_project_removes_rules_file(tmp_path, monkeypatch)` — [`L188`](../../../../../raw/code/graphify/tests/test_devin.py#L188) — Project-scope uninstall removes .windsurf/rules/graphify.md.
- `test_devin_uninstall_project_removes_skill_file(tmp_path, monkeypatch)` — [`L173`](../../../../../raw/code/graphify/tests/test_devin.py#L173) — Project-scope uninstall removes .devin/skills/graphify/SKILL.md.
- `test_devin_uninstall_user_noop_when_not_installed(tmp_path, capsys)` — [`L153`](../../../../../raw/code/graphify/tests/test_devin.py#L153) — User-scope uninstall prints an appropriate message when nothing is installed.
- `test_devin_uninstall_user_removes_skill_file(tmp_path)` — [`L141`](../../../../../raw/code/graphify/tests/test_devin.py#L141) — User-scope uninstall removes the skill file.

