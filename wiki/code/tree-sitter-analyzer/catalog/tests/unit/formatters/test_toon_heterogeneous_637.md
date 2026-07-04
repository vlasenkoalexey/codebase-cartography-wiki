---
title: 'Module: tests/unit/formatters/test_toon_heterogeneous_637.py'
type: catalog
provenance: extracted
module: tests/unit/formatters/test_toon_heterogeneous_637.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.formatters.test_toon_heterogeneous_637`/TestH
symbols:
  TestHeterogeneousArrayLosslessness.test_issue_637_minimal_repro_body_survives: eterogeneousArrayLosslessness#test_issue_637_minimal_repro_body_survives().
  TestHeterogeneousArrayLosslessness.test_union_schema_first_seen_order: eterogeneousArrayLosslessness#test_union_schema_first_seen_order().
  TestHeterogeneousArrayLosslessness.test_empty_dict_first_row_no_longer_erases_table: eterogeneousArrayLosslessness#test_empty_dict_first_row_no_longer_erases_table().
  TestHeterogeneousArrayLosslessness.test_nested_heterogeneous_array: eterogeneousArrayLosslessness#test_nested_heterogeneous_array().
  TestHeterogeneousArrayLosslessness.test_dict_column_annotation_from_first_row_having_key: eterogeneousArrayLosslessness#test_dict_column_annotation_from_first_row_having_key().
  TestHeterogeneousArrayLosslessness.test_issue_643_divergent_nested_subkeys_encode_inline: eterogeneousArrayLosslessness#test_issue_643_divergent_nested_subkeys_encode_inline().
  TestHeterogeneousArrayLosslessness.test_issue_643_matching_nested_subkeys_stay_compact: eterogeneousArrayLosslessness#test_issue_643_matching_nested_subkeys_stay_compact().
  TestHeterogeneousArrayLosslessness.test_mixed_dict_and_scalar_list_encodes_inline_not_crash: eterogeneousArrayLosslessness#test_mixed_dict_and_scalar_list_encodes_inline_not_crash().
  TestHeterogeneousArrayLosslessness.test_infer_schema_is_union: eterogeneousArrayLosslessness#test_infer_schema_is_union().
  TestHeterogeneousArrayLosslessness.test_public_encode_array_table_heterogeneous: eterogeneousArrayLosslessness#test_public_encode_array_table_heterogeneous().
  TestHomogeneousArraysUnchanged.test_homogeneous_table_byte_identical_pin: omogeneousArraysUnchanged#test_homogeneous_table_byte_identical_pin().
  TestHomogeneousArraysUnchanged.test_homogeneous_formatter_entry_byte_identical_pin: omogeneousArraysUnchanged#test_homogeneous_formatter_entry_byte_identical_pin().
  TestHomogeneousArraysUnchanged.test_top_level_heterogeneous_list_stays_inline: omogeneousArraysUnchanged#test_top_level_heterogeneous_list_stays_inline().
  TestHeterogeneousArrayLosslessness: eterogeneousArrayLosslessness#
  TestHomogeneousArraysUnchanged: omogeneousArraysUnchanged#
---
# Module: [`tests/unit/formatters/test_toon_heterogeneous_637.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_heterogeneous_637.py)

## Classes
### `TestHeterogeneousArrayLosslessness`
- def: [`tests/unit/formatters/test_toon_heterogeneous_637.py:24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_heterogeneous_637.py#L24)
- doc: Fields present in ANY row must appear in the TOON output.
- signature: `class TestHeterogeneousArrayLosslessness:`
- members:
  - `test_dict_column_annotation_from_first_row_having_key(self)` — [`L51`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_heterogeneous_637.py#L51) — Schema annotation (``key{subkeys}``) must come from the first row
  - `test_empty_dict_first_row_no_longer_erases_table(self)` — [`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_heterogeneous_637.py#L39) — Pre-fix: schema from ``{}`` was empty → EVERY field of every row
  - `test_infer_schema_is_union(self)` — [`L83`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_heterogeneous_637.py#L83)
  - `test_issue_637_minimal_repro_body_survives(self)` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_heterogeneous_637.py#L27) — The lead-verified repro: second row's ``body`` must survive.
  - `test_issue_643_divergent_nested_subkeys_encode_inline(self)` — [`L59`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_heterogeneous_637.py#L59) — #643: a dict cell whose subkeys DIVERGE from the header sample must
  - `test_issue_643_matching_nested_subkeys_stay_compact(self)` — [`L69`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_heterogeneous_637.py#L69) — Regression: cells whose subkeys MATCH the header sample keep the
  - `test_mixed_dict_and_scalar_list_encodes_inline_not_crash(self)` — [`L77`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_heterogeneous_637.py#L77) — A list whose first item is a dict but later items are scalars must
  - `test_nested_heterogeneous_array(self)` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_heterogeneous_637.py#L45) — Heterogeneous arrays inside nested dicts go through the same
  - `test_public_encode_array_table_heterogeneous(self)` — [`L87`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_heterogeneous_637.py#L87) — Public convenience API infers the union schema too.
  - `test_union_schema_first_seen_order(self)` — [`L34`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_heterogeneous_637.py#L34) — Union keeps first-seen key order across rows.
- uses (calls/refs, reference-scoped): [`ToonEncoder`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncoder), [`encode`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncoder.encode), [`ToonFormatter`](../../../tree_sitter_analyzer/formatters/toon_formatter.md#ToonFormatter), [`format`](../../../tree_sitter_analyzer/formatters/toon_formatter.md#ToonFormatter.format), [`encode_array_table`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncoder.encode_array_table), [`_infer_schema`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncoder._infer_schema)

### `TestHomogeneousArraysUnchanged`
- def: [`tests/unit/formatters/test_toon_heterogeneous_637.py:93`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_heterogeneous_637.py#L93)
- doc: The token-efficiency story: homogeneous tables are byte-identical.
- signature: `class TestHomogeneousArraysUnchanged:`
- members:
  - `test_homogeneous_formatter_entry_byte_identical_pin(self)` — [`L102`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_heterogeneous_637.py#L102)
  - `test_homogeneous_table_byte_identical_pin(self)` — [`L96`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_heterogeneous_637.py#L96) — Byte-pin captured on develop dbda9a3e BEFORE the #637 fix —
  - `test_top_level_heterogeneous_list_stays_inline(self)` — [`L108`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_heterogeneous_637.py#L108) — ``_handle_list_start``'s mixed-key inline form (already lossless)
- uses (calls/refs, reference-scoped): [`ToonEncoder`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncoder), [`encode`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncoder.encode), [`ToonFormatter`](../../../tree_sitter_analyzer/formatters/toon_formatter.md#ToonFormatter), [`format`](../../../tree_sitter_analyzer/formatters/toon_formatter.md#ToonFormatter.format)

