---
title: 'Module: tree_sitter_analyzer/cli/parser_readiness_sources.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/cli/parser_readiness_sources.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.cli.parser_readiness_sources`/
symbols:
  collect_readiness_inputs: collect_readiness_inputs().
  _add_parser_requirement: _add_parser_requirement().
  _collect_loader_modules: _collect_loader_modules().
  normalize_language: normalize_language().
  _collect_parser_packages: _collect_parser_packages().
  _package_language: _package_language().
  detect_parser_package_warnings: detect_parser_package_warnings().
  _add_extra_parser_requirements: _add_extra_parser_requirements().
  _is_parser_package: _is_parser_package().
  _requirement_package_name: _requirement_package_name().
  _collect_plugin_entrypoints: _collect_plugin_entrypoints().
  TREE_SITTER_PREFIX: TREE_SITTER_PREFIX.
  WIKI_READINESS_SIGNALS: WIKI_READINESS_SIGNALS.
  parser_package_requirements: parser_package_requirements().
  _append_unique: _append_unique().
  PACKAGE_NAME_RE: PACKAGE_NAME_RE.
  PACKAGE_LANGUAGE_ALIASES: PACKAGE_LANGUAGE_ALIASES.
  LANGUAGE_ALIASES: LANGUAGE_ALIASES.
  _build_parser_package_warning: _build_parser_package_warning().
  _load_pyproject: _load_pyproject().
  select_report_languages: select_report_languages().
---
# Module: [`tree_sitter_analyzer/cli/parser_readiness_sources.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness_sources.py)

## Functions
- `_add_extra_parser_requirements(packages: dict[str, dict[str, Any]], extra_name: str, requirements: list[str])` — [`L174`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness_sources.py#L174)
- `_add_parser_requirement(packages: dict[str, dict[str, Any]], requirement: str, source: str)` — [`L183`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness_sources.py#L183)
- `_append_unique(values: list[str], value: str)` — [`L204`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness_sources.py#L204)
- `_build_parser_package_warning(language: str, info: dict[str, Any], requirements: list[str])` — [`L99`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness_sources.py#L99) — Construct one ``parser_package_warnings`` entry.
- `_collect_loader_modules()` — [`L230`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness_sources.py#L230)
- `_collect_parser_packages(pyproject: dict[str, Any])` — [`L163`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness_sources.py#L163)
- `_collect_plugin_entrypoints(pyproject: dict[str, Any])` — [`L219`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness_sources.py#L219)
- `_is_parser_package(package_name: str)` — [`L200`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness_sources.py#L200)
- `_load_pyproject(project_root: Path)` — [`L150`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness_sources.py#L150)
- `_package_language(package_name: str)` — [`L214`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness_sources.py#L214)
- `_requirement_package_name(requirement: str)` — [`L209`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness_sources.py#L209)
- `collect_readiness_inputs(root: Path)` — [`L45`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness_sources.py#L45) — Collect local metadata sources used by the readiness advisor.
- `detect_parser_package_warnings(parser_packages: dict[str, dict[str, Any]])` — [`L65`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness_sources.py#L65) — Flag languages whose parser package is declared in multiple
- `normalize_language(language: str)` — [`L128`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness_sources.py#L128) — Normalize aliases and punctuation in user-facing language names.
- `parser_package_requirements(parser_packages: dict[str, dict[str, Any]])` — [`L55`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness_sources.py#L55) — Return parser package requirements keyed by normalized language.
- `select_report_languages(parser_packages: dict[str, dict[str, Any]], plugin_entrypoints: dict[str, str], *, requested_language: str | None, include_supported: bool)` — [`L134`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness_sources.py#L134) — Choose which normalized languages should appear in the report.

## Module values
- `LANGUAGE_ALIASES` — [`L26`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness_sources.py#L26)
- `PACKAGE_LANGUAGE_ALIASES` — [`L23`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness_sources.py#L23)
- `PACKAGE_NAME_RE` — [`L22`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness_sources.py#L22)
- `TREE_SITTER_PREFIX` — [`L21`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness_sources.py#L21)
- `WIKI_READINESS_SIGNALS` — [`L37`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness_sources.py#L37)

