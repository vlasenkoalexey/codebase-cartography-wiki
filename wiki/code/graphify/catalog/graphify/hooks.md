---
title: 'Module: graphify/hooks.py'
type: catalog
provenance: extracted
module: graphify/hooks.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `graphify.hooks`/
symbols:
  install: install().
  uninstall: uninstall().
  status: status().
  _PYTHON_DETECT: _PYTHON_DETECT.
  _HOOK_SCRIPT: _HOOK_SCRIPT.
  _CHECKOUT_SCRIPT: _CHECKOUT_SCRIPT.
  _hooks_dir: _hooks_dir().
  _HOOK_MARKER: _HOOK_MARKER.
  _detached_launch: _detached_launch().
  _REBUILD_BODY_COMMIT: _REBUILD_BODY_COMMIT.
  _CHECKOUT_MARKER: _CHECKOUT_MARKER.
  _REBUILD_BODY_CHECKOUT: _REBUILD_BODY_CHECKOUT.
  _reject_windows_path: _reject_windows_path().
  _git_root: _git_root().
  _user_hooks_dir: _user_hooks_dir().
  _install_hook: _install_hook().
  _uninstall_hook: _uninstall_hook().
  status._check: status()._check().
  _HOOK_MARKER_END: _HOOK_MARKER_END.
  _CHECKOUT_MARKER_END: _CHECKOUT_MARKER_END.
  _LAUNCHER_TEMPLATE: _LAUNCHER_TEMPLATE.
  _WINDOWS_DRIVE_RE: _WINDOWS_DRIVE_RE.
---
# Module: [`graphify/hooks.py`](../../../../../raw/code/graphify/graphify/hooks.py)

## Functions
- `_check(name: str, marker: str)` — [`L540`](../../../../../raw/code/graphify/graphify/hooks.py#L540) — documented in [graphify-hooks](../../concepts/graphify-hooks.md)
- `_detached_launch(rebuild_body: str)` — [`L230`](../../../../../raw/code/graphify/graphify/hooks.py#L230) — Return a POSIX-sh line that runs ``rebuild_body`` as a detached background — documented in [graphify-hooks](../../concepts/graphify-hooks.md)
- `_git_root(path: Path)` — [`L346`](../../../../../raw/code/graphify/graphify/hooks.py#L346) — Walk up to find .git directory. — documented in [graphify-hooks](../../concepts/graphify-hooks.md)
- `_hooks_dir(root: Path)` — [`L376`](../../../../../raw/code/graphify/graphify/hooks.py#L376) — Return the git hooks directory, respecting core.hooksPath if set (e.g. Husky). — documented in [graphify-hooks](../../concepts/graphify-hooks.md)
- `_install_hook(hooks_dir: Path, name: str, script: str, marker: str)` — [`L435`](../../../../../raw/code/graphify/graphify/hooks.py#L435) — Install a single git hook, appending if an existing hook is present. — documented in [graphify-hooks](../../concepts/graphify-hooks.md)
- `_reject_windows_path(value: str, source: str)` — [`L358`](../../../../../raw/code/graphify/graphify/hooks.py#L358) — Raise if a hooks path looks like a Windows absolute path (#1385). — documented in [graphify-hooks](../../concepts/graphify-hooks.md)
- `_uninstall_hook(hooks_dir: Path, name: str, marker: str, marker_end: str)` — [`L449`](../../../../../raw/code/graphify/graphify/hooks.py#L449) — Remove graphify section from a git hook using start/end markers. — documented in [graphify-hooks](../../concepts/graphify-hooks.md)
- `_user_hooks_dir(hooks_dir: Path)` — [`L470`](../../../../../raw/code/graphify/graphify/hooks.py#L470) — Return the user-editable hooks directory. — documented in [graphify-hooks](../../concepts/graphify-hooks.md)
- `install(path: Path = Path("."))` — [`L483`](../../../../../raw/code/graphify/graphify/hooks.py#L483) — Install graphify post-commit and post-checkout hooks in the nearest git repo. — documented in [graphify-__main__](../../concepts/graphify-__main__.md)
- `status(path: Path = Path("."))` — [`L533`](../../../../../raw/code/graphify/graphify/hooks.py#L533) — Check if graphify hooks are installed. — documented in [graphify-hooks](../../concepts/graphify-hooks.md)
- `uninstall(path: Path = Path("."))` — [`L520`](../../../../../raw/code/graphify/graphify/hooks.py#L520) — Remove graphify post-commit and post-checkout hooks. — documented in [graphify-__main__](../../concepts/graphify-__main__.md)

## Module values
- `_CHECKOUT_MARKER` — [`L11`](../../../../../raw/code/graphify/graphify/hooks.py#L11) — documented in [graphify-hooks](../../concepts/graphify-hooks.md)
- `_CHECKOUT_MARKER_END` — [`L12`](../../../../../raw/code/graphify/graphify/hooks.py#L12) — documented in [graphify-hooks](../../concepts/graphify-hooks.md)
- `_CHECKOUT_SCRIPT` — [`L297`](../../../../../raw/code/graphify/graphify/hooks.py#L297) — documented in [graphify-hooks](../../concepts/graphify-hooks.md)
- `_HOOK_MARKER` — [`L9`](../../../../../raw/code/graphify/graphify/hooks.py#L9) — documented in [graphify-hooks](../../concepts/graphify-hooks.md)
- `_HOOK_MARKER_END` — [`L10`](../../../../../raw/code/graphify/graphify/hooks.py#L10) — documented in [graphify-hooks](../../concepts/graphify-hooks.md)
- `_HOOK_SCRIPT` — [`L243`](../../../../../raw/code/graphify/graphify/hooks.py#L243) — documented in [graphify-hooks](../../concepts/graphify-hooks.md)
- `_LAUNCHER_TEMPLATE` — [`L206`](../../../../../raw/code/graphify/graphify/hooks.py#L206) — documented in [graphify-hooks](../../concepts/graphify-hooks.md)
- `_PYTHON_DETECT` — [`L20`](../../../../../raw/code/graphify/graphify/hooks.py#L20) — documented in [graphify-hooks](../../concepts/graphify-hooks.md)
- `_REBUILD_BODY_CHECKOUT` — [`L154`](../../../../../raw/code/graphify/graphify/hooks.py#L154) — documented in [graphify-hooks](../../concepts/graphify-hooks.md)
- `_REBUILD_BODY_COMMIT` — [`L107`](../../../../../raw/code/graphify/graphify/hooks.py#L107) — documented in [graphify-hooks](../../concepts/graphify-hooks.md)
- `_WINDOWS_DRIVE_RE` — [`L355`](../../../../../raw/code/graphify/graphify/hooks.py#L355) — documented in [graphify-hooks](../../concepts/graphify-hooks.md)

