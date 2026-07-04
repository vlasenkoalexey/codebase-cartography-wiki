---
title: 'Module: tree_sitter_analyzer/cli/info_commands.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/cli/info_commands.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.cli.info_commands`/
symbols:
  DescribeQueryCommand.execute: DescribeQueryCommand#execute().
  ShowLanguagesCommand.execute: ShowLanguagesCommand#execute().
  ShowLanguagesCommand: ShowLanguagesCommand#
  InfoCommand.args: InfoCommand#args.
  ListQueriesCommand.execute: ListQueriesCommand#execute().
  ShowExtensionsCommand.execute: ShowExtensionsCommand#execute().
  InfoCommand: InfoCommand#
  ListQueriesCommand: ListQueriesCommand#
  DescribeQueryCommand: DescribeQueryCommand#
  DescribeQueryCommand._emit_describe_query_response: DescribeQueryCommand#_emit_describe_query_response().
  DescribeQueryCommand._emit_missing_language_error: DescribeQueryCommand#_emit_missing_language_error().
  DescribeQueryCommand._emit_not_found_error: DescribeQueryCommand#_emit_not_found_error().
  DescribeQueryCommand._emit_value_error: DescribeQueryCommand#_emit_value_error().
  ShowExtensionsCommand: ShowExtensionsCommand#
  ListQueriesCommand._emit_text_query_block: ListQueriesCommand#_emit_text_query_block().
  ListQueriesCommand._emit_text_all_languages: ListQueriesCommand#_emit_text_all_languages().
  InfoCommand.execute: InfoCommand#execute().
  ListQueriesCommand._collect_query_descriptions: ListQueriesCommand#_collect_query_descriptions().
  _grammar_install_state: _grammar_install_state().
  ListQueriesCommand._emit_json: ListQueriesCommand#_emit_json().
  ListQueriesCommand._build_all_languages_envelope: ListQueriesCommand#_build_all_languages_envelope().
  ShowLanguagesCommand._build_language_entry: ShowLanguagesCommand#_build_language_entry().
  ListQueriesCommand._emit_text: ListQueriesCommand#_emit_text().
  ListQueriesCommand._emit_text_single_language: ListQueriesCommand#_emit_text_single_language().
  DescribeQueryCommand._resolve_language: DescribeQueryCommand#_resolve_language().
  ListQueriesCommand._build_single_language_envelope: ListQueriesCommand#_build_single_language_envelope().
  DescribeQueryCommand._build_describe_query_envelope: DescribeQueryCommand#_build_describe_query_envelope().
  ShowLanguagesCommand._emit_json: ShowLanguagesCommand#_emit_json().
  ShowLanguagesCommand._emit_text: ShowLanguagesCommand#_emit_text().
  _error_envelope: _error_envelope().
  InfoCommand.__init__: InfoCommand#__init__().
---
# Module: [`tree_sitter_analyzer/cli/info_commands.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/info_commands.py)

## Classes
### `DescribeQueryCommand`  ·  implements/extends InfoCommand
- def: [`tree_sitter_analyzer/cli/info_commands.py:194`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/info_commands.py#L194)
- doc: Command to describe a specific query.
- signature: `class DescribeQueryCommand(InfoCommand):`
- members:
  - `_build_describe_query_envelope(self, *, language: str, query_description: str, query_content: str)` — [`L293`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/info_commands.py#L293) — Construct the canonical ``--describe-query`` success envelope.
  - `_emit_describe_query_response(self, *, language: str, query_description: str, query_content: str)` — [`L270`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/info_commands.py#L270) — Emit the success response in JSON-envelope or legacy-text form.
  - `_emit_missing_language_error(self)` — [`L236`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/info_commands.py#L236) — ``--describe-query`` invoked without ``--language`` or a file path.
  - `_emit_not_found_error(self, language: str)` — [`L251`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/info_commands.py#L251) — Selected query key is unknown for ``language``.
  - `_emit_value_error(self, exc: ValueError)` — [`L262`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/info_commands.py#L262) — The query loader raised — surface its message in the active format.
  - `_resolve_language(self)` — [`L226`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/info_commands.py#L226) — Return the language to describe, or ``None`` when it cannot be inferred.
  - `execute(self)` — [`L204`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/info_commands.py#L204)
- uses (calls/refs, reference-scoped): [`detect_language_from_file`](../language_detector.md#detect_language_from_file), [`output_data`](../output_manager.md#output_data), [`query_loader`](../query_loader.md#query_loader), [`output_error`](../output_manager.md#output_error), [`output_info`](../output_manager.md#output_info), [`output_json`](../output_manager.md#output_json), [`wants_json_output`](output_format.md#wants_json_output), [`args`](info_commands.md#InfoCommand.args), [`InfoCommand`](info_commands.md#InfoCommand), [`get_query_description`](../query_loader.md#QueryLoader.get_query_description), [`get_query`](../query_loader.md#QueryLoader.get_query), [`_error_envelope`](info_commands.md#_error_envelope)
- used by: [`InfoCommand`](info_commands.md#InfoCommand), [`_create_info_command`](../cli_main.md#_create_info_command), [`execute`](info_commands.md#InfoCommand.execute)  (8 test-only)

### `InfoCommand`  ·  implements/extends ABC
- def: [`tree_sitter_analyzer/cli/info_commands.py:44`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/info_commands.py#L44)
- doc: Base class for information commands that don't require file analysis.
- signature: `class InfoCommand(ABC):`
- members:
  - `execute(self)` — [`L51`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/info_commands.py#L51) — Execute the information command.
  - `args` — [`L48`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/info_commands.py#L48)
- protocol/private: `__init__`[`L47`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/info_commands.py#L47)
- uses (calls/refs, reference-scoped): [`execute`](info_commands.md#DescribeQueryCommand.execute), [`execute`](info_commands.md#ShowLanguagesCommand.execute), [`ShowLanguagesCommand`](info_commands.md#ShowLanguagesCommand), [`execute`](info_commands.md#ListQueriesCommand.execute), [`execute`](info_commands.md#ShowExtensionsCommand.execute), [`DescribeQueryCommand`](info_commands.md#DescribeQueryCommand), [`ListQueriesCommand`](info_commands.md#ListQueriesCommand), [`ShowExtensionsCommand`](info_commands.md#ShowExtensionsCommand)
- used by: [`execute`](info_commands.md#DescribeQueryCommand.execute), [`execute`](info_commands.md#ShowLanguagesCommand.execute), [`ShowLanguagesCommand`](info_commands.md#ShowLanguagesCommand), [`execute`](info_commands.md#ListQueriesCommand.execute), [`execute`](info_commands.md#ShowExtensionsCommand.execute), [`DescribeQueryCommand`](info_commands.md#DescribeQueryCommand), [`ListQueriesCommand`](info_commands.md#ListQueriesCommand), [`_emit_describe_query_response`](info_commands.md#DescribeQueryCommand._emit_describe_query_response), [`ShowExtensionsCommand`](info_commands.md#ShowExtensionsCommand), [`_emit_missing_language_error`](info_commands.md#DescribeQueryCommand._emit_missing_language_error), [`_emit_not_found_error`](info_commands.md#DescribeQueryCommand._emit_not_found_error), [`_emit_value_error`](info_commands.md#DescribeQueryCommand._emit_value_error), [`_resolve_language`](info_commands.md#DescribeQueryCommand._resolve_language), [`_build_describe_query_envelope`](info_commands.md#DescribeQueryCommand._build_describe_query_envelope)  (2 test-only)

### `ListQueriesCommand`  ·  implements/extends InfoCommand
- def: [`tree_sitter_analyzer/cli/info_commands.py:56`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/info_commands.py#L56)
- doc: Command to list available queries.
- signature: `class ListQueriesCommand(InfoCommand):`
- members:
  - `_build_all_languages_envelope(self)` — [`L127`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/info_commands.py#L127) — Construct the ``--list-queries`` envelope for *all* languages.
  - `_build_single_language_envelope(self, language: str)` — [`L157`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/info_commands.py#L157) — Construct the ``--list-queries`` envelope for a single language.
  - `_collect_query_descriptions(language: str)` — [`L180`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/info_commands.py#L180) — Return ``[{key, description}]`` for every query in ``language``.
  - `_emit_json(self, language: str | None)` — [`L107`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/info_commands.py#L107) — r37ad (dogfood): JSON envelope path.
  - `_emit_text(self, language: str | None)` — [`L71`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/info_commands.py#L71) — Legacy text output (preserves backward compatibility).
  - `_emit_text_all_languages(self)` — [`L85`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/info_commands.py#L85) — Print every supported language and its queries in text form.
  - `_emit_text_query_block(language: str, *, indent: str)` — [`L98`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/info_commands.py#L98) — Emit ``"{indent}{key:<20} - {description}"`` for every query.
  - `_emit_text_single_language(self, language: str)` — [`L92`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/info_commands.py#L92) — Print the queries for a single language in text form.
  - `execute(self)` — [`L59`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/info_commands.py#L59)
- uses (calls/refs, reference-scoped): [`detect_language_from_file`](../language_detector.md#detect_language_from_file), [`query_loader`](../query_loader.md#query_loader), [`output_json`](../output_manager.md#output_json), [`wants_json_output`](output_format.md#wants_json_output), [`args`](info_commands.md#InfoCommand.args), [`InfoCommand`](info_commands.md#InfoCommand), [`get_query_description`](../query_loader.md#QueryLoader.get_query_description), [`output_list`](../output_manager.md#output_list), [`list_queries_for_language`](../query_loader.md#QueryLoader.list_queries_for_language), [`list_supported_languages`](../query_loader.md#QueryLoader.list_supported_languages)
- used by: [`InfoCommand`](info_commands.md#InfoCommand), [`_create_info_command`](../cli_main.md#_create_info_command), [`execute`](info_commands.md#InfoCommand.execute)  (9 test-only)

### `ShowExtensionsCommand`  ·  implements/extends InfoCommand
- def: [`tree_sitter_analyzer/cli/info_commands.py:390`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/info_commands.py#L390)
- doc: Command to show supported extensions.
- signature: `class ShowExtensionsCommand(InfoCommand):`
- members:
  - `execute(self)` — [`L393`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/info_commands.py#L393)
- uses (calls/refs, reference-scoped): [`detector`](../language_detector.md#detector), [`output_info`](../output_manager.md#output_info), [`output_json`](../output_manager.md#output_json), [`wants_json_output`](output_format.md#wants_json_output), [`args`](info_commands.md#InfoCommand.args), [`InfoCommand`](info_commands.md#InfoCommand), [`output_list`](../output_manager.md#output_list), [`get_supported_extensions`](../language_detector.md#LanguageDetector.get_supported_extensions)
- used by: [`InfoCommand`](info_commands.md#InfoCommand), [`_create_info_command`](../cli_main.md#_create_info_command), [`execute`](info_commands.md#InfoCommand.execute)  (4 test-only)

### `ShowLanguagesCommand`  ·  implements/extends InfoCommand
- def: [`tree_sitter_analyzer/cli/info_commands.py:324`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/info_commands.py#L324)
- doc: Command to show supported languages.
- signature: `class ShowLanguagesCommand(InfoCommand):`
- members:
  - `execute(self)` — [`L327`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/info_commands.py#L327)
- protocol/private: `_build_language_entry`[`L337`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/info_commands.py#L337), `_emit_json`[`L350`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/info_commands.py#L350), `_emit_text`[`L372`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/info_commands.py#L372)
- uses (calls/refs, reference-scoped): [`detector`](../language_detector.md#detector), [`output_json`](../output_manager.md#output_json), [`wants_json_output`](output_format.md#wants_json_output), [`args`](info_commands.md#InfoCommand.args), [`InfoCommand`](info_commands.md#InfoCommand), [`output_list`](../output_manager.md#output_list), [`get_language_info`](../language_detector.md#LanguageDetector.get_language_info), [`_grammar_install_state`](info_commands.md#_grammar_install_state), [`get_supported_languages`](../language_detector.md#LanguageDetector.get_supported_languages)
- used by: [`InfoCommand`](info_commands.md#InfoCommand), [`_create_info_command`](../cli_main.md#_create_info_command), [`execute`](info_commands.md#InfoCommand.execute)  (10 test-only)

## Functions
- `_error_envelope(message: str, *, error_type: str = "error", verdict: str = "ERROR")` — [`L432`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/info_commands.py#L432) — r37ae: shared error envelope shape for JSON info commands.
- `_grammar_install_state(language: str)` — [`L25`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/info_commands.py#L25) — Probe grammar availability without importing it.

