---
title: 'Module: tree_sitter_analyzer/_health_scorer_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/_health_scorer_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer._health_scorer_helpers`/
symbols:
  calculate_git_hotspot: calculate_git_hotspot().
  read_source_file: read_source_file().
  calculate_weighted_total: calculate_weighted_total().
  round_available_scores: round_available_scores().
  find_git_root: find_git_root().
  count_recent_commits: count_recent_commits().
  score_commit_frequency: score_commit_frequency().
---
# Module: [`tree_sitter_analyzer/_health_scorer_helpers.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_health_scorer_helpers.py)

## Functions
- `calculate_git_hotspot(file_path: str, low_commit_threshold: int, high_commit_threshold: int)` — [`L46`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_health_scorer_helpers.py#L46) — Score a file by recent git commit frequency.
- `calculate_weighted_total(dimensions: Mapping[str, float | None], weights: Mapping[str, float])` — [`L18`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_health_scorer_helpers.py#L18) — Combine available dimension scores using normalized active weights.
- `count_recent_commits(repo_root: Path, pathspec: str)` — [`L89`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_health_scorer_helpers.py#L89) — Count commits touching pathspec in the last 90 days.
- `find_git_root(start_dir: Path)` — [`L73`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_health_scorer_helpers.py#L73) — Return the git repository root for start_dir.
- `read_source_file(path: Path)` — [`L8`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_health_scorer_helpers.py#L8) — Return file text, or None when the file cannot be read.
- `round_available_scores(dimensions: Mapping[str, float | None])` — [`L37`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_health_scorer_helpers.py#L37) — Round available scores and drop unavailable dimensions.
- `score_commit_frequency(commit_count: int, low_commit_threshold: int, high_commit_threshold: int)` — [`L112`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_health_scorer_helpers.py#L112) — Convert recent commit count into a 0-100 stability score.

