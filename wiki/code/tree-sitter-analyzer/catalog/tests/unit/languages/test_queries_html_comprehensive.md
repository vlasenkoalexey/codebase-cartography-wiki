---
title: 'Module: tests/unit/languages/test_queries_html_comprehensive.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_queries_html_comprehensive.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_queries_html_comprehensive`/Test
symbols:
  TestHTMLQueries.test_all_queries_have_descriptions: HTMLQueries#test_all_queries_have_descriptions().
  TestGetHTMLQuery.test_get_html_query_all_defined_queries: GetHTMLQuery#test_get_html_query_all_defined_queries().
  TestGetHTMLQueryDescription.test_get_html_query_description_all_queries: GetHTMLQueryDescription#test_get_html_query_description_all_queries().
  TestGetAllQueries.test_get_all_queries_contains_all_html_queries: GetAllQueries#test_get_all_queries_contains_all_html_queries().
  TestListQueries.test_list_queries_contains_all_html_queries: ListQueries#test_list_queries_contains_all_html_queries().
  TestGetAvailableHTMLQueries.test_get_available_html_queries_matches_html_queries: GetAvailableHTMLQueries#test_get_available_html_queries_matches_html_queries().
  TestQueryConsistency.test_all_queries_count: QueryConsistency#test_all_queries_count().
  TestQueryConsistency.test_descriptions_match_queries: QueryConsistency#test_descriptions_match_queries().
  TestHTMLQueries.test_html_queries_dict_exists: HTMLQueries#test_html_queries_dict_exists().
  TestHTMLQueries.test_html_query_descriptions_dict_exists: HTMLQueries#test_html_query_descriptions_dict_exists().
  TestHTMLQueries.test_all_queries_dict_exists: HTMLQueries#test_all_queries_dict_exists().
  TestHTMLQueries.test_all_queries_have_query_string: HTMLQueries#test_all_queries_have_query_string().
  TestHTMLQueries.test_basic_element_queries: HTMLQueries#test_basic_element_queries().
  TestHTMLQueries.test_attribute_queries: HTMLQueries#test_attribute_queries().
  TestHTMLQueries.test_text_queries: HTMLQueries#test_text_queries().
  TestHTMLQueries.test_comment_queries: HTMLQueries#test_comment_queries().
  TestHTMLQueries.test_document_structure_queries: HTMLQueries#test_document_structure_queries().
  TestHTMLQueries.test_semantic_element_queries: HTMLQueries#test_semantic_element_queries().
  TestHTMLQueries.test_structure_element_queries: HTMLQueries#test_structure_element_queries().
  TestHTMLQueries.test_form_element_queries: HTMLQueries#test_form_element_queries().
  TestHTMLQueries.test_media_element_queries: HTMLQueries#test_media_element_queries().
  TestHTMLQueries.test_meta_element_queries: HTMLQueries#test_meta_element_queries().
  TestHTMLQueries.test_script_and_style_queries: HTMLQueries#test_script_and_style_queries().
  TestHTMLQueries.test_name_extraction_queries: HTMLQueries#test_name_extraction_queries().
  TestHTMLQueries.test_void_element_query: HTMLQueries#test_void_element_query().
  TestGetHTMLQuery.test_get_html_query_valid: GetHTMLQuery#test_get_html_query_valid().
  TestGetHTMLQuery.test_get_html_query_invalid: GetHTMLQuery#test_get_html_query_invalid().
  TestGetHTMLQuery.test_get_html_query_error_message: GetHTMLQuery#test_get_html_query_error_message().
  TestGetHTMLQueryDescription.test_get_html_query_description_valid: GetHTMLQueryDescription#test_get_html_query_description_valid().
  TestGetHTMLQueryDescription.test_get_html_query_description_invalid: GetHTMLQueryDescription#test_get_html_query_description_invalid().
  TestGetQuery.test_get_query_valid: GetQuery#test_get_query_valid().
  TestGetQuery.test_get_query_invalid: GetQuery#test_get_query_invalid().
  TestGetQuery.test_get_query_error_message: GetQuery#test_get_query_error_message().
  TestGetAllQueries.test_get_all_queries_returns_dict: GetAllQueries#test_get_all_queries_returns_dict().
  TestGetAllQueries.test_get_all_queries_structure: GetAllQueries#test_get_all_queries_structure().
  TestGetAllQueries.test_get_all_queries_contains_legacy_queries: GetAllQueries#test_get_all_queries_contains_legacy_queries().
  TestListQueries.test_list_queries_returns_list: ListQueries#test_list_queries_returns_list().
  TestListQueries.test_list_queries_no_duplicates: ListQueries#test_list_queries_no_duplicates().
  TestGetAvailableHTMLQueries.test_get_available_html_queries_returns_list: GetAvailableHTMLQueries#test_get_available_html_queries_returns_list().
  TestALLQueriesIntegration.test_all_queries_format: ALLQueriesIntegration#test_all_queries_format().
  TestALLQueriesIntegration.test_all_queries_query_strings_valid: ALLQueriesIntegration#test_all_queries_query_strings_valid().
  TestALLQueriesIntegration.test_all_queries_descriptions_valid: ALLQueriesIntegration#test_all_queries_descriptions_valid().
  TestLegacyQueries.test_legacy_queries_in_all_queries: LegacyQueries#test_legacy_queries_in_all_queries().
  TestLegacyQueries.test_legacy_elements_query: LegacyQueries#test_legacy_elements_query().
  TestLegacyQueries.test_legacy_attributes_query: LegacyQueries#test_legacy_attributes_query().
  TestLegacyQueries.test_legacy_comments_query: LegacyQueries#test_legacy_comments_query().
  TestLegacyQueries.test_legacy_text_content_query: LegacyQueries#test_legacy_text_content_query().
  TestQueryConsistency.test_html_queries_count: QueryConsistency#test_html_queries_count().
  TestEdgeCases.test_empty_query_name: EdgeCases#test_empty_query_name().
  TestEdgeCases.test_none_query_name: EdgeCases#test_none_query_name().
  TestEdgeCases.test_query_strings_are_tree_sitter_compatible: EdgeCases#test_query_strings_are_tree_sitter_compatible().
  TestEdgeCases.test_query_descriptions_not_empty: EdgeCases#test_query_descriptions_not_empty().
  TestSpecificQueries.test_element_query_pattern: SpecificQueries#test_element_query_pattern().
  TestSpecificQueries.test_attribute_query_pattern: SpecificQueries#test_attribute_query_pattern().
  TestSpecificQueries.test_class_attribute_query_pattern: SpecificQueries#test_class_attribute_query_pattern().
  TestSpecificQueries.test_id_attribute_query_pattern: SpecificQueries#test_id_attribute_query_pattern().
  TestSpecificQueries.test_heading_query_pattern: SpecificQueries#test_heading_query_pattern().
  TestSpecificQueries.test_void_element_query_pattern: SpecificQueries#test_void_element_query_pattern().
  TestHTMLQueries: HTMLQueries#
  TestGetHTMLQuery: GetHTMLQuery#
  TestGetHTMLQueryDescription: GetHTMLQueryDescription#
  TestGetQuery: GetQuery#
  TestGetAllQueries: GetAllQueries#
  TestListQueries: ListQueries#
  TestGetAvailableHTMLQueries: GetAvailableHTMLQueries#
  TestALLQueriesIntegration: ALLQueriesIntegration#
  TestLegacyQueries: LegacyQueries#
  TestQueryConsistency: QueryConsistency#
  TestEdgeCases: EdgeCases#
  TestSpecificQueries: SpecificQueries#
---
# Module: [`tests/unit/languages/test_queries_html_comprehensive.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_html_comprehensive.py)

## Classes
### `TestALLQueriesIntegration`
- def: [`tests/unit/languages/test_queries_html_comprehensive.py:298`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_html_comprehensive.py#L298)
- doc: Test ALL_QUERIES integration
- signature: `class TestALLQueriesIntegration:`
- members:
  - `test_all_queries_descriptions_valid(self)` — [`L314`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_html_comprehensive.py#L314) — Test all descriptions are valid
  - `test_all_queries_format(self)` — [`L301`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_html_comprehensive.py#L301) — Test ALL_QUERIES has correct format
  - `test_all_queries_query_strings_valid(self)` — [`L308`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_html_comprehensive.py#L308) — Test all query strings are valid
- uses (calls/refs, reference-scoped): [`ALL_QUERIES`](../../../tree_sitter_analyzer/queries/html.md#ALL_QUERIES)

### `TestEdgeCases`
- def: [`tests/unit/languages/test_queries_html_comprehensive.py:374`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_html_comprehensive.py#L374)
- doc: Test edge cases and error handling
- signature: `class TestEdgeCases:`
- members:
  - `test_empty_query_name(self)` — [`L377`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_html_comprehensive.py#L377) — Test empty query name
  - `test_none_query_name(self)` — [`L382`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_html_comprehensive.py#L382) — Test None query name
  - `test_query_descriptions_not_empty(self)` — [`L393`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_html_comprehensive.py#L393) — Test that no query description is empty
  - `test_query_strings_are_tree_sitter_compatible(self)` — [`L387`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_html_comprehensive.py#L387) — Test that query strings appear to be valid Tree-sitter syntax
- uses (calls/refs, reference-scoped): [`HTML_QUERIES`](../../../tree_sitter_analyzer/queries/html.md#HTML_QUERIES.HTML_QUERIES), [`get_html_query`](../../../tree_sitter_analyzer/queries/html.md#get_html_query), [`HTML_QUERY_DESCRIPTIONS`](../../../tree_sitter_analyzer/queries/html.md#HTML_QUERY_DESCRIPTIONS.HTML_QUERY_DESCRIPTIONS)

### `TestGetAllQueries`
- def: [`tests/unit/languages/test_queries_html_comprehensive.py:228`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_html_comprehensive.py#L228)
- doc: Test get_all_queries function
- signature: `class TestGetAllQueries:`
- members:
  - `test_get_all_queries_contains_all_html_queries(self)` — [`L247`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_html_comprehensive.py#L247) — Test that all HTML_QUERIES are in the result
  - `test_get_all_queries_contains_legacy_queries(self)` — [`L253`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_html_comprehensive.py#L253) — Test that legacy queries are included
  - `test_get_all_queries_returns_dict(self)` — [`L231`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_html_comprehensive.py#L231) — Test get_all_queries returns a dictionary
  - `test_get_all_queries_structure(self)` — [`L237`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_html_comprehensive.py#L237) — Test structure of returned queries
- uses (calls/refs, reference-scoped): [`HTML_QUERIES`](../../../tree_sitter_analyzer/queries/html.md#HTML_QUERIES.HTML_QUERIES), [`get_all_queries`](../../../tree_sitter_analyzer/queries/html.md#get_all_queries)

### `TestGetAvailableHTMLQueries`
- def: [`tests/unit/languages/test_queries_html_comprehensive.py:283`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_html_comprehensive.py#L283)
- doc: Test get_available_html_queries function
- signature: `class TestGetAvailableHTMLQueries:`
- members:
  - `test_get_available_html_queries_matches_html_queries(self)` — [`L292`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_html_comprehensive.py#L292) — Test that available queries match HTML_QUERIES keys
  - `test_get_available_html_queries_returns_list(self)` — [`L286`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_html_comprehensive.py#L286) — Test get_available_html_queries returns a list
- uses (calls/refs, reference-scoped): [`HTML_QUERIES`](../../../tree_sitter_analyzer/queries/html.md#HTML_QUERIES.HTML_QUERIES), [`get_available_html_queries`](../../../tree_sitter_analyzer/queries/html.md#get_available_html_queries)

### `TestGetHTMLQuery`
- def: [`tests/unit/languages/test_queries_html_comprehensive.py:159`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_html_comprehensive.py#L159)
- doc: Test get_html_query function
- signature: `class TestGetHTMLQuery:`
- members:
  - `test_get_html_query_all_defined_queries(self)` — [`L168`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_html_comprehensive.py#L168) — Test getting all defined queries
  - `test_get_html_query_error_message(self)` — [`L179`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_html_comprehensive.py#L179) — Test error message contains available queries
  - `test_get_html_query_invalid(self)` — [`L174`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_html_comprehensive.py#L174) — Test getting an invalid query raises ValueError
  - `test_get_html_query_valid(self)` — [`L162`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_html_comprehensive.py#L162) — Test getting a valid HTML query
- uses (calls/refs, reference-scoped): [`HTML_QUERIES`](../../../tree_sitter_analyzer/queries/html.md#HTML_QUERIES.HTML_QUERIES), [`get_html_query`](../../../tree_sitter_analyzer/queries/html.md#get_html_query)

### `TestGetHTMLQueryDescription`
- def: [`tests/unit/languages/test_queries_html_comprehensive.py:186`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_html_comprehensive.py#L186)
- doc: Test get_html_query_description function
- signature: `class TestGetHTMLQueryDescription:`
- members:
  - `test_get_html_query_description_all_queries(self)` — [`L195`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_html_comprehensive.py#L195) — Test getting descriptions for all queries
  - `test_get_html_query_description_invalid(self)` — [`L201`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_html_comprehensive.py#L201) — Test getting description for invalid query
  - `test_get_html_query_description_valid(self)` — [`L189`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_html_comprehensive.py#L189) — Test getting a valid query description
- uses (calls/refs, reference-scoped): [`HTML_QUERIES`](../../../tree_sitter_analyzer/queries/html.md#HTML_QUERIES.HTML_QUERIES), [`get_html_query_description`](../../../tree_sitter_analyzer/queries/html.md#get_html_query_description)

### `TestGetQuery`
- def: [`tests/unit/languages/test_queries_html_comprehensive.py:207`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_html_comprehensive.py#L207)
- doc: Test get_query function
- signature: `class TestGetQuery:`
- members:
  - `test_get_query_error_message(self)` — [`L221`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_html_comprehensive.py#L221) — Test error message contains available queries
  - `test_get_query_invalid(self)` — [`L216`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_html_comprehensive.py#L216) — Test getting invalid query raises ValueError
  - `test_get_query_valid(self)` — [`L210`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_html_comprehensive.py#L210) — Test getting a query using get_query
- uses (calls/refs, reference-scoped): [`get_query`](../../../tree_sitter_analyzer/queries/html.md#get_query)

### `TestHTMLQueries`
- def: [`tests/unit/languages/test_queries_html_comprehensive.py:24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_html_comprehensive.py#L24)
- doc: Test HTML query definitions
- signature: `class TestHTMLQueries:`
- members:
  - `test_all_queries_dict_exists(self)` — [`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_html_comprehensive.py#L37) — Test that ALL_QUERIES dictionary exists
  - `test_all_queries_have_descriptions(self)` — [`L42`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_html_comprehensive.py#L42) — Test that all queries in HTML_QUERIES have descriptions
  - `test_all_queries_have_query_string(self)` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_html_comprehensive.py#L49) — Test that all queries have non-empty query strings
  - `test_attribute_queries(self)` — [`L62`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_html_comprehensive.py#L62) — Test attribute-related queries exist
  - `test_basic_element_queries(self)` — [`L55`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_html_comprehensive.py#L55) — Test basic element queries exist
  - `test_comment_queries(self)` — [`L77`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_html_comprehensive.py#L77) — Test comment queries exist
  - `test_document_structure_queries(self)` — [`L81`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_html_comprehensive.py#L81) — Test document structure queries exist
  - `test_form_element_queries(self)` — [`L113`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_html_comprehensive.py#L113) — Test form element queries exist
  - `test_html_queries_dict_exists(self)` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_html_comprehensive.py#L27) — Test that HTML_QUERIES dictionary exists
  - `test_html_query_descriptions_dict_exists(self)` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_html_comprehensive.py#L32) — Test that HTML_QUERY_DESCRIPTIONS dictionary exists
  - `test_media_element_queries(self)` — [`L125`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_html_comprehensive.py#L125) — Test media element queries exist
  - `test_meta_element_queries(self)` — [`L134`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_html_comprehensive.py#L134) — Test meta element queries exist
  - `test_name_extraction_queries(self)` — [`L149`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_html_comprehensive.py#L149) — Test name extraction queries exist
  - `test_script_and_style_queries(self)` — [`L144`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_html_comprehensive.py#L144) — Test script and style element queries exist
  - `test_semantic_element_queries(self)` — [`L86`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_html_comprehensive.py#L86) — Test semantic element queries exist
  - `test_structure_element_queries(self)` — [`L98`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_html_comprehensive.py#L98) — Test structure element queries exist
  - `test_text_queries(self)` — [`L72`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_html_comprehensive.py#L72) — Test text-related queries exist
  - `test_void_element_query(self)` — [`L154`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_html_comprehensive.py#L154) — Test void element query exists
- uses (calls/refs, reference-scoped): [`HTML_QUERIES`](../../../tree_sitter_analyzer/queries/html.md#HTML_QUERIES.HTML_QUERIES), [`ALL_QUERIES`](../../../tree_sitter_analyzer/queries/html.md#ALL_QUERIES), [`HTML_QUERY_DESCRIPTIONS`](../../../tree_sitter_analyzer/queries/html.md#HTML_QUERY_DESCRIPTIONS.HTML_QUERY_DESCRIPTIONS)

### `TestLegacyQueries`
- def: [`tests/unit/languages/test_queries_html_comprehensive.py:321`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_html_comprehensive.py#L321)
- doc: Test legacy query definitions
- signature: `class TestLegacyQueries:`
- members:
  - `test_legacy_attributes_query(self)` — [`L337`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_html_comprehensive.py#L337) — Test legacy attributes query
  - `test_legacy_comments_query(self)` — [`L343`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_html_comprehensive.py#L343) — Test legacy comments query
  - `test_legacy_elements_query(self)` — [`L331`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_html_comprehensive.py#L331) — Test legacy elements query
  - `test_legacy_queries_in_all_queries(self)` — [`L324`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_html_comprehensive.py#L324) — Test that legacy queries are available in ALL_QUERIES
  - `test_legacy_text_content_query(self)` — [`L349`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_html_comprehensive.py#L349) — Test legacy text_content query
- uses (calls/refs, reference-scoped): [`ALL_QUERIES`](../../../tree_sitter_analyzer/queries/html.md#ALL_QUERIES)

### `TestListQueries`
- def: [`tests/unit/languages/test_queries_html_comprehensive.py:262`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_html_comprehensive.py#L262)
- doc: Test list_queries function
- signature: `class TestListQueries:`
- members:
  - `test_list_queries_contains_all_html_queries(self)` — [`L271`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_html_comprehensive.py#L271) — Test that all HTML queries are in the list
  - `test_list_queries_no_duplicates(self)` — [`L277`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_html_comprehensive.py#L277) — Test that there are no duplicates in the query list
  - `test_list_queries_returns_list(self)` — [`L265`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_html_comprehensive.py#L265) — Test list_queries returns a list
- uses (calls/refs, reference-scoped): [`HTML_QUERIES`](../../../tree_sitter_analyzer/queries/html.md#HTML_QUERIES.HTML_QUERIES), [`list_queries`](../../../tree_sitter_analyzer/queries/html.md#list_queries)

### `TestQueryConsistency`
- def: [`tests/unit/languages/test_queries_html_comprehensive.py:356`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_html_comprehensive.py#L356)
- doc: Test consistency between different query dictionaries
- signature: `class TestQueryConsistency:`
- members:
  - `test_all_queries_count(self)` — [`L363`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_html_comprehensive.py#L363) — Test ALL_QUERIES includes all HTML queries plus legacy
  - `test_descriptions_match_queries(self)` — [`L368`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_html_comprehensive.py#L368) — Test that every query in HTML_QUERIES has a description
  - `test_html_queries_count(self)` — [`L359`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_html_comprehensive.py#L359) — Test that we have a substantial number of queries
- uses (calls/refs, reference-scoped): [`HTML_QUERIES`](../../../tree_sitter_analyzer/queries/html.md#HTML_QUERIES.HTML_QUERIES), [`ALL_QUERIES`](../../../tree_sitter_analyzer/queries/html.md#ALL_QUERIES), [`HTML_QUERY_DESCRIPTIONS`](../../../tree_sitter_analyzer/queries/html.md#HTML_QUERY_DESCRIPTIONS.HTML_QUERY_DESCRIPTIONS)

### `TestSpecificQueries`
- def: [`tests/unit/languages/test_queries_html_comprehensive.py:400`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_html_comprehensive.py#L400)
- doc: Test specific query patterns
- signature: `class TestSpecificQueries:`
- members:
  - `test_attribute_query_pattern(self)` — [`L409`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_html_comprehensive.py#L409) — Test attribute query has expected pattern
  - `test_class_attribute_query_pattern(self)` — [`L415`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_html_comprehensive.py#L415) — Test class attribute query uses regex matching
  - `test_element_query_pattern(self)` — [`L403`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_html_comprehensive.py#L403) — Test element query has expected pattern
  - `test_heading_query_pattern(self)` — [`L427`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_html_comprehensive.py#L427) — Test heading query matches h1-h6
  - `test_id_attribute_query_pattern(self)` — [`L421`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_html_comprehensive.py#L421) — Test id attribute query uses regex matching
  - `test_void_element_query_pattern(self)` — [`L432`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_html_comprehensive.py#L432) — Test void element query matches expected elements
- uses (calls/refs, reference-scoped): [`get_html_query`](../../../tree_sitter_analyzer/queries/html.md#get_html_query)

