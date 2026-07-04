---
title: 'Module: scripts/gitflow_helper.py'
type: catalog
provenance: extracted
module: scripts/gitflow_helper.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `scripts.gitflow_helper`/
symbols:
  GitFlowHelper.run_command: GitFlowHelper#run_command().
  main: main().
  GitFlowHelper.get_current_branch: GitFlowHelper#get_current_branch().
  GitFlowHelper.start_feature: GitFlowHelper#start_feature().
  GitFlowHelper.finish_feature: GitFlowHelper#finish_feature().
  GitFlowHelper.start_release: GitFlowHelper#start_release().
  GitFlowHelper.finish_release: GitFlowHelper#finish_release().
  GitFlowHelper.start_hotfix: GitFlowHelper#start_hotfix().
  GitFlowHelper.finish_hotfix: GitFlowHelper#finish_hotfix().
  GitFlowHelper.show_status: GitFlowHelper#show_status().
  GitFlowHelper.check_branch_exists: GitFlowHelper#check_branch_exists().
  GitFlowHelper: GitFlowHelper#
  GitFlowHelper.project_root: GitFlowHelper#project_root.
  GitFlowHelper.__init__: GitFlowHelper#__init__().
---
# Module: [`scripts/gitflow_helper.py`](../../../../../raw/code/tree-sitter-analyzer/scripts/gitflow_helper.py)

## Classes
### `GitFlowHelper`
- def: [`scripts/gitflow_helper.py:15`](../../../../../raw/code/tree-sitter-analyzer/scripts/gitflow_helper.py#L15)
- signature: `class GitFlowHelper:`
- members:
  - `check_branch_exists(self, branch: str)` — [`L42`](../../../../../raw/code/tree-sitter-analyzer/scripts/gitflow_helper.py#L42) — Check if a branch exists locally or remotely
  - `finish_feature(self, feature_name: str)` — [`L73`](../../../../../raw/code/tree-sitter-analyzer/scripts/gitflow_helper.py#L73) — Finish a feature branch and merge back to develop
  - `finish_hotfix(self, hotfix_name: str)` — [`L198`](../../../../../raw/code/tree-sitter-analyzer/scripts/gitflow_helper.py#L198) — Finish a hotfix branch and merge to main and develop
  - `finish_release(self, version: str)` — [`L130`](../../../../../raw/code/tree-sitter-analyzer/scripts/gitflow_helper.py#L130) — Finish a release branch and merge to main and develop
  - `get_current_branch(self)` — [`L37`](../../../../../raw/code/tree-sitter-analyzer/scripts/gitflow_helper.py#L37) — Get the current git branch
  - `run_command(self, command: list[str], check: bool = True)` — [`L19`](../../../../../raw/code/tree-sitter-analyzer/scripts/gitflow_helper.py#L19) — Run a git command and return the result
  - `show_status(self)` — [`L247`](../../../../../raw/code/tree-sitter-analyzer/scripts/gitflow_helper.py#L247) — Show current GitFlow status
  - `start_feature(self, feature_name: str)` — [`L52`](../../../../../raw/code/tree-sitter-analyzer/scripts/gitflow_helper.py#L52) — Start a new feature branch from develop
  - `start_hotfix(self, hotfix_name: str)` — [`L177`](../../../../../raw/code/tree-sitter-analyzer/scripts/gitflow_helper.py#L177) — Start a new hotfix branch from main
  - `start_release(self, version: str)` — [`L108`](../../../../../raw/code/tree-sitter-analyzer/scripts/gitflow_helper.py#L108) — Start a new release branch from develop
  - `project_root` — [`L17`](../../../../../raw/code/tree-sitter-analyzer/scripts/gitflow_helper.py#L17)
- protocol/private: `__init__`[`L16`](../../../../../raw/code/tree-sitter-analyzer/scripts/gitflow_helper.py#L16)
- used by: [`main`](gitflow_helper.md#main)

## Functions
- `main()` — [`L261`](../../../../../raw/code/tree-sitter-analyzer/scripts/gitflow_helper.py#L261)

