---
title: 'Module: tree_sitter_analyzer/mcp/resources/_project_stats_resource_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/resources/_project_stats_resource_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.resources._project_stats_resource_helpers`/
symbols:
  file_complexity: file_complexity().
  collect_overview_scan: collect_overview_scan().
  collect_language_scan: collect_language_scan().
  collect_complexity_data: collect_complexity_data().
  collect_files_data: collect_files_data().
  iter_supported_code_files: iter_supported_code_files().
  read_line_count: read_line_count().
  SupportedFilePredicate: SupportedFilePredicate.
  require_project_dir: require_project_dir().
  build_overview_stats: build_overview_stats().
  build_languages_stats: build_languages_stats().
  build_complexity_stats: build_complexity_stats().
  build_files_stats: build_files_stats().
  LanguageResolver: LanguageResolver.
  current_timestamp: current_timestamp().
  build_languages_list: build_languages_list().
  java_analysis_complexity: java_analysis_complexity().
  analysis_result_complexity: analysis_result_complexity().
---
# Module: [`tree_sitter_analyzer/mcp/resources/_project_stats_resource_helpers.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/resources/_project_stats_resource_helpers.py)

## Functions
- `analysis_result_complexity(file_analysis_result: Any)` — [`L181`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/resources/_project_stats_resource_helpers.py#L181) — Extract total complexity from the generic analysis result shape.
- `build_complexity_stats(complexity_data: list[dict[str, Any]])` — [`L240`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/resources/_project_stats_resource_helpers.py#L240) — Build the public complexity response payload.
- `build_files_stats(files_data: list[dict[str, Any]])` — [`L296`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/resources/_project_stats_resource_helpers.py#L296) — Build the public files response payload.
- `build_languages_list(total_lines: int, language_data: dict[str, dict[str, int]])` — [`L136`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/resources/_project_stats_resource_helpers.py#L136) — Convert language counters to the public list format.
- `build_languages_stats(languages_list: list[dict[str, Any]])` — [`L158`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/resources/_project_stats_resource_helpers.py#L158) — Build the public languages response payload.
- `build_overview_stats(project_path: str | None, total_files: int, total_lines: int, language_counts: dict[str, int])` — [`L89`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/resources/_project_stats_resource_helpers.py#L89) — Build the public overview response payload.
- `collect_complexity_data(project_dir: Path, analysis_engine: Any, is_supported_file: SupportedFilePredicate, get_language: LanguageResolver, *, logger: logging.Logger)` — [`L211`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/resources/_project_stats_resource_helpers.py#L211) — Analyze supported files and collect positive complexity scores.
- `collect_files_data(project_dir: Path, is_supported_file: SupportedFilePredicate, get_language: LanguageResolver, *, logger: logging.Logger)` — [`L263`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/resources/_project_stats_resource_helpers.py#L263) — Collect per-file metadata for supported code files.
- `collect_language_scan(project_dir: Path, is_supported_file: SupportedFilePredicate, get_language: LanguageResolver, *, logger: logging.Logger)` — [`L105`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/resources/_project_stats_resource_helpers.py#L105) — Collect per-language file and line counts.
- `collect_overview_scan(project_dir: Path, is_supported_file: SupportedFilePredicate, get_language: LanguageResolver, *, logger: logging.Logger)` — [`L58`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/resources/_project_stats_resource_helpers.py#L58) — Collect file, line, and language counts for overview stats.
- `current_timestamp()` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/resources/_project_stats_resource_helpers.py#L25) — Return a consistent timestamp for stats responses.
- `file_complexity(file_path: Path, language: str, analysis_engine: Any)` — [`L196`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/resources/_project_stats_resource_helpers.py#L196) — Analyze a single file and return its total complexity.
- `iter_supported_code_files(project_dir: Path, is_supported_file: SupportedFilePredicate)` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/resources/_project_stats_resource_helpers.py#L30) — Collect supported code files under a project directory.
- `java_analysis_complexity(file_analysis: Any)` — [`L167`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/resources/_project_stats_resource_helpers.py#L167) — Extract complexity from Java analysis result shapes.
- `read_line_count(file_path: Path, *, logger: logging.Logger, failure_message: str, default: int | None)` — [`L42`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/resources/_project_stats_resource_helpers.py#L42) — Read a file line count with caller-selected failure behavior.
- `require_project_dir(project_path: str | None)` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/resources/_project_stats_resource_helpers.py#L18) — Return the configured project directory or raise the legacy error.

## Module values
- `LanguageResolver` — [`L15`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/resources/_project_stats_resource_helpers.py#L15)
- `SupportedFilePredicate` — [`L14`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/resources/_project_stats_resource_helpers.py#L14)

