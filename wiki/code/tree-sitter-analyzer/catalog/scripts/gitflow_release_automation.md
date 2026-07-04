---
title: 'Module: scripts/gitflow_release_automation.py'
type: catalog
provenance: extracted
module: scripts/gitflow_release_automation.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `scripts.gitflow_release_automation`/
symbols:
  GitFlowReleaseAutomation.execute_full_workflow: GitFlowReleaseAutomation#execute_full_workflow().
  GitFlowReleaseAutomation.run_command: GitFlowReleaseAutomation#run_command().
  GitFlowReleaseAutomation.create_release_branch: GitFlowReleaseAutomation#create_release_branch().
  GitFlowReleaseAutomation.release_branch: GitFlowReleaseAutomation#release_branch.
  GitFlowReleaseAutomation.project_root: GitFlowReleaseAutomation#project_root.
  GitFlowReleaseAutomation.sync_readme_statistics: GitFlowReleaseAutomation#sync_readme_statistics().
  GitFlowReleaseAutomation.push_release_branch: GitFlowReleaseAutomation#push_release_branch().
  main: main().
  GitFlowReleaseAutomation.version: GitFlowReleaseAutomation#version.
  GitFlowReleaseAutomation.check_prerequisites: GitFlowReleaseAutomation#check_prerequisites().
  GitFlowReleaseAutomation.run_tests: GitFlowReleaseAutomation#run_tests().
  GitFlowReleaseAutomation: GitFlowReleaseAutomation#
  GitFlowReleaseAutomation.wait_for_ci_completion: GitFlowReleaseAutomation#wait_for_ci_completion().
  GitFlowReleaseAutomation.complete_release: GitFlowReleaseAutomation#complete_release().
  GitFlowReleaseAutomation.__init__: GitFlowReleaseAutomation#__init__().
---
# Module: [`scripts/gitflow_release_automation.py`](../../../../../raw/code/tree-sitter-analyzer/scripts/gitflow_release_automation.py)

## Classes
### `GitFlowReleaseAutomation`
- def: [`scripts/gitflow_release_automation.py:23`](../../../../../raw/code/tree-sitter-analyzer/scripts/gitflow_release_automation.py#L23)
- signature: `class GitFlowReleaseAutomation:`
- members:
  - `check_prerequisites(self)` — [`L54`](../../../../../raw/code/tree-sitter-analyzer/scripts/gitflow_release_automation.py#L54) — Check if all prerequisites are met
  - `complete_release(self)` — [`L270`](../../../../../raw/code/tree-sitter-analyzer/scripts/gitflow_release_automation.py#L270) — Complete the release process after CI/CD success
  - `create_release_branch(self)` — [`L146`](../../../../../raw/code/tree-sitter-analyzer/scripts/gitflow_release_automation.py#L146) — Create and prepare release branch
  - `execute_full_workflow(self)` — [`L299`](../../../../../raw/code/tree-sitter-analyzer/scripts/gitflow_release_automation.py#L299) — Execute the complete GitFlow release workflow
  - `push_release_branch(self)` — [`L242`](../../../../../raw/code/tree-sitter-analyzer/scripts/gitflow_release_automation.py#L242) — Push release branch to trigger CI/CD
  - `run_command(self, command: list[str], check: bool = True)` — [`L29`](../../../../../raw/code/tree-sitter-analyzer/scripts/gitflow_release_automation.py#L29) — Run a git command and return the result
  - `run_tests(self)` — [`L128`](../../../../../raw/code/tree-sitter-analyzer/scripts/gitflow_release_automation.py#L128) — Run tests to ensure quality
  - `sync_readme_statistics(self)` — [`L88`](../../../../../raw/code/tree-sitter-analyzer/scripts/gitflow_release_automation.py#L88) — Sync README statistics to ensure consistency
  - `wait_for_ci_completion(self)` — [`L255`](../../../../../raw/code/tree-sitter-analyzer/scripts/gitflow_release_automation.py#L255) — Wait for CI/CD completion and provide status
  - `project_root` — [`L26`](../../../../../raw/code/tree-sitter-analyzer/scripts/gitflow_release_automation.py#L26)
  - `release_branch` — [`L27`](../../../../../raw/code/tree-sitter-analyzer/scripts/gitflow_release_automation.py#L27)
  - `version` — [`L25`](../../../../../raw/code/tree-sitter-analyzer/scripts/gitflow_release_automation.py#L25)
- protocol/private: `__init__`[`L24`](../../../../../raw/code/tree-sitter-analyzer/scripts/gitflow_release_automation.py#L24)
- used by: [`main`](gitflow_release_automation.md#main)

## Functions
- `main()` — [`L349`](../../../../../raw/code/tree-sitter-analyzer/scripts/gitflow_release_automation.py#L349)

