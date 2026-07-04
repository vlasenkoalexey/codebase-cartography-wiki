---
title: 'Module: tests/unit/test_codegraph_query_dsl.py'
type: catalog
provenance: extracted
module: tests/unit/test_codegraph_query_dsl.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_codegraph_query_dsl`/Test
symbols:
  TestParseChain.test_chain_argument_helpers_cover_defaults_and_fallbacks: ParseChain#test_chain_argument_helpers_cover_defaults_and_fallbacks().
  TestParseChain.test_parses_dotted_chain_without_splitting_inside_quotes: ParseChain#test_parses_dotted_chain_without_splitting_inside_quotes().
  TestParseChain.test_parses_semantic_search_step: ParseChain#test_parses_semantic_search_step().
  TestParseChain.test_parses_batch_seed_and_answer_pack_steps: ParseChain#test_parses_batch_seed_and_answer_pack_steps().
  TestParseChain.test_argument_helpers_cover_keyword_lists_and_limits: ParseChain#test_argument_helpers_cover_keyword_lists_and_limits().
  TestChainActionDocMatchesInner.test_chain_documented_params_subset_of_inner_schema: ChainActionDocMatchesInner#test_chain_documented_params_subset_of_inner_schema().
  TestParseChain.test_plain_query_expands_to_explore_related: ParseChain#test_plain_query_expands_to_explore_related().
  TestParseChain.test_quoted_pipe_is_legitimate_search_text: ParseChain#test_quoted_pipe_is_legitimate_search_text().
  TestParseChain.test_parses_uml_chain_step: ParseChain#test_parses_uml_chain_step().
  TestParseChain.test_parses_sort_by_confidence: ParseChain#test_parses_sort_by_confidence().
  TestParseChain.test_parses_selection_filter_steps: ParseChain#test_parses_selection_filter_steps().
  TestParseChain.test_parses_relation_aware_has_step: ParseChain#test_parses_relation_aware_has_step().
  TestParseChain.test_parses_kwargs_and_escaped_quotes: ParseChain#test_parses_kwargs_and_escaped_quotes().
  TestParseChain.test_accepts_js_style_bare_booleans: ParseChain#test_accepts_js_style_bare_booleans().
  TestParseChain.test_rejects_unsupported_step: ParseChain#test_rejects_unsupported_step().
  TestParseChain.test_pipe_separator_rejected_loudly: ParseChain#test_pipe_separator_rejected_loudly().
  TestParseChain.test_rejects_malformed_chains: ParseChain#test_rejects_malformed_chains().
  TestParseChain.test_parser_rejects_guardrail_violations: ParseChain#test_parser_rejects_guardrail_violations().
  TestParseChain: ParseChain#
  TestChainActionDocMatchesInner: ChainActionDocMatchesInner#
---
# Module: [`tests/unit/test_codegraph_query_dsl.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_dsl.py)

## Classes
### `TestChainActionDocMatchesInner`
- def: [`tests/unit/test_codegraph_query_dsl.py:224`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_dsl.py#L224)
- doc: #574: the search facade documented action=chain with params
- signature: `class TestChainActionDocMatchesInner:`
- members:
  - `test_chain_documented_params_subset_of_inner_schema(self)` — [`L231`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_dsl.py#L231)
- uses (calls/refs, reference-scoped): [`get_tool_definition`](../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.get_tool_definition), [`action_map`](../../tree_sitter_analyzer/mcp/tools/facade_tool.md#FacadeTool.action_map), [`build_search_facade`](../../tree_sitter_analyzer/mcp/tools/search_facade.md#build_search_facade), [`get_tool_definition`](../../tree_sitter_analyzer/mcp/tools/facade_tool.md#FacadeTool.get_tool_definition)

### `TestParseChain`
- def: [`tests/unit/test_codegraph_query_dsl.py:20`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_dsl.py#L20)
- signature: `class TestParseChain:`
- members:
  - `test_accepts_js_style_bare_booleans(self)` — [`L55`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_dsl.py#L55) — LLM agents naturally write true/false/null in this jQuery-style DSL.
  - `test_argument_helpers_cover_keyword_lists_and_limits(self)` — [`L213`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_dsl.py#L213)
  - `test_chain_argument_helpers_cover_defaults_and_fallbacks(self)` — [`L173`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_dsl.py#L173)
  - `test_parser_rejects_guardrail_violations(self, query, match)` — [`L209`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_dsl.py#L209)
  - `test_parses_batch_seed_and_answer_pack_steps(self)` — [`L90`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_dsl.py#L90)
  - `test_parses_dotted_chain_without_splitting_inside_quotes(self)` — [`L27`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_dsl.py#L27)
  - `test_parses_kwargs_and_escaped_quotes(self)` — [`L152`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_dsl.py#L152)
  - `test_parses_relation_aware_has_step(self)` — [`L133`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_dsl.py#L133)
  - `test_parses_selection_filter_steps(self)` — [`L113`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_dsl.py#L113)
  - `test_parses_semantic_search_step(self)` — [`L77`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_dsl.py#L77)
  - `test_parses_sort_by_confidence(self)` — [`L106`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_dsl.py#L106) — sort(by='confidence') is the BM25-relevance sort — README 'ahead' claim.
  - `test_parses_uml_chain_step(self)` — [`L84`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_dsl.py#L84)
  - `test_pipe_separator_rejected_loudly(self)` — [`L41`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_dsl.py#L41)
  - `test_plain_query_expands_to_explore_related(self)` — [`L21`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_dsl.py#L21)
  - `test_quoted_pipe_is_legitimate_search_text(self)` — [`L48`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_dsl.py#L48)
  - `test_rejects_malformed_chains(self, query, match)` — [`L169`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_dsl.py#L169)
  - `test_rejects_unsupported_step(self)` — [`L37`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_query_dsl.py#L37)
- uses (calls/refs, reference-scoped): [`_ChainStep`](../../tree_sitter_analyzer/mcp/tools/_codegraph_query_dsl.md#_ChainStep), [`parse_chain`](../../tree_sitter_analyzer/mcp/tools/_codegraph_query_dsl.md#parse_chain), [`kwargs`](../../tree_sitter_analyzer/mcp/tools/_codegraph_query_dsl.md#_ChainStep.kwargs), [`name`](../../tree_sitter_analyzer/mcp/tools/_codegraph_query_dsl.md#_ChainStep.name), [`bool_kw`](../../tree_sitter_analyzer/mcp/tools/_codegraph_query_dsl.md#bool_kw), [`int_kw`](../../tree_sitter_analyzer/mcp/tools/_codegraph_query_dsl.md#int_kw), [`string_args`](../../tree_sitter_analyzer/mcp/tools/_codegraph_query_dsl.md#string_args), [`args`](../../tree_sitter_analyzer/mcp/tools/_codegraph_query_dsl.md#_ChainStep.args), [`first_str`](../../tree_sitter_analyzer/mcp/tools/_codegraph_query_dsl.md#first_str), [`first_int`](../../tree_sitter_analyzer/mcp/tools/_codegraph_query_dsl.md#first_int)

