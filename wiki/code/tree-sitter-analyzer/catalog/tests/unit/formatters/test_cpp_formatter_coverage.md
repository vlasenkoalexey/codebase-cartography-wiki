---
title: 'Module: tests/unit/formatters/test_cpp_formatter_coverage.py'
type: catalog
provenance: extracted
module: tests/unit/formatters/test_cpp_formatter_coverage.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.formatters.test_cpp_formatter_coverage`/
symbols:
  test_other_methods_section: test_other_methods_section().
  test_private_methods_section: test_private_methods_section().
  test_global_fields_rendered: test_global_fields_rendered().
  test_cpp_formatter_complex: test_cpp_formatter_complex().
  test_imports_section_rendered: test_imports_section_rendered().
  test_convert_function_element_no_space_param: test_convert_function_element_no_space_param().
  test_convert_function_element_dict_param: test_convert_function_element_dict_param().
  test_convert_function_element_non_str_non_dict_param: test_convert_function_element_non_str_non_dict_param().
  test_convert_import_no_raw_text: test_convert_import_no_raw_text().
  test_convert_function_element_fallback_param: test_convert_function_element_fallback_param().
  test_cpp_formatter_with_namespace: test_cpp_formatter_with_namespace().
  test_single_package_renders_package_section: test_single_package_renders_package_section().
  test_cpp_formatter_global_functions_only: test_cpp_formatter_global_functions_only().
  test_cpp_formatter_compact_format: test_cpp_formatter_compact_format().
  test_packages_list_renders_namespaces_section: test_packages_list_renders_namespaces_section().
  test_cpp_formatter_basic: test_cpp_formatter_basic().
  formatter: formatter().
  test_compact_signature_string_params: test_compact_signature_string_params().
  test_shorten_type_none: test_shorten_type_none().
  test_shorten_type_pointers_and_arrays: test_shorten_type_pointers_and_arrays().
  test_shorten_type_qualifier_removal: test_shorten_type_qualifier_removal().
  test_shorten_type_map: test_shorten_type_map().
  test_shorten_type_unknown_passthrough: test_shorten_type_unknown_passthrough().
  test_format_table_json: test_format_table_json().
  test_format_advanced_csv: test_format_advanced_csv().
  test_format_advanced_full: test_format_advanced_full().
  test_format_summary: test_format_summary().
  test_compact_signature_dict_param_pointer: test_compact_signature_dict_param_pointer().
---
# Module: [`tests/unit/formatters/test_cpp_formatter_coverage.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_coverage.py)

## Functions
- `formatter()` — [`L15`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_coverage.py#L15)
- `test_compact_signature_dict_param_pointer(formatter)` — [`L408`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_coverage.py#L408) — Cover dict-format param where name starts with * (pointer).
- `test_compact_signature_string_params(formatter)` — [`L168`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_coverage.py#L168) — Cover _create_compact_signature branches for string-format params.
- `test_convert_function_element_dict_param(formatter)` — [`L312`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_coverage.py#L312) — Cover _convert_function_element with dict-format param.
- `test_convert_function_element_fallback_param(formatter)` — [`L422`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_coverage.py#L422) — Cover fallback when param_type or param_name is empty after split.
- `test_convert_function_element_no_space_param(formatter)` — [`L297`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_coverage.py#L297) — Cover _convert_function_element with param string having no space.
- `test_convert_function_element_non_str_non_dict_param(formatter)` — [`L327`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_coverage.py#L327) — Cover _convert_function_element with else-branch (non-str, non-dict param).
- `test_convert_import_no_raw_text(formatter)` — [`L345`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_coverage.py#L345) — Cover _convert_import_element when raw_text is empty.
- `test_cpp_formatter_basic(formatter)` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_coverage.py#L19)
- `test_cpp_formatter_compact_format(formatter)` — [`L78`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_coverage.py#L78) — Cover compact table path (non-full format).
- `test_cpp_formatter_complex(formatter)` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_coverage.py#L29)
- `test_cpp_formatter_global_functions_only(formatter)` — [`L67`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_coverage.py#L67) — Cover pure C-style global functions (no classes).
- `test_cpp_formatter_with_namespace(formatter)` — [`L51`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_coverage.py#L51) — Cover namespace/package rendering path.
- `test_format_advanced_csv(formatter)` — [`L272`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_coverage.py#L272) — Cover format_advanced csv path.
- `test_format_advanced_full(formatter)` — [`L283`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_coverage.py#L283) — Cover format_advanced non-json, non-csv → _format_full_table path.
- `test_format_summary(formatter)` — [`L366`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_coverage.py#L366) — Cover format_summary method.
- `test_format_table_json(formatter)` — [`L258`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_coverage.py#L258) — Cover format_table with json type.
- `test_global_fields_rendered(formatter)` — [`L148`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_coverage.py#L148) — Cover global variables table at lines 129-153.
- `test_imports_section_rendered(formatter)` — [`L129`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_coverage.py#L129) — Cover imports rendering at lines 52-59.
- `test_other_methods_section(formatter)` — [`L382`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_coverage.py#L382) — Cover 'Other Methods' rendering for non-public, non-private methods.
- `test_packages_list_renders_namespaces_section(formatter)` — [`L93`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_coverage.py#L93) — Cover the `packages` list path at line 44.
- `test_private_methods_section(formatter)` — [`L440`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_coverage.py#L440) — Cover 'Private Methods' rendering in _format_class_details.
- `test_shorten_type_map(formatter)` — [`L232`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_coverage.py#L232) — Cover _shorten_type type_map dict.
- `test_shorten_type_none(formatter)` — [`L213`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_coverage.py#L213) — Cover _shorten_type → None path.
- `test_shorten_type_pointers_and_arrays(formatter)` — [`L218`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_coverage.py#L218) — Cover _shorten_type pointer/ref/array early return.
- `test_shorten_type_qualifier_removal(formatter)` — [`L225`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_coverage.py#L225) — Cover _shorten_type const/volatile/static stripping.
- `test_shorten_type_unknown_passthrough(formatter)` — [`L249`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_coverage.py#L249) — Non-primitive types pass through unchanged.
- `test_single_package_renders_package_section(formatter)` — [`L113`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_cpp_formatter_coverage.py#L113) — Cover the elif branch for single package_name.

