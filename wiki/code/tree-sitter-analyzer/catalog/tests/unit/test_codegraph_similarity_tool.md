---
title: 'Module: tests/unit/test_codegraph_similarity_tool.py'
type: catalog
provenance: extracted
module: tests/unit/test_codegraph_similarity_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_codegraph_similarity_tool`/
symbols:
  TestFacadeRoutesSimilarityParams801.test_max_groups_via_facade: TestFacadeRoutesSimilarityParams801#test_max_groups_via_facade().
  TestPathFilter.test_path_filter_limits_similarity_scope: TestPathFilter#test_path_filter_limits_similarity_scope().
  TestFacadeIncludeBodiesSurvivesRouting.test_include_bodies_survives_facade_routing: TestFacadeIncludeBodiesSurvivesRouting#test_include_bodies_survives_facade_routing().
  TestFacadeIncludeBodiesSurvivesRouting.test_facade_default_no_bodies: TestFacadeIncludeBodiesSurvivesRouting#test_facade_default_no_bodies().
  tool_with_large_group: tool_with_large_group().
  TestFacadeSchemaExposesSimilarityParams801.test_viz_facade_schema_exposes_max_groups: TestFacadeSchemaExposesSimilarityParams801#test_viz_facade_schema_exposes_max_groups().
  TestFacadeSchemaExposesSimilarityParams801.test_viz_facade_schema_exposes_min_lines: TestFacadeSchemaExposesSimilarityParams801#test_viz_facade_schema_exposes_min_lines().
  TestFacadeSchemaExposesSimilarityParams801.test_viz_facade_schema_exposes_min_group_size: TestFacadeSchemaExposesSimilarityParams801#test_viz_facade_schema_exposes_min_group_size().
  TestFacadeSchemaExposesSimilarityParams801.test_viz_facade_schema_exposes_path_filter: TestFacadeSchemaExposesSimilarityParams801#test_viz_facade_schema_exposes_path_filter().
  TestFacadeRoutesSimilarityParams801.test_path_filter_via_facade: TestFacadeRoutesSimilarityParams801#test_path_filter_via_facade().
  tool: tool().
  tool_with_root: tool_with_root().
  tool_with_clones: tool_with_clones().
  _large_group_fixture_body: _large_group_fixture_body().
  TestToolDefinition: TestToolDefinition#
  TestToolDefinition.test_tool_name: TestToolDefinition#test_tool_name().
  TestToolDefinition.test_description_mentions_no_other: TestToolDefinition#test_description_mentions_no_other().
  TestToolDefinition.test_schema_mode_enum: TestToolDefinition#test_schema_mode_enum().
  TestToolDefinition.test_schema_output_format_default_toon: TestToolDefinition#test_schema_output_format_default_toon().
  TestExecute: TestExecute#
  TestExecute.test_runs_on_project: TestExecute#test_runs_on_project().
  TestExecute.test_toon_format_default: TestExecute#test_toon_format_default().
  TestIncludeBodiesSchema: TestIncludeBodiesSchema#
  TestIncludeBodiesSchema.test_include_bodies_in_schema: TestIncludeBodiesSchema#test_include_bodies_in_schema().
  TestIncludeBodiesSchema.test_include_bodies_default_false: TestIncludeBodiesSchema#test_include_bodies_default_false().
  TestIncludeBodiesSchema.test_schema_description_mentions_summary: TestIncludeBodiesSchema#test_schema_description_mentions_summary().
  TestIncludeBodiesSchema.test_path_filter_in_schema: TestIncludeBodiesSchema#test_path_filter_in_schema().
  TestSummaryDefaultNoBodies: TestSummaryDefaultNoBodies#
  TestSummaryDefaultNoBodies.test_default_no_snippet_in_functions: TestSummaryDefaultNoBodies#test_default_no_snippet_in_functions().
  TestPathFilter: TestPathFilter#
  TestPathFilter.test_include_bodies_true_has_snippet: TestPathFilter#test_include_bodies_true_has_snippet().
  TestPathFilter.test_default_response_smaller_than_with_bodies: TestPathFilter#test_default_response_smaller_than_with_bodies().
  TestFacadeIncludeBodiesSurvivesRouting: TestFacadeIncludeBodiesSurvivesRouting#
  TestBoundingParams801: TestBoundingParams801#
  TestBoundingParams801.test_max_groups_limits_output: TestBoundingParams801#test_max_groups_limits_output().
  TestBoundingParams801.test_max_groups_string_coercion: TestBoundingParams801#test_max_groups_string_coercion().
  TestBoundingParams801.test_min_lines_string_coercion: TestBoundingParams801#test_min_lines_string_coercion().
  TestBoundingParams801.test_min_group_size_string_coercion: TestBoundingParams801#test_min_group_size_string_coercion().
  TestBoundingParams801.test_compact_large_group_has_no_functions_key: TestBoundingParams801#test_compact_large_group_has_no_functions_key().
  TestBoundingParams801.test_include_bodies_true_not_capped: TestBoundingParams801#test_include_bodies_true_not_capped().
  TestBoundingParams801.test_no_truncated_flag_in_compact_mode: TestBoundingParams801#test_no_truncated_flag_in_compact_mode().
  TestFacadeSchemaExposesSimilarityParams801: TestFacadeSchemaExposesSimilarityParams801#
  TestFacadeRoutesSimilarityParams801: TestFacadeRoutesSimilarityParams801#
---
# Module: [`tests/unit/test_codegraph_similarity_tool.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_similarity_tool.py)

## Classes
### `TestBoundingParams801`
- def: [`tests/unit/test_codegraph_similarity_tool.py:294`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_similarity_tool.py#L294)
- doc: Issue #801 — max_groups / functions-cap / type coercion.
- signature: `class TestBoundingParams801:`
- members:
  - `test_compact_large_group_has_no_functions_key(self, tool_with_large_group)` — [`L327`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_similarity_tool.py#L327) — Compact mode (include_bodies=False) strips functions[]; exposes sample_files + function_count.
  - `test_include_bodies_true_not_capped(self, tool_with_large_group)` — [`L346`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_similarity_tool.py#L346) — include_bodies=True must NOT cap functions[] — all 15 returned.
  - `test_max_groups_limits_output(self, tool_with_clones)` — [`L297`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_similarity_tool.py#L297) — max_groups=1 must limit the groups list to exactly 1 entry.
  - `test_max_groups_string_coercion(self, tool_with_clones)` — [`L305`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_similarity_tool.py#L305) — max_groups passed as a string (MCP transport) must be coerced to int.
  - `test_min_group_size_string_coercion(self, tool_with_clones)` — [`L320`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_similarity_tool.py#L320) — min_group_size passed as string must not crash — coerced to int.
  - `test_min_lines_string_coercion(self, tool_with_clones)` — [`L313`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_similarity_tool.py#L313) — min_lines passed as string must not crash — coerced to int.
  - `test_no_truncated_flag_in_compact_mode(self, tool_with_clones)` — [`L361`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_similarity_tool.py#L361) — Compact mode never sets 'truncated' — it strips functions[] entirely instead.

### `TestExecute`
- def: [`tests/unit/test_codegraph_similarity_tool.py:70`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_similarity_tool.py#L70)
- signature: `class TestExecute:`
- members:
  - `test_runs_on_project(self, tool_with_root)` — [`L71`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_similarity_tool.py#L71)
  - `test_toon_format_default(self, tool_with_root)` — [`L75`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_similarity_tool.py#L75)

### `TestFacadeIncludeBodiesSurvivesRouting`
- def: [`tests/unit/test_codegraph_similarity_tool.py:197`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_similarity_tool.py#L197)
- doc: include_bodies must survive _project_args projection through the viz facade.
- signature: `class TestFacadeIncludeBodiesSurvivesRouting:`
- members:
  - `test_facade_default_no_bodies(self, tmp_path)` — [`L236`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_similarity_tool.py#L236) — via the viz facade: default (no include_bodies) must strip snippets.
  - `test_include_bodies_survives_facade_routing(self, tmp_path)` — [`L200`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_similarity_tool.py#L200) — via the viz facade: include_bodies=True reaches the inner tool.
- uses (calls/refs, reference-scoped): [`execute`](../../tree_sitter_analyzer/mcp/tools/facade_tool.md#FacadeTool.execute), [`build_viz_facade`](../../tree_sitter_analyzer/mcp/tools/viz_facade.md#build_viz_facade)

### `TestFacadeRoutesSimilarityParams801`
- def: [`tests/unit/test_codegraph_similarity_tool.py:416`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_similarity_tool.py#L416)
- doc: Issue #801 — similarity params must route through the viz facade correctly.
- signature: `class TestFacadeRoutesSimilarityParams801:`
- members:
  - `test_max_groups_via_facade(self, tmp_path)` — [`L419`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_similarity_tool.py#L419) — max_groups=1 passed via viz facade must limit groups to exactly 1.
  - `test_path_filter_via_facade(self, tmp_path)` — [`L431`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_similarity_tool.py#L431) — path_filter passed via viz facade must limit similarity scope.
- uses (calls/refs, reference-scoped): [`execute`](../../tree_sitter_analyzer/mcp/tools/facade_tool.md#FacadeTool.execute), [`build_viz_facade`](../../tree_sitter_analyzer/mcp/tools/viz_facade.md#build_viz_facade)  (1 test-only)

### `TestFacadeSchemaExposesSimilarityParams801`
- def: [`tests/unit/test_codegraph_similarity_tool.py:371`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_similarity_tool.py#L371)
- doc: Issue #801 — similarity bounding params must be discoverable in the viz facade schema.
- signature: `class TestFacadeSchemaExposesSimilarityParams801:`
- members:
  - `test_viz_facade_schema_exposes_max_groups(self)` — [`L374`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_similarity_tool.py#L374) — max_groups must appear in the viz facade's public schema.
  - `test_viz_facade_schema_exposes_min_group_size(self)` — [`L394`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_similarity_tool.py#L394) — min_group_size must appear in the viz facade's public schema.
  - `test_viz_facade_schema_exposes_min_lines(self)` — [`L384`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_similarity_tool.py#L384) — min_lines must appear in the viz facade's public schema.
  - `test_viz_facade_schema_exposes_path_filter(self)` — [`L404`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_similarity_tool.py#L404) — path_filter must appear in the viz facade's public schema.
- uses (calls/refs, reference-scoped): [`build_viz_facade`](../../tree_sitter_analyzer/mcp/tools/viz_facade.md#build_viz_facade), [`get_tool_schema`](../../tree_sitter_analyzer/mcp/tools/facade_tool.md#FacadeTool.get_tool_schema)

### `TestIncludeBodiesSchema`
- def: [`tests/unit/test_codegraph_similarity_tool.py:81`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_similarity_tool.py#L81)
- doc: include_bodies param is declared in the inner tool's schema.
- signature: `class TestIncludeBodiesSchema:`
- members:
  - `test_include_bodies_default_false(self, tool)` — [`L91`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_similarity_tool.py#L91)
  - `test_include_bodies_in_schema(self, tool)` — [`L84`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_similarity_tool.py#L84)
  - `test_path_filter_in_schema(self, tool)` — [`L102`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_similarity_tool.py#L102)
  - `test_schema_description_mentions_summary(self, tool)` — [`L95`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_similarity_tool.py#L95) — Description must state that default is summary / bodies require include_bodies.

### `TestPathFilter`
- def: [`tests/unit/test_codegraph_similarity_tool.py:127`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_similarity_tool.py#L127)
- signature: `class TestPathFilter:`
- members:
  - `test_default_response_smaller_than_with_bodies(self, tool_with_clones)` — [`L181`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_similarity_tool.py#L181) — Summary response (no bodies) must produce fewer bytes than include_bodies=True.
  - `test_include_bodies_true_has_snippet(self, tool_with_clones)` — [`L167`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_similarity_tool.py#L167) — include_bodies=True: function entries must have 'snippet' key.
  - `test_path_filter_limits_similarity_scope(self, tmp_path)` — [`L128`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_similarity_tool.py#L128)
- uses (calls/refs, reference-scoped): [`execute`](../../tree_sitter_analyzer/mcp/tools/code_similarity_tool.md#CodeGraphSimilarityTool.execute), [`CodeGraphSimilarityTool`](../../tree_sitter_analyzer/mcp/tools/code_similarity_tool.md#CodeGraphSimilarityTool)

### `TestSummaryDefaultNoBodies`
- def: [`tests/unit/test_codegraph_similarity_tool.py:109`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_similarity_tool.py#L109)
- doc: Default response must NOT include code snippets in function entries.
- signature: `class TestSummaryDefaultNoBodies:`
- members:
  - `test_default_no_snippet_in_functions(self, tool_with_clones)` — [`L112`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_similarity_tool.py#L112) — Default: function entries must not have 'snippet' key; groups must be non-empty.

### `TestToolDefinition`
- def: [`tests/unit/test_codegraph_similarity_tool.py:25`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_similarity_tool.py#L25)
- signature: `class TestToolDefinition:`
- members:
  - `test_description_mentions_no_other(self, tool)` — [`L29`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_similarity_tool.py#L29)
  - `test_schema_mode_enum(self, tool)` — [`L33`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_similarity_tool.py#L33)
  - `test_schema_output_format_default_toon(self, tool)` — [`L38`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_similarity_tool.py#L38)
  - `test_tool_name(self, tool)` — [`L26`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_similarity_tool.py#L26)

## Functions
- `_large_group_fixture_body()` — [`L271`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_similarity_tool.py#L271) — Generate 15 structurally identical 5-line functions for cap tests.
- `tool()` — [`L13`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_similarity_tool.py#L13)
- `tool_with_clones(tmp_path)` — [`L45`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_similarity_tool.py#L45) — Project with two structurally identical 5-line functions (guaranteed clone group).
- `tool_with_large_group(tmp_path)` — [`L287`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_similarity_tool.py#L287) — Project with 15 structurally identical functions in one file.
- `tool_with_root(tmp_path)` — [`L18`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_similarity_tool.py#L18)

