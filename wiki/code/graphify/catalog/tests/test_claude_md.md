---
title: 'Module: tests/test_claude_md.py'
type: catalog
provenance: extracted
module: tests/test_claude_md.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_claude_md`/test_
symbols:
  test_uninstall_removes_section: uninstall_removes_section().
  test_uninstall_preserves_other_content: uninstall_preserves_other_content().
  test_install_creates_claude_md: install_creates_claude_md().
  test_install_appends_to_existing_claude_md: install_appends_to_existing_claude_md().
  test_install_is_idempotent: install_is_idempotent().
  test_uninstall_removes_settings_hook: uninstall_removes_settings_hook().
  test_install_contains_expected_rules: install_contains_expected_rules().
  test_install_idempotent_message: install_idempotent_message().
  test_uninstall_no_op_when_not_installed: uninstall_no_op_when_not_installed().
  test_uninstall_no_op_when_no_file: uninstall_no_op_when_no_file().
  test_install_creates_settings_json: install_creates_settings_json().
  test_install_settings_json_idempotent: install_settings_json_idempotent().
---
# Module: [`tests/test_claude_md.py`](../../../../../raw/code/graphify/tests/test_claude_md.py)

## Functions
- `test_install_appends_to_existing_claude_md(tmp_path)` — [`L28`](../../../../../raw/code/graphify/tests/test_claude_md.py#L28) — Appends to an existing CLAUDE.md without clobbering it.
- `test_install_contains_expected_rules(tmp_path)` — [`L19`](../../../../../raw/code/graphify/tests/test_claude_md.py#L19) — Written section includes the three rules.
- `test_install_creates_claude_md(tmp_path)` — [`L11`](../../../../../raw/code/graphify/tests/test_claude_md.py#L11) — Creates CLAUDE.md when none exists.
- `test_install_creates_settings_json(tmp_path)` — [`L104`](../../../../../raw/code/graphify/tests/test_claude_md.py#L104) — claude_install also writes .claude/settings.json with PreToolUse hook.
- `test_install_idempotent_message(tmp_path, capsys)` — [`L48`](../../../../../raw/code/graphify/tests/test_claude_md.py#L48) — Second install prints the 'already configured' message.
- `test_install_is_idempotent(tmp_path, capsys)` — [`L38`](../../../../../raw/code/graphify/tests/test_claude_md.py#L38) — Running install twice does not duplicate the section.
- `test_install_settings_json_idempotent(tmp_path)` — [`L115`](../../../../../raw/code/graphify/tests/test_claude_md.py#L115) — Running claude_install twice does not duplicate the PreToolUse hook.
- `test_uninstall_no_op_when_no_file(tmp_path, capsys)` — [`L93`](../../../../../raw/code/graphify/tests/test_claude_md.py#L93) — Uninstall when no CLAUDE.md exists prints a message and exits cleanly.
- `test_uninstall_no_op_when_not_installed(tmp_path, capsys)` — [`L84`](../../../../../raw/code/graphify/tests/test_claude_md.py#L84) — Uninstall on a CLAUDE.md without graphify section prints a message and exits cleanly.
- `test_uninstall_preserves_other_content(tmp_path)` — [`L71`](../../../../../raw/code/graphify/tests/test_claude_md.py#L71) — Uninstall keeps pre-existing content outside the graphify section.
- `test_uninstall_removes_section(tmp_path)` — [`L61`](../../../../../raw/code/graphify/tests/test_claude_md.py#L61) — Removes the graphify section after it was installed.
- `test_uninstall_removes_settings_hook(tmp_path)` — [`L127`](../../../../../raw/code/graphify/tests/test_claude_md.py#L127) — claude_uninstall removes the PreToolUse hook from settings.json.

