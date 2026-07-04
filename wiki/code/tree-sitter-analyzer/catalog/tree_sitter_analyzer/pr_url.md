---
title: 'Module: tree_sitter_analyzer/pr_url.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/pr_url.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.pr_url`/
symbols:
  parse_pr_url: parse_pr_url().
  ParsedPRUrl: ParsedPRUrl#
  ParsedPRUrl.pr_number: ParsedPRUrl#pr_number.
  fetch_pr_changed_files: fetch_pr_changed_files().
  fetch_pr_diff_stat: fetch_pr_diff_stat().
  fetch_pr_diff: fetch_pr_diff().
  ParsedPRUrl.owner: ParsedPRUrl#owner.
  ParsedPRUrl.repo: ParsedPRUrl#repo.
  ParsedPRUrl.slug: ParsedPRUrl#slug().
  check_gh_available: check_gh_available().
  ParsedPRUrl.url: ParsedPRUrl#url().
  _run_gh: _run_gh().
  _GITHUB_PR_PATTERN: _GITHUB_PR_PATTERN.
  _GITHUB_PR_API_PATTERN: _GITHUB_PR_API_PATTERN.
---
# Module: [`tree_sitter_analyzer/pr_url.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/pr_url.py)

## Classes
### `ParsedPRUrl`
- def: [`tree_sitter_analyzer/pr_url.py:11`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/pr_url.py#L11)
- doc: Components extracted from a GitHub PR URL.
- signature: `class ParsedPRUrl:`
- members:
  - `slug(self)` — [`L19`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/pr_url.py#L19)
  - `url(self)` — [`L23`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/pr_url.py#L23)
  - `owner` — [`L14`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/pr_url.py#L14)
  - `pr_number` — [`L16`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/pr_url.py#L16)
  - `repo` — [`L15`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/pr_url.py#L15)
- used by: [`parse_pr_url`](pr_url.md#parse_pr_url), [`fetch_pr_changed_files`](pr_url.md#fetch_pr_changed_files), [`fetch_pr_diff`](pr_url.md#fetch_pr_diff), [`fetch_pr_diff_stat`](pr_url.md#fetch_pr_diff_stat)  (16 test-only)

## Functions
- `_run_gh(args: list[str], timeout: int = 30)` — [`L70`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/pr_url.py#L70) — Run a gh CLI subprocess and return (returncode, stdout).
- `check_gh_available()` — [`L136`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/pr_url.py#L136) — Check if the gh CLI is installed and authenticated.
- `fetch_pr_changed_files(pr: ParsedPRUrl)` — [`L86`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/pr_url.py#L86) — Fetch the list of changed files in a PR via gh CLI.
- `fetch_pr_diff(pr: ParsedPRUrl)` — [`L121`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/pr_url.py#L121) — Fetch the full diff for a PR via gh CLI.
- `fetch_pr_diff_stat(pr: ParsedPRUrl)` — [`L106`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/pr_url.py#L106) — Fetch the diff stat summary for a PR via gh CLI.
- `parse_pr_url(url: str)` — [`L36`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/pr_url.py#L36) — Parse a GitHub PR URL into owner, repo, and PR number.

## Module values
- `_GITHUB_PR_API_PATTERN` — [`L31`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/pr_url.py#L31)
- `_GITHUB_PR_PATTERN` — [`L27`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/pr_url.py#L27)

