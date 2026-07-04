---
title: 'Module: tests/test_install_upgrade.py'
type: catalog
provenance: extracted
module: tests/test_install_upgrade.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_install_upgrade`/
symbols:
  test_claude_install_upgrades_stale_section: test_claude_install_upgrades_stale_section().
  test_agents_install_upgrades_stale_section: test_agents_install_upgrades_stale_section().
  test_gemini_install_upgrades_stale_section: test_gemini_install_upgrades_stale_section().
  test_vscode_install_upgrades_stale_section: test_vscode_install_upgrades_stale_section().
  test_claude_install_upgrades_stale_hook_payload: test_claude_install_upgrades_stale_hook_payload().
  test_cursor_install_upgrades_stale_rule: test_cursor_install_upgrades_stale_rule().
  test_kiro_install_upgrades_stale_steering: test_kiro_install_upgrades_stale_steering().
  test_kiro_install_ships_references_sidecar_and_version_stamp: test_kiro_install_ships_references_sidecar_and_version_stamp().
  _assert_query_first: _assert_query_first().
  _OLD_CLAUDE_SECTION: _OLD_CLAUDE_SECTION.
  _assert_no_report_first: _assert_no_report_first().
  _OLD_AGENTS_SECTION: _OLD_AGENTS_SECTION.
  _OLD_GEMINI_SECTION: _OLD_GEMINI_SECTION.
  _OLD_HOOK_PAYLOAD_SNIPPET: _OLD_HOOK_PAYLOAD_SNIPPET.
  _OLD_VSCODE_SECTION: _OLD_VSCODE_SECTION.
  _OLD_CURSOR_RULE: _OLD_CURSOR_RULE.
  _OLD_KIRO_STEERING: _OLD_KIRO_STEERING.
---
# Module: [`tests/test_install_upgrade.py`](../../../../../raw/code/graphify/tests/test_install_upgrade.py)

## Functions
- `_assert_no_report_first(text: str, ctx: str)` — [`L78`](../../../../../raw/code/graphify/tests/test_install_upgrade.py#L78)
- `_assert_query_first(text: str, ctx: str)` — [`L87`](../../../../../raw/code/graphify/tests/test_install_upgrade.py#L87)
- `test_agents_install_upgrades_stale_section(tmp_path, monkeypatch)` — [`L153`](../../../../../raw/code/graphify/tests/test_install_upgrade.py#L153) — Same upgrade behavior for AGENTS.md (Codex / OpenCode / Aider / Trae).
- `test_claude_install_upgrades_stale_hook_payload(tmp_path, monkeypatch)` — [`L111`](../../../../../raw/code/graphify/tests/test_install_upgrade.py#L111) — The Claude install must also rewrite a stale .claude/settings.json hook
- `test_claude_install_upgrades_stale_section(tmp_path, monkeypatch)` — [`L93`](../../../../../raw/code/graphify/tests/test_install_upgrade.py#L93) — A pre-fix CLAUDE.md gets the new section in place when the user runs
- `test_cursor_install_upgrades_stale_rule(tmp_path, monkeypatch)` — [`L197`](../../../../../raw/code/graphify/tests/test_install_upgrade.py#L197) — Same upgrade behavior for .cursor/rules/graphify.mdc.
- `test_gemini_install_upgrades_stale_section(tmp_path, monkeypatch)` — [`L168`](../../../../../raw/code/graphify/tests/test_install_upgrade.py#L168) — Same upgrade behavior for GEMINI.md.
- `test_kiro_install_ships_references_sidecar_and_version_stamp(tmp_path, monkeypatch)` — [`L236`](../../../../../raw/code/graphify/tests/test_install_upgrade.py#L236) — _kiro_install routes through _copy_skill_file so the references/ sidecar
- `test_kiro_install_upgrades_stale_steering(tmp_path, monkeypatch)` — [`L215`](../../../../../raw/code/graphify/tests/test_install_upgrade.py#L215) — Same upgrade behavior for .kiro/steering/graphify.md (wholly owned).
- `test_vscode_install_upgrades_stale_section(tmp_path, monkeypatch)` — [`L182`](../../../../../raw/code/graphify/tests/test_install_upgrade.py#L182) — Same upgrade behavior for .github/copilot-instructions.md (VS Code).

## Module values
- `_OLD_AGENTS_SECTION` — [`L36`](../../../../../raw/code/graphify/tests/test_install_upgrade.py#L36)
- `_OLD_CLAUDE_SECTION` — [`L23`](../../../../../raw/code/graphify/tests/test_install_upgrade.py#L23)
- `_OLD_CURSOR_RULE` — [`L50`](../../../../../raw/code/graphify/tests/test_install_upgrade.py#L50)
- `_OLD_GEMINI_SECTION` — [`L38`](../../../../../raw/code/graphify/tests/test_install_upgrade.py#L38)
- `_OLD_HOOK_PAYLOAD_SNIPPET` — [`L75`](../../../../../raw/code/graphify/tests/test_install_upgrade.py#L75)
- `_OLD_KIRO_STEERING` — [`L63`](../../../../../raw/code/graphify/tests/test_install_upgrade.py#L63)
- `_OLD_VSCODE_SECTION` — [`L40`](../../../../../raw/code/graphify/tests/test_install_upgrade.py#L40)

