---
title: 'Module: tree_sitter_analyzer/cli/commands/query_command.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/cli/commands/query_command.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.cli.commands.query_command`/
symbols:
  QueryCommand: QueryCommand#
  QueryCommand._resolve_query: QueryCommand#_resolve_query().
  QueryCommand.execute_query: QueryCommand#execute_query().
  QueryCommand._emit_query_results: QueryCommand#_emit_query_results().
  QueryCommand.execute_async: QueryCommand#execute_async().
  QueryCommand.query_service: QueryCommand#query_service.
  _toon_available: _toon_available.
  QueryCommand._build_query_envelope: QueryCommand#_build_query_envelope().
  QueryCommand.__init__: QueryCommand#__init__().
---
# Module: [`tree_sitter_analyzer/cli/commands/query_command.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/query_command.py)

## Classes
### `QueryCommand`  ·  implements/extends BaseCommand
- def: [`tree_sitter_analyzer/cli/commands/query_command.py:23`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/query_command.py#L23)
- doc: Command for executing queries.
- signature: `class QueryCommand(BaseCommand):`
- members:
  - `__init__(self, args: Any)` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/query_command.py#L26) — Initialize the query command with QueryService.
  - `_build_query_envelope(self, *, language: str, query_to_execute: str, query_name: str, results: list[dict[str, Any]] | None)` — [`L122`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/query_command.py#L122) — Wrap ``results`` in the r37ac canonical envelope.
  - `_emit_query_results(self, envelope: dict[str, Any], results: list[dict[str, Any]] | None)` — [`L163`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/query_command.py#L163) — Output ``envelope`` via json / toon / text per ``--output-format``.
  - `_resolve_query(self, language: str)` — [`L88`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/query_command.py#L88) — Return ``(query_to_execute, query_name)`` or an exit code on error. — documented in [tree_sitter_analyzer-security-validator](../../../../concepts/tree_sitter_analyzer-security-validator.md)
  - `execute_async(self, language: str)` — [`L62`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/query_command.py#L62) — Run the requested query and emit the canonical response envelope.
  - `execute_query(self, language: str, query: str, query_name: str = "custom")` — [`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/query_command.py#L31) — Execute a specific tree-sitter query using QueryService.
  - `query_service` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/query_command.py#L29)
- uses (calls/refs, reference-scoped): [`ToonFormatter`](../../formatters/toon_formatter.md#ToonFormatter), [`args`](base_command.md#BaseCommand.args), [`QueryService`](../../core/query_service.md#QueryService), [`execute_query`](../../core/query_service.md#QueryService.execute_query), [`output_data`](../../output_manager.md#output_data), [`output_error`](../../output_manager.md#output_error), [`validate_pattern`](../../security/regex_checker.md#RegexSafetyChecker.validate_pattern), [`BaseCommand`](base_command.md#BaseCommand), [`format`](../../formatters/toon_formatter.md#ToonFormatter.format), [`output_info`](../../output_manager.md#output_info), [`output_json`](../../output_manager.md#output_json), [`sanitize_input`](../../security/validator.md#SecurityValidator.sanitize_input), [`get_available_queries`](../../core/query_service.md#QueryService.get_available_queries), [`regex_checker`](../../security/validator.md#SecurityValidator.regex_checker), [`security_validator`](base_command.md#BaseCommand.security_validator), [`_toon_available`](query_command.md#_toon_available), [`__init__`](base_command.md#BaseCommand.__init__)
- used by: [`BaseCommand`](base_command.md#BaseCommand), [`execute_async`](base_command.md#BaseCommand.execute_async), [`_create_file_command`](../../cli_main.md#_create_file_command)  (17 test-only)

## Module values
- `_toon_available` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/query_command.py#L18)

