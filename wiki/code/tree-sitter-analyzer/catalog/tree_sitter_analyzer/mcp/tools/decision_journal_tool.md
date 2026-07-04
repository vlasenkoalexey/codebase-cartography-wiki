---
title: 'Module: tree_sitter_analyzer/mcp/tools/decision_journal_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/decision_journal_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.decision_journal_tool`/
symbols:
  DecisionJournalTool._mode_record: DecisionJournalTool#_mode_record().
  DecisionJournalTool._mode_get: DecisionJournalTool#_mode_get().
  DecisionJournalTool._mode_supersede: DecisionJournalTool#_mode_supersede().
  DecisionJournalTool._mode_search: DecisionJournalTool#_mode_search().
  DecisionJournalTool.execute: DecisionJournalTool#execute().
  DecisionJournalTool._dispatch_mode: DecisionJournalTool#_dispatch_mode().
  _record_to_envelope_dict: _record_to_envelope_dict().
  DecisionJournalTool._get_journal: DecisionJournalTool#_get_journal().
  DecisionJournalTool: DecisionJournalTool#
  _summary_line_for_mode: _summary_line_for_mode().
  _next_step_for_mode: _next_step_for_mode().
  DecisionJournalTool.get_tool_schema: DecisionJournalTool#get_tool_schema().
  DecisionJournalTool.validate_arguments: DecisionJournalTool#validate_arguments().
  DecisionJournalTool._error_envelope: DecisionJournalTool#_error_envelope().
  DecisionJournalTool.__init__: DecisionJournalTool#__init__().
  DecisionJournalTool._journal: DecisionJournalTool#_journal.
  _VALID_MODES: _VALID_MODES.
  DecisionJournalTool._on_project_root_changed: DecisionJournalTool#_on_project_root_changed().
  DecisionJournalTool.get_tool_definition: DecisionJournalTool#get_tool_definition().
---
# Module: [`tree_sitter_analyzer/mcp/tools/decision_journal_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/decision_journal_tool.py)

## Classes
### `DecisionJournalTool`  ·  implements/extends BaseMCPTool
- def: [`tree_sitter_analyzer/mcp/tools/decision_journal_tool.py:78`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/decision_journal_tool.py#L78)
- doc: MCP tool exposing the decision journal across record/get/search/supersede.
- signature: `class DecisionJournalTool(BaseMCPTool):`
- members:
  - `execute(self, arguments: dict[str, Any])` — [`L225`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/decision_journal_tool.py#L225)
  - `get_tool_definition(self)` — [`L99`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/decision_journal_tool.py#L99)
  - `get_tool_schema(self)` — [`L146`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/decision_journal_tool.py#L146)
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L205`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/decision_journal_tool.py#L205)
- protocol/private: `__init__`[`L81`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/decision_journal_tool.py#L81), `_dispatch_mode`[`L238`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/decision_journal_tool.py#L238), `_error_envelope`[`L396`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/decision_journal_tool.py#L396), `_get_journal`[`L89`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/decision_journal_tool.py#L89), `_journal`[`L82`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/decision_journal_tool.py#L82), `_mode_get`[`L283`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/decision_journal_tool.py#L283), `_mode_record`[`L255`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/decision_journal_tool.py#L255), `_mode_search`[`L319`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/decision_journal_tool.py#L319), `_mode_supersede`[`L358`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/decision_journal_tool.py#L358), `_on_project_root_changed`[`L85`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/decision_journal_tool.py#L85)
- uses (calls/refs, reference-scoped): [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`project_root`](base_tool.md#BaseMCPTool.project_root), [`apply_toon_format_to_response`](../utils/format_helper.md#apply_toon_format_to_response), [`record`](../../decision_journal.md#DecisionJournal.record), [`__init__`](base_tool.md#BaseMCPTool.__init__), [`mirror_summary_line`](base_tool.md#mirror_summary_line), [`DecisionJournal`](../../decision_journal.md#DecisionJournal), [`invalid_enum_error`](_validators.md#invalid_enum_error), [`JournalValidationError`](../../decision_journal.md#JournalValidationError), [`search`](../../decision_journal.md#DecisionJournal.search), [`_canonicalize_verdict`](base_tool.md#_canonicalize_verdict), [`id`](../../decision_journal.md#DecisionRecord.id), [`supersede`](../../decision_journal.md#DecisionJournal.supersede), [`get`](../../decision_journal.md#DecisionJournal.get), [`_record_to_envelope_dict`](decision_journal_tool.md#_record_to_envelope_dict), [`verdict`](../../decision_journal.md#DecisionRecord.verdict), [`_LEGAL_VERDICTS`](../../decision_journal.md#_LEGAL_VERDICTS._LEGAL_VERDICTS), [`_next_step_for_mode`](decision_journal_tool.md#_next_step_for_mode), [`_summary_line_for_mode`](decision_journal_tool.md#_summary_line_for_mode), [`_VALID_MODES`](decision_journal_tool.md#_VALID_MODES)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments), [`_on_project_root_changed`](base_tool.md#BaseMCPTool._on_project_root_changed), [`build_project_facade`](project_facade.md#build_project_facade)  (1 test-only)

## Functions
- `_next_step_for_mode(mode: str, verdict: str)` — [`L58`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/decision_journal_tool.py#L58) — Actionable hint embedded in agent_summary.next_step.
- `_record_to_envelope_dict(rec: DecisionRecord)` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/decision_journal_tool.py#L36) — Coerce a frozen record to the canonical envelope shape.
- `_summary_line_for_mode(mode: str, count: int | None, rec_id: str | None)` — [`L41`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/decision_journal_tool.py#L41) — Produce a single agent-readable headline.

## Module values
- `_VALID_MODES` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/decision_journal_tool.py#L33)

