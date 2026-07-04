---
title: 'Module: compatibility_test/scripts/_analyze_differences_json_severity.py'
type: catalog
provenance: extracted
module: compatibility_test/scripts/_analyze_differences_json_severity.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `compatibility_test.scripts._analyze_differences_json_severity`/
symbols:
  determine_field_severity: determine_field_severity().
  FieldSeverityFunc: FieldSeverityFunc.
  determine_severity: determine_severity().
  BREAKING_FIELDS: BREAKING_FIELDS.
  PERFORMANCE_FIELDS: PERFORMANCE_FIELDS.
  _is_large_string_change: _is_large_string_change().
  _is_removed_string_value: _is_removed_string_value().
---
# Module: [`compatibility_test/scripts/_analyze_differences_json_severity.py`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/_analyze_differences_json_severity.py)

## Functions
- `_is_large_string_change(old_value: Any, new_value: Any)` — [`L53`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/_analyze_differences_json_severity.py#L53)
- `_is_removed_string_value(old_value: Any, new_value: Any)` — [`L62`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/_analyze_differences_json_severity.py#L62)
- `determine_field_severity(field_name: str, old_value: Any, new_value: Any)` — [`L30`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/_analyze_differences_json_severity.py#L30) — Determine severity from a changed field name and values.
- `determine_severity(differences: list[dict[str, Any]])` — [`L43`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/_analyze_differences_json_severity.py#L43) — Determine overall severity from a difference list.

## Module values
- `BREAKING_FIELDS` — [`L8`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/_analyze_differences_json_severity.py#L8)
- `FieldSeverityFunc` — [`L6`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/_analyze_differences_json_severity.py#L6)
- `PERFORMANCE_FIELDS` — [`L20`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/_analyze_differences_json_severity.py#L20)

