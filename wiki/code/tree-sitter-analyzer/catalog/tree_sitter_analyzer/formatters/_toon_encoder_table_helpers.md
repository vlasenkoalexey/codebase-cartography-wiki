---
title: 'Module: tree_sitter_analyzer/formatters/_toon_encoder_table_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/formatters/_toon_encoder_table_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.formatters._toon_encoder_table_helpers`/
symbols:
  encode_array_table_lines: encode_array_table_lines().
  encode_public_array_table: encode_public_array_table().
  encode_table_rows: encode_table_rows().
  EncodeValue: EncodeValue.
  _encode_table_cell: _encode_table_cell().
  union_schema: union_schema().
  InferSchema: InferSchema.
  _sample_dict_subkeys: _sample_dict_subkeys().
  build_table_schema_parts: build_table_schema_parts().
---
# Module: [`tree_sitter_analyzer/formatters/_toon_encoder_table_helpers.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_toon_encoder_table_helpers.py)

## Functions
- `_encode_table_cell(value: Any, delimiter: str, encode_value: EncodeValue, seen_ids: set[int], expected_subkeys: tuple[str, ...] | None = None)` — [`L152`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_toon_encoder_table_helpers.py#L152) — Encode a single TOON table cell.
- `_sample_dict_subkeys(items: list[dict[str, Any]], schema: list[str])` — [`L82`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_toon_encoder_table_helpers.py#L82) — Per dict-valued column, the subkeys sampled for the header annotation.
- `build_table_schema_parts(items: list[dict[str, Any]], schema: list[str], delimiter: str)` — [`L102`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_toon_encoder_table_helpers.py#L102) — Build TOON table schema labels with compact nested value annotations.
- `encode_array_table_lines(items: list[dict[str, Any]], schema: list[str], delimiter: str, indent_str: str, encode_value: EncodeValue, seen_ids: set[int])` — [`L56`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_toon_encoder_table_helpers.py#L56) — Encode an array of dictionaries as TOON table lines.
- `encode_public_array_table(items: list[dict[str, Any]], schema: list[str] | None, indent: int, delimiter: str, encode_value: EncodeValue, infer_schema: InferSchema)` — [`L29`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_toon_encoder_table_helpers.py#L29) — Encode the public ``ToonEncoder.encode_array_table`` payload.
- `encode_table_rows(items: list[dict[str, Any]], schema: list[str], delimiter: str, indent_str: str, encode_value: EncodeValue, seen_ids: set[int], expected_subkeys: dict[str, tuple[str, ...]] | None = None)` — [`L125`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_toon_encoder_table_helpers.py#L125) — Encode table rows using an existing value encoder and circular-ref set.
- `union_schema(items: list[dict[str, Any]])` — [`L10`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_toon_encoder_table_helpers.py#L10) — Union of all rows' keys, in first-seen order (issue #637).

## Module values
- `EncodeValue` — [`L6`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_toon_encoder_table_helpers.py#L6)
- `InferSchema` — [`L7`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_toon_encoder_table_helpers.py#L7)

