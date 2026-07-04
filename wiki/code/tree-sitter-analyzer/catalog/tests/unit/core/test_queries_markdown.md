---
title: 'Module: tests/unit/core/test_queries_markdown.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_queries_markdown.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_queries_markdown`/TestMarkdownQuer
symbols:
  TestMarkdownQueryValidation.test_all_aliases_point_to_valid_queries: yValidation#test_all_aliases_point_to_valid_queries().
  TestMarkdownQueries.test_query_aliases_exist: ies#test_query_aliases_exist().
  TestMarkdownQueries.test_markdown_queries_exist: ies#test_markdown_queries_exist().
  TestMarkdownQueries.test_get_query_direct: ies#test_get_query_direct().
  TestMarkdownQueries.test_get_query_alias: ies#test_get_query_alias().
  TestMarkdownQueries.test_get_query_unknown: ies#test_get_query_unknown().
  TestMarkdownQueries.test_get_available_queries: ies#test_get_available_queries().
  TestMarkdownQueries.test_get_query_info_direct: ies#test_get_query_info_direct().
  TestMarkdownQueries.test_get_query_info_alias: ies#test_get_query_info_alias().
  TestMarkdownQueries.test_get_query_info_unknown: ies#test_get_query_info_unknown().
  TestMarkdownQueries.test_query_descriptions: ies#test_query_descriptions().
  TestMarkdownQueryContent.test_headers_query_content: yContent#test_headers_query_content().
  TestMarkdownQueryContent.test_code_blocks_query_content: yContent#test_code_blocks_query_content().
  TestMarkdownQueryContent.test_links_query_content: yContent#test_links_query_content().
  TestMarkdownQueryContent.test_images_query_content: yContent#test_images_query_content().
  TestMarkdownQueryContent.test_lists_query_content: yContent#test_lists_query_content().
  TestMarkdownQueryContent.test_emphasis_query_content: yContent#test_emphasis_query_content().
  TestMarkdownQueryContent.test_blockquotes_query_content: yContent#test_blockquotes_query_content().
  TestMarkdownQueryContent.test_tables_query_content: yContent#test_tables_query_content().
  TestMarkdownQueryContent.test_footnotes_query_content: yContent#test_footnotes_query_content().
  TestMarkdownQueryContent.test_all_elements_query_content: yContent#test_all_elements_query_content().
  TestMarkdownQueryAliases.test_header_level_aliases: yAliases#test_header_level_aliases().
  TestMarkdownQueryAliases.test_code_aliases: yAliases#test_code_aliases().
  TestMarkdownQueryAliases.test_link_aliases: yAliases#test_link_aliases().
  TestMarkdownQueryAliases.test_image_aliases: yAliases#test_image_aliases().
  TestMarkdownQueryAliases.test_list_aliases: yAliases#test_list_aliases().
  TestMarkdownQueryAliases.test_emphasis_aliases: yAliases#test_emphasis_aliases().
  TestMarkdownQueryAliases.test_comprehensive_aliases: yAliases#test_comprehensive_aliases().
  TestMarkdownQueryValidation.test_all_queries_are_strings: yValidation#test_all_queries_are_strings().
  TestMarkdownQueryValidation.test_no_circular_aliases: yValidation#test_no_circular_aliases().
  TestMarkdownQueryValidation.test_query_capture_names: yValidation#test_query_capture_names().
  TestMarkdownQueryValidation.test_query_syntax_basics: yValidation#test_query_syntax_basics().
  TestMarkdownQueryEdgeCases.test_empty_query_name: yEdgeCases#test_empty_query_name().
  TestMarkdownQueryEdgeCases.test_none_query_name: yEdgeCases#test_none_query_name().
  TestMarkdownQueryEdgeCases.test_case_sensitivity: yEdgeCases#test_case_sensitivity().
  TestMarkdownQueryEdgeCases.test_whitespace_in_query_name: yEdgeCases#test_whitespace_in_query_name().
  TestMarkdownQueryEdgeCases.test_special_characters_in_query_name: yEdgeCases#test_special_characters_in_query_name().
  TestMarkdownQueries: ies#
  TestMarkdownQueryContent: yContent#
  TestMarkdownQueryAliases: yAliases#
  TestMarkdownQueryValidation: yValidation#
  TestMarkdownQueryEdgeCases: yEdgeCases#
---
# Module: [`tests/unit/core/test_queries_markdown.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_markdown.py)

## Classes
### `TestMarkdownQueries`
- def: [`tests/unit/core/test_queries_markdown.py:20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_markdown.py#L20)
- doc: Test Markdown query definitions
- signature: `class TestMarkdownQueries:`
- members:
  - `test_get_available_queries(self)` — [`L110`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_markdown.py#L110) — Test getting list of available queries
  - `test_get_query_alias(self)` — [`L99`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_markdown.py#L99) — Test getting queries via aliases
  - `test_get_query_direct(self)` — [`L93`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_markdown.py#L93) — Test getting queries directly
  - `test_get_query_info_alias(self)` — [`L129`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_markdown.py#L129) — Test getting query info for alias
  - `test_get_query_info_direct(self)` — [`L119`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_markdown.py#L119) — Test getting query info for direct query
  - `test_get_query_info_unknown(self)` — [`L139`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_markdown.py#L139) — Test getting query info for unknown query
  - `test_get_query_unknown(self)` — [`L105`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_markdown.py#L105) — Test getting unknown query raises KeyError
  - `test_markdown_queries_exist(self)` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_markdown.py#L23) — Test that all expected queries exist
  - `test_query_aliases_exist(self)` — [`L51`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_markdown.py#L51) — Test that query aliases are properly defined
  - `test_query_descriptions(self)` — [`L146`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_markdown.py#L146) — Test query descriptions
- uses (calls/refs, reference-scoped): [`get_query`](../../../tree_sitter_analyzer/queries/markdown.md#get_query), [`MARKDOWN_QUERIES`](../../../tree_sitter_analyzer/queries/markdown.md#MARKDOWN_QUERIES.MARKDOWN_QUERIES), [`QUERY_ALIASES`](../../../tree_sitter_analyzer/queries/markdown.md#QUERY_ALIASES.QUERY_ALIASES), [`get_query_info`](../../../tree_sitter_analyzer/queries/markdown.md#get_query_info), [`get_available_queries`](../../../tree_sitter_analyzer/queries/markdown.md#get_available_queries), [`_get_query_description`](../../../tree_sitter_analyzer/queries/markdown.md#_get_query_description)

### `TestMarkdownQueryAliases`
- def: [`tests/unit/core/test_queries_markdown.py:234`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_markdown.py#L234)
- doc: Test specific query aliases
- signature: `class TestMarkdownQueryAliases:`
- members:
  - `test_code_aliases(self)` — [`L244`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_markdown.py#L244) — Test code-related aliases
  - `test_comprehensive_aliases(self)` — [`L277`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_markdown.py#L277) — Test comprehensive aliases
  - `test_emphasis_aliases(self)` — [`L269`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_markdown.py#L269) — Test emphasis-related aliases
  - `test_header_level_aliases(self)` — [`L237`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_markdown.py#L237) — Test header level aliases all point to headers
  - `test_image_aliases(self)` — [`L256`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_markdown.py#L256) — Test image-related aliases
  - `test_link_aliases(self)` — [`L250`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_markdown.py#L250) — Test link-related aliases
  - `test_list_aliases(self)` — [`L262`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_markdown.py#L262) — Test list-related aliases
- uses (calls/refs, reference-scoped): [`get_query`](../../../tree_sitter_analyzer/queries/markdown.md#get_query)

### `TestMarkdownQueryContent`
- def: [`tests/unit/core/test_queries_markdown.py:158`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_markdown.py#L158)
- doc: Test the content of specific Markdown queries
- signature: `class TestMarkdownQueryContent:`
- members:
  - `test_all_elements_query_content(self)` — [`L221`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_markdown.py#L221) — Test all_elements query contains major patterns
  - `test_blockquotes_query_content(self)` — [`L201`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_markdown.py#L201) — Test blockquotes query contains expected patterns
  - `test_code_blocks_query_content(self)` — [`L168`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_markdown.py#L168) — Test code blocks query contains expected patterns
  - `test_emphasis_query_content(self)` — [`L195`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_markdown.py#L195) — Test emphasis query contains expected patterns
  - `test_footnotes_query_content(self)` — [`L213`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_markdown.py#L213) — Test footnotes query contains expected patterns
  - `test_headers_query_content(self)` — [`L161`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_markdown.py#L161) — Test headers query contains expected patterns
  - `test_images_query_content(self)` — [`L181`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_markdown.py#L181) — Test images query contains expected patterns
  - `test_links_query_content(self)` — [`L175`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_markdown.py#L175) — Test links query contains expected patterns
  - `test_lists_query_content(self)` — [`L187`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_markdown.py#L187) — Test lists query contains expected patterns
  - `test_tables_query_content(self)` — [`L207`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_markdown.py#L207) — Test tables query contains expected patterns
- uses (calls/refs, reference-scoped): [`get_query`](../../../tree_sitter_analyzer/queries/markdown.md#get_query)

### `TestMarkdownQueryEdgeCases`
- def: [`tests/unit/core/test_queries_markdown.py:330`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_markdown.py#L330)
- doc: Test edge cases and error conditions
- signature: `class TestMarkdownQueryEdgeCases:`
- members:
  - `test_case_sensitivity(self)` — [`L343`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_markdown.py#L343) — Test that query names are case sensitive
  - `test_empty_query_name(self)` — [`L333`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_markdown.py#L333) — Test handling of empty query name
  - `test_none_query_name(self)` — [`L338`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_markdown.py#L338) — Test handling of None query name
  - `test_special_characters_in_query_name(self)` — [`L358`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_markdown.py#L358) — Test handling of special characters in query names
  - `test_whitespace_in_query_name(self)` — [`L353`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_markdown.py#L353) — Test handling of whitespace in query names
- uses (calls/refs, reference-scoped): [`get_query`](../../../tree_sitter_analyzer/queries/markdown.md#get_query)

### `TestMarkdownQueryValidation`
- def: [`tests/unit/core/test_queries_markdown.py:284`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_markdown.py#L284)
- doc: Test query validation and edge cases
- signature: `class TestMarkdownQueryValidation:`
- members:
  - `test_all_aliases_point_to_valid_queries(self)` — [`L295`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_markdown.py#L295) — Test that all aliases point to valid queries
  - `test_all_queries_are_strings(self)` — [`L287`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_markdown.py#L287) — Test that all queries are valid strings
  - `test_no_circular_aliases(self)` — [`L303`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_markdown.py#L303) — Test that there are no circular alias references
  - `test_query_capture_names(self)` — [`L309`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_markdown.py#L309) — Test that queries have reasonable capture names
  - `test_query_syntax_basics(self)` — [`L319`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_queries_markdown.py#L319) — Test basic query syntax
- uses (calls/refs, reference-scoped): [`get_query`](../../../tree_sitter_analyzer/queries/markdown.md#get_query), [`MARKDOWN_QUERIES`](../../../tree_sitter_analyzer/queries/markdown.md#MARKDOWN_QUERIES.MARKDOWN_QUERIES), [`QUERY_ALIASES`](../../../tree_sitter_analyzer/queries/markdown.md#QUERY_ALIASES.QUERY_ALIASES)

