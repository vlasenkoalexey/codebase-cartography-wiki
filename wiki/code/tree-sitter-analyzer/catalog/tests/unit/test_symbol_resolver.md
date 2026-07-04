---
title: 'Module: tests/unit/test_symbol_resolver.py'
type: catalog
provenance: extracted
module: tests/unit/test_symbol_resolver.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_symbol_resolver`/
symbols:
  TestSymbolResolverEngine.test_definition_location_to_dict: TestSymbolResolverEngine#test_definition_location_to_dict().
  TestSymbolResolverEngine.test_reference_location_to_dict: TestSymbolResolverEngine#test_reference_location_to_dict().
  TestConstantNavigation.test_resolve_constant_definition: TestConstantNavigation#test_resolve_constant_definition().
  TestSymbolResolverEngine.test_resolve_function: TestSymbolResolverEngine#test_resolve_function().
  TestSymbolResolverEngine.test_resolve_class: TestSymbolResolverEngine#test_resolve_class().
  TestSymbolResolverEngine.test_find_references: TestSymbolResolverEngine#test_find_references().
  TestSymbolResolverEngine.test_resolve_method: TestSymbolResolverEngine#test_resolve_method().
  TestSymbolResolverEngine.test_resolve_variable_from_symbol_rows: TestSymbolResolverEngine#test_resolve_variable_from_symbol_rows().
  TestSymbolResolverEngine.test_qualified_name_resolution: TestSymbolResolverEngine#test_qualified_name_resolution().
  TestConstantNavigation.test_find_defs_in_file_kind_filter_includes_constant: TestConstantNavigation#test_find_defs_in_file_kind_filter_includes_constant().
  TestSymbolResolverEngine.test_find_defs_in_file_returns_enum: TestSymbolResolverEngine#test_find_defs_in_file_returns_enum().
  TestSymbolResolverEngine.test_resolve_nonexistent: TestSymbolResolverEngine#test_resolve_nonexistent().
  TestSymbolResolverEngine.test_resolve_to_dict: TestSymbolResolverEngine#test_resolve_to_dict().
  indexed_project: indexed_project().
  constant_project: constant_project().
  TestSymbolResolverEngine.test_resolve_variable_from_symbol_rows.Cache._get_conn: TestSymbolResolverEngine#test_resolve_variable_from_symbol_rows().Cache#_get_conn().
  TestSymbolResolverEngine.test_find_defs_in_file_returns_enum.Cache._get_conn: TestSymbolResolverEngine#test_find_defs_in_file_returns_enum().Cache#_get_conn().
  TestCodeGraphSymbolResolveToolDefinition.test_tool_name: TestCodeGraphSymbolResolveToolDefinition#test_tool_name().
  TestCodeGraphSymbolResolveToolDefinition.test_schema_requires_symbol: TestCodeGraphSymbolResolveToolDefinition#test_schema_requires_symbol().
  TestCodeGraphSymbolResolveToolDefinition.test_schema_has_mode: TestCodeGraphSymbolResolveToolDefinition#test_schema_has_mode().
  TestCodeGraphSymbolResolveValidation.test_validate_requires_symbol: TestCodeGraphSymbolResolveValidation#test_validate_requires_symbol().
  TestCodeGraphSymbolResolveValidation.test_validate_passes_with_symbol: TestCodeGraphSymbolResolveValidation#test_validate_passes_with_symbol().
  TestCodeGraphSymbolResolveExecution.test_resolve_mode: TestCodeGraphSymbolResolveExecution#test_resolve_mode().
  TestCodeGraphSymbolResolveExecution.test_references_mode: TestCodeGraphSymbolResolveExecution#test_references_mode().
  TestCodeGraphSymbolResolveExecution.test_nonexistent_symbol: TestCodeGraphSymbolResolveExecution#test_nonexistent_symbol().
  TestCodeGraphSymbolResolveExecution.test_toon_format: TestCodeGraphSymbolResolveExecution#test_toon_format().
  TestCodeGraphSymbolResolveExecution.test_empty_cache_error: TestCodeGraphSymbolResolveExecution#test_empty_cache_error().
  TestCodeGraphSymbolResolveExecution.test_resolve_function_definition: TestCodeGraphSymbolResolveExecution#test_resolve_function_definition().
  TestCodeGraphSymbolResolveExecution.test_resolve_class_in_different_file: TestCodeGraphSymbolResolveExecution#test_resolve_class_in_different_file().
  TestSymbolResolverEngine.test_resolve_variable_from_symbol_rows.Cache: TestSymbolResolverEngine#test_resolve_variable_from_symbol_rows().Cache#
  TestSymbolResolverEngine.test_find_defs_in_file_returns_enum.Cache: TestSymbolResolverEngine#test_find_defs_in_file_returns_enum().Cache#
  TestSymbolResolverEngine.test_resolve_variable_from_symbol_rows.Cache.get_conn: TestSymbolResolverEngine#test_resolve_variable_from_symbol_rows().Cache#get_conn().
  TestSymbolResolverEngine.test_find_defs_in_file_returns_enum.Cache.get_conn: TestSymbolResolverEngine#test_find_defs_in_file_returns_enum().Cache#get_conn().
  TestSymbolResolverEngine: TestSymbolResolverEngine#
  TestSymbolResolverEngine.test_resolve_variable_from_symbol_rows.Cache._fts5_available: TestSymbolResolverEngine#test_resolve_variable_from_symbol_rows().Cache#_fts5_available.
  TestSymbolResolverEngine.test_resolve_variable_from_symbol_rows.Cache.fts5_available: TestSymbolResolverEngine#test_resolve_variable_from_symbol_rows().Cache#fts5_available.
  TestSymbolResolverEngine.test_find_defs_in_file_returns_enum.Cache._fts5_available: TestSymbolResolverEngine#test_find_defs_in_file_returns_enum().Cache#_fts5_available.
  TestSymbolResolverEngine.test_find_defs_in_file_returns_enum.Cache.fts5_available: TestSymbolResolverEngine#test_find_defs_in_file_returns_enum().Cache#fts5_available.
  TestCodeGraphSymbolResolveToolDefinition: TestCodeGraphSymbolResolveToolDefinition#
  TestCodeGraphSymbolResolveValidation: TestCodeGraphSymbolResolveValidation#
  TestCodeGraphSymbolResolveExecution: TestCodeGraphSymbolResolveExecution#
  TestConstantNavigation: TestConstantNavigation#
---
# Module: [`tests/unit/test_symbol_resolver.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbol_resolver.py)

## Classes
### `Cache`
- def: [`tests/unit/test_symbol_resolver.py:140`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbol_resolver.py#L140)
- signature: `class Cache:`
- members:
  - `get_conn()` — [`L107`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbol_resolver.py#L107)
  - `get_conn()` — [`L145`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbol_resolver.py#L145)
  - `fts5_available` — [`L104`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbol_resolver.py#L104)
  - `fts5_available` — [`L142`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbol_resolver.py#L142)
- protocol/private: `_fts5_available`[`L103`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbol_resolver.py#L103), `_fts5_available`[`L141`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbol_resolver.py#L141), `_get_conn`[`L111`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbol_resolver.py#L111), `_get_conn`[`L149`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbol_resolver.py#L149)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `TestCodeGraphSymbolResolveExecution`
- def: [`tests/unit/test_symbol_resolver.py:263`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbol_resolver.py#L263)
- signature: `class TestCodeGraphSymbolResolveExecution:`
- members:
  - `test_empty_cache_error(self, tmp_path)` — [`L299`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbol_resolver.py#L299)
  - `test_nonexistent_symbol(self, indexed_project)` — [`L285`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbol_resolver.py#L285)
  - `test_references_mode(self, indexed_project)` — [`L275`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbol_resolver.py#L275)
  - `test_resolve_class_in_different_file(self, indexed_project)` — [`L315`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbol_resolver.py#L315)
  - `test_resolve_function_definition(self, indexed_project)` — [`L307`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbol_resolver.py#L307)
  - `test_resolve_mode(self, indexed_project)` — [`L264`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbol_resolver.py#L264)
  - `test_toon_format(self, indexed_project)` — [`L294`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbol_resolver.py#L294)
- uses (calls/refs, reference-scoped): [`execute`](../../tree_sitter_analyzer/mcp/tools/symbol_resolve_tool.md#CodeGraphSymbolResolveTool.execute), [`CodeGraphSymbolResolveTool`](../../tree_sitter_analyzer/mcp/tools/symbol_resolve_tool.md#CodeGraphSymbolResolveTool)

### `TestCodeGraphSymbolResolveToolDefinition`
- def: [`tests/unit/test_symbol_resolver.py:231`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbol_resolver.py#L231)
- signature: `class TestCodeGraphSymbolResolveToolDefinition:`
- members:
  - `test_schema_has_mode(self)` — [`L243`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbol_resolver.py#L243)
  - `test_schema_requires_symbol(self)` — [`L237`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbol_resolver.py#L237)
  - `test_tool_name(self)` — [`L232`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbol_resolver.py#L232)
- uses (calls/refs, reference-scoped): [`CodeGraphSymbolResolveTool`](../../tree_sitter_analyzer/mcp/tools/symbol_resolve_tool.md#CodeGraphSymbolResolveTool), [`get_tool_schema`](../../tree_sitter_analyzer/mcp/tools/symbol_resolve_tool.md#CodeGraphSymbolResolveTool.get_tool_schema), [`get_tool_definition`](../../tree_sitter_analyzer/mcp/tools/symbol_resolve_tool.md#CodeGraphSymbolResolveTool.get_tool_definition)

### `TestCodeGraphSymbolResolveValidation`
- def: [`tests/unit/test_symbol_resolver.py:251`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbol_resolver.py#L251)
- signature: `class TestCodeGraphSymbolResolveValidation:`
- members:
  - `test_validate_passes_with_symbol(self)` — [`L257`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbol_resolver.py#L257)
  - `test_validate_requires_symbol(self)` — [`L252`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbol_resolver.py#L252)
- uses (calls/refs, reference-scoped): [`CodeGraphSymbolResolveTool`](../../tree_sitter_analyzer/mcp/tools/symbol_resolve_tool.md#CodeGraphSymbolResolveTool), [`validate_arguments`](../../tree_sitter_analyzer/mcp/tools/symbol_resolve_tool.md#CodeGraphSymbolResolveTool.validate_arguments)

### `TestConstantNavigation`
- def: [`tests/unit/test_symbol_resolver.py:345`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbol_resolver.py#L345)
- doc: Issue #610 — kind=constant rows must be searchable AND navigable.
- signature: `class TestConstantNavigation:`
- members:
  - `test_find_defs_in_file_kind_filter_includes_constant(self, constant_project)` — [`L360`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbol_resolver.py#L360)
  - `test_resolve_constant_definition(self, constant_project)` — [`L348`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbol_resolver.py#L348)
- uses (calls/refs, reference-scoped): [`ASTCache`](../../tree_sitter_analyzer/ast_cache.md#ASTCache), [`close`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.close), [`definitions`](../../tree_sitter_analyzer/symbol_resolver.md#ResolveResult.definitions), [`_find_defs_in_file`](../../tree_sitter_analyzer/symbol_resolver.md#SymbolResolver._find_defs_in_file), [`SymbolResolver`](../../tree_sitter_analyzer/symbol_resolver.md#SymbolResolver), [`resolve`](../../tree_sitter_analyzer/symbol_resolver.md#SymbolResolver.resolve), [`name`](../../tree_sitter_analyzer/symbol_resolver.md#DefinitionLocation.name), [`kind`](../../tree_sitter_analyzer/symbol_resolver.md#DefinitionLocation.kind), [`file`](../../tree_sitter_analyzer/symbol_resolver.md#DefinitionLocation.file), [`line`](../../tree_sitter_analyzer/symbol_resolver.md#DefinitionLocation.line)

### `TestSymbolResolverEngine`
- def: [`tests/unit/test_symbol_resolver.py:56`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbol_resolver.py#L56)
- signature: `class TestSymbolResolverEngine:`
- members:
  - `test_definition_location_to_dict(self)` — [`L195`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbol_resolver.py#L195)
  - `test_find_defs_in_file_returns_enum(self)` — [`L121`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbol_resolver.py#L121) — #961 split: ``enum`` is a definition kind in _find_defs_in_file.
  - `test_find_references(self, indexed_project)` — [`L176`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbol_resolver.py#L176)
  - `test_qualified_name_resolution(self, indexed_project)` — [`L187`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbol_resolver.py#L187)
  - `test_reference_location_to_dict(self)` — [`L214`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbol_resolver.py#L214)
  - `test_resolve_class(self, indexed_project)` — [`L67`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbol_resolver.py#L67)
  - `test_resolve_function(self, indexed_project)` — [`L57`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbol_resolver.py#L57)
  - `test_resolve_method(self, indexed_project)` — [`L76`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbol_resolver.py#L76)
  - `test_resolve_nonexistent(self, indexed_project)` — [`L158`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbol_resolver.py#L158)
  - `test_resolve_to_dict(self, indexed_project)` — [`L165`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbol_resolver.py#L165)
  - `test_resolve_variable_from_symbol_rows(self)` — [`L84`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbol_resolver.py#L84)
- uses (calls/refs, reference-scoped): [`ASTCache`](../../tree_sitter_analyzer/ast_cache.md#ASTCache), [`close`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.close), [`definitions`](../../tree_sitter_analyzer/symbol_resolver.md#ResolveResult.definitions), [`_find_defs_in_file`](../../tree_sitter_analyzer/symbol_resolver.md#SymbolResolver._find_defs_in_file), [`DefinitionLocation`](../../tree_sitter_analyzer/symbol_resolver.md#DefinitionLocation), [`to_dict`](../../tree_sitter_analyzer/symbol_resolver.md#DefinitionLocation.to_dict), [`SymbolResolver`](../../tree_sitter_analyzer/symbol_resolver.md#SymbolResolver), [`resolve`](../../tree_sitter_analyzer/symbol_resolver.md#SymbolResolver.resolve), [`find_references`](../../tree_sitter_analyzer/symbol_resolver.md#SymbolResolver.find_references), [`to_dict`](../../tree_sitter_analyzer/symbol_resolver.md#ReferenceLocation.to_dict), [`to_dict`](../../tree_sitter_analyzer/symbol_resolver.md#ResolveResult.to_dict), [`name`](../../tree_sitter_analyzer/symbol_resolver.md#DefinitionLocation.name), [`kind`](../../tree_sitter_analyzer/symbol_resolver.md#DefinitionLocation.kind), [`file`](../../tree_sitter_analyzer/symbol_resolver.md#DefinitionLocation.file), [`references`](../../tree_sitter_analyzer/symbol_resolver.md#ResolveResult.references), [`ReferenceLocation`](../../tree_sitter_analyzer/symbol_resolver.md#ReferenceLocation), [`line`](../../tree_sitter_analyzer/symbol_resolver.md#DefinitionLocation.line), [`confidence`](../../tree_sitter_analyzer/symbol_resolver.md#DefinitionLocation.confidence), [`end_line`](../../tree_sitter_analyzer/symbol_resolver.md#DefinitionLocation.end_line), [`file`](../../tree_sitter_analyzer/symbol_resolver.md#ReferenceLocation.file), [`language`](../../tree_sitter_analyzer/symbol_resolver.md#DefinitionLocation.language), [`line`](../../tree_sitter_analyzer/symbol_resolver.md#ReferenceLocation.line), [`kind`](../../tree_sitter_analyzer/symbol_resolver.md#ReferenceLocation.kind), [`language`](../../tree_sitter_analyzer/symbol_resolver.md#ReferenceLocation.language), [`name`](../../tree_sitter_analyzer/symbol_resolver.md#ReferenceLocation.name), [`end_line`](../../tree_sitter_analyzer/symbol_resolver.md#ReferenceLocation.end_line), [`reference_type`](../../tree_sitter_analyzer/symbol_resolver.md#ReferenceLocation.reference_type), [`context`](../../tree_sitter_analyzer/symbol_resolver.md#DefinitionLocation.context)  (2 test-only)

## Functions
- `constant_project(tmp_path)` — [`L330`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbol_resolver.py#L330)
- `indexed_project(tmp_path)` — [`L16`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_symbol_resolver.py#L16)

