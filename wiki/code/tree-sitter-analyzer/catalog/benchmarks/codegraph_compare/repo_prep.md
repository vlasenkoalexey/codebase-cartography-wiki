---
title: 'Module: benchmarks/codegraph_compare/repo_prep.py'
type: catalog
provenance: extracted
module: benchmarks/codegraph_compare/repo_prep.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `benchmarks.codegraph_compare.repo_prep`/
symbols:
  prepare_repo: prepare_repo().
  _prepared_repo_from_dict: _prepared_repo_from_dict().
  _cmd_prepare: _cmd_prepare().
  _cmd_status: _cmd_status().
  load_repos_config: load_repos_config().
  prepare_all: prepare_all().
  _stderr: _stderr().
  RepoSpec.id: RepoSpec#id.
  PreparedRepo: PreparedRepo#
  PreparedRepo.error: PreparedRepo#error.
  save_prepared_manifest: save_prepared_manifest().
  PreparedRepo.id: PreparedRepo#id.
  load_prepared_manifest: load_prepared_manifest().
  main: main().
  RepoSpec: RepoSpec#
  RepoSpec.commit: RepoSpec#commit.
  PreparedRepo.actual_commit: PreparedRepo#actual_commit.
  _collect_stats: _collect_stats().
  _checkout_commit: _checkout_commit().
  _prepared_repo_to_dict: _prepared_repo_to_dict().
  _build_parser: _build_parser().
  RepoSpec.language: RepoSpec#language.
  PreparedRepo.language: PreparedRepo#language.
  PreparedRepo.local_path: PreparedRepo#local_path.
  _get_current_commit: _get_current_commit().
  DEFAULT_BASE_DIR: DEFAULT_BASE_DIR.
  RepoSpec.name: RepoSpec#name.
  PreparedRepo.file_count: PreparedRepo#file_count.
  PreparedRepo.source_file_count: PreparedRepo#source_file_count.
  PreparedRepo.size_bytes: PreparedRepo#size_bytes.
  _is_excluded: _is_excluded().
  _clone_repo: _clone_repo().
  _get_default_branch_head: _get_default_branch_head().
  RepoSpec.url: RepoSpec#url.
  PreparedRepo.name: PreparedRepo#name.
  PreparedRepo.prepared_at: PreparedRepo#prepared_at.
  _run_git: _run_git().
  _DEFAULT_MANIFEST: _DEFAULT_MANIFEST.
  RepoSpec.description: RepoSpec#description.
  REPOS_CONFIG: REPOS_CONFIG.
  _EXCLUDED_DIRS: _EXCLUDED_DIRS.
  _SOURCE_EXTENSIONS: _SOURCE_EXTENSIONS.
  _PLACEHOLDER_SHA: _PLACEHOLDER_SHA.
  _fmt_size: _fmt_size().
---
# Module: [`benchmarks/codegraph_compare/repo_prep.py`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/repo_prep.py)

## Classes
### `PreparedRepo`
- def: [`benchmarks/codegraph_compare/repo_prep.py:87`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/repo_prep.py#L87)
- doc: Result of successfully (or unsuccessfully) preparing a repository.
- signature: `class PreparedRepo:`
- members:
  - `actual_commit` — [`L94`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/repo_prep.py#L94)
  - `error` — [`L99`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/repo_prep.py#L99)
  - `file_count` — [`L95`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/repo_prep.py#L95)
  - `id` — [`L90`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/repo_prep.py#L90)
  - `language` — [`L92`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/repo_prep.py#L92)
  - `local_path` — [`L93`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/repo_prep.py#L93)
  - `name` — [`L91`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/repo_prep.py#L91)
  - `prepared_at` — [`L98`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/repo_prep.py#L98)
  - `size_bytes` — [`L97`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/repo_prep.py#L97)
  - `source_file_count` — [`L96`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/repo_prep.py#L96)
- used by: (10 test-only callers)

### `RepoSpec`
- def: [`benchmarks/codegraph_compare/repo_prep.py:75`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/repo_prep.py#L75)
- doc: Specification for a repository to benchmark.
- signature: `class RepoSpec:`
- members:
  - `commit` — [`L82`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/repo_prep.py#L82)
  - `description` — [`L83`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/repo_prep.py#L83)
  - `id` — [`L78`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/repo_prep.py#L78)
  - `language` — [`L81`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/repo_prep.py#L81)
  - `name` — [`L79`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/repo_prep.py#L79)
  - `url` — [`L80`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/repo_prep.py#L80)
- used by: (7 test-only callers)

## Functions
- `_build_parser()` — [`L551`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/repo_prep.py#L551)
- `_checkout_commit(repo_dir: Path, commit: str)` — [`L228`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/repo_prep.py#L228) — Hard-checkout a specific commit (detached HEAD).
- `_clone_repo(url: str, dest: Path)` — [`L215`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/repo_prep.py#L215) — Clone a repo from url into dest (must not exist yet).
- `_cmd_prepare(args: argparse.Namespace)` — [`L445`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/repo_prep.py#L445) — Handle ``prepare`` subcommand.
- `_cmd_status(args: argparse.Namespace)` — [`L492`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/repo_prep.py#L492) — Handle ``status`` subcommand — print a table from the manifest.
- `_collect_stats(repo_dir: Path)` — [`L188`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/repo_prep.py#L188) — Walk repo_dir and return (file_count, source_file_count, size_bytes).
- `_fmt_size(size_bytes: int)` — [`L436`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/repo_prep.py#L436) — Human-readable file size.
- `_get_current_commit(repo_dir: Path)` — [`L173`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/repo_prep.py#L173) — Return the current HEAD commit SHA in the given repo dir.
- `_get_default_branch_head(repo_dir: Path)` — [`L234`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/repo_prep.py#L234) — Return the current HEAD SHA without checking out anything extra.
- `_is_excluded(path: Path, base: Path)` — [`L178`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/repo_prep.py#L178) — Return True if the path is inside an excluded directory.
- `_prepared_repo_from_dict(d: dict[str, Any])` — [`L379`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/repo_prep.py#L379) — Reconstruct a PreparedRepo from a plain dict (e.g. loaded from JSON).
- `_prepared_repo_to_dict(pr: PreparedRepo)` — [`L372`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/repo_prep.py#L372) — Convert a PreparedRepo to a JSON-serializable dict.
- `_run_git(args: list[str], cwd: Path | None = None, check: bool = True)` — [`L158`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/repo_prep.py#L158) — Run a git command and return stdout as a stripped string.
- `_stderr(*args: Any, **kwargs: Any)` — [`L153`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/repo_prep.py#L153) — Print progress messages to stderr so stdout stays machine-readable.
- `load_prepared_manifest(path: Path)` — [`L416`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/repo_prep.py#L416) — Load a list of PreparedRepo objects from a JSON manifest file.
- `load_repos_config(path: Path = REPOS_CONFIG)` — [`L107`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/repo_prep.py#L107) — Load repo specs from a YAML config file.
- `main(argv: list[str] | None = None)` — [`L584`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/repo_prep.py#L584)
- `prepare_all(repos: list[RepoSpec], base_dir: Path = DEFAULT_BASE_DIR)` — [`L350`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/repo_prep.py#L350) — Prepare every repo in ``repos`` sequentially, collecting all results.
- `prepare_repo(repo: RepoSpec, base_dir: Path = DEFAULT_BASE_DIR)` — [`L248`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/repo_prep.py#L248) — Clone repo to ``base_dir/<repo.id>/``, pin to commit, collect metadata.
- `save_prepared_manifest(repos: list[PreparedRepo], path: Path)` — [`L395`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/repo_prep.py#L395) — Serialize ``repos`` to a JSON file at ``path``.

## Module values
- `DEFAULT_BASE_DIR` — [`L40`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/repo_prep.py#L40)
- `REPOS_CONFIG` — [`L42`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/repo_prep.py#L42)
- `_DEFAULT_MANIFEST` — [`L433`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/repo_prep.py#L433)
- `_EXCLUDED_DIRS` — [`L45`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/repo_prep.py#L45)
- `_PLACEHOLDER_SHA` — [`L66`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/repo_prep.py#L66)
- `_SOURCE_EXTENSIONS` — [`L48`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/repo_prep.py#L48)

