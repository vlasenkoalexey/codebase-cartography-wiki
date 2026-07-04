---
title: 'Module: tests/unit/test_ast_cache_tool.py'
type: catalog
provenance: extracted
module: tests/unit/test_ast_cache_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_ast_cache_tool`/Test
symbols:
  TestASTCacheToolInit.test_set_project_path_resets_cache: ASTCacheToolInit#test_set_project_path_resets_cache().
  TestASTCacheToolInit.test_default_init: ASTCacheToolInit#test_default_init().
  TestASTCacheToolInit.test_init_with_project_root: ASTCacheToolInit#test_init_with_project_root().
  TestGetCache.test_raises_without_project_root: GetCache#test_raises_without_project_root().
  TestGetCache.test_creates_cache_with_project_root: GetCache#test_creates_cache_with_project_root().
  TestGetCache.test_reuses_existing_cache: GetCache#test_reuses_existing_cache().
  TestGetToolDefinition.test_definition_shape: GetToolDefinition#test_definition_shape().
  TestGetToolSchema.test_mode_is_optional_in_schema: GetToolSchema#test_mode_is_optional_in_schema().
  TestGetToolSchema.test_resolve_mode_defaults_to_search_with_query: GetToolSchema#test_resolve_mode_defaults_to_search_with_query().
  TestGetToolSchema.test_symbol_declared_in_schema: GetToolSchema#test_symbol_declared_in_schema().
  TestGetToolSchema.test_valid_modes: GetToolSchema#test_valid_modes().
  TestSymbolAliasesQuery.test_symbol_aliases_query_into_search_mode: SymbolAliasesQuery#test_symbol_aliases_query_into_search_mode().
  TestSymbolAliasesQuery.test_explicit_query_wins_over_symbol: SymbolAliasesQuery#test_explicit_query_wins_over_symbol().
  TestValidateArguments.test_valid_stats_mode: ValidateArguments#test_valid_stats_mode().
  TestValidateArguments.test_invalid_mode: ValidateArguments#test_invalid_mode().
  TestValidateArguments.test_lookup_requires_file_path: ValidateArguments#test_lookup_requires_file_path().
  TestValidateArguments.test_invalidate_requires_file_path: ValidateArguments#test_invalidate_requires_file_path().
  TestValidateArguments.test_search_requires_query: ValidateArguments#test_search_requires_query().
  TestValidateArguments.test_fts_search_requires_query: ValidateArguments#test_fts_search_requires_query().
  TestValidateArguments.test_valid_lookup_with_file_path: ValidateArguments#test_valid_lookup_with_file_path().
  TestValidateArguments.test_valid_search_with_query: ValidateArguments#test_valid_search_with_query().
  TestExecute.tool_with_mock_cache: Execute#tool_with_mock_cache().
  TestAstCacheSearchTruncated.test_search_not_truncated_when_below_limit: AstCacheSearchTruncated#test_search_not_truncated_when_below_limit().
  TestAstCacheSearchTruncated.test_search_truncated_when_results_equal_limit: AstCacheSearchTruncated#test_search_truncated_when_results_equal_limit().
  TestAstCacheSearchTruncated.test_search_truncated_measured_before_split_expansion: AstCacheSearchTruncated#test_search_truncated_measured_before_split_expansion().
  TestASTCacheToolInit: ASTCacheToolInit#
  TestGetCache: GetCache#
  TestGetToolDefinition: GetToolDefinition#
  TestGetToolSchema: GetToolSchema#
  TestSymbolAliasesQuery: SymbolAliasesQuery#
  TestValidateArguments: ValidateArguments#
  TestExecute: Execute#
  TestExecute.test_stats_mode: Execute#test_stats_mode().
  TestExecute.test_lookup_found: Execute#test_lookup_found().
  TestExecute.test_lookup_not_found: Execute#test_lookup_not_found().
  TestExecute.test_search_mode: Execute#test_search_mode().
  TestExecute.test_empty_search_with_fts5_says_no_match_not_populate: Execute#test_empty_search_with_fts5_says_no_match_not_populate().
  TestExecute.test_empty_search_without_fts5_says_rebuild: Execute#test_empty_search_without_fts5_says_rebuild().
  TestExecute.test_fts_search_mode: Execute#test_fts_search_mode().
  TestExecute.test_index_single_file: Execute#test_index_single_file().
  TestExecute.test_index_project: Execute#test_index_project().
  TestExecute.test_index_project_threads_language_filter: Execute#test_index_project_threads_language_filter().
  TestExecute.test_index_project_can_include_activation: Execute#test_index_project_can_include_activation().
  TestExecute.test_invalidate_mode: Execute#test_invalidate_mode().
  TestAstCacheSearchTruncated: AstCacheSearchTruncated#
---
# Module: [`tests/unit/test_ast_cache_tool.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_tool.py)

## Classes
### `TestASTCacheToolInit`
- def: [`tests/unit/test_ast_cache_tool.py:10`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_tool.py#L10)
- doc: Tests for ASTCacheTool initialization.
- signature: `class TestASTCacheToolInit:`
- members:
  - `test_default_init(self)` — [`L13`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_tool.py#L13)
  - `test_init_with_project_root(self)` — [`L17`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_tool.py#L17)
  - `test_set_project_path_resets_cache(self, tmp_path)` — [`L21`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_tool.py#L21)
- uses (calls/refs, reference-scoped): [`project_root`](../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.project_root), [`ASTCacheTool`](../../tree_sitter_analyzer/mcp/tools/ast_cache_tool.md#ASTCacheTool), [`set_project_path`](../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.set_project_path), [`_cache`](../../tree_sitter_analyzer/mcp/tools/ast_cache_tool.md#ASTCacheTool._cache), [`cache_initialized`](../../tree_sitter_analyzer/mcp/tools/ast_cache_tool.md#ASTCacheTool.cache_initialized)

### `TestAstCacheSearchTruncated`
- def: [`tests/unit/test_ast_cache_tool.py:349`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_tool.py#L349)
- doc: #737: ast_cache mode=search must report truncated=True when results hit the limit.
- signature: `class TestAstCacheSearchTruncated:`
- members:
  - `test_search_not_truncated_when_below_limit(self, tmp_path)` — [`L353`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_tool.py#L353)
  - `test_search_truncated_measured_before_split_expansion(self, tmp_path)` — [`L379`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_tool.py#L379) — #737: truncated is measured on raw_results BEFORE _apply_legacy_import_split.
  - `test_search_truncated_when_results_equal_limit(self, tmp_path)` — [`L365`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_tool.py#L365)
- uses (calls/refs, reference-scoped): [`ASTCacheTool`](../../tree_sitter_analyzer/mcp/tools/ast_cache_tool.md#ASTCacheTool), [`execute`](../../tree_sitter_analyzer/mcp/tools/ast_cache_tool.md#ASTCacheTool.execute)

### `TestExecute`
- def: [`tests/unit/test_ast_cache_tool.py:178`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_tool.py#L178)
- doc: Tests for execute method — uses mocked cache.
- signature: `class TestExecute:`
- members:
  - `test_empty_search_with_fts5_says_no_match_not_populate(self, tool_with_mock_cache)` — [`L235`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_tool.py#L235) — Wave 1b (audit index-05): an empty result while FTS5 is available is a
  - `test_empty_search_without_fts5_says_rebuild(self, tool_with_mock_cache)` — [`L251`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_tool.py#L251) — index-05: when FTS5 is unavailable, the rebuild hint is correct.
  - `test_fts_search_mode(self, tool_with_mock_cache)` — [`L262`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_tool.py#L262)
  - `test_index_project(self, tool_with_mock_cache)` — [`L286`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_tool.py#L286)
  - `test_index_project_can_include_activation(self, tool_with_mock_cache)` — [`L320`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_tool.py#L320)
  - `test_index_project_threads_language_filter(self, tool_with_mock_cache)` — [`L303`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_tool.py#L303) — #1018: --ast-cache-language / language arg reaches index_project.
  - `test_index_single_file(self, tool_with_mock_cache)` — [`L275`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_tool.py#L275)
  - `test_invalidate_mode(self, tool_with_mock_cache)` — [`L339`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_tool.py#L339)
  - `test_lookup_found(self, tool_with_mock_cache)` — [`L198`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_tool.py#L198)
  - `test_lookup_not_found(self, tool_with_mock_cache)` — [`L209`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_tool.py#L209)
  - `test_search_mode(self, tool_with_mock_cache)` — [`L219`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_tool.py#L219)
  - `test_stats_mode(self, tool_with_mock_cache)` — [`L189`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_tool.py#L189)
  - `tool_with_mock_cache(self, tmp_path)` — [`L182`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_tool.py#L182)
- uses (calls/refs, reference-scoped): [`ASTCacheTool`](../../tree_sitter_analyzer/mcp/tools/ast_cache_tool.md#ASTCacheTool), [`_cache`](../../tree_sitter_analyzer/mcp/tools/ast_cache_tool.md#ASTCacheTool._cache)

### `TestGetCache`
- def: [`tests/unit/test_ast_cache_tool.py:28`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_tool.py#L28)
- doc: Tests for get_cache lazy initialization.
- signature: `class TestGetCache:`
- members:
  - `test_creates_cache_with_project_root(self, tmp_path)` — [`L36`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_tool.py#L36)
  - `test_raises_without_project_root(self)` — [`L31`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_tool.py#L31)
  - `test_reuses_existing_cache(self, tmp_path)` — [`L41`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_tool.py#L41)
- uses (calls/refs, reference-scoped): [`ASTCacheTool`](../../tree_sitter_analyzer/mcp/tools/ast_cache_tool.md#ASTCacheTool), [`get_cache`](../../tree_sitter_analyzer/mcp/tools/ast_cache_tool.md#ASTCacheTool.get_cache)

### `TestGetToolDefinition`
- def: [`tests/unit/test_ast_cache_tool.py:48`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_tool.py#L48)
- doc: Tests for get_tool_definition.
- signature: `class TestGetToolDefinition:`
- members:
  - `test_definition_shape(self)` — [`L51`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_tool.py#L51)
- uses (calls/refs, reference-scoped): [`ASTCacheTool`](../../tree_sitter_analyzer/mcp/tools/ast_cache_tool.md#ASTCacheTool), [`get_tool_definition`](../../tree_sitter_analyzer/mcp/tools/ast_cache_tool.md#ASTCacheTool.get_tool_definition)

### `TestGetToolSchema`
- def: [`tests/unit/test_ast_cache_tool.py:60`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_tool.py#L60)
- doc: Tests for get_tool_schema.
- signature: `class TestGetToolSchema:`
- members:
  - `test_mode_is_optional_in_schema(self)` — [`L63`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_tool.py#L63)
  - `test_resolve_mode_defaults_to_search_with_query(self)` — [`L72`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_tool.py#L72)
  - `test_symbol_declared_in_schema(self)` — [`L79`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_tool.py#L79)
  - `test_valid_modes(self)` — [`L84`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_tool.py#L84)
- uses (calls/refs, reference-scoped): [`ASTCacheTool`](../../tree_sitter_analyzer/mcp/tools/ast_cache_tool.md#ASTCacheTool), [`_resolve_mode`](../../tree_sitter_analyzer/mcp/tools/ast_cache_tool.md#ASTCacheTool._resolve_mode), [`get_tool_schema`](../../tree_sitter_analyzer/mcp/tools/ast_cache_tool.md#ASTCacheTool.get_tool_schema)

### `TestSymbolAliasesQuery`
- def: [`tests/unit/test_ast_cache_tool.py:109`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_tool.py#L109)
- doc: #575: `cache symbol=X` must search for the symbol, not silently fall back
- signature: `class TestSymbolAliasesQuery:`
- members:
  - `test_explicit_query_wins_over_symbol(self, tmp_path)` — [`L125`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_tool.py#L125)
  - `test_symbol_aliases_query_into_search_mode(self, tmp_path)` — [`L113`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_tool.py#L113)
- uses (calls/refs, reference-scoped): [`ASTCacheTool`](../../tree_sitter_analyzer/mcp/tools/ast_cache_tool.md#ASTCacheTool), [`execute`](../../tree_sitter_analyzer/mcp/tools/ast_cache_tool.md#ASTCacheTool.execute)

### `TestValidateArguments`
- def: [`tests/unit/test_ast_cache_tool.py:135`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_tool.py#L135)
- doc: Tests for validate_arguments.
- signature: `class TestValidateArguments:`
- members:
  - `test_fts_search_requires_query(self)` — [`L162`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_tool.py#L162)
  - `test_invalid_mode(self)` — [`L142`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_tool.py#L142)
  - `test_invalidate_requires_file_path(self)` — [`L152`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_tool.py#L152)
  - `test_lookup_requires_file_path(self)` — [`L147`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_tool.py#L147)
  - `test_search_requires_query(self)` — [`L157`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_tool.py#L157)
  - `test_valid_lookup_with_file_path(self)` — [`L167`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_tool.py#L167)
  - `test_valid_search_with_query(self)` — [`L173`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_tool.py#L173)
  - `test_valid_stats_mode(self)` — [`L138`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_tool.py#L138)
- uses (calls/refs, reference-scoped): [`ASTCacheTool`](../../tree_sitter_analyzer/mcp/tools/ast_cache_tool.md#ASTCacheTool), [`validate_arguments`](../../tree_sitter_analyzer/mcp/tools/ast_cache_tool.md#ASTCacheTool.validate_arguments)

