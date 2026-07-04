---
title: 'Module: evaluation/utils/file_management.py'
type: catalog
provenance: extracted
module: evaluation/utils/file_management.py
status: fresh
symbol_base: scip-python python claude-context 0.0.0 `evaluation.utils.file_management`/
symbols:
  ContextManager.__enter__: ContextManager#__enter__().
  clone_repo: clone_repo().
  get_remaining_instances: get_remaining_instances().
  ContextManager.repo: ContextManager#repo.
  logger: logger.
  ContextManager: ContextManager#
  ContextManager.base_commit: ContextManager#base_commit.
  list_files: list_files().
  ContextManager.get_readme_files: ContextManager#get_readme_files().
  ContextManager.repo_path: ContextManager#repo_path.
  is_test: is_test().
  ContextManager.verbose: ContextManager#verbose.
  ContextManager.__init__: ContextManager#__init__().
  ContextManager.__exit__: ContextManager#__exit__().
---
# Module: [`evaluation/utils/file_management.py`](../../../../../../raw/code/claude-context/evaluation/utils/file_management.py)

## Classes
### `ContextManager`
- def: [`evaluation/utils/file_management.py:62`](../../../../../../raw/code/claude-context/evaluation/utils/file_management.py#L62)
- doc: A context manager for managing a Git repository at a specific commit.
- signature: `class ContextManager:`
- members:
  - `get_readme_files(self)` — [`L101`](../../../../../../raw/code/claude-context/evaluation/utils/file_management.py#L101)
  - `base_commit` — [`L85`](../../../../../../raw/code/claude-context/evaluation/utils/file_management.py#L85)
  - `repo` — [`L87`](../../../../../../raw/code/claude-context/evaluation/utils/file_management.py#L87)
  - `repo_path` — [`L84`](../../../../../../raw/code/claude-context/evaluation/utils/file_management.py#L84)
  - `verbose` — [`L86`](../../../../../../raw/code/claude-context/evaluation/utils/file_management.py#L86)
- protocol/private: `__enter__`[`L89`](../../../../../../raw/code/claude-context/evaluation/utils/file_management.py#L89), `__exit__`[`L107`](../../../../../../raw/code/claude-context/evaluation/utils/file_management.py#L107), `__init__`[`L83`](../../../../../../raw/code/claude-context/evaluation/utils/file_management.py#L83)
- uses (calls/refs, reference-scoped): [`logger`](file_management.md#logger)
- used by: [`async_run`](../retrieval/custom.md#CustomRetrieval.async_run), [`run`](../retrieval/base.md#BaseRetrieval.run)

## Functions
- `clone_repo(repo, root_dir, token)` — [`L111`](../../../../../../raw/code/claude-context/evaluation/utils/file_management.py#L111) — Clones a GitHub repository to a specified directory.
- `get_remaining_instances(instances, output_file)` — [`L13`](../../../../../../raw/code/claude-context/evaluation/utils/file_management.py#L13) — Filters a list of instances to exclude those that have already been processed and saved in a file.
- `is_test(name, test_phrases=None)` — [`L46`](../../../../../../raw/code/claude-context/evaluation/utils/file_management.py#L46)
- `list_files(root_dir, include_tests=False)` — [`L53`](../../../../../../raw/code/claude-context/evaluation/utils/file_management.py#L53)

## Module values
- `logger` — [`L10`](../../../../../../raw/code/claude-context/evaluation/utils/file_management.py#L10)

