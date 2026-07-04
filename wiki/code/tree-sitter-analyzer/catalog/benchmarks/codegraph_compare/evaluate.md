---
title: 'Module: benchmarks/codegraph_compare/evaluate.py'
type: catalog
provenance: extracted
module: benchmarks/codegraph_compare/evaluate.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `benchmarks.codegraph_compare.evaluate`/
symbols:
  _evaluate_run_inner: _evaluate_run_inner().
  evaluate_all: evaluate_all().
  evaluate_run: evaluate_run().
  _stderr: _stderr().
  _build_eval_prompt: _build_eval_prompt().
  _minimal_error_record: _minimal_error_record().
  _call_llm: _call_llm().
  _cmd_evaluate: _cmd_evaluate().
  main: main().
  _SAFE_DEFAULT_SCORES._SAFE_DEFAULT_SCORES: _SAFE_DEFAULT_SCORES._SAFE_DEFAULT_SCORES.
  _EVALUATOR_PROMPT_FILE: _EVALUATOR_PROMPT_FILE.
  _ERROR_SCORE: _ERROR_SCORE.
  _DRY_RUN_SCORE: _DRY_RUN_SCORE.
  _append_jsonl: _append_jsonl().
  _extract_cited_paths: _extract_cited_paths().
  _check_citations: _check_citations().
  _load_repo_paths: _load_repo_paths().
  _load_runs: _load_runs().
  _build_record: _build_record().
  _run_arm_id: _run_arm_id().
  _CODE_EXTENSIONS: _CODE_EXTENSIONS.
  _PROMPTS_DIR: _PROMPTS_DIR.
  _DEFAULT_EVALUATOR_PROMPT: _DEFAULT_EVALUATOR_PROMPT.
  _require_anthropic: _require_anthropic().
  _check_key_points: _check_key_points().
  _render_eval_template: _render_eval_template().
  _apply_penalties: _apply_penalties().
  _compute_overall: _compute_overall().
  _run_repo_id: _run_repo_id().
  _load_questions: _load_questions().
  _build_parser: _build_parser().
---
# Module: [`benchmarks/codegraph_compare/evaluate.py`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/evaluate.py)

## Functions
- `_append_jsonl(path: Path, record: dict)` — [`L407`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/evaluate.py#L407) — Append a single JSON record to a JSONL file, creating it if needed.
- `_apply_penalties(scores: dict[str, Any], bad_citations: list[str], missing_key_points: list[str], total_key_points: int)` — [`L370`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/evaluate.py#L370) — Return a new scores dict with caps applied.
- `_build_eval_prompt(question_text: str, expected_key_points: list[str], answer: str)` — [`L240`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/evaluate.py#L240) — Build the full evaluation prompt string.
- `_build_parser()` — [`L832`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/evaluate.py#L832)
- `_build_record(*, run_id: str, question_id: str, arm_id: str, repo_path: str, correctness: int, completeness: int, citation_quality: int, hallucination_risk: int, overall: float, bad_citations: list[str], missing_key_points: list[str], reasoning: str, evaluated_with_llm: bool, eval_model: str)` — [`L618`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/evaluate.py#L618) — Assemble a canonical EvalRecord dict.
- `_call_llm(prompt: str, model: str)` — [`L291`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/evaluate.py#L291) — Call the Claude API and parse the returned JSON scores.
- `_check_citations(citations: list[str], repo_path: Path)` — [`L189`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/evaluate.py#L189) — Check citation strings against the file system.
- `_check_key_points(answer: str, expected_key_points: list[str])` — [`L217`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/evaluate.py#L217) — Return ``(covered_points, missing_points)`` based on case-insensitive
- `_cmd_evaluate(args: argparse.Namespace)` — [`L874`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/evaluate.py#L874)
- `_compute_overall(scores: dict[str, Any])` — [`L395`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/evaluate.py#L395) — Compute the mean of the four scored dimensions.
- `_evaluate_run_inner(run: dict, question: dict, repo_path: Path, model: str, dry_run: bool, results_dir: Path | None)` — [`L473`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/evaluate.py#L473)
- `_extract_cited_paths(citations: list[str])` — [`L163`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/evaluate.py#L163) — Extract strings from citations that look like file paths.
- `_load_questions(questions_yaml: Path)` — [`L757`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/evaluate.py#L757) — Load questions from YAML and index them by ``id``.
- `_load_repo_paths(manifest_path: Path)` — [`L789`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/evaluate.py#L789) — Load ``{repo_id: local_path}`` from a prepared_repos.json manifest.
- `_load_runs(runs_jsonl: Path)` — [`L809`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/evaluate.py#L809) — Load all RunRecord dicts from a JSONL file.
- `_minimal_error_record(run: dict, question: dict, reason: str)` — [`L598`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/evaluate.py#L598) — Build a zero-score EvalRecord for a failed or un-evaluable run.
- `_render_eval_template(*, template: str, question_text: str, expected_key_points: list[str], answer: str)` — [`L259`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/evaluate.py#L259) — Render evaluator input without treating JSON braces as format fields.
- `_require_anthropic()` — [`L144`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/evaluate.py#L144) — Return the ``anthropic`` module, raising a clear error if not installed.
- `_run_arm_id(run: dict)` — [`L657`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/evaluate.py#L657) — Return the arm id across historical and current RunRecord schemas.
- `_run_repo_id(run: dict)` — [`L662`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/evaluate.py#L662) — Return the repo id across historical and current RunRecord schemas.
- `_stderr(*args: Any, **kwargs: Any)` — [`L135`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/evaluate.py#L135)
- `evaluate_all(runs_jsonl: Path, questions_yaml: Path, prepared_manifest: Path, results_dir: Path, model: str = "claude-haiku-4-5-20251001", dry_run: bool = False)` — [`L672`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/evaluate.py#L672) — Batch-evaluate every run in ``runs_jsonl``.
- `evaluate_run(run: dict, question: dict, repo_path: Path, model: str = "claude-haiku-4-5-20251001", dry_run: bool = False, results_dir: Path | None = None)` — [`L419`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/evaluate.py#L419) — Evaluate one RunRecord against its QuestionSpec.
- `main(argv: list[str] | None = None)` — [`L901`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/evaluate.py#L901)

## Module values
- `_CODE_EXTENSIONS` — [`L44`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/evaluate.py#L44)
- `_DEFAULT_EVALUATOR_PROMPT` — [`L80`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/evaluate.py#L80)
- `_DRY_RUN_SCORE` — [`L117`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/evaluate.py#L117)
- `_ERROR_SCORE` — [`L116`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/evaluate.py#L116)
- `_EVALUATOR_PROMPT_FILE` — [`L77`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/evaluate.py#L77)
- `_PROMPTS_DIR` — [`L76`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/evaluate.py#L76)
- `_SAFE_DEFAULT_SCORES` — [`L120`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/evaluate.py#L120)

