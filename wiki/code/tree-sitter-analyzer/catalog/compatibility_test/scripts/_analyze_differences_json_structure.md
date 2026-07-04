---
title: 'Module: compatibility_test/scripts/_analyze_differences_json_structure.py'
type: catalog
provenance: extracted
module: compatibility_test/scripts/_analyze_differences_json_structure.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `compatibility_test.scripts._analyze_differences_json_structure`/
symbols:
  compare_json_structure: compare_json_structure().
  _compare_dict_structure: _compare_dict_structure().
  _compare_list_structure: _compare_list_structure().
  _changed_common_key_diffs: _changed_common_key_diffs().
  _common_key_diffs: _common_key_diffs().
  _list_item_diffs: _list_item_diffs().
  _value_change: _value_change().
  _added_key_diffs: _added_key_diffs().
  _removed_key_diffs: _removed_key_diffs().
  _list_length_change: _list_length_change().
  _type_change: _type_change().
---
# Module: [`compatibility_test/scripts/_analyze_differences_json_structure.py`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/_analyze_differences_json_structure.py)

## Functions
- `_added_key_diffs(obj_b: dict[str, Any], added_keys: set[str], path: str)` — [`L113`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/_analyze_differences_json_structure.py#L113)
- `_changed_common_key_diffs(obj_a: dict[str, Any], obj_b: dict[str, Any], key: str, path: str, field_severity: FieldSeverityFunc)` — [`L83`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/_analyze_differences_json_structure.py#L83)
- `_common_key_diffs(obj_a: dict[str, Any], obj_b: dict[str, Any], common_keys: set[str], path: str, field_severity: FieldSeverityFunc)` — [`L65`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/_analyze_differences_json_structure.py#L65)
- `_compare_dict_structure(obj_a: dict[str, Any], obj_b: dict[str, Any], path: str, field_severity: FieldSeverityFunc)` — [`L29`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/_analyze_differences_json_structure.py#L29)
- `_compare_list_structure(obj_a: list[Any], obj_b: list[Any], path: str, field_severity: FieldSeverityFunc)` — [`L47`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/_analyze_differences_json_structure.py#L47)
- `_list_item_diffs(item_a: Any, item_b: Any, path: str, field_severity: FieldSeverityFunc)` — [`L95`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/_analyze_differences_json_structure.py#L95)
- `_list_length_change(obj_a: list[Any], obj_b: list[Any], path: str)` — [`L141`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/_analyze_differences_json_structure.py#L141)
- `_removed_key_diffs(obj_a: dict[str, Any], removed_keys: set[str], path: str)` — [`L127`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/_analyze_differences_json_structure.py#L127)
- `_type_change(path: str, obj_a: Any, obj_b: Any)` — [`L153`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/_analyze_differences_json_structure.py#L153)
- `_value_change(key: str, path: str, old_value: Any, new_value: Any, field_severity: FieldSeverityFunc)` — [`L163`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/_analyze_differences_json_structure.py#L163)
- `compare_json_structure(obj_a: Any, obj_b: Any, path: str, field_severity: FieldSeverityFunc)` — [`L10`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/_analyze_differences_json_structure.py#L10) — Recursively compare JSON structures.

