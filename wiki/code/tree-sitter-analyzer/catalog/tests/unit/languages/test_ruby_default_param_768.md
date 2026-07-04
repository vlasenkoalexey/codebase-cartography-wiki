---
title: 'Module: tests/unit/languages/test_ruby_default_param_768.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_ruby_default_param_768.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_ruby_default_param_768`/
symbols:
  TestRubyInTypeSuffixLanguages.test_ruby_in_type_suffix_languages: TestRubyInTypeSuffixLanguages#test_ruby_in_type_suffix_languages().
  TestRubyDefaultValuedParameters.test_array_default: TestRubyDefaultValuedParameters#test_array_default().
  TestRubyDefaultValuedParameters.test_hash_default: TestRubyDefaultValuedParameters#test_hash_default().
  TestRubyDefaultValuedParameters.test_string_default: TestRubyDefaultValuedParameters#test_string_default().
  TestRubyDefaultValuedParameters.test_integer_default: TestRubyDefaultValuedParameters#test_integer_default().
  TestRubyDefaultValuedParameters.test_nil_default: TestRubyDefaultValuedParameters#test_nil_default().
  TestRubyDefaultValuedParameters.test_no_default_unchanged: TestRubyDefaultValuedParameters#test_no_default_unchanged().
  TestRubyDefaultValuedParameters.test_splat_param: TestRubyDefaultValuedParameters#test_splat_param().
  TestRubyDefaultValuedParameters.test_double_splat_param: TestRubyDefaultValuedParameters#test_double_splat_param().
  TestRubyDefaultValuedParameters.test_type_not_garbled: TestRubyDefaultValuedParameters#test_type_not_garbled().
  pytestmark: pytestmark.
  TestRubyInTypeSuffixLanguages: TestRubyInTypeSuffixLanguages#
  TestRubyDefaultValuedParameters: TestRubyDefaultValuedParameters#
---
# Module: [`tests/unit/languages/test_ruby_default_param_768.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_default_param_768.py)

## Classes
### `TestRubyDefaultValuedParameters`
- def: [`tests/unit/languages/test_ruby_default_param_768.py:29`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_default_param_768.py#L29)
- doc: Default-valued Ruby params must extract the name, not the default literal.
- signature: `class TestRubyDefaultValuedParameters:`
- members:
  - `test_array_default(self)` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_default_param_768.py#L32) — permissions = [] → name='permissions', not '[]'.
  - `test_double_splat_param(self)` — [`L71`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_default_param_768.py#L71) — **kwargs → name='**kwargs', type='Any'.
  - `test_hash_default(self)` — [`L40`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_default_param_768.py#L40) — opts = {} → name='opts'.
  - `test_integer_default(self)` — [`L50`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_default_param_768.py#L50) — limit = 10 → name='limit'.
  - `test_nil_default(self)` — [`L55`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_default_param_768.py#L55) — options = nil → name='options'.
  - `test_no_default_unchanged(self)` — [`L60`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_default_param_768.py#L60) — Bare params without defaults must still extract correctly.
  - `test_splat_param(self)` — [`L66`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_default_param_768.py#L66) — *args → name='*args', type='Any' (no mangling).
  - `test_string_default(self)` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_default_param_768.py#L45) — role = 'admin' → name='role'.
  - `test_type_not_garbled(self)` — [`L76`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_default_param_768.py#L76) — Type must be 'Any' (Ruby has no type annotations).
- uses (calls/refs, reference-scoped): [`_process_single_parameter`](../../../tree_sitter_analyzer/cli/commands/table_command_helpers.md#_process_single_parameter)

### `TestRubyInTypeSuffixLanguages`
- def: [`tests/unit/languages/test_ruby_default_param_768.py:19`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_default_param_768.py#L19)
- doc: Ruby must route through the suffix (name-first) path — tracked: #768.
- signature: `class TestRubyInTypeSuffixLanguages:`
- members:
  - `test_ruby_in_type_suffix_languages(self)` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_default_param_768.py#L22)
- uses (calls/refs, reference-scoped): [`TYPE_SUFFIX_LANGUAGES`](../../../tree_sitter_analyzer/cli/commands/table_command_helpers.md#TYPE_SUFFIX_LANGUAGES)

## Module values
- `pytestmark` — [`L16`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_ruby_default_param_768.py#L16)

