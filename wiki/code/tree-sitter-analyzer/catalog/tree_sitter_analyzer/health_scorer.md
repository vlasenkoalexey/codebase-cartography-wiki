---
title: 'Module: tree_sitter_analyzer/health_scorer.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/health_scorer.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.health_scorer`/
symbols:
  HealthScorer: HealthScorer#
  HealthScorer.score_file: HealthScorer#score_file().
  score_dependencies: score_dependencies().
  score_complexity: score_complexity().
  HealthScore: HealthScore#
  HealthScore.file_path: HealthScore#file_path.
  HealthScorer.score_project_with_stats: HealthScorer#score_project_with_stats().
  PROJECT_HEALTH_SOURCE_EXTS: PROJECT_HEALTH_SOURCE_EXTS.
  HealthScore.total: HealthScore#total.
  HealthScorer._score_dimensions: HealthScorer#_score_dimensions().
  _score_deps_fallback: _score_deps_fallback().
  score_structure: score_structure().
  HealthScore.grade: HealthScore#grade().
  HealthScore.dimensions: HealthScore#dimensions.
  HealthScorer.score_project: HealthScorer#score_project().
  HealthScorer._score_file_with_cache: HealthScorer#_score_file_with_cache().
  HealthScore.to_dict: HealthScore#to_dict().
  score_git_hotspot: score_git_hotspot().
  HealthScorer._load_coverage_data: HealthScorer#_load_coverage_data().
  DIMENSION_WEIGHTS: DIMENSION_WEIGHTS.
  HealthScorer._coverage_cache: HealthScorer#_coverage_cache.
  HealthScorer._iter_source_files: HealthScorer#_iter_source_files().
  DEP_IDEAL: DEP_IDEAL.
  score_size: score_size().
  CC_IDEAL: CC_IDEAL.
  HealthScorer._EXCLUDE_DIRS: HealthScorer#_EXCLUDE_DIRS.
  HealthScorer._is_excluded: HealthScorer#_is_excluded().
  score_structure.walk: score_structure().walk().
  logger: logger.
  DEP_MAX: DEP_MAX.
  CC_MODERATE: CC_MODERATE.
  HealthScorer.weights: HealthScorer#weights.
  HealthScorer.source_extensions: HealthScorer#source_extensions.
  HealthScorer._score_coverage: HealthScorer#_score_coverage().
  SIZE_IDEAL: SIZE_IDEAL.
  STRUCTURE_DEPTH_IDEAL: STRUCTURE_DEPTH_IDEAL.
  SIZE_MAX: SIZE_MAX.
  CC_COMPLEX: CC_COMPLEX.
  STRUCTURE_DEPTH_MAX: STRUCTURE_DEPTH_MAX.
  _NEUTRAL_DEP_SCORE: _NEUTRAL_DEP_SCORE.
  _DEPENDENCY_ANALYZABLE_LANGS._DEPENDENCY_ANALYZABLE_LANGS: _DEPENDENCY_ANALYZABLE_LANGS._DEPENDENCY_ANALYZABLE_LANGS.
  HOTSPOT_COMMITS_LOW: HOTSPOT_COMMITS_LOW.
  HOTSPOT_COMMITS_HIGH: HOTSPOT_COMMITS_HIGH.
  _coverage_json_is_stale: _coverage_json_is_stale().
  find_project_root: find_project_root().
  score_duplication: score_duplication().
  NESTING_MAX_DEPTH: NESTING_MAX_DEPTH.
  HealthScorer.__init__: HealthScorer#__init__().
---
# Module: [`tree_sitter_analyzer/health_scorer.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_scorer.py)

## Classes
### `HealthScore`
- def: [`tree_sitter_analyzer/health_scorer.py:101`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_scorer.py#L101)
- doc: Health score for a single source file.
- signature: `class HealthScore:`
- members:
  - `grade(self)` — [`L116`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_scorer.py#L116) — Letter grade based on total score.
  - `to_dict(self)` — [`L128`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_scorer.py#L128) — Serialize to dictionary.
  - `dimensions` — [`L113`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_scorer.py#L113)
  - `file_path` — [`L111`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_scorer.py#L111)
  - `total` — [`L112`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_scorer.py#L112)
- used by: [`_build_profile`](mcp/tools/smart_context_tool.md#SmartContextTool._build_profile), [`_collect_safe_to_edit_facts`](mcp/tools/utils/safe_to_edit_helpers.md#_collect_safe_to_edit_facts), [`score_file`](health_scorer.md#HealthScorer.score_file), [`health_facet`](mcp/tools/_codegraph_query_facets.md#health_facet), [`score_project_with_stats`](health_scorer.md#HealthScorer.score_project_with_stats), [`_collect_health_metrics`](mcp/tools/codegraph_metrics_tool.md#CodeGraphMetricsTool._collect_health_metrics), [`_score_and_echo_metrics`](mcp/tools/file_health_tool.md#FileHealthTool._score_and_echo_metrics), [`score_project`](health_scorer.md#HealthScorer.score_project), [`_score_file_with_cache`](health_scorer.md#HealthScorer._score_file_with_cache)  (20 test-only)

### `HealthScorer`
- def: [`tree_sitter_analyzer/health_scorer.py:138`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_scorer.py#L138)
- doc: Compute health scores for source files.
- signature: `class HealthScorer:`
- members:
  - `__init__(self, weights: dict[str, float] | None = None, source_extensions: set[str] | None = None)` — [`L153`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_scorer.py#L153) — Initialize the scorer.
  - `_is_excluded(self, file_path: Path, root: Path)` — [`L246`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_scorer.py#L246) — Return True when the file lives under an excluded directory.
  - `_iter_source_files(self, root: Path)` — [`L264`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_scorer.py#L264) — Return source files and a count of pruned generated/hidden dirs.
  - `_load_coverage_data(self)` — [`L408`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_scorer.py#L408) — Load coverage data from coverage.json in current or parent directories.
  - `_score_coverage(self, file_path: str)` — [`L450`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_scorer.py#L450) — Score based on test coverage. Returns None if no coverage data available.
  - `_score_dimensions(self, file_path: str, source: str, language: str | None, *, fast_dependencies: bool = False)` — [`L202`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_scorer.py#L202) — Score each health dimension for a source file.
  - `_score_file_with_cache(self, file_path: str, cache: Any)` — [`L376`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_scorer.py#L376) — Look up a cached score, fall back to fresh scoring on miss/error.
  - `score_file(self, file_path: str, *, fast_dependencies: bool = False)` — [`L173`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_scorer.py#L173) — Score a single file.
  - `score_project(self, project_root: str, *, use_cache: bool = True)` — [`L283`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_scorer.py#L283) — Score all source files; returns just the score list.
  - `score_project_with_stats(self, project_root: str, *, use_cache: bool = True)` — [`L302`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_scorer.py#L302) — Score all source files AND return walker coverage statistics.
  - `source_extensions` — [`L170`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_scorer.py#L170)
  - `weights` — [`L169`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_scorer.py#L169)
- protocol/private: `_EXCLUDE_DIRS`[`L238`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_scorer.py#L238), `_coverage_cache`[`L171`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_scorer.py#L171)
- uses (calls/refs, reference-scoped): [`EXT_TO_LANG`](_lang_extension_map.md#EXT_TO_LANG.EXT_TO_LANG), [`score_dependencies`](health_scorer.md#score_dependencies), [`score_complexity`](health_scorer.md#score_complexity), [`HealthScore`](health_scorer.md#HealthScore), [`file_path`](health_scorer.md#HealthScore.file_path), [`PROJECT_HEALTH_SOURCE_EXTS`](health_scorer.md#PROJECT_HEALTH_SOURCE_EXTS), [`total`](health_scorer.md#HealthScore.total), [`_score_deps_fallback`](health_scorer.md#_score_deps_fallback), [`score_structure`](health_scorer.md#score_structure), [`dimensions`](health_scorer.md#HealthScore.dimensions), [`EXCLUDE_DIRS`](constants.md#EXCLUDE_DIRS.EXCLUDE_DIRS), [`score_git_hotspot`](health_scorer.md#score_git_hotspot), [`close`](_health_score_cache.md#HealthScoreCache.close), [`HealthScoreCache`](_health_score_cache.md#HealthScoreCache), [`DIMENSION_WEIGHTS`](health_scorer.md#DIMENSION_WEIGHTS), [`score_size`](health_scorer.md#score_size), [`logger`](health_scorer.md#logger), [`calculate_weighted_total`](_health_scorer_helpers.md#calculate_weighted_total), [`read_source_file`](_health_scorer_helpers.md#read_source_file), [`round_available_scores`](_health_scorer_helpers.md#round_available_scores), [`_coverage_json_is_stale`](health_scorer.md#_coverage_json_is_stale), [`score_duplication`](health_scorer.md#score_duplication)
- used by: [`_build_profile`](mcp/tools/smart_context_tool.md#SmartContextTool._build_profile), [`_collect_safe_to_edit_facts`](mcp/tools/utils/safe_to_edit_helpers.md#_collect_safe_to_edit_facts), [`run_watch_health`](health_homeostasis.md#run_watch_health), [`execute`](mcp/tools/project_health_tool.md#ProjectHealthTool.execute), [`health_facet`](mcp/tools/_codegraph_query_facets.md#health_facet), [`_collect_health_metrics`](mcp/tools/codegraph_metrics_tool.md#CodeGraphMetricsTool._collect_health_metrics), [`_score_and_echo_metrics`](mcp/tools/file_health_tool.md#FileHealthTool._score_and_echo_metrics), [`_scorer`](mcp/tools/file_health_tool.md#FileHealthTool._scorer), [`_scorer`](mcp/tools/safe_to_edit_tool.md#SafeToEditTool._scorer), [`_scorer`](mcp/tools/smart_context_tool.md#SmartContextTool._scorer), [`_add_health_data`](mcp/tools/project_overview_tool.md#_add_health_data), [`_get_scorer`](mcp/tools/file_health_tool.md#FileHealthTool._get_scorer), [`_get_scorer`](mcp/tools/safe_to_edit_tool.md#SafeToEditTool._get_scorer), [`_get_scorer`](mcp/tools/smart_context_tool.md#SmartContextTool._get_scorer), [`scorer`](mcp/tools/utils/safe_to_edit_helpers.md#SafeToEditContext.scorer)  (17 test-only)

## Functions
- `_coverage_json_is_stale(cov_file: Path, coverage_db: Path)` — [`L482`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_scorer.py#L482) — Return True when pytest-cov data is newer than the JSON report.
- `_score_deps_fallback(file_path: str)` — [`L593`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_scorer.py#L593) — Fallback: score based on raw import count.
- `find_project_root(path: Path)` — [`L573`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_scorer.py#L573) — Walk up from file path to find project root.
- `score_complexity(file_path: str, source: str, language: str | None)` — [`L507`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_scorer.py#L507) — Score based on McCabe Cyclomatic Complexity.
- `score_dependencies(file_path: str)` — [`L646`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_scorer.py#L646) — Score based on real dependency graph (fan-out + fan-in).
- `score_duplication(source: str, language: str | None)` — [`L692`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_scorer.py#L692) — Score based on repeated code blocks (line-level hashing).
- `score_git_hotspot(file_path: str)` — [`L756`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_scorer.py#L756) — Score based on git commit frequency (Tornhill's hotspot analysis).
- `score_size(line_count: int)` — [`L495`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_scorer.py#L495) — Score based on file length. Smaller files get higher scores.
- `score_structure(file_path: str, source: str, language: str | None)` — [`L720`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_scorer.py#L720) — Score based on AST nesting depth relative to file size.
- `walk(node: Any, depth: int)` — [`L734`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_scorer.py#L734)

## Module values
- `CC_COMPLEX` — [`L68`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_scorer.py#L68)
- `CC_IDEAL` — [`L66`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_scorer.py#L66)
- `CC_MODERATE` — [`L67`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_scorer.py#L67)
- `DEP_IDEAL` — [`L64`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_scorer.py#L64)
- `DEP_MAX` — [`L65`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_scorer.py#L65)
- `DIMENSION_WEIGHTS` — [`L34`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_scorer.py#L34)
- `HOTSPOT_COMMITS_HIGH` — [`L75`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_scorer.py#L75)
- `HOTSPOT_COMMITS_LOW` — [`L74`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_scorer.py#L74)
- `NESTING_MAX_DEPTH` — [`L69`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_scorer.py#L69)
- `PROJECT_HEALTH_SOURCE_EXTS` — [`L44`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_scorer.py#L44)
- `SIZE_IDEAL` — [`L62`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_scorer.py#L62)
- `SIZE_MAX` — [`L63`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_scorer.py#L63)
- `STRUCTURE_DEPTH_IDEAL` — [`L70`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_scorer.py#L70)
- `STRUCTURE_DEPTH_MAX` — [`L73`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_scorer.py#L73)
- `_DEPENDENCY_ANALYZABLE_LANGS` — [`L87`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_scorer.py#L87)
- `_NEUTRAL_DEP_SCORE` — [`L97`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_scorer.py#L97)
- `logger` — [`L31`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_scorer.py#L31)

