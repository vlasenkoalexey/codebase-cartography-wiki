---
title: 'Module: benchmarks/codegraph_compare/run.py'
type: catalog
provenance: extracted
module: benchmarks/codegraph_compare/run.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `benchmarks.codegraph_compare.run`/
symbols:
  cmd_run: cmd_run().
  cmd_run_matrix: cmd_run_matrix().
  cmd_prepare: cmd_prepare().
  PHASE_PRESETS.PHASE_PRESETS: PHASE_PRESETS.PHASE_PRESETS.
  _phase_to_matrix_args: _phase_to_matrix_args().
  _die: _die().
  main: main().
  RESULTS_DIR: RESULTS_DIR.
  _load_yaml: _load_yaml().
  cmd_phase: cmd_phase().
  PREPARED_MANIFEST: PREPARED_MANIFEST.
  REPOS_YAML: REPOS_YAML.
  BENCHMARKS_DIR: BENCHMARKS_DIR.
  PhasePreset.min_repeats: PhasePreset#min_repeats.
  _limited_questions_for_repo: _limited_questions_for_repo().
  cmd_status: cmd_status().
  QUESTIONS_YAML: QUESTIONS_YAML.
  PhasePreset: PhasePreset#
  PhasePreset.repos: PhasePreset#repos.
  PhasePreset.arms: PhasePreset#arms.
  PhasePreset.repeats: PhasePreset#repeats.
  PhasePreset.question_limit: PhasePreset#question_limit.
  PhasePreset.description: PhasePreset#description.
  ARMS_YAML: ARMS_YAML.
  _get_repo: _get_repo().
  _get_arm: _get_arm().
  _repo_local_path: _repo_local_path().
  _get_question: _get_question().
  _questions_for_repo: _questions_for_repo().
  _assert_question_matches_repo: _assert_question_matches_repo().
  _build_parser: _build_parser().
  _all_repos: _all_repos().
  _all_arms: _all_arms().
  _all_questions: _all_questions().
---
# Module: [`benchmarks/codegraph_compare/run.py`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/run.py)

## Classes
### `PhasePreset`
- def: [`benchmarks/codegraph_compare/run.py:52`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/run.py#L52)
- doc: Named benchmark phase with reproducible defaults.
- signature: `class PhasePreset:`
- members:
  - `arms` — [`L56`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/run.py#L56)
  - `description` — [`L60`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/run.py#L60)
  - `min_repeats` — [`L58`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/run.py#L58)
  - `question_limit` — [`L59`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/run.py#L59)
  - `repeats` — [`L57`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/run.py#L57)
  - `repos` — [`L55`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/run.py#L55)
- used by: (3 test-only callers)

## Functions
- `_all_arms(arms: dict | list)` — [`L183`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/run.py#L183)
- `_all_questions(questions: dict | list)` — [`L187`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/run.py#L187)
- `_all_repos(repos: dict | list)` — [`L179`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/run.py#L179)
- `_assert_question_matches_repo(question_entry: dict, repo_id: str)` — [`L206`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/run.py#L206)
- `_build_parser()` — [`L621`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/run.py#L621)
- `_die(message: str, code: int = 1)` — [`L133`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/run.py#L133) — Print *message* to stderr and exit with *code*.
- `_get_arm(arms: dict | list, arm_id: str)` — [`L154`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/run.py#L154) — Return the arm entry matching *arm_id* from the loaded arms config.
- `_get_question(questions: dict | list, question_id: str)` — [`L164`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/run.py#L164) — Return the question entry matching *question_id* from loaded questions config.
- `_get_repo(repos: dict | list, repo_id: str)` — [`L144`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/run.py#L144) — Return the repo entry matching *repo_id* from the loaded repos config.
- `_limited_questions_for_repo(questions: dict | list, repo_id: str, limit: int | None)` — [`L195`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/run.py#L195)
- `_load_yaml(path: Path)` — [`L104`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/run.py#L104) — Load a YAML file and return the parsed content.
- `_phase_to_matrix_args(args: argparse.Namespace)` — [`L221`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/run.py#L221) — Expand a named phase into the same namespace used by run-matrix.
- `_questions_for_repo(questions: dict | list, repo_id: str)` — [`L191`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/run.py#L191)
- `_repo_local_path(repo_entry: dict)` — [`L215`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/run.py#L215) — Return the local path for a repo: .benchmark-repos/<id>.
- `cmd_phase(args: argparse.Namespace)` — [`L525`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/run.py#L525) — Run a named benchmark phase with reproducible defaults.
- `cmd_prepare(args: argparse.Namespace)` — [`L258`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/run.py#L258) — Prepare one or all repos — delegates to repo_prep.
- `cmd_run(args: argparse.Namespace)` — [`L310`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/run.py#L310) — Run a single (repo, question, arm, repeat) trial.
- `cmd_run_matrix(args: argparse.Namespace)` — [`L399`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/run.py#L399) — Run all combinations of repos × arms × questions × repeats.
- `cmd_status(_args: argparse.Namespace)` — [`L538`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/run.py#L538) — Print summary of prepared repos and run statistics.
- `main(argv: list[str] | None = None)` — [`L814`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/run.py#L814) — Parse arguments and dispatch to the appropriate sub-command handler.

## Module values
- `ARMS_YAML` — [`L45`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/run.py#L45)
- `BENCHMARKS_DIR` — [`L43`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/run.py#L43)
- `PHASE_PRESETS` — [`L63`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/run.py#L63)
- `PREPARED_MANIFEST` — [`L48`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/run.py#L48)
- `QUESTIONS_YAML` — [`L46`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/run.py#L46)
- `REPOS_YAML` — [`L44`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/run.py#L44)
- `RESULTS_DIR` — [`L47`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/run.py#L47)

