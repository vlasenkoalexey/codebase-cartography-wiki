---
title: 'Module: tree_sitter_analyzer/cli/parser_readiness_records.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/cli/parser_readiness_records.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.cli.parser_readiness_records`/
symbols:
  _build_language_record: _build_language_record().
  _local_parser_package_signals: _local_parser_package_signals().
  _build_language_signals: _build_language_signals().
  _readiness_status: _readiness_status().
  _next_steps: _next_steps().
  _upstream_next_steps: _upstream_next_steps().
  build_language_records: build_language_records().
  _packaged_file_signal: _packaged_file_signal().
  _scanner_signal: _scanner_signal().
  _module_name_for_language: _module_name_for_language().
  _count_matching_files: _count_matching_files().
  _language_record_actions: _language_record_actions().
  _artifact_signals: _artifact_signals().
  _has_loader_mapping: _has_loader_mapping().
  _loader_keys: _loader_keys().
  _readiness_score: _readiness_score().
  _maintenance_check_url: _maintenance_check_url().
  _metadata_signals: _metadata_signals().
  _is_supported: _is_supported().
  LOADER_ALIASES: LOADER_ALIASES.
  _semantic_version_text: _semantic_version_text().
  _relative_display: _relative_display().
  _module_is_installed: _module_is_installed().
  _path_matches_language: _path_matches_language().
  _verification_commands: _verification_commands().
  SCORE_WEIGHTS: SCORE_WEIGHTS.
  _language_record_metadata: _language_record_metadata().
  _first_project_url: _first_project_url().
  _parser_language_signals: _parser_language_signals().
  _unknown_upstream_signals: _unknown_upstream_signals().
  NEXT_STEP_RULES: NEXT_STEP_RULES.
  _package_root: _package_root().
  _append_unresolved_parser_artifact_steps: _append_unresolved_parser_artifact_steps().
---
# Module: [`tree_sitter_analyzer/cli/parser_readiness_records.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness_records.py)

## Functions
- `_append_unresolved_parser_artifact_steps(steps: list[str], signals: dict[str, Any])` — [`L373`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness_records.py#L373)
- `_artifact_signals(project_root: Path, language: str)` — [`L156`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness_records.py#L156) — Build local test and fixture presence signals.
- `_build_language_record(project_root: Path, language: str, parser_packages: dict[str, dict[str, Any]], plugin_entrypoints: dict[str, str], loader_modules: dict[str, str])` — [`L65`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness_records.py#L65)
- `_build_language_signals(project_root: Path, language: str, parser_info: dict[str, Any], plugin_entrypoints: dict[str, str], loader_modules: dict[str, str], module_name: str)` — [`L124`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness_records.py#L124) — Build local and upstream-to-verify readiness signals for one language.
- `_count_matching_files(root: Path, language: str)` — [`L312`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness_records.py#L312)
- `_first_project_url(project_urls: dict[str, str])` — [`L397`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness_records.py#L397)
- `_has_loader_mapping(language: str, loader_modules: dict[str, str])` — [`L304`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness_records.py#L304)
- `_is_supported(signals: dict[str, Any])` — [`L341`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness_records.py#L341)
- `_language_record_actions(language: str, signals: dict[str, Any])` — [`L112`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness_records.py#L112) — Return action fields for a language readiness record.
- `_language_record_metadata(language: str, parser_info: dict[str, Any], plugin_entrypoints: dict[str, str], status: str, score: int)` — [`L93`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness_records.py#L93) — Return non-action fields for a language readiness record.
- `_loader_keys(language: str)` — [`L308`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness_records.py#L308)
- `_local_parser_package_signals(module_name: str, parser_info: dict[str, Any])` — [`L174`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness_records.py#L174) — Return upstream-risk signals that can be checked from the local package.
- `_maintenance_check_url(signals: dict[str, Any])` — [`L403`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness_records.py#L403)
- `_metadata_signals(language: str, parser_info: dict[str, Any], plugin_entrypoints: dict[str, str], loader_modules: dict[str, str])` — [`L142`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness_records.py#L142) — Build local metadata presence signals.
- `_module_is_installed(module_name: str)` — [`L288`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness_records.py#L288)
- `_module_name_for_language(language: str, parser_info: dict[str, Any], loader_modules: dict[str, str])` — [`L292`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness_records.py#L292)
- `_next_steps(language: str, signals: dict[str, Any])` — [`L354`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness_records.py#L354)
- `_package_root(spec: Any)` — [`L224`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness_records.py#L224)
- `_packaged_file_signal(package_root: Path | None, filename: str)` — [`L258`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness_records.py#L258)
- `_parser_language_signals(module_name: str)` — [`L229`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness_records.py#L229)
- `_path_matches_language(path: Path, language: str)` — [`L322`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness_records.py#L322)
- `_readiness_score(signals: dict[str, Any])` — [`L327`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness_records.py#L327)
- `_readiness_status(signals: dict[str, Any])` — [`L331`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness_records.py#L331)
- `_relative_display(root: Path, path: Path)` — [`L281`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness_records.py#L281)
- `_scanner_signal(package_root: Path | None)` — [`L267`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness_records.py#L267)
- `_semantic_version_text(semantic_version: Any)` — [`L252`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness_records.py#L252)
- `_unknown_upstream_signals()` — [`L208`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness_records.py#L208) — Return upstream parser signals that still need parser availability.
- `_upstream_next_steps(signals: dict[str, Any])` — [`L363`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness_records.py#L363)
- `_verification_commands(language: str)` — [`L412`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness_records.py#L412)
- `build_language_records(root: Path, report_languages: list[str], inputs: dict[str, Any])` — [`L47`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness_records.py#L47) — Build readiness records for selected languages.

## Module values
- `LOADER_ALIASES` — [`L16`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness_records.py#L16)
- `NEXT_STEP_RULES` — [`L29`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness_records.py#L29)
- `SCORE_WEIGHTS` — [`L21`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness_records.py#L21)

