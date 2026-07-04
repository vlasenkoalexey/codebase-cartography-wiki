---
title: 'Module: tests/unit/languages/test_queries_module_contract.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_queries_module_contract.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_queries_module_contract`/
symbols:
  _queries_dict: _queries_dict().
  TestQueryModuleContract.test_all_queries_have_descriptions: TestQueryModuleContract#test_all_queries_have_descriptions().
  TestQueryModuleContract: TestQueryModuleContract#
  TestQueryModuleContract.test_lang_queries_dict_nonempty: TestQueryModuleContract#test_lang_queries_dict_nonempty().
  TestQueryModuleContract.test_descriptions_dict_nonempty: TestQueryModuleContract#test_descriptions_dict_nonempty().
  TestQueryModuleContract.test_all_queries_have_nonempty_strings: TestQueryModuleContract#test_all_queries_have_nonempty_strings().
  TestQueryModuleContract.test_get_query_valid_key: TestQueryModuleContract#test_get_query_valid_key().
  TestQueryModuleContract.test_all_query_strings_have_capture_syntax: TestQueryModuleContract#test_all_query_strings_have_capture_syntax().
  _descriptions_dict: _descriptions_dict().
  _MODULES: _MODULES.
  TestQueryModuleContract.test_all_queries_dict_exists: TestQueryModuleContract#test_all_queries_dict_exists().
  TestQueryModuleContract.test_get_all_queries_returns_dict: TestQueryModuleContract#test_get_all_queries_returns_dict().
  TestQueryModuleContract.test_list_queries_returns_nonempty_list: TestQueryModuleContract#test_list_queries_returns_nonempty_list().
  TestQueryModuleContract.test_get_query_invalid_key_raises: TestQueryModuleContract#test_get_query_invalid_key_raises().
---
# Module: [`tests/unit/languages/test_queries_module_contract.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_module_contract.py)

## Classes
### `TestQueryModuleContract`
- def: [`tests/unit/languages/test_queries_module_contract.py:66`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_module_contract.py#L66)
- doc: Every query module must satisfy these 10 invariants.
- signature: `class TestQueryModuleContract:`
- members:
  - `test_all_queries_dict_exists(self, mod: types.ModuleType)` — [`L81`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_module_contract.py#L81)
  - `test_all_queries_have_descriptions(self, mod: types.ModuleType)` — [`L84`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_module_contract.py#L84)
  - `test_all_queries_have_nonempty_strings(self, mod: types.ModuleType)` — [`L90`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_module_contract.py#L90)
  - `test_all_query_strings_have_capture_syntax(self, mod: types.ModuleType)` — [`L114`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_module_contract.py#L114)
  - `test_descriptions_dict_nonempty(self, mod: types.ModuleType)` — [`L75`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_module_contract.py#L75)
  - `test_get_all_queries_returns_dict(self, mod: types.ModuleType)` — [`L94`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_module_contract.py#L94)
  - `test_get_query_invalid_key_raises(self, mod: types.ModuleType)` — [`L110`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_module_contract.py#L110)
  - `test_get_query_valid_key(self, mod: types.ModuleType)` — [`L105`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_module_contract.py#L105)
  - `test_lang_queries_dict_nonempty(self, mod: types.ModuleType)` — [`L69`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_module_contract.py#L69)
  - `test_list_queries_returns_nonempty_list(self, mod: types.ModuleType)` — [`L98`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_module_contract.py#L98)
- uses (calls/refs, reference-scoped): (3 test-only callers)

## Functions
- `_descriptions_dict(mod: types.ModuleType)` — [`L58`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_module_contract.py#L58)
- `_queries_dict(mod: types.ModuleType)` — [`L50`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_module_contract.py#L50) — Return the language-specific LANG_QUERIES dict.

## Module values
- `_MODULES` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_module_contract.py#L35)

