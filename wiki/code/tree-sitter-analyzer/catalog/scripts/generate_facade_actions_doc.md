---
title: 'Module: scripts/generate_facade_actions_doc.py'
type: catalog
provenance: extracted
module: scripts/generate_facade_actions_doc.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `scripts.generate_facade_actions_doc`/
symbols:
  collect_rows: collect_rows().
  generate_markdown: generate_markdown().
  _cli_twin_map: _cli_twin_map().
  _bespoke_params_cell: _bespoke_params_cell().
  main: main().
  PROJECT_ROOT: PROJECT_ROOT.
  DOC_PATH: DOC_PATH.
  CONTRACTS_TEST_PATH: CONTRACTS_TEST_PATH.
  ActionRow: ActionRow#
  BESPOKE_ROUTE_SPECS.BESPOKE_ROUTE_SPECS: BESPOKE_ROUTE_SPECS.BESPOKE_ROUTE_SPECS.
  _load_tool_to_cli: _load_tool_to_cli().
  NO_CLI_TWIN: NO_CLI_TWIN.
  ActionRow.action: ActionRow#action.
  ActionRow.cli_twin: ActionRow#cli_twin.
  _escape_cell: _escape_cell().
  ActionRow.params: ActionRow#params.
  ActionRow.response_keys: ActionRow#response_keys.
  _render_cli_entry: _render_cli_entry().
  _input_schema_of: _input_schema_of().
  _params_cell_from_schema: _params_cell_from_schema().
  _response_cell: _response_cell().
  CONDITIONAL_PARAM_NOTES.CONDITIONAL_PARAM_NOTES: CONDITIONAL_PARAM_NOTES.CONDITIONAL_PARAM_NOTES.
  REGEN_COMMAND: REGEN_COMMAND.
  DRIFT_TEST: DRIFT_TEST.
---
# Module: [`scripts/generate_facade_actions_doc.py`](../../../../../raw/code/tree-sitter-analyzer/scripts/generate_facade_actions_doc.py)

## Classes
### `ActionRow`
- def: [`scripts/generate_facade_actions_doc.py:150`](../../../../../raw/code/tree-sitter-analyzer/scripts/generate_facade_actions_doc.py#L150)
- doc: One rendered table row: a routable (facade, action) pair.
- signature: `class ActionRow:`
- members:
  - `action` — [`L153`](../../../../../raw/code/tree-sitter-analyzer/scripts/generate_facade_actions_doc.py#L153)
  - `cli_twin` — [`L156`](../../../../../raw/code/tree-sitter-analyzer/scripts/generate_facade_actions_doc.py#L156)
  - `params` — [`L154`](../../../../../raw/code/tree-sitter-analyzer/scripts/generate_facade_actions_doc.py#L154)
  - `response_keys` — [`L155`](../../../../../raw/code/tree-sitter-analyzer/scripts/generate_facade_actions_doc.py#L155)
- used by: [`collect_rows`](generate_facade_actions_doc.md#collect_rows), [`generate_markdown`](generate_facade_actions_doc.md#generate_markdown)

## Functions
- `_bespoke_params_cell(facade_name: str, action: str, spec: dict[str, Any])` — [`L281`](../../../../../raw/code/tree-sitter-analyzer/scripts/generate_facade_actions_doc.py#L281) — Render a bespoke route's params cell from its pinned spec.
- `_cli_twin_map()` — [`L197`](../../../../../raw/code/tree-sitter-analyzer/scripts/generate_facade_actions_doc.py#L197) — Build ``{(facade, action): rendered CLI twin cell}`` from the crosswalk.
- `_escape_cell(text: str)` — [`L361`](../../../../../raw/code/tree-sitter-analyzer/scripts/generate_facade_actions_doc.py#L361) — Escape pipes so cells never break the markdown table.
- `_input_schema_of(tool: Any)` — [`L227`](../../../../../raw/code/tree-sitter-analyzer/scripts/generate_facade_actions_doc.py#L227)
- `_load_tool_to_cli()` — [`L164`](../../../../../raw/code/tree-sitter-analyzer/scripts/generate_facade_actions_doc.py#L164) — Extract the ``tool_to_cli`` parity table from the agent-contracts test.
- `_params_cell_from_schema(schema: dict[str, Any])` — [`L233`](../../../../../raw/code/tree-sitter-analyzer/scripts/generate_facade_actions_doc.py#L233) — Render the params cell: required first (marked ``*``), then optional.
- `_render_cli_entry(kind: str, name: str)` — [`L190`](../../../../../raw/code/tree-sitter-analyzer/scripts/generate_facade_actions_doc.py#L190) — Render one CLI parity entry (main flag vs console script).
- `_response_cell(tool: Any)` — [`L258`](../../../../../raw/code/tree-sitter-analyzer/scripts/generate_facade_actions_doc.py#L258) — Render the statically-declared response surface (ToolResponse envelope).
- `collect_rows()` — [`L303`](../../../../../raw/code/tree-sitter-analyzer/scripts/generate_facade_actions_doc.py#L303) — Walk the live facade registry into ``{facade: [ActionRow, ...]}``.
- `generate_markdown()` — [`L366`](../../../../../raw/code/tree-sitter-analyzer/scripts/generate_facade_actions_doc.py#L366) — Render the full reference document as a string (deterministic).
- `main()` — [`L439`](../../../../../raw/code/tree-sitter-analyzer/scripts/generate_facade_actions_doc.py#L439)

## Module values
- `BESPOKE_ROUTE_SPECS` — [`L83`](../../../../../raw/code/tree-sitter-analyzer/scripts/generate_facade_actions_doc.py#L83)
- `CONDITIONAL_PARAM_NOTES` — [`L73`](../../../../../raw/code/tree-sitter-analyzer/scripts/generate_facade_actions_doc.py#L73)
- `CONTRACTS_TEST_PATH` — [`L50`](../../../../../raw/code/tree-sitter-analyzer/scripts/generate_facade_actions_doc.py#L50)
- `DOC_PATH` — [`L49`](../../../../../raw/code/tree-sitter-analyzer/scripts/generate_facade_actions_doc.py#L49)
- `DRIFT_TEST` — [`L54`](../../../../../raw/code/tree-sitter-analyzer/scripts/generate_facade_actions_doc.py#L54)
- `NO_CLI_TWIN` — [`L57`](../../../../../raw/code/tree-sitter-analyzer/scripts/generate_facade_actions_doc.py#L57)
- `PROJECT_ROOT` — [`L48`](../../../../../raw/code/tree-sitter-analyzer/scripts/generate_facade_actions_doc.py#L48)
- `REGEN_COMMAND` — [`L53`](../../../../../raw/code/tree-sitter-analyzer/scripts/generate_facade_actions_doc.py#L53)

