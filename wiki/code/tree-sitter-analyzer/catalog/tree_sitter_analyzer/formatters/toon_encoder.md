---
title: 'Module: tree_sitter_analyzer/formatters/toon_encoder.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/formatters/toon_encoder.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.formatters.toon_encoder`/
symbols:
  ToonEncoder: ToonEncoder#
  ToonEncoder.encode: ToonEncoder#encode().
  ToonEncoder.encode_value: ToonEncoder#encode_value().
  _Task: _Task#
  ToonEncodeError: ToonEncodeError#
  ToonEncoder.encode_safe: ToonEncoder#encode_safe().
  ToonEncoder._handle_dict_key: ToonEncoder#_handle_dict_key().
  ToonEncoder._encode_iterative: ToonEncoder#_encode_iterative().
  _TaskType: _TaskType#
  ToonEncoder.encode_array_table: ToonEncoder#encode_array_table().
  ToonEncoder._handle_list_item: ToonEncoder#_handle_list_item().
  ToonEncoder._handle_array_table: ToonEncoder#_handle_array_table().
  ToonEncoder._encode_simple_list: ToonEncoder#_encode_simple_list().
  ToonEncoder._encode_inline_dict: ToonEncoder#_encode_inline_dict().
  ToonEncoder._handle_dict_start: ToonEncoder#_handle_dict_start().
  ToonEncoder._handle_list_start: ToonEncoder#_handle_list_start().
  _Task.indent: _Task#indent.
  ToonEncoder._encode_string: ToonEncoder#_encode_string().
  ToonEncoder.encode_dict: ToonEncoder#encode_dict().
  ToonEncoder.delimiter: ToonEncoder#delimiter.
  ToonEncoder._fallback_to_json: ToonEncoder#_fallback_to_json().
  ToonEncodeError.cause: ToonEncodeError#cause.
  ToonEncoder._infer_schema: ToonEncoder#_infer_schema().
  ToonEncodeError.message: ToonEncodeError#message.
  ToonEncoder.encode_array_header: ToonEncoder#encode_array_header().
  ToonEncoder.fallback_to_json: ToonEncoder#fallback_to_json.
  logger: logger.
  _Task.task_type: _Task#task_type.
  ToonEncoder.encode_list: ToonEncoder#encode_list().
  ToonEncodeError.data: ToonEncodeError#data.
  ToonEncodeError.__str__: ToonEncodeError#__str__().
  _TaskType.ENCODE_LIST_START: _TaskType#ENCODE_LIST_START.
  _Task.data: _Task#data.
  ToonEncoder.detect_circular_reference: ToonEncoder#detect_circular_reference().
  ToonEncoder.max_depth: ToonEncoder#max_depth.
  _TaskType.ENCODE_DICT_START: _TaskType#ENCODE_DICT_START.
  _TaskType.ENCODE_ARRAY_TABLE: _TaskType#ENCODE_ARRAY_TABLE.
  _pick_list_str_column_name: _pick_list_str_column_name().
  ToonEncoder.use_tabs: ToonEncoder#use_tabs.
  ToonEncoder.normalize_paths: ToonEncoder#normalize_paths.
  _TaskType.ENCODE_LIST_ITEM: _TaskType#ENCODE_LIST_ITEM.
  ToonEncoder.handle_dict_start: ToonEncoder#handle_dict_start.
  ToonEncoder.handle_dict_key: ToonEncoder#handle_dict_key.
  ToonEncoder.handle_list_start: ToonEncoder#handle_list_start.
  ToonEncoder.handle_list_item: ToonEncoder#handle_list_item.
  ToonEncoder.handle_array_table: ToonEncoder#handle_array_table.
  _Task.key: _Task#key.
  ToonEncoder.encode_to_json: ToonEncoder#encode_to_json.
  _TaskType.ENCODE_DICT_KEY: _TaskType#ENCODE_DICT_KEY.
  _TaskType.ENCODE_DICT_END: _TaskType#ENCODE_DICT_END.
  _FLAT_STR_LIST_THRESHOLD: _FLAT_STR_LIST_THRESHOLD.
  _LIST_STR_COLUMN_NAMES: _LIST_STR_COLUMN_NAMES.
  ToonEncoder._normalize_path_string: ToonEncoder#_normalize_path_string().
  ToonEncodeError.__init__: ToonEncodeError#__init__().
  _TaskType.ENCODE_VALUE: _TaskType#ENCODE_VALUE.
  _TaskType.ENCODE_LIST_END: _TaskType#ENCODE_LIST_END.
  _Task.output_index: _Task#output_index.
  _Task.is_inline: _Task#is_inline.
  ToonEncoder.MAX_DEPTH: ToonEncoder#MAX_DEPTH.
  ToonEncoder.__init__: ToonEncoder#__init__().
---
# Module: [`tree_sitter_analyzer/formatters/toon_encoder.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_encoder.py)

## Classes
### `ToonEncodeError`  ·  implements/extends Exception
- def: [`tree_sitter_analyzer/formatters/toon_encoder.py:28`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_encoder.py#L28)
- doc: Exception raised when TOON encoding fails.
- signature: `class ToonEncodeError(Exception):`
- members:
  - `__init__(self, message: str, data: Any = None, cause: Exception | None = None)` — [`L38`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_encoder.py#L38) — Initialize ToonEncodeError.
  - `__str__(self)` — [`L52`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_encoder.py#L52) — Return string representation of the error.
  - `cause` — [`L50`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_encoder.py#L50)
  - `data` — [`L49`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_encoder.py#L49)
  - `message` — [`L48`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_encoder.py#L48)
- used by: [`encode`](toon_encoder.md#ToonEncoder.encode), [`format`](toon_formatter.md#ToonFormatter.format), [`encode_safe`](toon_encoder.md#ToonEncoder.encode_safe), [`_encode_iterative`](toon_encoder.md#ToonEncoder._encode_iterative)  (18 test-only)

### `ToonEncoder`
- def: [`tree_sitter_analyzer/formatters/toon_encoder.py:128`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_encoder.py#L128) — documented in [tree_sitter_analyzer-formatters-toon_encoder](../../../concepts/tree_sitter_analyzer-formatters-toon_encoder.md)
- doc: Low-level encoder for TOON format.
- signature: `class ToonEncoder:`
- members:
  - `__init__(self, use_tabs: bool = False, fallback_to_json: bool = True, max_depth: int = 100, normalize_paths: bool = True)` — [`L144`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_encoder.py#L144) — Initialize TOON encoder.
  - `_encode_inline_dict(self, data: dict[str, Any], seen_ids: set[int])` — [`L467`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_encoder.py#L467) — Encode a dict inline (for dicts inside simple lists). — documented in [tree_sitter_analyzer-formatters-toon_encoder](../../../concepts/tree_sitter_analyzer-formatters-toon_encoder.md)
  - `_encode_iterative(self, data: Any, initial_indent: int = 0)` — [`L200`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_encoder.py#L200) — Iterative encoding using explicit stack. — documented in [tree_sitter_analyzer-formatters-toon_encoder](../../../concepts/tree_sitter_analyzer-formatters-toon_encoder.md)
  - `_encode_simple_list(self, items: list[Any], seen_ids: set[int])` — [`L429`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_encoder.py#L429) — Encode a simple list (non-homogeneous dicts) inline. — documented in [tree_sitter_analyzer-formatters-toon_encoder](../../../concepts/tree_sitter_analyzer-formatters-toon_encoder.md)
  - `_encode_string(self, s: str)` — [`L549`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_encoder.py#L549) — Encode string with proper escaping. — documented in [tree_sitter_analyzer-formatters-toon_encoder](../../../concepts/tree_sitter_analyzer-formatters-toon_encoder.md)
  - `_fallback_to_json(self, data: Any)` — [`L504`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_encoder.py#L504) — Fall back to JSON encoding when TOON encoding fails. — documented in [tree_sitter_analyzer-formatters-toon_encoder](../../../concepts/tree_sitter_analyzer-formatters-toon_encoder.md)
  - `_handle_array_table(self, task: _Task, output: list[str], seen_ids: set[int])` — [`L388`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_encoder.py#L388) — Handle encoding of homogeneous array as table. — documented in [tree_sitter_analyzer-formatters-toon_encoder](../../../concepts/tree_sitter_analyzer-formatters-toon_encoder.md)
  - `_handle_dict_key(self, task: _Task, stack: list[_Task], output: list[str], seen_ids: set[int])` — [`L276`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_encoder.py#L276) — Handle encoding of a dict key-value pair. — documented in [tree_sitter_analyzer-formatters-toon_encoder](../../../concepts/tree_sitter_analyzer-formatters-toon_encoder.md)
  - `_handle_dict_start(self, task: _Task, stack: list[_Task], output: list[str], seen_ids: set[int])` — [`L240`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_encoder.py#L240) — Handle start of dict encoding. — documented in [tree_sitter_analyzer-formatters-toon_encoder](../../../concepts/tree_sitter_analyzer-formatters-toon_encoder.md)
  - `_handle_list_item(self, task: _Task, stack: list[_Task], output: list[str], seen_ids: set[int])` — [`L368`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_encoder.py#L368) — Handle encoding of a list item. — documented in [tree_sitter_analyzer-formatters-toon_encoder](../../../concepts/tree_sitter_analyzer-formatters-toon_encoder.md)
  - `_handle_list_start(self, task: _Task, stack: list[_Task], output: list[str], seen_ids: set[int])` — [`L329`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_encoder.py#L329) — Handle start of list encoding.
  - `_infer_schema(self, items: list[dict[str, Any]])` — [`L697`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_encoder.py#L697) — Infer common schema from array items.
  - `_normalize_path_string(self, s: str)` — [`L572`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_encoder.py#L572) — Normalize Windows-style paths to forward slashes.
  - `detect_circular_reference(data: Any, seen: set[int] | None = None)` — [`L740`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_encoder.py#L740) — Check if data contains circular references using iterative approach.
  - `encode(self, data: Any, indent: int = 0)` — [`L167`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_encoder.py#L167) — Encode arbitrary data as TOON format using iterative approach. — documented in [tree_sitter_analyzer-formatters-toon_encoder](../../../concepts/tree_sitter_analyzer-formatters-toon_encoder.md)
  - `encode_array_header(self, count: int, schema: list[str] | None = None)` — [`L645`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_encoder.py#L645) — Generate array header with optional schema.
  - `encode_array_table(self, items: list[dict[str, Any]], schema: list[str] | None = None, indent: int = 0)` — [`L665`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_encoder.py#L665) — Encode homogeneous array as compact table. — documented in [tree_sitter_analyzer-formatters-toon_encoder](../../../concepts/tree_sitter_analyzer-formatters-toon_encoder.md)
  - `encode_dict(self, data: dict[str, Any], indent: int = 0)` — [`L615`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_encoder.py#L615) — Encode dictionary as TOON object.
  - `encode_list(self, items: list[Any], indent: int = 0)` — [`L630`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_encoder.py#L630) — Encode list as TOON array.
  - `encode_safe(self, data: Any, indent: int = 0)` — [`L712`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_encoder.py#L712) — Safely encode data, always returning a string. — documented in [tree_sitter_analyzer-formatters-toon_encoder](../../../concepts/tree_sitter_analyzer-formatters-toon_encoder.md)
  - `encode_value(self, value: Any, seen_ids: set[int] | None = None)` — [`L520`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_encoder.py#L520) — Encode single value for TOON output. — documented in [tree_sitter_analyzer-formatters-toon_encoder](../../../concepts/tree_sitter_analyzer-formatters-toon_encoder.md)
  - `MAX_DEPTH` — [`L142`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_encoder.py#L142)
  - `delimiter` — [`L162`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_encoder.py#L162) — documented in [tree_sitter_analyzer-formatters-toon_encoder](../../../concepts/tree_sitter_analyzer-formatters-toon_encoder.md)
  - `encode_to_json` — [`L781`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_encoder.py#L781)
  - `fallback_to_json` — [`L163`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_encoder.py#L163) — documented in [tree_sitter_analyzer-formatters-toon_encoder](../../../concepts/tree_sitter_analyzer-formatters-toon_encoder.md)
  - `handle_array_table` — [`L778`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_encoder.py#L778)
  - `handle_dict_key` — [`L775`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_encoder.py#L775)
  - `handle_dict_start` — [`L774`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_encoder.py#L774)
  - `handle_list_item` — [`L777`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_encoder.py#L777)
  - `handle_list_start` — [`L776`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_encoder.py#L776)
  - `max_depth` — [`L164`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_encoder.py#L164)
  - `normalize_paths` — [`L165`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_encoder.py#L165)
  - `use_tabs` — [`L161`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_encoder.py#L161)
- uses (calls/refs, reference-scoped): [`_Task`](toon_encoder.md#_Task), [`ToonEncodeError`](toon_encoder.md#ToonEncodeError), [`_TaskType`](toon_encoder.md#_TaskType), [`indent`](toon_encoder.md#_Task.indent), [`encode_array_table_lines`](_toon_encoder_table_helpers.md#encode_array_table_lines), [`encode_public_array_table`](_toon_encoder_table_helpers.md#encode_public_array_table), [`message`](toon_encoder.md#ToonEncodeError.message), [`needs_quotes`](_toon_encoder_string_helpers.md#needs_quotes), [`logger`](toon_encoder.md#logger), [`task_type`](toon_encoder.md#_Task.task_type), [`ENCODE_LIST_START`](toon_encoder.md#_TaskType.ENCODE_LIST_START), [`data`](toon_encoder.md#_Task.data), [`ENCODE_ARRAY_TABLE`](toon_encoder.md#_TaskType.ENCODE_ARRAY_TABLE), [`ENCODE_DICT_START`](toon_encoder.md#_TaskType.ENCODE_DICT_START), [`_pick_list_str_column_name`](toon_encoder.md#_pick_list_str_column_name), [`union_schema`](_toon_encoder_table_helpers.md#union_schema), [`build_task_handlers`](_toon_encoder_task_helpers.md#build_task_handlers), [`escape_string`](_toon_encoder_string_helpers.md#escape_string), [`key`](toon_encoder.md#_Task.key), [`ENCODE_DICT_END`](toon_encoder.md#_TaskType.ENCODE_DICT_END), [`ENCODE_DICT_KEY`](toon_encoder.md#_TaskType.ENCODE_DICT_KEY), [`_FLAT_STR_LIST_THRESHOLD`](toon_encoder.md#_FLAT_STR_LIST_THRESHOLD)
- used by: [`format_analysis_result`](toon_formatter.md#ToonFormatter.format_analysis_result), [`format`](toon_formatter.md#ToonFormatter.format), [`_format_internal`](toon_formatter.md#ToonFormatter._format_internal), [`encoder`](toon_formatter.md#ToonFormatter.encoder), [`_emit_method_lines`](toon_formatter.md#ToonFormatter._emit_method_lines), [`format_structure`](toon_formatter.md#ToonFormatter.format_structure), [`format_advanced`](toon_formatter.md#ToonFormatter.format_advanced), [`format_summary`](toon_formatter.md#ToonFormatter.format_summary), [`format_table`](toon_formatter.md#ToonFormatter.format_table), [`format_mcp_response`](toon_formatter.md#ToonFormatter.format_mcp_response)  (184 test-only)

### `_Task`
- def: [`tree_sitter_analyzer/formatters/toon_encoder.py:74`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_encoder.py#L74) — documented in [tree_sitter_analyzer-formatters-toon_encoder](../../../concepts/tree_sitter_analyzer-formatters-toon_encoder.md)
- doc: A single encoding task for the iterative encoder.
- signature: `class _Task:`
- members:
  - `data` — [`L78`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_encoder.py#L78)
  - `indent` — [`L79`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_encoder.py#L79)
  - `is_inline` — [`L82`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_encoder.py#L82)
  - `key` — [`L80`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_encoder.py#L80)
  - `output_index` — [`L81`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_encoder.py#L81)
  - `task_type` — [`L77`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_encoder.py#L77)
- uses (calls/refs, reference-scoped): [`_TaskType`](toon_encoder.md#_TaskType)
- used by: [`_handle_dict_key`](toon_encoder.md#ToonEncoder._handle_dict_key), [`_encode_iterative`](toon_encoder.md#ToonEncoder._encode_iterative), [`_handle_list_item`](toon_encoder.md#ToonEncoder._handle_list_item), [`_handle_array_table`](toon_encoder.md#ToonEncoder._handle_array_table), [`_handle_dict_start`](toon_encoder.md#ToonEncoder._handle_dict_start), [`_handle_list_start`](toon_encoder.md#ToonEncoder._handle_list_start)  (7 test-only)

### `_TaskType`  ·  implements/extends Enum
- def: [`tree_sitter_analyzer/formatters/toon_encoder.py:60`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_encoder.py#L60)
- doc: Types of encoding tasks for the iterative encoder.
- signature: `class _TaskType(Enum):`
- members:
  - `ENCODE_ARRAY_TABLE` — [`L70`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_encoder.py#L70)
  - `ENCODE_DICT_END` — [`L66`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_encoder.py#L66)
  - `ENCODE_DICT_KEY` — [`L65`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_encoder.py#L65)
  - `ENCODE_DICT_START` — [`L64`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_encoder.py#L64)
  - `ENCODE_LIST_END` — [`L69`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_encoder.py#L69)
  - `ENCODE_LIST_ITEM` — [`L68`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_encoder.py#L68)
  - `ENCODE_LIST_START` — [`L67`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_encoder.py#L67)
  - `ENCODE_VALUE` — [`L63`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_encoder.py#L63)
- used by: [`_handle_dict_key`](toon_encoder.md#ToonEncoder._handle_dict_key), [`_encode_iterative`](toon_encoder.md#ToonEncoder._encode_iterative), [`_handle_list_item`](toon_encoder.md#ToonEncoder._handle_list_item), [`_handle_dict_start`](toon_encoder.md#ToonEncoder._handle_dict_start), [`_handle_list_start`](toon_encoder.md#ToonEncoder._handle_list_start), [`task_type`](toon_encoder.md#_Task.task_type)  (7 test-only)

## Functions
- `_pick_list_str_column_name(key: str | None)` — [`L113`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_encoder.py#L113) — Choose a single-column header for a flat ``list[str]`` value.

## Module values
- `_FLAT_STR_LIST_THRESHOLD` — [`L98`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_encoder.py#L98)
- `_LIST_STR_COLUMN_NAMES` — [`L101`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_encoder.py#L101)
- `logger` — [`L25`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/toon_encoder.py#L25) — documented in [tree_sitter_analyzer-formatters-toon_encoder](../../../concepts/tree_sitter_analyzer-formatters-toon_encoder.md)

