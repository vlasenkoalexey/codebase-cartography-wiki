---
title: 'Module: tests/unit/test_codegraph_navigate_tool.py'
type: catalog
provenance: extracted
module: tests/unit/test_codegraph_navigate_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_codegraph_navigate_tool`/
symbols:
  TestDefinitionBodyInlining.indexed: TestDefinitionBodyInlining#indexed().
  TestTransitiveHelpers.test_transitive_callers_bounded: TestTransitiveHelpers#test_transitive_callers_bounded().
  TestTransitiveHelpers.test_transitive_callees_no_cycles: TestTransitiveHelpers#test_transitive_callees_no_cycles().
  TestDefinitionBodyInlining.test_definition_inlines_body: TestDefinitionBodyInlining#test_definition_inlines_body().
  TestDefinitionBodyInlining.test_definition_body_survives_toon: TestDefinitionBodyInlining#test_definition_body_survives_toon().
  tool: tool().
  tool_with_root: tool_with_root().
  TestExecuteHierarchy.test_hierarchy_transitive_depth: TestExecuteHierarchy#test_hierarchy_transitive_depth().
  TestExecuteHierarchy.test_hierarchy_lists_capped_but_counts_full: TestExecuteHierarchy#test_hierarchy_lists_capped_but_counts_full().
  TestExecuteHierarchy.callers_of: TestExecuteHierarchy#callers_of().
  TestTransitiveHelpers.callers_of: TestTransitiveHelpers#callers_of().
  TestTransitiveHelpers.callees_of: TestTransitiveHelpers#callees_of().
  TestToolDefinition: TestToolDefinition#
  TestToolDefinition.test_tool_name: TestToolDefinition#test_tool_name().
  TestToolDefinition.test_schema_requires_symbol: TestToolDefinition#test_schema_requires_symbol().
  TestToolDefinition.test_schema_modes: TestToolDefinition#test_schema_modes().
  TestValidateArguments: TestValidateArguments#
  TestValidateArguments.test_missing_symbol_raises: TestValidateArguments#test_missing_symbol_raises().
  TestValidateArguments.test_valid_symbol: TestValidateArguments#test_valid_symbol().
  TestExecuteDefinition: TestExecuteDefinition#
  TestExecuteDefinition.test_definition_no_cache: TestExecuteDefinition#test_definition_no_cache().
  TestExecuteDefinition.test_definition_with_cache: TestExecuteDefinition#test_definition_with_cache().
  TestExecuteHierarchy: TestExecuteHierarchy#
  TestExecuteHierarchy.test_hierarchy_no_graph: TestExecuteHierarchy#test_hierarchy_no_graph().
  TestExecuteHierarchy.test_hierarchy_with_callers_and_callees: TestExecuteHierarchy#test_hierarchy_with_callers_and_callees().
  TestExecuteFull: TestExecuteFull#
  TestExecuteFull.test_full_mode: TestExecuteFull#test_full_mode().
  TestExecuteOutputFormat: TestExecuteOutputFormat#
  TestExecuteOutputFormat.test_toon_format: TestExecuteOutputFormat#test_toon_format().
  TestExecuteOutputFormat.test_json_format: TestExecuteOutputFormat#test_json_format().
  TestTransitiveHelpers: TestTransitiveHelpers#
  TestProjectRootChanged: TestProjectRootChanged#
  TestProjectRootChanged.test_resets_caches: TestProjectRootChanged#test_resets_caches().
  TestDefinitionBodyInlining: TestDefinitionBodyInlining#
---
# Module: [`tests/unit/test_codegraph_navigate_tool.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_navigate_tool.py)

## Classes
### `TestDefinitionBodyInlining`
- def: [`tests/unit/test_codegraph_navigate_tool.py:278`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_navigate_tool.py#L278)
- doc: P2: nav navigate inlines the definition body (coordinates -&gt; content).
- signature: `class TestDefinitionBodyInlining:`
- members:
  - `indexed(self, tmp_path)` — [`L282`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_navigate_tool.py#L282)
  - `test_definition_body_survives_toon(self, indexed)` — [`L313`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_navigate_tool.py#L313)
  - `test_definition_inlines_body(self, indexed)` — [`L300`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_navigate_tool.py#L300)
- uses (calls/refs, reference-scoped): [`ASTCache`](../../tree_sitter_analyzer/ast_cache.md#ASTCache), [`close`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.close), [`index_project`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.index_project), [`execute`](../../tree_sitter_analyzer/mcp/tools/codegraph_navigate_tool.md#CodeGraphNavigateTool.execute), [`CodeGraphNavigateTool`](../../tree_sitter_analyzer/mcp/tools/codegraph_navigate_tool.md#CodeGraphNavigateTool)

### `TestExecuteDefinition`
- def: [`tests/unit/test_codegraph_navigate_tool.py:54`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_navigate_tool.py#L54)
- signature: `class TestExecuteDefinition:`
- members:
  - `test_definition_no_cache(self, tool)` — [`L56`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_navigate_tool.py#L56)
  - `test_definition_with_cache(self, tool_with_root)` — [`L65`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_navigate_tool.py#L65)

### `TestExecuteFull`
- def: [`tests/unit/test_codegraph_navigate_tool.py:190`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_navigate_tool.py#L190)
- signature: `class TestExecuteFull:`
- members:
  - `test_full_mode(self, tool)` — [`L192`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_navigate_tool.py#L192)

### `TestExecuteHierarchy`
- def: [`tests/unit/test_codegraph_navigate_tool.py:91`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_navigate_tool.py#L91)
- signature: `class TestExecuteHierarchy:`
- members:
  - `callers_of(name, fp=None)` — [`L133`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_navigate_tool.py#L133)
  - `test_hierarchy_lists_capped_but_counts_full(self, tool)` — [`L162`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_navigate_tool.py#L162) — Wave 1b (audit nav-08b): emitted caller/callee lists are capped so a
  - `test_hierarchy_no_graph(self, tool)` — [`L93`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_navigate_tool.py#L93)
  - `test_hierarchy_transitive_depth(self, tool)` — [`L129`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_navigate_tool.py#L129)
  - `test_hierarchy_with_callers_and_callees(self, tool)` — [`L105`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_navigate_tool.py#L105)
- uses (calls/refs, reference-scoped): [`_MAX_LISTED`](../../tree_sitter_analyzer/mcp/tools/codegraph_navigate_tool.md#_MAX_LISTED)

### `TestExecuteOutputFormat`
- def: [`tests/unit/test_codegraph_navigate_tool.py:210`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_navigate_tool.py#L210)
- signature: `class TestExecuteOutputFormat:`
- members:
  - `test_json_format(self, tool)` — [`L223`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_navigate_tool.py#L223)
  - `test_toon_format(self, tool)` — [`L212`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_navigate_tool.py#L212)

### `TestProjectRootChanged`
- def: [`tests/unit/test_codegraph_navigate_tool.py:269`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_navigate_tool.py#L269)
- signature: `class TestProjectRootChanged:`
- members:
  - `test_resets_caches(self, tool_with_root)` — [`L270`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_navigate_tool.py#L270)

### `TestToolDefinition`
- def: [`tests/unit/test_codegraph_navigate_tool.py:26`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_navigate_tool.py#L26)
- signature: `class TestToolDefinition:`
- members:
  - `test_schema_modes(self, tool)` — [`L36`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_navigate_tool.py#L36)
  - `test_schema_requires_symbol(self, tool)` — [`L31`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_navigate_tool.py#L31)
  - `test_tool_name(self, tool)` — [`L27`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_navigate_tool.py#L27)

### `TestTransitiveHelpers`
- def: [`tests/unit/test_codegraph_navigate_tool.py:234`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_navigate_tool.py#L234)
- signature: `class TestTransitiveHelpers:`
- members:
  - `callees_of(name, fp=None)` — [`L255`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_navigate_tool.py#L255)
  - `callers_of(name, fp=None)` — [`L238`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_navigate_tool.py#L238)
  - `test_transitive_callees_no_cycles(self)` — [`L252`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_navigate_tool.py#L252)
  - `test_transitive_callers_bounded(self)` — [`L235`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_navigate_tool.py#L235)
- uses (calls/refs, reference-scoped): [`_transitive_callees`](../../tree_sitter_analyzer/mcp/tools/codegraph_navigate_tool.md#_transitive_callees), [`_transitive_callers`](../../tree_sitter_analyzer/mcp/tools/codegraph_navigate_tool.md#_transitive_callers)

### `TestValidateArguments`
- def: [`tests/unit/test_codegraph_navigate_tool.py:45`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_navigate_tool.py#L45)
- signature: `class TestValidateArguments:`
- members:
  - `test_missing_symbol_raises(self, tool)` — [`L46`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_navigate_tool.py#L46)
  - `test_valid_symbol(self, tool)` — [`L50`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_navigate_tool.py#L50)

## Functions
- `tool()` — [`L17`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_navigate_tool.py#L17)
- `tool_with_root(tmp_path)` — [`L22`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_navigate_tool.py#L22)

