---
title: 'Module: tree_sitter_analyzer/output_manager.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/output_manager.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.output_manager`/
symbols:
  OutputManager: OutputManager#
  output_data: output_data().
  output_error: output_error().
  OutputManager.data: OutputManager#data().
  output_info: output_info().
  output_json: output_json().
  output_list: output_list().
  _output_manager: _output_manager.
  set_output_mode: set_output_mode().
  OutputManager.quiet: OutputManager#quiet.
  output_section: output_section().
  OutputManager._formatter_registry: OutputManager#_formatter_registry.
  OutputManager.warning: OutputManager#warning().
  get_output_manager: get_output_manager().
  OutputManager.info: OutputManager#info().
  OutputManager._init_formatters: OutputManager#_init_formatters().
  OutputManager.output_list: OutputManager#output_list().
  OutputManager.output_format: OutputManager#output_format.
  output_warning: output_warning().
  output_success: output_success().
  output_query_results: output_query_results().
  output_statistics: output_statistics().
  output_languages: output_languages().
  output_queries: output_queries().
  output_extensions: output_extensions().
  OutputManager.success: OutputManager#success().
  OutputManager.results_header: OutputManager#results_header().
  OutputManager.query_result: OutputManager#query_result().
  OutputManager.error: OutputManager#error().
  OutputManager.language_list: OutputManager#language_list().
  OutputManager.query_list: OutputManager#query_list().
  OutputManager.extension_list: OutputManager#extension_list().
  OutputManager.json_output: OutputManager#json_output.
  OutputManager._format_data: OutputManager#_format_data().
  OutputManager.output_info: OutputManager#output_info().
  OutputManager.output_warning: OutputManager#output_warning().
  OutputManager.output_success: OutputManager#output_success().
  OutputManager.analysis_summary: OutputManager#analysis_summary().
  OutputManager.output_section: OutputManager#output_section().
  OutputManager.output_query_results: OutputManager#output_query_results().
  OutputManager.output_statistics: OutputManager#output_statistics().
  OutputManager.output_extensions: OutputManager#output_extensions().
  OutputManager.output_data: OutputManager#output_data().
  OutputManager.output_error: OutputManager#output_error().
  OutputManager.output_languages: OutputManager#output_languages().
  OutputManager.output_queries: OutputManager#output_queries().
  output_toon: output_toon().
  _JsonFormatter: _JsonFormatter#
  _YamlFormatter: _YamlFormatter#
  OutputManager.output_json: OutputManager#output_json().
  _JsonFormatter.format: _JsonFormatter#format().
  _YamlFormatter.format: _YamlFormatter#format().
  OutputManager.SUPPORTED_FORMATS: OutputManager#SUPPORTED_FORMATS.
  OutputManager.__init__: OutputManager#__init__().
---
# Module: [`tree_sitter_analyzer/output_manager.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/output_manager.py)

## Classes
### `OutputManager`
- def: [`tree_sitter_analyzer/output_manager.py:43`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/output_manager.py#L43)
- doc: Manages different types of output for CLI
- signature: `class OutputManager:`
- members:
  - `_format_data(self, data: Any)` — [`L177`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/output_manager.py#L177) — Format data for human-readable output
  - `_init_formatters(self)` — [`L59`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/output_manager.py#L59) — Initialize format registry with unified Formatter interface.
  - `analysis_summary(self, stats: dict[str, Any])` — [`L205`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/output_manager.py#L205) — Output analysis summary
  - `data(self, data: Any, format_type: str | None = None)` — [`L125`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/output_manager.py#L125) — Output structured data in specified format.
  - `error(self, message: str)` — [`L100`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/output_manager.py#L100) — Output error message
  - `extension_list(self, extensions: list[str])` — [`L228`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/output_manager.py#L228) — Output supported extensions
  - `info(self, message: str)` — [`L89`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/output_manager.py#L89) — Output informational message to user (stderr — keeps stdout clean for JSON/TOON).
  - `language_list(self, languages: list[str], title: str = "Supported Languages")` — [`L212`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/output_manager.py#L212) — Output language list
  - `output_data(self, data: Any, format_type: str = "json")` — [`L282`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/output_manager.py#L282) — Output data (alias for data)
  - `output_error(self, message: str)` — [`L117`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/output_manager.py#L117) — Output error message (alias for error)
  - `output_extensions(self, extensions: list[str])` — [`L278`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/output_manager.py#L278) — Output file extensions
  - `output_info(self, message: str)` — [`L109`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/output_manager.py#L109) — Output info message (alias for info)
  - `output_json(self, data: Any)` — [`L241`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/output_manager.py#L241) — Output JSON data
  - `output_languages(self, languages: list[str])` — [`L269`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/output_manager.py#L269) — Output available languages
  - `output_list(self, items: str | list[Any], title: str | None = None)` — [`L245`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/output_manager.py#L245) — Output a list of items
  - `output_queries(self, queries: list[str])` — [`L273`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/output_manager.py#L273) — Output available queries
  - `output_query_results(self, results: Any)` — [`L261`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/output_manager.py#L261) — Output query results
  - `output_section(self, title: str)` — [`L256`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/output_manager.py#L256) — Output a section header
  - `output_statistics(self, stats: dict[str, Any])` — [`L265`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/output_manager.py#L265) — Output statistics
  - `output_success(self, message: str)` — [`L121`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/output_manager.py#L121) — Output success message (alias for success)
  - `output_warning(self, message: str)` — [`L113`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/output_manager.py#L113) — Output warning message (alias for warning)
  - `query_list(self, queries: dict[str, str], language: str)` — [`L221`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/output_manager.py#L221) — Output query list for a language
  - `query_result(self, index: int, result: dict[str, Any])` — [`L193`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/output_manager.py#L193) — Output query result in formatted way
  - `results_header(self, title: str)` — [`L188`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/output_manager.py#L188) — Output results section header
  - `success(self, message: str)` — [`L104`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/output_manager.py#L104) — Output success message (stderr — diagnostic, not machine-readable data).
  - `warning(self, message: str)` — [`L94`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/output_manager.py#L94) — Output warning message
  - `SUPPORTED_FORMATS` — [`L46`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/output_manager.py#L46)
  - `json_output` — [`L55`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/output_manager.py#L55)
  - `output_format` — [`L56`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/output_manager.py#L56)
  - `quiet` — [`L54`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/output_manager.py#L54)
- protocol/private: `__init__`[`L48`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/output_manager.py#L48), `_formatter_registry`[`L57`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/output_manager.py#L57)
- uses (calls/refs, reference-scoped): [`log_warning`](utils/logging.md#log_warning), [`ToonFormatter`](formatters/toon_formatter.md#ToonFormatter), [`_JsonFormatter`](output_manager.md#_JsonFormatter), [`_YamlFormatter`](output_manager.md#_YamlFormatter)
- used by: [`output_data`](output_manager.md#output_data), [`output_error`](output_manager.md#output_error), [`output_info`](output_manager.md#output_info), [`output_json`](output_manager.md#output_json), [`output_list`](output_manager.md#output_list), [`_output_manager`](output_manager.md#_output_manager), [`set_output_mode`](output_manager.md#set_output_mode), [`output_section`](output_manager.md#output_section), [`get_output_manager`](output_manager.md#get_output_manager), [`output_extensions`](output_manager.md#output_extensions), [`output_languages`](output_manager.md#output_languages), [`output_queries`](output_manager.md#output_queries), [`output_query_results`](output_manager.md#output_query_results), [`output_statistics`](output_manager.md#output_statistics), [`output_success`](output_manager.md#output_success), [`output_warning`](output_manager.md#output_warning)  (69 test-only)

### `_JsonFormatter`
- def: [`tree_sitter_analyzer/output_manager.py:15`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/output_manager.py#L15)
- doc: JSON formatter — pretty-prints non-string data, passes strings through.
- signature: `class _JsonFormatter:`
- members:
  - `format(self, data: Any)` — [`L21`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/output_manager.py#L21)
- used by: [`_init_formatters`](output_manager.md#OutputManager._init_formatters)

### `_YamlFormatter`
- def: [`tree_sitter_analyzer/output_manager.py:27`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/output_manager.py#L27)
- doc: YAML formatter — defers the `yaml` import to `format()`.
- signature: `class _YamlFormatter:`
- members:
  - `format(self, data: Any)` — [`L35`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/output_manager.py#L35)
- used by: [`_init_formatters`](output_manager.md#OutputManager._init_formatters)

## Functions
- `get_output_manager()` — [`L297`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/output_manager.py#L297) — Get current output manager
- `output_data(data: Any, format_type: str = "json")` — [`L383`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/output_manager.py#L383) — Output structured data
- `output_error(message: str)` — [`L313`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/output_manager.py#L313) — Output error message using the global output manager
- `output_extensions(extensions: list[str])` — [`L378`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/output_manager.py#L378) — Output file extensions
- `output_info(message: str)` — [`L303`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/output_manager.py#L303) — Output info message
- `output_json(data: Any)` — [`L323`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/output_manager.py#L323) — Output JSON data using the global output manager
- `output_languages(languages: list[str], title: str = "Supported Languages")` — [`L367`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/output_manager.py#L367) — Output available languages
- `output_list(items: str | list[Any], title: str | None = None)` — [`L347`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/output_manager.py#L347) — Output a list of items
- `output_queries(queries: list[str], language: str = "All")` — [`L372`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/output_manager.py#L372) — Output available queries
- `output_query_results(results: Any)` — [`L357`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/output_manager.py#L357) — Output query results
- `output_section(title: str)` — [`L352`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/output_manager.py#L352) — Output a section header
- `output_statistics(stats: dict[str, Any])` — [`L362`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/output_manager.py#L362) — Output statistics
- `output_success(message: str)` — [`L318`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/output_manager.py#L318) — Output success message using the global output manager
- `output_toon(toon_content: str)` — [`L328`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/output_manager.py#L328) — Emit a pre-rendered TOON payload to stdout.
- `output_warning(message: str)` — [`L308`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/output_manager.py#L308) — Output warning message
- `set_output_mode(quiet: bool = False, json_output: bool = False)` — [`L291`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/output_manager.py#L291) — Set global output mode

## Module values
- `_output_manager` — [`L288`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/output_manager.py#L288)

