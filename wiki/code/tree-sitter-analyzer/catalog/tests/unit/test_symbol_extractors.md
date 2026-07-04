---
title: 'Module: tests/unit/test_symbol_extractors.py'
type: catalog
provenance: extracted
module: tests/unit/test_symbol_extractors.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_symbol_extractors`/
symbols:
  _write: _write().
  TestPythonTopLevel.test_simple_def_and_class: TestPythonTopLevel#test_simple_def_and_class().
  TestPythonTopLevel.test_nested_def_is_excluded: TestPythonTopLevel#test_nested_def_is_excluded().
  TestPythonTopLevel.test_class_methods_are_excluded: TestPythonTopLevel#test_class_methods_are_excluded().
  TestPythonTopLevel.test_decorated_def_unwrapped: TestPythonTopLevel#test_decorated_def_unwrapped().
  TestPythonTopLevel.test_decorated_class_unwrapped: TestPythonTopLevel#test_decorated_class_unwrapped().
  TestPythonTopLevel.test_def_inside_if_main_is_excluded: TestPythonTopLevel#test_def_inside_if_main_is_excluded().
  TestPythonTopLevel.test_empty_file_returns_empty_set: TestPythonTopLevel#test_empty_file_returns_empty_set().
  TestPythonTopLevel.test_file_with_only_imports: TestPythonTopLevel#test_file_with_only_imports().
  TestPythonTopLevel.test_unicode_identifiers: TestPythonTopLevel#test_unicode_identifiers().
  TestPythonTopLevel.test_multiple_decorators_still_unwrap_once: TestPythonTopLevel#test_multiple_decorators_still_unwrap_once().
  TestNonPythonLanguages.test_non_python_returns_empty_set: TestNonPythonLanguages#test_non_python_returns_empty_set().
  TestNonPythonLanguages.test_unknown_language_returns_empty_set: TestNonPythonLanguages#test_unknown_language_returns_empty_set().
  TestFailureModes.test_syntactically_broken_python_returns_empty_set: TestFailureModes#test_syntactically_broken_python_returns_empty_set().
  TestFailureModes.test_missing_file_returns_empty_set: TestFailureModes#test_missing_file_returns_empty_set().
  TestPythonTopLevel: TestPythonTopLevel#
  TestNonPythonLanguages: TestNonPythonLanguages#
  TestFailureModes: TestFailureModes#
---
# Module: [`tests/unit/test_symbol_extractors.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbol_extractors.py)

## Classes
### `TestFailureModes`
- def: [`tests/unit/test_symbol_extractors.py:177`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbol_extractors.py#L177)
- signature: `class TestFailureModes:`
- members:
  - `test_missing_file_returns_empty_set(self)` — [`L178`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbol_extractors.py#L178)
  - `test_syntactically_broken_python_returns_empty_set(self, tmp_path: Path)` — [`L184`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbol_extractors.py#L184)
- uses (calls/refs, reference-scoped): [`extract_top_level_defs_from_file`](../../tree_sitter_analyzer/symbol_extractors.md#extract_top_level_defs_from_file)  (1 test-only)

### `TestNonPythonLanguages`
- def: [`tests/unit/test_symbol_extractors.py:144`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbol_extractors.py#L144)
- signature: `class TestNonPythonLanguages:`
- members:
  - `test_non_python_returns_empty_set(self, tmp_path: Path, language: str)` — [`L161`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbol_extractors.py#L161)
  - `test_unknown_language_returns_empty_set(self, tmp_path: Path)` — [`L170`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbol_extractors.py#L170)
- uses (calls/refs, reference-scoped): [`extract_top_level_defs_from_file`](../../tree_sitter_analyzer/symbol_extractors.md#extract_top_level_defs_from_file)  (1 test-only)

### `TestPythonTopLevel`
- def: [`tests/unit/test_symbol_extractors.py:38`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbol_extractors.py#L38)
- signature: `class TestPythonTopLevel:`
- members:
  - `test_class_methods_are_excluded(self, tmp_path: Path)` — [`L58`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbol_extractors.py#L58)
  - `test_decorated_class_unwrapped(self, tmp_path: Path)` — [`L86`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbol_extractors.py#L86)
  - `test_decorated_def_unwrapped(self, tmp_path: Path)` — [`L71`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbol_extractors.py#L71)
  - `test_def_inside_if_main_is_excluded(self, tmp_path: Path)` — [`L98`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbol_extractors.py#L98)
  - `test_empty_file_returns_empty_set(self, tmp_path: Path)` — [`L113`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbol_extractors.py#L113)
  - `test_file_with_only_imports(self, tmp_path: Path)` — [`L117`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbol_extractors.py#L117)
  - `test_multiple_decorators_still_unwrap_once(self, tmp_path: Path)` — [`L129`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbol_extractors.py#L129)
  - `test_nested_def_is_excluded(self, tmp_path: Path)` — [`L51`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbol_extractors.py#L51)
  - `test_simple_def_and_class(self, tmp_path: Path)` — [`L39`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbol_extractors.py#L39)
  - `test_unicode_identifiers(self, tmp_path: Path)` — [`L122`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbol_extractors.py#L122)
- uses (calls/refs, reference-scoped): [`extract_top_level_defs_from_file`](../../tree_sitter_analyzer/symbol_extractors.md#extract_top_level_defs_from_file)  (1 test-only)

## Functions
- `_write(tmp_path: Path, body: str, name: str = "sample.py")` — [`L30`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbol_extractors.py#L30) — Write ``body`` to ``<tmp_path>/<name>`` and return the absolute path.

