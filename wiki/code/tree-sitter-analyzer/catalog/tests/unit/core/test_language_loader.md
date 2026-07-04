---
title: 'Module: tests/unit/core/test_language_loader.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_language_loader.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_language_loader`/test_
symbols:
  test_caching_behavior: caching_behavior().
  test_empty_language_name: empty_language_name().
  test_none_language_name: none_language_name().
  test_loader_instance: loader_instance().
  test_supported_languages: supported_languages().
  test_is_language_available_known_languages: is_language_available_known_languages().
  test_is_language_available_unknown_language: is_language_available_unknown_language().
  test_typescript_dialects: typescript_dialects().
  test_load_language_with_import_error: load_language_with_import_error().
  test_load_language_with_missing_language_function: load_language_with_missing_language_function().
  test_create_parser_success: create_parser_success().
  test_special_typescript_handling: special_typescript_handling().
  test_case_sensitivity: case_sensitivity().
  test_create_parser_safely_with_available_language: create_parser_safely_with_available_language().
  test_create_parser_safely_with_unavailable_language: create_parser_safely_with_unavailable_language().
  test_check_language_availability_function: check_language_availability_function().
---
# Module: [`tests/unit/core/test_language_loader.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_loader.py)

## Functions
- `test_caching_behavior()` — [`L115`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_loader.py#L115) — Test that loaded languages are cached
- `test_case_sensitivity()` — [`L166`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_loader.py#L166) — Test case sensitivity of language names
- `test_check_language_availability_function()` — [`L72`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_loader.py#L72) — Test the standalone availability check function
- `test_create_parser_safely_with_available_language()` — [`L57`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_loader.py#L57) — Test parser creation for available languages
- `test_create_parser_safely_with_unavailable_language()` — [`L66`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_loader.py#L66) — Test parser creation for unavailable languages
- `test_create_parser_success()` — [`L105`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_loader.py#L105) — Test successful parser creation with available language
- `test_empty_language_name()` — [`L154`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_loader.py#L154) — Test handling of empty language names
- `test_is_language_available_known_languages()` — [`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_loader.py#L38) — Test availability check for known languages
- `test_is_language_available_unknown_language()` — [`L51`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_loader.py#L51) — Test availability check for unknown languages
- `test_load_language_with_import_error()` — [`L91`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_loader.py#L91) — Test language loading when import fails for unknown language
- `test_load_language_with_missing_language_function()` — [`L98`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_loader.py#L98) — Test language loading when module lacks language() function
- `test_loader_instance()` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_loader.py#L21) — Test that loader instance is properly initialized
- `test_none_language_name()` — [`L160`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_loader.py#L160) — Test handling of None language names
- `test_special_typescript_handling()` — [`L135`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_loader.py#L135) — Test special handling for TypeScript variants
- `test_supported_languages()` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_loader.py#L27) — Test that supported languages are defined
- `test_typescript_dialects()` — [`L83`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_language_loader.py#L83) — Test TypeScript dialect handling

