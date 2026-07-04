---
title: 'Module: tree_sitter_analyzer/languages/sql_plugin/trigger_extractor.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/sql_plugin/trigger_extractor.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.sql_plugin.trigger_extractor`/
symbols:
  extract_sql_triggers: extract_sql_triggers().
  _append_sql_trigger_match: _append_sql_trigger_match().
  _append_legacy_trigger_match: _append_legacy_trigger_match().
  extract_legacy_triggers: extract_legacy_triggers().
  _append_legacy_triggers_from_error_node: _append_legacy_triggers_from_error_node().
  _SQLTriggerExtractionContext.trigger_factory: _SQLTriggerExtractionContext#trigger_factory.
  _LEGACY_RESERVED_TRIGGER_NAMES: _LEGACY_RESERVED_TRIGGER_NAMES.
  _is_valid_enhanced_trigger_name: _is_valid_enhanced_trigger_name().
  _is_valid_legacy_trigger_name: _is_valid_legacy_trigger_name().
  _SQLTriggerExtractionContext.processed_triggers: _SQLTriggerExtractionContext#processed_triggers.
  _ENHANCED_RESERVED_TRIGGER_NAMES: _ENHANCED_RESERVED_TRIGGER_NAMES.
  _SQLTriggerExtractionContext: _SQLTriggerExtractionContext#
  _SQLTriggerExtractionContext.source_code: _SQLTriggerExtractionContext#source_code.
  _SQLTriggerExtractionContext.sql_elements: _SQLTriggerExtractionContext#sql_elements.
  _SQLTriggerExtractionContext.is_valid_identifier_fn: _SQLTriggerExtractionContext#is_valid_identifier_fn.
  _trigger_text_span: _trigger_text_span().
  extract_trigger_metadata: extract_trigger_metadata().
---
# Module: [`tree_sitter_analyzer/languages/sql_plugin/trigger_extractor.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/trigger_extractor.py)

## Classes
### `_SQLTriggerExtractionContext`
- def: [`tree_sitter_analyzer/languages/sql_plugin/trigger_extractor.py:51`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/trigger_extractor.py#L51)
- signature: `class _SQLTriggerExtractionContext:`
- members:
  - `is_valid_identifier_fn` — [`L56`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/trigger_extractor.py#L56)
  - `processed_triggers` — [`L54`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/trigger_extractor.py#L54)
  - `source_code` — [`L52`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/trigger_extractor.py#L52)
  - `sql_elements` — [`L53`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/trigger_extractor.py#L53)
  - `trigger_factory` — [`L55`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/trigger_extractor.py#L55)
- uses (calls/refs, reference-scoped): [`SQLTrigger`](../../models/sql_models.md#SQLTrigger)
- used by: [`extract_sql_triggers`](trigger_extractor.md#extract_sql_triggers), [`_append_sql_trigger_match`](trigger_extractor.md#_append_sql_trigger_match)

## Functions
- `_append_legacy_trigger_match(node: tree_sitter.Node, node_text: str, match: re.Match[str], functions: list[Function], is_valid_identifier_fn: Callable[[str], bool])` — [`L231`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/trigger_extractor.py#L231) — Append one legacy trigger Function from a regex match when it is valid.
- `_append_legacy_triggers_from_error_node(node: tree_sitter.Node, functions: list[Function], get_node_text: Callable[..., str], is_valid_identifier_fn: Callable[[str], bool])` — [`L201`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/trigger_extractor.py#L201) — Append legacy Function trigger elements from one ERROR node.
- `_append_sql_trigger_match(match: re.Match[str], context: _SQLTriggerExtractionContext)` — [`L89`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/trigger_extractor.py#L89) — Append one enhanced SQL trigger from a regex match when it is valid.
- `_is_valid_enhanced_trigger_name(trigger_name: str, processed_triggers: set[str], is_valid_identifier_fn: Callable[[str], bool])` — [`L124`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/trigger_extractor.py#L124) — Return whether a regex trigger name should become an SQLTrigger.
- `_is_valid_legacy_trigger_name(trigger_name: str, is_valid_identifier_fn: Callable[[str], bool])` — [`L258`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/trigger_extractor.py#L258) — Return whether a legacy Function trigger name is usable.
- `_trigger_text_span(source_code: str, match: re.Match[str])` — [`L138`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/trigger_extractor.py#L138) — Return start line, end line, and raw trigger text for a match.
- `extract_legacy_triggers(root_node: tree_sitter.Node, functions: list[Function], traverse_nodes: Callable[..., Iterator[Any]], get_node_text: Callable[..., str], is_valid_identifier_fn: Callable[[str], bool])` — [`L182`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/trigger_extractor.py#L182) — Extract CREATE TRIGGER statements as generic Function elements.
- `extract_sql_triggers(source_code: str, sql_elements: list, *, trigger_factory: Callable[..., SQLTrigger] = SQLTrigger, is_valid_identifier_fn: Callable[[str], bool] = is_valid_identifier)` — [`L59`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/trigger_extractor.py#L59) — Extract CREATE TRIGGER statements with enhanced metadata.
- `extract_trigger_metadata(trigger_text: str)` — [`L157`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/trigger_extractor.py#L157) — Extract trigger timing, event, and target table.

## Module values
- `_ENHANCED_RESERVED_TRIGGER_NAMES` — [`L17`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/trigger_extractor.py#L17)
- `_LEGACY_RESERVED_TRIGGER_NAMES` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/trigger_extractor.py#L26)

