---
title: 'Module: tests/unit/test_symbols_json_enrichment.py'
type: catalog
provenance: extracted
module: tests/unit/test_symbols_json_enrichment.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_symbols_json_enrichment`/
symbols:
  _symbols_for: _symbols_for().
  _FakeChild: _FakeChild#
  TestPythonDocstringSerialized._by_name: TestPythonDocstringSerialized#_by_name().
  TestReturnTypeAndParamsSerialized._by_name: TestReturnTypeAndParamsSerialized#_by_name().
  TestBashSubscriptBaseFallback.test_name_field_present_returns_field_node: TestBashSubscriptBaseFallback#test_name_field_present_returns_field_node().
  TestBashSubscriptBaseFallback.test_no_name_field_falls_back_to_variable_name_child: TestBashSubscriptBaseFallback#test_no_name_field_falls_back_to_variable_name_child().
  TestBashSubscriptBaseFallback.test_no_name_field_falls_back_to_word_child: TestBashSubscriptBaseFallback#test_no_name_field_falls_back_to_word_child().
  TestBashSubscriptBaseFallback.test_no_base_anywhere_returns_none: TestBashSubscriptBaseFallback#test_no_base_anywhere_returns_none().
  TestPythonDocstringSerialized.test_docstring_capped_at_exactly_500_chars: TestPythonDocstringSerialized#test_docstring_capped_at_exactly_500_chars().
  TestExtractorVersionBump.test_extractor_version_matches_in_both_sites: TestExtractorVersionBump#test_extractor_version_matches_in_both_sites().
  _FakeSubscript: _FakeSubscript#
  TestPythonDocstringSerialized.test_function_docstring_serialized: TestPythonDocstringSerialized#test_function_docstring_serialized().
  TestPythonDocstringSerialized.test_method_docstring_serialized: TestPythonDocstringSerialized#test_method_docstring_serialized().
  TestPythonDocstringSerialized.test_class_docstring_serialized: TestPythonDocstringSerialized#test_class_docstring_serialized().
  TestPythonDocstringSerialized.test_absent_docstring_field_absent_not_empty_string: TestPythonDocstringSerialized#test_absent_docstring_field_absent_not_empty_string().
  TestPythonDocstringSerialized.test_whitespace_only_docstring_field_absent: TestPythonDocstringSerialized#test_whitespace_only_docstring_field_absent().
  TestPythonDocstringSerialized.test_incomplete_function_without_body_is_safe: TestPythonDocstringSerialized#test_incomplete_function_without_body_is_safe().
  TestPythonDocstringSerialized.test_multiline_docstring_stripped_and_preserved: TestPythonDocstringSerialized#test_multiline_docstring_stripped_and_preserved().
  TestReturnTypeAndParamsSerialized.test_return_type_serialized: TestReturnTypeAndParamsSerialized#test_return_type_serialized().
  TestReturnTypeAndParamsSerialized.test_absent_return_type_field_absent: TestReturnTypeAndParamsSerialized#test_absent_return_type_field_absent().
  TestReturnTypeAndParamsSerialized.test_params_already_serialized: TestReturnTypeAndParamsSerialized#test_params_already_serialized().
  TestReturnTypeAndParamsSerialized.test_rust_return_type_serialized: TestReturnTypeAndParamsSerialized#test_rust_return_type_serialized().
  TestReturnTypeAndParamsSerialized.test_non_python_function_has_no_docstring: TestReturnTypeAndParamsSerialized#test_non_python_function_has_no_docstring().
  TestBashVariableAssignmentScope.test_command_prefix_env_var_not_recorded: TestBashVariableAssignmentScope#test_command_prefix_env_var_not_recorded().
  TestBashVariableAssignmentScope.test_standalone_assignment_recorded: TestBashVariableAssignmentScope#test_standalone_assignment_recorded().
  TestBashVariableAssignmentScope.test_subscript_assignment_target_unwrapped_to_base: TestBashVariableAssignmentScope#test_subscript_assignment_target_unwrapped_to_base().
  _FakeSubscript.child_by_field_name: _FakeSubscript#child_by_field_name().
  TestCodexP2sOn621.test_concatenated_string_docstring_preserved: TestCodexP2sOn621#test_concatenated_string_docstring_preserved().
  TestCodexP2sOn621.test_typescript_return_annotation_stripped: TestCodexP2sOn621#test_typescript_return_annotation_stripped().
  _PY_SRC: _PY_SRC.
  _FakeSubscript._named_base: _FakeSubscript#_named_base.
  TestPythonDocstringSerialized: TestPythonDocstringSerialized#
  TestReturnTypeAndParamsSerialized: TestReturnTypeAndParamsSerialized#
  TestExtractorVersionBump: TestExtractorVersionBump#
  TestBashVariableAssignmentScope: TestBashVariableAssignmentScope#
  _FakeChild.__init__: _FakeChild#__init__().
  _FakeSubscript.__init__: _FakeSubscript#__init__().
  _FakeSubscript.children: _FakeSubscript#children.
  TestBashSubscriptBaseFallback: TestBashSubscriptBaseFallback#
  TestCodexP2sOn621: TestCodexP2sOn621#
---
# Module: [`tests/unit/test_symbols_json_enrichment.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbols_json_enrichment.py)

## Classes
### `TestBashSubscriptBaseFallback`
- def: [`tests/unit/test_symbols_json_enrichment.py:199`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbols_json_enrichment.py#L199)
- doc: #949 — `_bash_subscript_base` field-vs-fallback-vs-None branches.
- signature: `class TestBashSubscriptBaseFallback:`
- members:
  - `test_name_field_present_returns_field_node(self)` — [`L202`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbols_json_enrichment.py#L202)
  - `test_no_base_anywhere_returns_none(self)` — [`L235`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbols_json_enrichment.py#L235)
  - `test_no_name_field_falls_back_to_variable_name_child(self)` — [`L213`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbols_json_enrichment.py#L213)
  - `test_no_name_field_falls_back_to_word_child(self)` — [`L224`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbols_json_enrichment.py#L224)
- uses (calls/refs, reference-scoped): [`_bash_subscript_base`](../../tree_sitter_analyzer/_ast_extraction.md#_bash_subscript_base)  (2 test-only)

### `TestBashVariableAssignmentScope`
- def: [`tests/unit/test_symbols_json_enrichment.py:149`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbols_json_enrichment.py#L149)
- doc: #949 Codex P2 — bash variable_assignment extraction edge cases.
- signature: `class TestBashVariableAssignmentScope:`
- members:
  - `test_command_prefix_env_var_not_recorded(self)` — [`L152`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbols_json_enrichment.py#L152)
  - `test_standalone_assignment_recorded(self)` — [`L162`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbols_json_enrichment.py#L162)
  - `test_subscript_assignment_target_unwrapped_to_base(self)` — [`L167`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbols_json_enrichment.py#L167)
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `TestCodexP2sOn621`
- def: [`tests/unit/test_symbols_json_enrichment.py:246`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbols_json_enrichment.py#L246)
- signature: `class TestCodexP2sOn621:`
- members:
  - `test_concatenated_string_docstring_preserved(self)` — [`L247`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbols_json_enrichment.py#L247)
  - `test_typescript_return_annotation_stripped(self)` — [`L252`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbols_json_enrichment.py#L252)
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `TestExtractorVersionBump`
- def: [`tests/unit/test_symbols_json_enrichment.py:138`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbols_json_enrichment.py#L138)
- signature: `class TestExtractorVersionBump:`
- members:
  - `test_extractor_version_matches_in_both_sites(self)` — [`L139`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbols_json_enrichment.py#L139)
- uses (calls/refs, reference-scoped): [`_AST_CACHE_EXTRACTOR_VERSION`](../../tree_sitter_analyzer/ast_cache.md#_AST_CACHE_EXTRACTOR_VERSION), [`_AST_CACHE_EXTRACTOR_VERSION`](../../tree_sitter_analyzer/_ast_cache_indexer.md#_AST_CACHE_EXTRACTOR_VERSION)

### `TestPythonDocstringSerialized`
- def: [`tests/unit/test_symbols_json_enrichment.py:58`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbols_json_enrichment.py#L58)
- signature: `class TestPythonDocstringSerialized:`
- members:
  - `test_absent_docstring_field_absent_not_empty_string(self)` — [`L79`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbols_json_enrichment.py#L79)
  - `test_class_docstring_serialized(self)` — [`L73`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbols_json_enrichment.py#L73)
  - `test_docstring_capped_at_exactly_500_chars(self)` — [`L84`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbols_json_enrichment.py#L84)
  - `test_function_docstring_serialized(self)` — [`L62`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbols_json_enrichment.py#L62)
  - `test_incomplete_function_without_body_is_safe(self)` — [`L97`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbols_json_enrichment.py#L97)
  - `test_method_docstring_serialized(self)` — [`L69`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbols_json_enrichment.py#L69)
  - `test_multiline_docstring_stripped_and_preserved(self)` — [`L105`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbols_json_enrichment.py#L105)
  - `test_whitespace_only_docstring_field_absent(self)` — [`L92`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbols_json_enrichment.py#L92)
- protocol/private: `_by_name`[`L59`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbols_json_enrichment.py#L59)
- uses (calls/refs, reference-scoped): [`_DOCSTRING_MAX_CHARS`](../../tree_sitter_analyzer/_ast_extraction.md#_DOCSTRING_MAX_CHARS)  (2 test-only)

### `TestReturnTypeAndParamsSerialized`
- def: [`tests/unit/test_symbols_json_enrichment.py:111`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbols_json_enrichment.py#L111)
- signature: `class TestReturnTypeAndParamsSerialized:`
- members:
  - `test_absent_return_type_field_absent(self)` — [`L119`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbols_json_enrichment.py#L119)
  - `test_non_python_function_has_no_docstring(self)` — [`L132`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbols_json_enrichment.py#L132)
  - `test_params_already_serialized(self)` — [`L123`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbols_json_enrichment.py#L123)
  - `test_return_type_serialized(self)` — [`L115`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbols_json_enrichment.py#L115)
  - `test_rust_return_type_serialized(self)` — [`L127`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbols_json_enrichment.py#L127)
- protocol/private: `_by_name`[`L112`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbols_json_enrichment.py#L112)
- uses (calls/refs, reference-scoped): (2 test-only callers)

### `_FakeChild`
- def: [`tests/unit/test_symbols_json_enrichment.py:174`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbols_json_enrichment.py#L174)
- doc: Minimal stand-in for a tree-sitter child node (only `.type` is read).
- signature: `class _FakeChild:`
- protocol/private: `__init__`[`L177`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbols_json_enrichment.py#L177)
- used by: (4 test-only callers)

### `_FakeSubscript`
- def: [`tests/unit/test_symbols_json_enrichment.py:181`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbols_json_enrichment.py#L181)
- doc: Minimal stand-in for a `subscript` node exercising the fallback path.
- signature: `class _FakeSubscript:`
- members:
  - `child_by_field_name(self, field: str)` — [`L195`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbols_json_enrichment.py#L195)
  - `children` — [`L193`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbols_json_enrichment.py#L193)
- protocol/private: `__init__`[`L191`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbols_json_enrichment.py#L191), `_named_base`[`L192`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbols_json_enrichment.py#L192)
- used by: (4 test-only callers)

## Functions
- `_symbols_for(source: str, lang: str)` — [`L22`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbols_json_enrichment.py#L22)

## Module values
- `_PY_SRC` — [`L31`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbols_json_enrichment.py#L31)

