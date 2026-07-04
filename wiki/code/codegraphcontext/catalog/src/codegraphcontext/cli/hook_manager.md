---
title: 'Module: src/codegraphcontext/cli/hook_manager.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/cli/hook_manager.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.cli.hook_manager`/
symbols:
  get_hook_status: get_hook_status().
  install_hooks: install_hooks().
  uninstall_hooks: uninstall_hooks().
  find_git_repository: find_git_repository().
  GitRepository.root: GitRepository#root.
  HookStatus.installed: HookStatus#installed().
  HookError: HookError#
  GitRepository.git_dir: GitRepository#git_dir.
  _hook_script: _hook_script().
  _is_managed_hook: _is_managed_hook().
  GITATTRIBUTES_ENTRY: GITATTRIBUTES_ENTRY.
  HookStatus: HookStatus#
  HookStatus.repo_root: HookStatus#repo_root.
  _read_worktree_gitdir: _read_worktree_gitdir().
  _ensure_gitattributes: _ensure_gitattributes().
  _remove_gitattributes_entry: _remove_gitattributes_entry().
  _has_gitattributes_entry: _has_gitattributes_entry().
  _configure_merge_driver: _configure_merge_driver().
  HOOK_NAMES: HOOK_NAMES.
  GitRepository: GitRepository#
  HookStatus.git_dir: HookStatus#git_dir.
  HookStatus.installed_hooks: HookStatus#installed_hooks.
  HookStatus.has_merge_driver: HookStatus#has_merge_driver.
  HookStatus.has_gitattributes_entry: HookStatus#has_gitattributes_entry.
  MANAGED_MARKER: MANAGED_MARKER.
  HookStatus.unmanaged_hooks: HookStatus#unmanaged_hooks.
  _git_config: _git_config().
  _unset_git_config: _unset_git_config().
  _sh_quote: _sh_quote().
  _has_git_config: _has_git_config().
---
# Module: [`src/codegraphcontext/cli/hook_manager.py`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/hook_manager.py)

## Classes
### `GitRepository`
- def: [`src/codegraphcontext/cli/hook_manager.py:21`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/hook_manager.py#L21)
- signature: `class GitRepository:`
- members:
  - `git_dir` — [`L23`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/hook_manager.py#L23)
  - `root` — [`L22`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/hook_manager.py#L22)
- used by: [`get_hook_status`](hook_manager.md#get_hook_status), [`install_hooks`](hook_manager.md#install_hooks), [`uninstall_hooks`](hook_manager.md#uninstall_hooks), [`find_git_repository`](hook_manager.md#find_git_repository)

### `HookError`  ·  implements/extends RuntimeError
- def: [`src/codegraphcontext/cli/hook_manager.py:16`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/hook_manager.py#L16)
- doc: Raised when hook installation cannot proceed safely.
- signature: `class HookError(RuntimeError):`
- used by: [`install_hooks`](hook_manager.md#install_hooks), [`hook_status`](main.md#hook_status), [`find_git_repository`](hook_manager.md#find_git_repository), [`hook_install`](main.md#hook_install), [`hook_uninstall`](main.md#hook_uninstall), [`_read_worktree_gitdir`](hook_manager.md#_read_worktree_gitdir)

### `HookStatus`
- def: [`src/codegraphcontext/cli/hook_manager.py:27`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/hook_manager.py#L27)
- signature: `class HookStatus:`
- members:
  - `installed(self)` — [`L36`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/hook_manager.py#L36)
  - `git_dir` — [`L29`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/hook_manager.py#L29)
  - `has_gitattributes_entry` — [`L33`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/hook_manager.py#L33)
  - `has_merge_driver` — [`L32`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/hook_manager.py#L32)
  - `installed_hooks` — [`L30`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/hook_manager.py#L30)
  - `repo_root` — [`L28`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/hook_manager.py#L28)
  - `unmanaged_hooks` — [`L31`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/hook_manager.py#L31)
- used by: [`get_hook_status`](hook_manager.md#get_hook_status), [`install_hooks`](hook_manager.md#install_hooks), [`hook_status`](main.md#hook_status), [`uninstall_hooks`](hook_manager.md#uninstall_hooks), [`hook_install`](main.md#hook_install), [`hook_uninstall`](main.md#hook_uninstall)

## Functions
- `_configure_merge_driver(repo_root: Path)` — [`L200`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/hook_manager.py#L200)
- `_ensure_gitattributes(repo_root: Path)` — [`L161`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/hook_manager.py#L161)
- `_git_config(repo_root: Path, key: str, value: str)` — [`L205`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/hook_manager.py#L205)
- `_has_git_config(repo_root: Path, key: str)` — [`L213`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/hook_manager.py#L213)
- `_has_gitattributes_entry(repo_root: Path)` — [`L190`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/hook_manager.py#L190)
- `_hook_script(repo_root: Path)` — [`L136`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/hook_manager.py#L136)
- `_is_managed_hook(path: Path)` — [`L154`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/hook_manager.py#L154)
- `_read_worktree_gitdir(git_file: Path)` — [`L123`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/hook_manager.py#L123)
- `_remove_gitattributes_entry(repo_root: Path)` — [`L174`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/hook_manager.py#L174)
- `_sh_quote(value: str)` — [`L150`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/hook_manager.py#L150)
- `_unset_git_config(repo_root: Path, key: str)` — [`L209`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/hook_manager.py#L209)
- `find_git_repository(start: Path | str | None = None)` — [`L44`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/hook_manager.py#L44) — Find the nearest Git repository root and git directory.
- `get_hook_status(start: Path | str | None = None)` — [`L98`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/hook_manager.py#L98)
- `install_hooks(start: Path | str | None = None, *, force: bool = False)` — [`L61`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/hook_manager.py#L61)
- `uninstall_hooks(start: Path | str | None = None)` — [`L83`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/hook_manager.py#L83)

## Module values
- `GITATTRIBUTES_ENTRY` — [`L13`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/hook_manager.py#L13)
- `HOOK_NAMES` — [`L12`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/hook_manager.py#L12)
- `MANAGED_MARKER` — [`L11`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/hook_manager.py#L11)

