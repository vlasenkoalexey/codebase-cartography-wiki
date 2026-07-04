---
title: 'Module: tests/unit/test_decision_journal.py'
type: catalog
provenance: extracted
module: tests/unit/test_decision_journal.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_decision_journal`/Test
symbols:
  TestRecord.test_record_creates_row_and_returns_record: Record#test_record_creates_row_and_returns_record().
  TestGet.test_get_returns_recorded_row: Get#test_get_returns_recorded_row().
  TestSupersede.test_supersede_links_old_to_new: Supersede#test_supersede_links_old_to_new().
  TestSupersede.test_supersede_rejects_self_link: Supersede#test_supersede_rejects_self_link().
  TestPersistence.test_storage_persists_across_journal_instances: Persistence#test_storage_persists_across_journal_instances().
  TestSearch.test_search_returns_newest_first: Search#test_search_returns_newest_first().
  TestSearch.test_search_substring_matches_title_and_rationale: Search#test_search_substring_matches_title_and_rationale().
  TestSearch.test_search_filter_by_verdict: Search#test_search_filter_by_verdict().
  TestSupersede.test_supersede_unknown_old_returns_none: Supersede#test_supersede_unknown_old_returns_none().
  TestRecord.test_record_rejects_invalid_verdict: Record#test_record_rejects_invalid_verdict().
  TestRecord.test_record_rejects_empty_title: Record#test_record_rejects_empty_title().
  TestRecord.test_record_rejects_oversize_rationale: Record#test_record_rejects_oversize_rationale().
  TestRecord.test_record_rejects_path_traversal_in_scope_paths: Record#test_record_rejects_path_traversal_in_scope_paths().
  TestRecord.test_record_caps_alternatives_at_16: Record#test_record_caps_alternatives_at_16().
  TestRecord.test_record_accepts_well_formed_alternatives: Record#test_record_accepts_well_formed_alternatives().
  TestSearch.test_search_rejects_invalid_verdict_filter: Search#test_search_rejects_invalid_verdict_filter().
  TestSearch.test_search_respects_limit: Search#test_search_respects_limit().
  TestPersistence.test_to_dict_roundtrip: Persistence#test_to_dict_roundtrip().
  TestVocabularyContract.test_storage_vocab_matches_base_tool: VocabularyContract#test_storage_vocab_matches_base_tool().
  TestGet.test_get_unknown_id_returns_none: Get#test_get_unknown_id_returns_none().
  TestSearch.test_search_clamps_limit_to_max: Search#test_search_clamps_limit_to_max().
  TestPersistence.test_db_file_lives_under_ast_cache_dir: Persistence#test_db_file_lives_under_ast_cache_dir().
  TestVocabularyContract: VocabularyContract#
  TestRecord: Record#
  TestGet: Get#
  TestSearch: Search#
  TestSupersede: Supersede#
  TestPersistence: Persistence#
---
# Module: [`tests/unit/test_decision_journal.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_decision_journal.py)

## Classes
### `TestGet`
- def: [`tests/unit/test_decision_journal.py:115`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_decision_journal.py#L115)
- signature: `class TestGet:`
- members:
  - `test_get_returns_recorded_row(self, tmp_path: Path)` — [`L116`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_decision_journal.py#L116)
  - `test_get_unknown_id_returns_none(self, tmp_path: Path)` — [`L124`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_decision_journal.py#L124)
- uses (calls/refs, reference-scoped): [`record`](../../tree_sitter_analyzer/decision_journal.md#DecisionJournal.record), [`DecisionJournal`](../../tree_sitter_analyzer/decision_journal.md#DecisionJournal), [`id`](../../tree_sitter_analyzer/decision_journal.md#DecisionRecord.id), [`get`](../../tree_sitter_analyzer/decision_journal.md#DecisionJournal.get), [`tags`](../../tree_sitter_analyzer/decision_journal.md#DecisionRecord.tags)

### `TestPersistence`
- def: [`tests/unit/test_decision_journal.py:216`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_decision_journal.py#L216)
- signature: `class TestPersistence:`
- members:
  - `test_db_file_lives_under_ast_cache_dir(self, tmp_path: Path)` — [`L226`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_decision_journal.py#L226)
  - `test_storage_persists_across_journal_instances(self, tmp_path: Path)` — [`L217`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_decision_journal.py#L217)
  - `test_to_dict_roundtrip(self, tmp_path: Path)` — [`L231`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_decision_journal.py#L231)
- uses (calls/refs, reference-scoped): [`record`](../../tree_sitter_analyzer/decision_journal.md#DecisionJournal.record), [`DecisionJournal`](../../tree_sitter_analyzer/decision_journal.md#DecisionJournal), [`id`](../../tree_sitter_analyzer/decision_journal.md#DecisionRecord.id), [`get`](../../tree_sitter_analyzer/decision_journal.md#DecisionJournal.get), [`title`](../../tree_sitter_analyzer/decision_journal.md#DecisionRecord.title), [`db_path`](../../tree_sitter_analyzer/decision_journal.md#DecisionJournal.db_path), [`to_dict`](../../tree_sitter_analyzer/decision_journal.md#DecisionRecord.to_dict)

### `TestRecord`
- def: [`tests/unit/test_decision_journal.py:45`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_decision_journal.py#L45)
- signature: `class TestRecord:`
- members:
  - `test_record_accepts_well_formed_alternatives(self, tmp_path: Path)` — [`L95`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_decision_journal.py#L95)
  - `test_record_caps_alternatives_at_16(self, tmp_path: Path)` — [`L89`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_decision_journal.py#L89)
  - `test_record_creates_row_and_returns_record(self, tmp_path: Path)` — [`L46`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_decision_journal.py#L46)
  - `test_record_rejects_empty_title(self, tmp_path: Path)` — [`L62`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_decision_journal.py#L62)
  - `test_record_rejects_invalid_verdict(self, tmp_path: Path)` — [`L57`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_decision_journal.py#L57)
  - `test_record_rejects_oversize_rationale(self, tmp_path: Path)` — [`L67`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_decision_journal.py#L67)
  - `test_record_rejects_path_traversal_in_scope_paths(self, tmp_path: Path)` — [`L72`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_decision_journal.py#L72)
- uses (calls/refs, reference-scoped): [`record`](../../tree_sitter_analyzer/decision_journal.md#DecisionJournal.record), [`DecisionJournal`](../../tree_sitter_analyzer/decision_journal.md#DecisionJournal), [`JournalValidationError`](../../tree_sitter_analyzer/decision_journal.md#JournalValidationError), [`id`](../../tree_sitter_analyzer/decision_journal.md#DecisionRecord.id), [`DecisionRecord`](../../tree_sitter_analyzer/decision_journal.md#DecisionRecord), [`verdict`](../../tree_sitter_analyzer/decision_journal.md#DecisionRecord.verdict), [`title`](../../tree_sitter_analyzer/decision_journal.md#DecisionRecord.title), [`alternatives`](../../tree_sitter_analyzer/decision_journal.md#DecisionRecord.alternatives), [`superseded_by`](../../tree_sitter_analyzer/decision_journal.md#DecisionRecord.superseded_by)

### `TestSearch`
- def: [`tests/unit/test_decision_journal.py:134`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_decision_journal.py#L134)
- signature: `class TestSearch:`
- members:
  - `test_search_clamps_limit_to_max(self, tmp_path: Path)` — [`L178`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_decision_journal.py#L178)
  - `test_search_filter_by_verdict(self, tmp_path: Path)` — [`L158`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_decision_journal.py#L158)
  - `test_search_rejects_invalid_verdict_filter(self, tmp_path: Path)` — [`L167`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_decision_journal.py#L167)
  - `test_search_respects_limit(self, tmp_path: Path)` — [`L172`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_decision_journal.py#L172)
  - `test_search_returns_newest_first(self, tmp_path: Path)` — [`L135`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_decision_journal.py#L135)
  - `test_search_substring_matches_title_and_rationale(self, tmp_path: Path)` — [`L147`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_decision_journal.py#L147)
- uses (calls/refs, reference-scoped): [`record`](../../tree_sitter_analyzer/decision_journal.md#DecisionJournal.record), [`DecisionJournal`](../../tree_sitter_analyzer/decision_journal.md#DecisionJournal), [`JournalValidationError`](../../tree_sitter_analyzer/decision_journal.md#JournalValidationError), [`search`](../../tree_sitter_analyzer/decision_journal.md#DecisionJournal.search), [`id`](../../tree_sitter_analyzer/decision_journal.md#DecisionRecord.id), [`verdict`](../../tree_sitter_analyzer/decision_journal.md#DecisionRecord.verdict), [`title`](../../tree_sitter_analyzer/decision_journal.md#DecisionRecord.title)

### `TestSupersede`
- def: [`tests/unit/test_decision_journal.py:190`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_decision_journal.py#L190)
- signature: `class TestSupersede:`
- members:
  - `test_supersede_links_old_to_new(self, tmp_path: Path)` — [`L191`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_decision_journal.py#L191)
  - `test_supersede_rejects_self_link(self, tmp_path: Path)` — [`L204`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_decision_journal.py#L204)
  - `test_supersede_unknown_old_returns_none(self, tmp_path: Path)` — [`L199`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_decision_journal.py#L199)
- uses (calls/refs, reference-scoped): [`record`](../../tree_sitter_analyzer/decision_journal.md#DecisionJournal.record), [`DecisionJournal`](../../tree_sitter_analyzer/decision_journal.md#DecisionJournal), [`JournalValidationError`](../../tree_sitter_analyzer/decision_journal.md#JournalValidationError), [`id`](../../tree_sitter_analyzer/decision_journal.md#DecisionRecord.id), [`supersede`](../../tree_sitter_analyzer/decision_journal.md#DecisionJournal.supersede), [`superseded_by`](../../tree_sitter_analyzer/decision_journal.md#DecisionRecord.superseded_by)

### `TestVocabularyContract`
- def: [`tests/unit/test_decision_journal.py:27`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_decision_journal.py#L27)
- doc: Storage-side `_LEGAL_VERDICTS` must mirror the MCP envelope SOT.
- signature: `class TestVocabularyContract:`
- members:
  - `test_storage_vocab_matches_base_tool(self)` — [`L30`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_decision_journal.py#L30)
- uses (calls/refs, reference-scoped): [`_LEGAL_VERDICTS`](../../tree_sitter_analyzer/mcp/tools/base_tool.md#_LEGAL_VERDICTS._LEGAL_VERDICTS), [`_LEGAL_VERDICTS`](../../tree_sitter_analyzer/decision_journal.md#_LEGAL_VERDICTS._LEGAL_VERDICTS)

