---
title: 'Module: tree_sitter_analyzer/decision_journal.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/decision_journal.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.decision_journal`/
symbols:
  DecisionJournal.record: DecisionJournal#record().
  DecisionJournal: DecisionJournal#
  _row_to_record: _row_to_record().
  JournalValidationError: JournalValidationError#
  DecisionJournal.search: DecisionJournal#search().
  DecisionRecord.id: DecisionRecord#id.
  DecisionJournal.supersede: DecisionJournal#supersede().
  DecisionJournal.get: DecisionJournal#get().
  DecisionRecord: DecisionRecord#
  _require_str: _require_str().
  DecisionRecord.verdict: DecisionRecord#verdict.
  _validate_alternatives: _validate_alternatives().
  DecisionJournal._connect: DecisionJournal#_connect().
  _require_verdict: _require_verdict().
  _validate_string_list: _validate_string_list().
  DecisionJournal._db_path: DecisionJournal#_db_path.
  _LEGAL_VERDICTS._LEGAL_VERDICTS: _LEGAL_VERDICTS._LEGAL_VERDICTS.
  DecisionJournal._project_root: DecisionJournal#_project_root.
  DecisionJournal._init_schema: DecisionJournal#_init_schema().
  DecisionRecord.title: DecisionRecord#title.
  DecisionJournal.db_path: DecisionJournal#db_path().
  DecisionRecord.alternatives: DecisionRecord#alternatives.
  DecisionRecord.superseded_by: DecisionRecord#superseded_by.
  _validate_path_list: _validate_path_list().
  DecisionRecord.tags: DecisionRecord#tags.
  DecisionRecord.to_dict: DecisionRecord#to_dict().
  _MAX_TEXT_CHARS: _MAX_TEXT_CHARS.
  _MAX_ALTERNATIVES: _MAX_ALTERNATIVES.
  _MAX_SEARCH_LIMIT: _MAX_SEARCH_LIMIT.
  DecisionRecord.created_at: DecisionRecord#created_at.
  DecisionRecord.rationale: DecisionRecord#rationale.
  DecisionRecord.scope_paths: DecisionRecord#scope_paths.
  DecisionRecord.related_symbols: DecisionRecord#related_symbols.
  _DB_FILENAME: _DB_FILENAME.
  _CACHE_DIR: _CACHE_DIR.
  _MAX_TAGS: _MAX_TAGS.
  _MAX_RELATED_SYMBOLS: _MAX_RELATED_SYMBOLS.
  _MAX_SCOPE_PATHS: _MAX_SCOPE_PATHS.
  _DEFAULT_SEARCH_LIMIT: _DEFAULT_SEARCH_LIMIT.
  _SCHEMA: _SCHEMA.
  _utc_now_iso: _utc_now_iso().
  _new_id: _new_id().
  DecisionJournal.__init__: DecisionJournal#__init__().
---
# Module: [`tree_sitter_analyzer/decision_journal.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/decision_journal.py)

## Classes
### `DecisionJournal`
- def: [`tree_sitter_analyzer/decision_journal.py:227`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/decision_journal.py#L227)
- doc: SQLite-backed decision journal.
- signature: `class DecisionJournal:`
- members:
  - `db_path(self)` — [`L238`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/decision_journal.py#L238)
  - `get(self, decision_id: str)` — [`L307`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/decision_journal.py#L307)
  - `record(self, *, title: str, rationale: str, verdict: str, scope_paths: list[str] | None = None, alternatives: list[dict[str, str]] | None = None, related_symbols: list[str] | None = None, tags: list[str] | None = None)` — [`L254`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/decision_journal.py#L254) — Insert a new decision and return its record.
  - `search(self, *, query: str | None = None, verdict_filter: str | None = None, path_scope: str | None = None, limit: int = _DEFAULT_SEARCH_LIMIT)` — [`L314`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/decision_journal.py#L314)
  - `supersede(self, old_id: str, new_id: str)` — [`L345`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/decision_journal.py#L345) — Mark ``old_id`` as superseded by ``new_id``. Returns updated row.
- protocol/private: `__init__`[`L230`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/decision_journal.py#L230), `_connect`[`L241`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/decision_journal.py#L241), `_db_path`[`L234`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/decision_journal.py#L234), `_init_schema`[`L246`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/decision_journal.py#L246), `_project_root`[`L231`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/decision_journal.py#L231)
- uses (calls/refs, reference-scoped): [`_row_to_record`](decision_journal.md#_row_to_record), [`JournalValidationError`](decision_journal.md#JournalValidationError), [`id`](decision_journal.md#DecisionRecord.id), [`DecisionRecord`](decision_journal.md#DecisionRecord), [`_require_str`](decision_journal.md#_require_str), [`verdict`](decision_journal.md#DecisionRecord.verdict), [`_validate_alternatives`](decision_journal.md#_validate_alternatives), [`_require_verdict`](decision_journal.md#_require_verdict), [`_validate_string_list`](decision_journal.md#_validate_string_list), [`title`](decision_journal.md#DecisionRecord.title), [`alternatives`](decision_journal.md#DecisionRecord.alternatives), [`superseded_by`](decision_journal.md#DecisionRecord.superseded_by), [`_validate_path_list`](decision_journal.md#_validate_path_list), [`tags`](decision_journal.md#DecisionRecord.tags), [`_MAX_SEARCH_LIMIT`](decision_journal.md#_MAX_SEARCH_LIMIT), [`created_at`](decision_journal.md#DecisionRecord.created_at), [`rationale`](decision_journal.md#DecisionRecord.rationale), [`related_symbols`](decision_journal.md#DecisionRecord.related_symbols), [`scope_paths`](decision_journal.md#DecisionRecord.scope_paths), [`_CACHE_DIR`](decision_journal.md#_CACHE_DIR), [`_DB_FILENAME`](decision_journal.md#_DB_FILENAME), [`_DEFAULT_SEARCH_LIMIT`](decision_journal.md#_DEFAULT_SEARCH_LIMIT), [`_MAX_RELATED_SYMBOLS`](decision_journal.md#_MAX_RELATED_SYMBOLS), [`_MAX_SCOPE_PATHS`](decision_journal.md#_MAX_SCOPE_PATHS), [`_MAX_TAGS`](decision_journal.md#_MAX_TAGS), [`_SCHEMA`](decision_journal.md#_SCHEMA), [`_new_id`](decision_journal.md#_new_id), [`_utc_now_iso`](decision_journal.md#_utc_now_iso)
- used by: [`_mode_get`](mcp/tools/decision_journal_tool.md#DecisionJournalTool._mode_get), [`_mode_record`](mcp/tools/decision_journal_tool.md#DecisionJournalTool._mode_record), [`_mode_supersede`](mcp/tools/decision_journal_tool.md#DecisionJournalTool._mode_supersede), [`_mode_search`](mcp/tools/decision_journal_tool.md#DecisionJournalTool._mode_search), [`_dispatch_mode`](mcp/tools/decision_journal_tool.md#DecisionJournalTool._dispatch_mode), [`_enrich_with_journal_decisions`](mcp/tools/change_impact_tool.md#_enrich_with_journal_decisions), [`_get_journal`](mcp/tools/decision_journal_tool.md#DecisionJournalTool._get_journal), [`__init__`](mcp/tools/decision_journal_tool.md#DecisionJournalTool.__init__)  (21 test-only)

### `DecisionRecord`
- def: [`tree_sitter_analyzer/decision_journal.py:88`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/decision_journal.py#L88)
- doc: Immutable in-memory view of a journal row.
- signature: `class DecisionRecord:`
- members:
  - `to_dict(self)` — [`L102`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/decision_journal.py#L102) — Return a plain dict suitable for JSON / TOON envelopes.
  - `alternatives` — [`L97`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/decision_journal.py#L97)
  - `created_at` — [`L92`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/decision_journal.py#L92)
  - `id` — [`L91`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/decision_journal.py#L91)
  - `rationale` — [`L94`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/decision_journal.py#L94)
  - `related_symbols` — [`L98`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/decision_journal.py#L98)
  - `scope_paths` — [`L96`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/decision_journal.py#L96)
  - `superseded_by` — [`L100`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/decision_journal.py#L100)
  - `tags` — [`L99`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/decision_journal.py#L99)
  - `title` — [`L93`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/decision_journal.py#L93)
  - `verdict` — [`L95`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/decision_journal.py#L95)
- used by: [`record`](decision_journal.md#DecisionJournal.record), [`_row_to_record`](decision_journal.md#_row_to_record), [`search`](decision_journal.md#DecisionJournal.search), [`_mode_get`](mcp/tools/decision_journal_tool.md#DecisionJournalTool._mode_get), [`_mode_record`](mcp/tools/decision_journal_tool.md#DecisionJournalTool._mode_record), [`_mode_supersede`](mcp/tools/decision_journal_tool.md#DecisionJournalTool._mode_supersede), [`_mode_search`](mcp/tools/decision_journal_tool.md#DecisionJournalTool._mode_search), [`supersede`](decision_journal.md#DecisionJournal.supersede), [`_enrich_with_journal_decisions`](mcp/tools/change_impact_tool.md#_enrich_with_journal_decisions), [`get`](decision_journal.md#DecisionJournal.get), [`_record_to_envelope_dict`](mcp/tools/decision_journal_tool.md#_record_to_envelope_dict)  (11 test-only)

### `JournalValidationError`  ·  implements/extends ValueError
- def: [`tree_sitter_analyzer/decision_journal.py:121`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/decision_journal.py#L121)
- doc: Raised by `record` / `supersede` for boundary violations.
- signature: `class JournalValidationError(ValueError):`
- used by: [`search`](decision_journal.md#DecisionJournal.search), [`execute`](mcp/tools/decision_journal_tool.md#DecisionJournalTool.execute), [`supersede`](decision_journal.md#DecisionJournal.supersede), [`_require_str`](decision_journal.md#_require_str), [`_validate_alternatives`](decision_journal.md#_validate_alternatives), [`_require_verdict`](decision_journal.md#_require_verdict), [`_validate_string_list`](decision_journal.md#_validate_string_list), [`_validate_path_list`](decision_journal.md#_validate_path_list)  (7 test-only)

## Functions
- `_new_id()` — [`L223`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/decision_journal.py#L223)
- `_require_str(value: Any, field_name: str, *, allow_empty: bool = False)` — [`L125`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/decision_journal.py#L125)
- `_require_verdict(value: Any)` — [`L137`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/decision_journal.py#L137)
- `_row_to_record(row: sqlite3.Row)` — [`L369`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/decision_journal.py#L369)
- `_utc_now_iso()` — [`L218`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/decision_journal.py#L218) — ISO-8601 UTC timestamp with seconds precision (test-friendly).
- `_validate_alternatives(items: Any)` — [`L170`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/decision_journal.py#L170)
- `_validate_path_list(paths: Any, field_name: str, max_items: int)` — [`L145`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/decision_journal.py#L145)
- `_validate_string_list(items: Any, field_name: str, max_items: int)` — [`L196`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/decision_journal.py#L196)

## Module values
- `_CACHE_DIR` — [`L46`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/decision_journal.py#L46)
- `_DB_FILENAME` — [`L45`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/decision_journal.py#L45)
- `_DEFAULT_SEARCH_LIMIT` — [`L53`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/decision_journal.py#L53)
- `_LEGAL_VERDICTS` — [`L60`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/decision_journal.py#L60)
- `_MAX_ALTERNATIVES` — [`L49`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/decision_journal.py#L49)
- `_MAX_RELATED_SYMBOLS` — [`L51`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/decision_journal.py#L51)
- `_MAX_SCOPE_PATHS` — [`L52`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/decision_journal.py#L52)
- `_MAX_SEARCH_LIMIT` — [`L54`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/decision_journal.py#L54)
- `_MAX_TAGS` — [`L50`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/decision_journal.py#L50)
- `_MAX_TEXT_CHARS` — [`L48`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/decision_journal.py#L48)
- `_SCHEMA` — [`L64`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/decision_journal.py#L64)

