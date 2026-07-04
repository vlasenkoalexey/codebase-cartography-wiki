---
title: 'Module: tests/unit/languages/test_queries_css_comprehensive.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_queries_css_comprehensive.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_queries_css_comprehensive`/Test
symbols:
  TestCSSQueries.test_all_queries_have_descriptions: CSSQueries#test_all_queries_have_descriptions().
  TestGetCSSQuery.test_get_css_query_all_defined_queries: GetCSSQuery#test_get_css_query_all_defined_queries().
  TestGetCSSQueryDescription.test_get_css_query_description_all_queries: GetCSSQueryDescription#test_get_css_query_description_all_queries().
  TestGetAllQueries.test_get_all_queries_contains_all_css_queries: GetAllQueries#test_get_all_queries_contains_all_css_queries().
  TestListQueries.test_list_queries_contains_all_css_queries: ListQueries#test_list_queries_contains_all_css_queries().
  TestGetAvailableCSSQueries.test_get_available_css_queries_matches_css_queries: GetAvailableCSSQueries#test_get_available_css_queries_matches_css_queries().
  TestQueryConsistency.test_all_queries_count: QueryConsistency#test_all_queries_count().
  TestQueryConsistency.test_descriptions_match_queries: QueryConsistency#test_descriptions_match_queries().
  TestCSSQueries.test_css_queries_dict_exists: CSSQueries#test_css_queries_dict_exists().
  TestCSSQueries.test_css_query_descriptions_dict_exists: CSSQueries#test_css_query_descriptions_dict_exists().
  TestCSSQueries.test_all_queries_dict_exists: CSSQueries#test_all_queries_dict_exists().
  TestCSSQueries.test_all_queries_have_query_string: CSSQueries#test_all_queries_have_query_string().
  TestCSSQueries.test_basic_rule_queries: CSSQueries#test_basic_rule_queries().
  TestCSSQueries.test_selector_queries: CSSQueries#test_selector_queries().
  TestCSSQueries.test_at_rule_queries: CSSQueries#test_at_rule_queries().
  TestCSSQueries.test_media_query_queries: CSSQueries#test_media_query_queries().
  TestCSSQueries.test_value_queries: CSSQueries#test_value_queries().
  TestCSSQueries.test_css_function_queries: CSSQueries#test_css_function_queries().
  TestCSSQueries.test_unit_queries: CSSQueries#test_unit_queries().
  TestCSSQueries.test_layout_property_queries: CSSQueries#test_layout_property_queries().
  TestCSSQueries.test_box_model_queries: CSSQueries#test_box_model_queries().
  TestCSSQueries.test_typography_queries: CSSQueries#test_typography_queries().
  TestCSSQueries.test_background_queries: CSSQueries#test_background_queries().
  TestCSSQueries.test_flexbox_queries: CSSQueries#test_flexbox_queries().
  TestCSSQueries.test_grid_queries: CSSQueries#test_grid_queries().
  TestCSSQueries.test_animation_queries: CSSQueries#test_animation_queries().
  TestCSSQueries.test_comment_queries: CSSQueries#test_comment_queries().
  TestCSSQueries.test_custom_property_queries: CSSQueries#test_custom_property_queries().
  TestCSSQueries.test_important_queries: CSSQueries#test_important_queries().
  TestCSSQueries.test_keyframe_queries: CSSQueries#test_keyframe_queries().
  TestCSSQueries.test_name_extraction_queries: CSSQueries#test_name_extraction_queries().
  TestGetCSSQuery.test_get_css_query_valid: GetCSSQuery#test_get_css_query_valid().
  TestGetCSSQuery.test_get_css_query_invalid: GetCSSQuery#test_get_css_query_invalid().
  TestGetCSSQuery.test_get_css_query_error_message: GetCSSQuery#test_get_css_query_error_message().
  TestGetCSSQueryDescription.test_get_css_query_description_valid: GetCSSQueryDescription#test_get_css_query_description_valid().
  TestGetCSSQueryDescription.test_get_css_query_description_invalid: GetCSSQueryDescription#test_get_css_query_description_invalid().
  TestGetQuery.test_get_query_valid: GetQuery#test_get_query_valid().
  TestGetQuery.test_get_query_invalid: GetQuery#test_get_query_invalid().
  TestGetQuery.test_get_query_error_message: GetQuery#test_get_query_error_message().
  TestGetAllQueries.test_get_all_queries_returns_dict: GetAllQueries#test_get_all_queries_returns_dict().
  TestGetAllQueries.test_get_all_queries_structure: GetAllQueries#test_get_all_queries_structure().
  TestGetAllQueries.test_get_all_queries_contains_legacy_queries: GetAllQueries#test_get_all_queries_contains_legacy_queries().
  TestListQueries.test_list_queries_returns_list: ListQueries#test_list_queries_returns_list().
  TestListQueries.test_list_queries_no_duplicates: ListQueries#test_list_queries_no_duplicates().
  TestGetAvailableCSSQueries.test_get_available_css_queries_returns_list: GetAvailableCSSQueries#test_get_available_css_queries_returns_list().
  TestALLQueriesIntegration.test_all_queries_format: ALLQueriesIntegration#test_all_queries_format().
  TestALLQueriesIntegration.test_all_queries_query_strings_valid: ALLQueriesIntegration#test_all_queries_query_strings_valid().
  TestALLQueriesIntegration.test_all_queries_descriptions_valid: ALLQueriesIntegration#test_all_queries_descriptions_valid().
  TestLegacyQueries.test_legacy_queries_in_all_queries: LegacyQueries#test_legacy_queries_in_all_queries().
  TestLegacyQueries.test_legacy_rules_query: LegacyQueries#test_legacy_rules_query().
  TestLegacyQueries.test_legacy_selectors_query: LegacyQueries#test_legacy_selectors_query().
  TestLegacyQueries.test_legacy_declarations_query: LegacyQueries#test_legacy_declarations_query().
  TestLegacyQueries.test_legacy_comments_query: LegacyQueries#test_legacy_comments_query().
  TestLegacyQueries.test_legacy_at_rules_query: LegacyQueries#test_legacy_at_rules_query().
  TestQueryConsistency.test_css_queries_count: QueryConsistency#test_css_queries_count().
  TestEdgeCases.test_empty_query_name: EdgeCases#test_empty_query_name().
  TestEdgeCases.test_none_query_name: EdgeCases#test_none_query_name().
  TestEdgeCases.test_query_strings_are_tree_sitter_compatible: EdgeCases#test_query_strings_are_tree_sitter_compatible().
  TestEdgeCases.test_query_descriptions_not_empty: EdgeCases#test_query_descriptions_not_empty().
  TestSpecificQueries.test_rule_set_query_pattern: SpecificQueries#test_rule_set_query_pattern().
  TestSpecificQueries.test_declaration_query_pattern: SpecificQueries#test_declaration_query_pattern().
  TestSpecificQueries.test_class_selector_query_pattern: SpecificQueries#test_class_selector_query_pattern().
  TestSpecificQueries.test_id_selector_query_pattern: SpecificQueries#test_id_selector_query_pattern().
  TestSpecificQueries.test_media_statement_query_pattern: SpecificQueries#test_media_statement_query_pattern().
  TestSpecificQueries.test_url_function_query_pattern: SpecificQueries#test_url_function_query_pattern().
  TestSpecificQueries.test_calc_function_query_pattern: SpecificQueries#test_calc_function_query_pattern().
  TestSpecificQueries.test_var_function_query_pattern: SpecificQueries#test_var_function_query_pattern().
  TestSpecificQueries.test_custom_property_query_pattern: SpecificQueries#test_custom_property_query_pattern().
  TestSpecificQueries.test_important_query_pattern: SpecificQueries#test_important_query_pattern().
  TestPropertyQueries.test_display_property_query: PropertyQueries#test_display_property_query().
  TestPropertyQueries.test_position_property_query: PropertyQueries#test_position_property_query().
  TestPropertyQueries.test_flex_property_query: PropertyQueries#test_flex_property_query().
  TestPropertyQueries.test_grid_property_query: PropertyQueries#test_grid_property_query().
  TestPropertyQueries.test_animation_property_query: PropertyQueries#test_animation_property_query().
  TestPropertyQueries.test_transform_property_query: PropertyQueries#test_transform_property_query().
  TestColorFunctionQueries.test_rgb_function_query: ColorFunctionQueries#test_rgb_function_query().
  TestColorFunctionQueries.test_rgba_function_query: ColorFunctionQueries#test_rgba_function_query().
  TestColorFunctionQueries.test_hsl_function_query: ColorFunctionQueries#test_hsl_function_query().
  TestColorFunctionQueries.test_hsla_function_query: ColorFunctionQueries#test_hsla_function_query().
  TestCSSQueries: CSSQueries#
  TestGetCSSQuery: GetCSSQuery#
  TestGetCSSQueryDescription: GetCSSQueryDescription#
  TestGetQuery: GetQuery#
  TestGetAllQueries: GetAllQueries#
  TestListQueries: ListQueries#
  TestGetAvailableCSSQueries: GetAvailableCSSQueries#
  TestALLQueriesIntegration: ALLQueriesIntegration#
  TestLegacyQueries: LegacyQueries#
  TestQueryConsistency: QueryConsistency#
  TestEdgeCases: EdgeCases#
  TestSpecificQueries: SpecificQueries#
  TestPropertyQueries: PropertyQueries#
  TestColorFunctionQueries: ColorFunctionQueries#
---
# Module: [`tests/unit/languages/test_queries_css_comprehensive.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py)

## Classes
### `TestALLQueriesIntegration`
- def: [`tests/unit/languages/test_queries_css_comprehensive.py:339`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L339)
- doc: Test ALL_QUERIES integration
- signature: `class TestALLQueriesIntegration:`
- members:
  - `test_all_queries_descriptions_valid(self)` — [`L355`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L355) — Test all descriptions are valid
  - `test_all_queries_format(self)` — [`L342`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L342) — Test ALL_QUERIES has correct format
  - `test_all_queries_query_strings_valid(self)` — [`L349`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L349) — Test all query strings are valid
- uses (calls/refs, reference-scoped): [`ALL_QUERIES`](../../../tree_sitter_analyzer/queries/css.md#ALL_QUERIES.ALL_QUERIES)

### `TestCSSQueries`
- def: [`tests/unit/languages/test_queries_css_comprehensive.py:24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L24)
- doc: Test CSS query definitions
- signature: `class TestCSSQueries:`
- members:
  - `test_all_queries_dict_exists(self)` — [`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L37) — Test that ALL_QUERIES dictionary exists
  - `test_all_queries_have_descriptions(self)` — [`L42`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L42) — Test that all queries in CSS_QUERIES have descriptions
  - `test_all_queries_have_query_string(self)` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L49) — Test that all queries have non-empty query strings
  - `test_animation_queries(self)` — [`L167`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L167) — Test animation property queries exist
  - `test_at_rule_queries(self)` — [`L80`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L80) — Test at-rule queries exist
  - `test_background_queries(self)` — [`L152`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L152) — Test background property queries exist
  - `test_basic_rule_queries(self)` — [`L55`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L55) — Test basic rule queries exist
  - `test_box_model_queries(self)` — [`L134`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L134) — Test box model property queries exist
  - `test_comment_queries(self)` — [`L173`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L173) — Test comment queries exist
  - `test_css_function_queries(self)` — [`L108`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L108) — Test CSS function queries exist
  - `test_css_queries_dict_exists(self)` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L27) — Test that CSS_QUERIES dictionary exists
  - `test_css_query_descriptions_dict_exists(self)` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L32) — Test that CSS_QUERY_DESCRIPTIONS dictionary exists
  - `test_custom_property_queries(self)` — [`L177`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L177) — Test custom property (CSS variable) queries exist
  - `test_flexbox_queries(self)` — [`L156`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L156) — Test flexbox property queries exist
  - `test_grid_queries(self)` — [`L163`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L163) — Test grid property queries exist
  - `test_important_queries(self)` — [`L181`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L181) — Test !important queries exist
  - `test_keyframe_queries(self)` — [`L185`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L185) — Test keyframe-related queries exist
  - `test_layout_property_queries(self)` — [`L124`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L124) — Test layout property queries exist
  - `test_media_query_queries(self)` — [`L92`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L92) — Test media query-related queries exist
  - `test_name_extraction_queries(self)` — [`L192`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L192) — Test name extraction queries exist
  - `test_selector_queries(self)` — [`L64`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L64) — Test selector-related queries exist
  - `test_typography_queries(self)` — [`L143`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L143) — Test typography property queries exist
  - `test_unit_queries(self)` — [`L118`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L118) — Test unit-related queries exist
  - `test_value_queries(self)` — [`L98`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L98) — Test value-related queries exist
- uses (calls/refs, reference-scoped): [`CSS_QUERIES`](../../../tree_sitter_analyzer/queries/css.md#CSS_QUERIES.CSS_QUERIES), [`ALL_QUERIES`](../../../tree_sitter_analyzer/queries/css.md#ALL_QUERIES.ALL_QUERIES), [`CSS_QUERY_DESCRIPTIONS`](../../../tree_sitter_analyzer/queries/css.md#CSS_QUERY_DESCRIPTIONS.CSS_QUERY_DESCRIPTIONS)

### `TestColorFunctionQueries`
- def: [`tests/unit/languages/test_queries_css_comprehensive.py:553`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L553)
- doc: Test color function queries
- signature: `class TestColorFunctionQueries:`
- members:
  - `test_hsl_function_query(self)` — [`L568`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L568) — Test hsl() function query
  - `test_hsla_function_query(self)` — [`L574`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L574) — Test hsla() function query
  - `test_rgb_function_query(self)` — [`L556`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L556) — Test rgb() function query
  - `test_rgba_function_query(self)` — [`L562`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L562) — Test rgba() function query
- uses (calls/refs, reference-scoped): [`get_css_query`](../../../tree_sitter_analyzer/queries/css.md#get_css_query)

### `TestEdgeCases`
- def: [`tests/unit/languages/test_queries_css_comprehensive.py:422`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L422)
- doc: Test edge cases and error handling
- signature: `class TestEdgeCases:`
- members:
  - `test_empty_query_name(self)` — [`L425`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L425) — Test empty query name
  - `test_none_query_name(self)` — [`L430`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L430) — Test None query name
  - `test_query_descriptions_not_empty(self)` — [`L441`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L441) — Test that no query description is empty
  - `test_query_strings_are_tree_sitter_compatible(self)` — [`L435`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L435) — Test that query strings appear to be valid Tree-sitter syntax
- uses (calls/refs, reference-scoped): [`CSS_QUERIES`](../../../tree_sitter_analyzer/queries/css.md#CSS_QUERIES.CSS_QUERIES), [`get_css_query`](../../../tree_sitter_analyzer/queries/css.md#get_css_query), [`CSS_QUERY_DESCRIPTIONS`](../../../tree_sitter_analyzer/queries/css.md#CSS_QUERY_DESCRIPTIONS.CSS_QUERY_DESCRIPTIONS)

### `TestGetAllQueries`
- def: [`tests/unit/languages/test_queries_css_comprehensive.py:268`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L268)
- doc: Test get_all_queries function
- signature: `class TestGetAllQueries:`
- members:
  - `test_get_all_queries_contains_all_css_queries(self)` — [`L287`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L287) — Test that all CSS_QUERIES are in the result
  - `test_get_all_queries_contains_legacy_queries(self)` — [`L293`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L293) — Test that legacy queries are included
  - `test_get_all_queries_returns_dict(self)` — [`L271`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L271) — Test get_all_queries returns a dictionary
  - `test_get_all_queries_structure(self)` — [`L277`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L277) — Test structure of returned queries
- uses (calls/refs, reference-scoped): [`CSS_QUERIES`](../../../tree_sitter_analyzer/queries/css.md#CSS_QUERIES.CSS_QUERIES), [`get_all_queries`](../../../tree_sitter_analyzer/queries/css.md#get_all_queries)

### `TestGetAvailableCSSQueries`
- def: [`tests/unit/languages/test_queries_css_comprehensive.py:324`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L324)
- doc: Test get_available_css_queries function
- signature: `class TestGetAvailableCSSQueries:`
- members:
  - `test_get_available_css_queries_matches_css_queries(self)` — [`L333`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L333) — Test that available queries match CSS_QUERIES keys
  - `test_get_available_css_queries_returns_list(self)` — [`L327`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L327) — Test get_available_css_queries returns a list
- uses (calls/refs, reference-scoped): [`CSS_QUERIES`](../../../tree_sitter_analyzer/queries/css.md#CSS_QUERIES.CSS_QUERIES), [`get_available_css_queries`](../../../tree_sitter_analyzer/queries/css.md#get_available_css_queries)

### `TestGetCSSQuery`
- def: [`tests/unit/languages/test_queries_css_comprehensive.py:199`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L199)
- doc: Test get_css_query function
- signature: `class TestGetCSSQuery:`
- members:
  - `test_get_css_query_all_defined_queries(self)` — [`L208`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L208) — Test getting all defined queries
  - `test_get_css_query_error_message(self)` — [`L219`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L219) — Test error message contains available queries
  - `test_get_css_query_invalid(self)` — [`L214`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L214) — Test getting an invalid query raises ValueError
  - `test_get_css_query_valid(self)` — [`L202`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L202) — Test getting a valid CSS query
- uses (calls/refs, reference-scoped): [`CSS_QUERIES`](../../../tree_sitter_analyzer/queries/css.md#CSS_QUERIES.CSS_QUERIES), [`get_css_query`](../../../tree_sitter_analyzer/queries/css.md#get_css_query)

### `TestGetCSSQueryDescription`
- def: [`tests/unit/languages/test_queries_css_comprehensive.py:226`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L226)
- doc: Test get_css_query_description function
- signature: `class TestGetCSSQueryDescription:`
- members:
  - `test_get_css_query_description_all_queries(self)` — [`L235`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L235) — Test getting descriptions for all queries
  - `test_get_css_query_description_invalid(self)` — [`L241`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L241) — Test getting description for invalid query
  - `test_get_css_query_description_valid(self)` — [`L229`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L229) — Test getting a valid query description
- uses (calls/refs, reference-scoped): [`CSS_QUERIES`](../../../tree_sitter_analyzer/queries/css.md#CSS_QUERIES.CSS_QUERIES), [`get_css_query_description`](../../../tree_sitter_analyzer/queries/css.md#get_css_query_description)

### `TestGetQuery`
- def: [`tests/unit/languages/test_queries_css_comprehensive.py:247`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L247)
- doc: Test get_query function
- signature: `class TestGetQuery:`
- members:
  - `test_get_query_error_message(self)` — [`L261`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L261) — Test error message contains available queries
  - `test_get_query_invalid(self)` — [`L256`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L256) — Test getting invalid query raises ValueError
  - `test_get_query_valid(self)` — [`L250`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L250) — Test getting a query using get_query
- uses (calls/refs, reference-scoped): [`get_query`](../../../tree_sitter_analyzer/queries/css.md#get_query)

### `TestLegacyQueries`
- def: [`tests/unit/languages/test_queries_css_comprehensive.py:362`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L362)
- doc: Test legacy query definitions
- signature: `class TestLegacyQueries:`
- members:
  - `test_legacy_at_rules_query(self)` — [`L397`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L397) — Test legacy at_rules query
  - `test_legacy_comments_query(self)` — [`L391`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L391) — Test legacy comments query
  - `test_legacy_declarations_query(self)` — [`L385`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L385) — Test legacy declarations query
  - `test_legacy_queries_in_all_queries(self)` — [`L365`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L365) — Test that legacy queries are available in ALL_QUERIES
  - `test_legacy_rules_query(self)` — [`L373`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L373) — Test legacy rules query
  - `test_legacy_selectors_query(self)` — [`L379`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L379) — Test legacy selectors query
- uses (calls/refs, reference-scoped): [`ALL_QUERIES`](../../../tree_sitter_analyzer/queries/css.md#ALL_QUERIES.ALL_QUERIES)

### `TestListQueries`
- def: [`tests/unit/languages/test_queries_css_comprehensive.py:303`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L303)
- doc: Test list_queries function
- signature: `class TestListQueries:`
- members:
  - `test_list_queries_contains_all_css_queries(self)` — [`L312`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L312) — Test that all CSS queries are in the list
  - `test_list_queries_no_duplicates(self)` — [`L318`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L318) — Test that there are no duplicates in the query list
  - `test_list_queries_returns_list(self)` — [`L306`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L306) — Test list_queries returns a list
- uses (calls/refs, reference-scoped): [`CSS_QUERIES`](../../../tree_sitter_analyzer/queries/css.md#CSS_QUERIES.CSS_QUERIES), [`list_queries`](../../../tree_sitter_analyzer/queries/css.md#list_queries)

### `TestPropertyQueries`
- def: [`tests/unit/languages/test_queries_css_comprehensive.py:513`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L513)
- doc: Test specific property queries
- signature: `class TestPropertyQueries:`
- members:
  - `test_animation_property_query(self)` — [`L540`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L540) — Test animation property query
  - `test_display_property_query(self)` — [`L516`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L516) — Test display property query
  - `test_flex_property_query(self)` — [`L528`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L528) — Test flex property query
  - `test_grid_property_query(self)` — [`L534`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L534) — Test grid property query
  - `test_position_property_query(self)` — [`L522`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L522) — Test position property query
  - `test_transform_property_query(self)` — [`L546`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L546) — Test transform property query
- uses (calls/refs, reference-scoped): [`get_css_query`](../../../tree_sitter_analyzer/queries/css.md#get_css_query)

### `TestQueryConsistency`
- def: [`tests/unit/languages/test_queries_css_comprehensive.py:404`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L404)
- doc: Test consistency between different query dictionaries
- signature: `class TestQueryConsistency:`
- members:
  - `test_all_queries_count(self)` — [`L411`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L411) — Test ALL_QUERIES includes all CSS queries plus legacy
  - `test_css_queries_count(self)` — [`L407`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L407) — Test that we have a substantial number of queries
  - `test_descriptions_match_queries(self)` — [`L416`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L416) — Test that every query in CSS_QUERIES has a description
- uses (calls/refs, reference-scoped): [`CSS_QUERIES`](../../../tree_sitter_analyzer/queries/css.md#CSS_QUERIES.CSS_QUERIES), [`ALL_QUERIES`](../../../tree_sitter_analyzer/queries/css.md#ALL_QUERIES.ALL_QUERIES), [`CSS_QUERY_DESCRIPTIONS`](../../../tree_sitter_analyzer/queries/css.md#CSS_QUERY_DESCRIPTIONS.CSS_QUERY_DESCRIPTIONS)

### `TestSpecificQueries`
- def: [`tests/unit/languages/test_queries_css_comprehensive.py:448`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L448)
- doc: Test specific query patterns
- signature: `class TestSpecificQueries:`
- members:
  - `test_calc_function_query_pattern(self)` — [`L488`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L488) — Test calc() function query
  - `test_class_selector_query_pattern(self)` — [`L464`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L464) — Test class selector query
  - `test_custom_property_query_pattern(self)` — [`L500`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L500) — Test custom property (CSS variable) query
  - `test_declaration_query_pattern(self)` — [`L457`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L457) — Test declaration query has expected pattern
  - `test_id_selector_query_pattern(self)` — [`L470`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L470) — Test id selector query
  - `test_important_query_pattern(self)` — [`L506`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L506) — Test !important query
  - `test_media_statement_query_pattern(self)` — [`L476`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L476) — Test media statement query
  - `test_rule_set_query_pattern(self)` — [`L451`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L451) — Test rule_set query has expected pattern
  - `test_url_function_query_pattern(self)` — [`L482`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L482) — Test url() function query
  - `test_var_function_query_pattern(self)` — [`L494`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_queries_css_comprehensive.py#L494) — Test var() function query
- uses (calls/refs, reference-scoped): [`get_css_query`](../../../tree_sitter_analyzer/queries/css.md#get_css_query)

