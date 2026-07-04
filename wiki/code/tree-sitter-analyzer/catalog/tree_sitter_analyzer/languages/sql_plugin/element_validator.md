---
title: 'Module: tree_sitter_analyzer/languages/sql_plugin/element_validator.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/sql_plugin/element_validator.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.sql_plugin.element_validator`/
symbols:
  _build_recovered_view: _build_recovered_view().
  validate_and_fix_elements: validate_and_fix_elements().
  _fix_function_name: _fix_function_name().
  _recover_missing_views: _recover_missing_views().
  _fix_trigger_name: _fix_trigger_name().
  _fix_element_name: _fix_element_name().
  _is_phantom_element: _is_phantom_element().
  _FUNCTION_NAME_REGEX: _FUNCTION_NAME_REGEX.
  _GARBAGE_FUNCTION_NAMES: _GARBAGE_FUNCTION_NAMES.
  _TRIGGER_NAME_REGEX: _TRIGGER_NAME_REGEX.
  _CREATE_VIEW_LINE_REGEX: _CREATE_VIEW_LINE_REGEX.
  _VIEW_SOURCE_TABLES_REGEX: _VIEW_SOURCE_TABLES_REGEX.
  _record_unique: _record_unique().
---
# Module: [`tree_sitter_analyzer/languages/sql_plugin/element_validator.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/element_validator.py)

## Functions
- `_build_recovered_view(source_code: str, match: re.Match[str], view_name: str)` — [`L157`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/element_validator.py#L157) — Assemble a SQLView from a regex hit on the raw source.
- `_fix_element_name(elem: Any)` — [`L79`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/element_validator.py#L79) — Fix wrong names in-place. Return False to drop the element entirely.
- `_fix_function_name(elem: Any)` — [`L105`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/element_validator.py#L105) — Fix function name in-place. Return False if the element should be dropped.
- `_fix_trigger_name(elem: Any)` — [`L94`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/element_validator.py#L94) — Overwrite ``elem.name`` with the regex-extracted CREATE TRIGGER name.
- `_is_phantom_element(elem: Any)` — [`L61`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/element_validator.py#L61) — Drop trigger/function elements whose raw_text doesn't match their type.
- `_record_unique(elem: Any, seen_names: set[tuple[Any, str, Any]])` — [`L127`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/element_validator.py#L127) — Track ``(type, name, start_line)`` triples — return False on duplicates.
- `_recover_missing_views(source_code: str, validated: list[Any])` — [`L139`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/element_validator.py#L139) — Append SQLView entries for views found in raw SQL that weren't extracted.
- `validate_and_fix_elements(elements: list[Any], source_code: str)` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/element_validator.py#L33) — Post-process elements to fix parsing errors caused by platform-specific behavior.

## Module values
- `_CREATE_VIEW_LINE_REGEX` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/element_validator.py#L24)
- `_FUNCTION_NAME_REGEX` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/element_validator.py#L20)
- `_GARBAGE_FUNCTION_NAMES` — [`L16`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/element_validator.py#L16)
- `_TRIGGER_NAME_REGEX` — [`L17`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/element_validator.py#L17)
- `_VIEW_SOURCE_TABLES_REGEX` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/element_validator.py#L28)

