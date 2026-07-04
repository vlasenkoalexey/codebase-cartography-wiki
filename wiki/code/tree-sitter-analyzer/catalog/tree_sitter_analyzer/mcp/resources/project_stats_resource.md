---
title: 'Module: tree_sitter_analyzer/mcp/resources/project_stats_resource.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/resources/project_stats_resource.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.resources.project_stats_resource`/
symbols:
  ProjectStatsResource: ProjectStatsResource#
  ProjectStatsResource.read_resource: ProjectStatsResource#read_resource().
  ProjectStatsResource._generate_languages_stats: ProjectStatsResource#_generate_languages_stats().
  ProjectStatsResource._generate_complexity_stats: ProjectStatsResource#_generate_complexity_stats().
  ProjectStatsResource.set_project_path: ProjectStatsResource#set_project_path().
  ProjectStatsResource._generate_overview_stats: ProjectStatsResource#_generate_overview_stats().
  ProjectStatsResource._generate_files_stats: ProjectStatsResource#_generate_files_stats().
  ProjectStatsResource._project_path: ProjectStatsResource#_project_path.
  logger: logger.
  ProjectStatsResource.project_root: ProjectStatsResource#project_root().
  ProjectStatsResource.matches_uri: ProjectStatsResource#matches_uri().
  ProjectStatsResource._is_supported_code_file: ProjectStatsResource#_is_supported_code_file().
  ProjectStatsResource._generate_stats: ProjectStatsResource#_generate_stats().
  ProjectStatsResource._get_language_from_file: ProjectStatsResource#_get_language_from_file().
  ProjectStatsResource._supported_stats_types: ProjectStatsResource#_supported_stats_types.
  ProjectStatsResource.get_resource_info: ProjectStatsResource#get_resource_info().
  ProjectStatsResource.analysis_engine: ProjectStatsResource#analysis_engine.
  ProjectStatsResource.__repr__: ProjectStatsResource#__repr__().
  ProjectStatsResource._extract_stats_type: ProjectStatsResource#_extract_stats_type().
  ProjectStatsResource._validate_project_path: ProjectStatsResource#_validate_project_path().
  ProjectStatsResource.get_supported_stats_types: ProjectStatsResource#get_supported_stats_types().
  ProjectStatsResource._uri_pattern: ProjectStatsResource#_uri_pattern.
  ProjectStatsResource.get_supported_schemes: ProjectStatsResource#get_supported_schemes().
  ProjectStatsResource.get_supported_resource_types: ProjectStatsResource#get_supported_resource_types().
  ProjectStatsResource.__init__: ProjectStatsResource#__init__().
  ProjectStatsResource.__str__: ProjectStatsResource#__str__().
---
# Module: [`tree_sitter_analyzer/mcp/resources/project_stats_resource.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/resources/project_stats_resource.py)

## Classes
### `ProjectStatsResource`
- def: [`tree_sitter_analyzer/mcp/resources/project_stats_resource.py:38`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/resources/project_stats_resource.py#L38) — documented in [tree_sitter_analyzer-mcp-server](../../../../concepts/tree_sitter_analyzer-mcp-server.md)
- doc: MCP resource for accessing project statistics and analysis data
- signature: `class ProjectStatsResource:`
- members:
  - `__init__(self)` — [`L61`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/resources/project_stats_resource.py#L61) — Initialize the project statistics resource
  - `__repr__(self)` — [`L385`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/resources/project_stats_resource.py#L385) — Detailed string representation of the resource
  - `__str__(self)` — [`L381`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/resources/project_stats_resource.py#L381) — String representation of the resource
  - `_extract_stats_type(self, uri: str)` — [`L109`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/resources/project_stats_resource.py#L109) — Extract statistics type from URI
  - `_generate_complexity_stats(self)` — [`L256`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/resources/project_stats_resource.py#L256) — Generate complexity statistics
  - `_generate_files_stats(self)` — [`L279`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/resources/project_stats_resource.py#L279) — Generate file-level statistics
  - `_generate_languages_stats(self)` — [`L235`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/resources/project_stats_resource.py#L235) — Generate language-specific statistics
  - `_generate_overview_stats(self)` — [`L213`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/resources/project_stats_resource.py#L213) — Generate overview statistics for the project
  - `_generate_stats(self, stats_type: str)` — [`L341`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/resources/project_stats_resource.py#L341) — Dispatch a supported stats type to its generator.
  - `_get_language_from_file(self, file_path: Path)` — [`L196`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/resources/project_stats_resource.py#L196) — Get language from file using language detector
  - `_is_supported_code_file(self, file_path: Path)` — [`L178`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/resources/project_stats_resource.py#L178) — Check if file is a supported code file using language detection
  - `_validate_project_path(self)` — [`L154`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/resources/project_stats_resource.py#L154) — Validate that project path is set and exists
  - `get_resource_info(self)` — [`L81`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/resources/project_stats_resource.py#L81) — Get resource information for MCP registration
  - `get_supported_resource_types(self)` — [`L363`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/resources/project_stats_resource.py#L363) — Get list of supported resource types
  - `get_supported_schemes(self)` — [`L354`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/resources/project_stats_resource.py#L354) — Get list of supported URI schemes
  - `get_supported_stats_types(self)` — [`L372`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/resources/project_stats_resource.py#L372) — Get list of supported statistics types
  - `matches_uri(self, uri: str)` — [`L95`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/resources/project_stats_resource.py#L95) — Check if the URI matches this resource pattern
  - `project_root(self)` — [`L72`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/resources/project_stats_resource.py#L72) — Get current project root path
  - `read_resource(self, uri: str)` — [`L299`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/resources/project_stats_resource.py#L299) — Read resource content from URI
  - `set_project_path(self, project_path: str)` — [`L130`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/resources/project_stats_resource.py#L130) — Set the project path for analysis
  - `analysis_engine` — [`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/resources/project_stats_resource.py#L65)
- protocol/private: `_project_path`[`L64`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/resources/project_stats_resource.py#L64), `_supported_stats_types`[`L69`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/resources/project_stats_resource.py#L69), `_uri_pattern`[`L63`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/resources/project_stats_resource.py#L63)
- uses (calls/refs, reference-scoped): [`detect_language_from_file`](../../language_detector.md#detect_language_from_file), [`get_analysis_engine`](../../core/analysis_engine.md#get_analysis_engine), [`is_language_supported`](../../language_detector.md#is_language_supported), [`logger`](project_stats_resource.md#logger), [`collect_complexity_data`](_project_stats_resource_helpers.md#collect_complexity_data), [`collect_files_data`](_project_stats_resource_helpers.md#collect_files_data), [`collect_language_scan`](_project_stats_resource_helpers.md#collect_language_scan), [`collect_overview_scan`](_project_stats_resource_helpers.md#collect_overview_scan), [`require_project_dir`](_project_stats_resource_helpers.md#require_project_dir), [`build_complexity_stats`](_project_stats_resource_helpers.md#build_complexity_stats), [`build_files_stats`](_project_stats_resource_helpers.md#build_files_stats), [`build_languages_stats`](_project_stats_resource_helpers.md#build_languages_stats), [`build_overview_stats`](_project_stats_resource_helpers.md#build_overview_stats), [`build_languages_list`](_project_stats_resource_helpers.md#build_languages_list)
- used by: [`set_project_path`](../server.md#TreeSitterAnalyzerMCPServer.set_project_path), [`project_stats_resource`](../server.md#TreeSitterAnalyzerMCPServer.project_stats_resource)  (68 test-only)

## Module values
- `logger` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/resources/project_stats_resource.py#L35)

