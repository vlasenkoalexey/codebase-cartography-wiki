---
title: 'Module: tests/unit/languages/test_go_param_name_type_swap.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_go_param_name_type_swap.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_go_param_name_type_swap`/Test
symbols:
  TestGoParamExtractionEndToEnd._extract_functions: GoParamExtractionEndToEnd#_extract_functions().
  TestGoParamExtractionEndToEnd.test_phi_signature_in_table: GoParamExtractionEndToEnd#test_phi_signature_in_table().
  TestGoSignatureRendering.test_single_param_renders_correctly: GoSignatureRendering#test_single_param_renders_correctly().
  TestGoSignatureRendering.test_two_params_render_correctly: GoSignatureRendering#test_two_params_render_correctly().
  TestGoSignatureRendering.test_return_type_appended: GoSignatureRendering#test_return_type_appended().
  TestGoSignatureRendering.test_multi_return_type: GoSignatureRendering#test_multi_return_type().
  TestGoSignatureRendering.test_no_params: GoSignatureRendering#test_no_params().
  TestGoSignatureRendering._func_dict: GoSignatureRendering#_func_dict().
  TestProcessParametersGo.test_single_param_name_before_type: ProcessParametersGo#test_single_param_name_before_type().
  TestProcessParametersGo.test_single_param_plain_int: ProcessParametersGo#test_single_param_plain_int().
  TestProcessParametersGo.test_two_params_same_type: ProcessParametersGo#test_two_params_same_type().
  TestProcessParametersGo.test_multi_word_type: ProcessParametersGo#test_multi_word_type().
  TestProcessParametersGo.test_pointer_param: ProcessParametersGo#test_pointer_param().
  TestProcessParametersGo.test_variadic_param: ProcessParametersGo#test_variadic_param().
  TestProcessParametersGo.test_empty_list: ProcessParametersGo#test_empty_list().
  TestGoParamExtractionEndToEnd.test_phi_param_extraction: GoParamExtractionEndToEnd#test_phi_param_extraction().
  TestGoParamExtractionEndToEnd.test_combinations_param_extraction: GoParamExtractionEndToEnd#test_combinations_param_extraction().
  TestProcessParametersGo: ProcessParametersGo#
  TestGoSignatureRendering: GoSignatureRendering#
  TestGoParamExtractionEndToEnd: GoParamExtractionEndToEnd#
  TestGoParamExtractionEndToEnd.phi_fixture: GoParamExtractionEndToEnd#phi_fixture().
  TestGoParamExtractionEndToEnd.combinations_fixture: GoParamExtractionEndToEnd#combinations_fixture().
---
# Module: [`tests/unit/languages/test_go_param_name_type_swap.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_param_name_type_swap.py)

## Classes
### `TestGoParamExtractionEndToEnd`
- def: [`tests/unit/languages/test_go_param_name_type_swap.py:154`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_param_name_type_swap.py#L154)
- doc: Parse a real Go snippet; verify the params and signature are correct.
- signature: `class TestGoParamExtractionEndToEnd:`
- members:
  - `_extract_functions(self, file_path: str)` — [`L174`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_param_name_type_swap.py#L174) — Run the Go plugin against a file and return Function elements.
  - `combinations_fixture(self, tmp_path)` — [`L165`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_param_name_type_swap.py#L165) — Write a minimal Go fixture with func Combinations(n int, k int) (int, error).
  - `phi_fixture(self, tmp_path)` — [`L158`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_param_name_type_swap.py#L158) — Write a minimal Go fixture with func Phi(n int64) int64.
  - `test_combinations_param_extraction(self, combinations_fixture)` — [`L200`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_param_name_type_swap.py#L200) — func Combinations(n int, k int) — params extracted as strings.
  - `test_phi_param_extraction(self, phi_fixture)` — [`L192`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_param_name_type_swap.py#L192) — func Phi(n int64) int64 — extracted params must have name='n', type='int64'.
  - `test_phi_signature_in_table(self, phi_fixture)` — [`L207`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_param_name_type_swap.py#L207) — GoTableFormatter must render (n int64) int64, not raw dicts.
- uses (calls/refs, reference-scoped): [`GoTableFormatter`](../../../tree_sitter_analyzer/formatters/go_formatter.md#GoTableFormatter), [`GoElementExtractor`](../../../tree_sitter_analyzer/languages/go_plugin.md#GoElementExtractor), [`extract_functions`](../../../tree_sitter_analyzer/languages/go_plugin.md#GoElementExtractor.extract_functions), [`_get_node_text`](../../../tree_sitter_analyzer/languages/go_plugin.md#GoElementExtractor._get_node_text), [`process_parameters`](../../../tree_sitter_analyzer/cli/commands/table_command_helpers.md#process_parameters), [`_create_go_signature`](../../../tree_sitter_analyzer/formatters/go_formatter.md#GoTableFormatter._create_go_signature)

### `TestGoSignatureRendering`
- def: [`tests/unit/languages/test_go_param_name_type_swap.py:88`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_param_name_type_swap.py#L88)
- doc: Signature must show 'n int64', never the raw dict repr.
- signature: `class TestGoSignatureRendering:`
- members:
  - `test_multi_return_type(self)` — [`L132`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_param_name_type_swap.py#L132) — (int, error) return type is preserved.
  - `test_no_params(self)` — [`L141`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_param_name_type_swap.py#L141) — () — zero-param function renders clean parens.
  - `test_return_type_appended(self)` — [`L123`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_param_name_type_swap.py#L123) — Return type is appended after the param list.
  - `test_single_param_renders_correctly(self)` — [`L101`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_param_name_type_swap.py#L101) — (n int64) int64 — no raw dict repr in output.
  - `test_two_params_render_correctly(self)` — [`L113`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_param_name_type_swap.py#L113) — (n int, k int) — two params rendered without dict repr.
- protocol/private: `_func_dict`[`L91`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_param_name_type_swap.py#L91)
- uses (calls/refs, reference-scoped): [`GoTableFormatter`](../../../tree_sitter_analyzer/formatters/go_formatter.md#GoTableFormatter), [`_create_go_signature`](../../../tree_sitter_analyzer/formatters/go_formatter.md#GoTableFormatter._create_go_signature)

### `TestProcessParametersGo`
- def: [`tests/unit/languages/test_go_param_name_type_swap.py:30`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_param_name_type_swap.py#L30)
- doc: Go params are name-before-type: 'n int64' → name='n', type='int64'.
- signature: `class TestProcessParametersGo:`
- members:
  - `test_empty_list(self)` — [`L77`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_param_name_type_swap.py#L77) — Empty param list returns empty list.
  - `test_multi_word_type(self)` — [`L56`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_param_name_type_swap.py#L56) — Pointer receiver type: 'p []byte' → name='p', type='[]byte'.
  - `test_pointer_param(self)` — [`L63`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_param_name_type_swap.py#L63) — 'config *Config' → name='config', type='*Config'.
  - `test_single_param_name_before_type(self)` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_param_name_type_swap.py#L33) — 'n int64' must parse as name='n', type='int64', not swapped.
  - `test_single_param_plain_int(self)` — [`L40`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_param_name_type_swap.py#L40) — 'n int' must parse as name='n', type='int'.
  - `test_two_params_same_type(self)` — [`L47`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_param_name_type_swap.py#L47) — 'n int, k int' — each individually parsed.
  - `test_variadic_param(self)` — [`L70`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_param_name_type_swap.py#L70) — 'numbers ...int' → name='numbers', type='...int'.
- uses (calls/refs, reference-scoped): [`process_parameters`](../../../tree_sitter_analyzer/cli/commands/table_command_helpers.md#process_parameters)

