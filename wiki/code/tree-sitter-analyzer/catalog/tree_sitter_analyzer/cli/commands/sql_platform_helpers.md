---
title: 'Module: tree_sitter_analyzer/cli/commands/sql_platform_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/cli/commands/sql_platform_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.cli.commands.sql_platform_helpers`/
symbols:
  handle_sql_platform_info: handle_sql_platform_info().
  _load_profile: _load_profile().
  handle_record_sql_profile: handle_record_sql_profile().
  handle_compare_sql_profiles: handle_compare_sql_profiles().
  _emit_sql_platform_json: _emit_sql_platform_json().
  _sql_platform_profile_payload: _sql_platform_profile_payload().
  _emit_sql_platform_text: _emit_sql_platform_text().
---
# Module: [`tree_sitter_analyzer/cli/commands/sql_platform_helpers.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/sql_platform_helpers.py)

## Functions
- `_emit_sql_platform_json(output_json_fn: Any, info: Any, profile: Any)` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/sql_platform_helpers.py#L19) — Emit the canonical JSON envelope for ``sql_platform_info``.
- `_emit_sql_platform_text(output_list_fn: Any, info: Any, profile: Any)` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/sql_platform_helpers.py#L49) — Emit the legacy human-readable text output (multi-line list).
- `_load_profile(path: pathlib.Path)` — [`L166`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/sql_platform_helpers.py#L166) — Load a BehaviorProfile from a JSON file.
- `_sql_platform_profile_payload(profile: Any)` — [`L8`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/sql_platform_helpers.py#L8) — Project the loaded ``BehaviorProfile`` into the JSON envelope shape.
- `handle_compare_sql_profiles(profile_paths: list[str], output_error_fn: Any)` — [`L133`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/sql_platform_helpers.py#L133) — Compare two SQL behavior profiles.
- `handle_record_sql_profile(output_info_fn: Any, output_error_fn: Any)` — [`L112`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/sql_platform_helpers.py#L112) — Record a SQL behavior profile for the current platform.
- `handle_sql_platform_info(output_list_fn: Any, output_json_fn: Any = None, args: Any = None)` — [`L82`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/sql_platform_helpers.py#L82) — Display SQL platform detection details.

