---
title: 'Module: tests/unit/mcp/test_resources/test_project_stats_resource.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_resources/test_project_stats_resource.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_resources.test_project_stats_resource`/Test
symbols:
  TestProjectStatsResourceInit.test_project_path_initially_none: ProjectStatsResourceInit#test_project_path_initially_none().
  TestProjectStatsResourceInit.test_supported_stats_types: ProjectStatsResourceInit#test_supported_stats_types().
  TestProjectPathProperty.test_get_project_root_default: ProjectPathProperty#test_get_project_root_default().
  TestProjectPathProperty.test_set_project_root: ProjectPathProperty#test_set_project_root().
  TestGetSupportedSchemes.test_get_supported_schemes: GetSupportedSchemes#test_get_supported_schemes().
  TestGetSupportedResourceTypes.test_get_supported_resource_types: GetSupportedResourceTypes#test_get_supported_resource_types().
  TestGetSupportedStatsTypes.test_get_supported_stats_types: GetSupportedStatsTypes#test_get_supported_stats_types().
  TestMatchesUri.resource: MatchesUri#resource().
  TestMatchesUri.test_matches_uri_with_anyurl_type: MatchesUri#test_matches_uri_with_anyurl_type().
  TestExtractStatsType.resource: ExtractStatsType#resource().
  TestSetProjectPath.resource: SetProjectPath#resource().
  TestValidateProjectPath.resource: ValidateProjectPath#resource().
  TestIsSupportedCodeFile.resource: IsSupportedCodeFile#resource().
  TestGetLanguageFromFile.resource: GetLanguageFromFile#resource().
  TestGenerateOverviewStats.resource: GenerateOverviewStats#resource().
  TestGenerateLanguagesStats.resource: GenerateLanguagesStats#resource().
  TestGenerateComplexityStats.resource: GenerateComplexityStats#resource().
  TestGenerateFilesStats.resource: GenerateFilesStats#resource().
  TestReadResource.resource: ReadResource#resource().
  TestStringRepresentations.test_str_representation: StringRepresentations#test_str_representation().
  TestStringRepresentations.test_repr_representation: StringRepresentations#test_repr_representation().
  TestMatchesUri.test_matches_uri_with_anyurl_type.MockAnyUrl: MatchesUri#test_matches_uri_with_anyurl_type().MockAnyUrl#
  TestProjectStatsResourceInit: ProjectStatsResourceInit#
  TestMatchesUri: MatchesUri#
  TestMatchesUri.test_matches_uri_with_anyurl_type.MockAnyUrl.__str__: MatchesUri#test_matches_uri_with_anyurl_type().MockAnyUrl#__str__().
  TestExtractStatsType: ExtractStatsType#
  TestExtractStatsType.test_extract_valid_stats_type: ExtractStatsType#test_extract_valid_stats_type().
  TestExtractStatsType.test_extract_invalid_uri_raises_error: ExtractStatsType#test_extract_invalid_uri_raises_error().
  TestProjectPathProperty: ProjectPathProperty#
  TestSetProjectPath: SetProjectPath#
  TestSetProjectPath.test_set_valid_project_path: SetProjectPath#test_set_valid_project_path().
  TestSetProjectPath.test_set_empty_path_raises_error: SetProjectPath#test_set_empty_path_raises_error().
  TestSetProjectPath.test_set_non_string_path_raises_error: SetProjectPath#test_set_non_string_path_raises_error().
  TestValidateProjectPath: ValidateProjectPath#
  TestValidateProjectPath.test_validate_path_not_set_raises_error: ValidateProjectPath#test_validate_path_not_set_raises_error().
  TestValidateProjectPath.test_validate_nonexistent_path_raises_error: ValidateProjectPath#test_validate_nonexistent_path_raises_error().
  TestValidateProjectPath.test_validate_file_path_raises_error: ValidateProjectPath#test_validate_file_path_raises_error().
  TestValidateProjectPath.test_validate_valid_directory: ValidateProjectPath#test_validate_valid_directory().
  TestIsSupportedCodeFile: IsSupportedCodeFile#
  TestIsSupportedCodeFile.tmp_path: IsSupportedCodeFile#tmp_path().
  TestIsSupportedCodeFile.test_is_supported_python_file: IsSupportedCodeFile#test_is_supported_python_file().
  TestIsSupportedCodeFile.test_is_supported_javascript_file: IsSupportedCodeFile#test_is_supported_javascript_file().
  TestIsSupportedCodeFile.test_unsupported_file: IsSupportedCodeFile#test_unsupported_file().
  TestGetLanguageFromFile: GetLanguageFromFile#
  TestGetLanguageFromFile.tmp_path: GetLanguageFromFile#tmp_path().
  TestGetLanguageFromFile.test_get_python_language: GetLanguageFromFile#test_get_python_language().
  TestGetLanguageFromFile.test_get_javascript_language: GetLanguageFromFile#test_get_javascript_language().
  TestGetLanguageFromFile.test_get_unknown_language: GetLanguageFromFile#test_get_unknown_language().
  TestGenerateOverviewStats: GenerateOverviewStats#
  TestGenerateOverviewStats.tmp_path: GenerateOverviewStats#tmp_path().
  TestGenerateOverviewStats.test_generate_overview_success: GenerateOverviewStats#test_generate_overview_success().
  TestGenerateOverviewStats.test_generate_overview_no_project_path: GenerateOverviewStats#test_generate_overview_no_project_path().
  TestGenerateLanguagesStats: GenerateLanguagesStats#
  TestGenerateLanguagesStats.tmp_path: GenerateLanguagesStats#tmp_path().
  TestGenerateLanguagesStats.test_generate_languages_success: GenerateLanguagesStats#test_generate_languages_success().
  TestGenerateLanguagesStats.test_generate_languages_percentage: GenerateLanguagesStats#test_generate_languages_percentage().
  TestGenerateLanguagesStats.test_generate_languages_no_project_path: GenerateLanguagesStats#test_generate_languages_no_project_path().
  TestGenerateComplexityStats: GenerateComplexityStats#
  TestGenerateComplexityStats.tmp_path: GenerateComplexityStats#tmp_path().
  TestGenerateComplexityStats.test_generate_complexity_success: GenerateComplexityStats#test_generate_complexity_success().
  TestGenerateComplexityStats.test_generate_complexity_no_project_path: GenerateComplexityStats#test_generate_complexity_no_project_path().
  TestGenerateFilesStats: GenerateFilesStats#
  TestGenerateFilesStats.tmp_path: GenerateFilesStats#tmp_path().
  TestGenerateFilesStats.test_generate_files_success: GenerateFilesStats#test_generate_files_success().
  TestGenerateFilesStats.test_generate_files_sorted: GenerateFilesStats#test_generate_files_sorted().
  TestGenerateFilesStats.test_generate_files_no_project_path: GenerateFilesStats#test_generate_files_no_project_path().
  TestReadResource: ReadResource#
  TestReadResource.tmp_path: ReadResource#tmp_path().
  TestReadResource.test_read_overview_resource: ReadResource#test_read_overview_resource().
  TestReadResource.test_read_languages_resource: ReadResource#test_read_languages_resource().
  TestReadResource.test_read_complexity_resource: ReadResource#test_read_complexity_resource().
  TestReadResource.test_read_files_resource: ReadResource#test_read_files_resource().
  TestReadResource.test_read_invalid_uri: ReadResource#test_read_invalid_uri().
  TestReadResource.test_read_unsupported_stats_type: ReadResource#test_read_unsupported_stats_type().
  TestReadResource.test_read_no_project_path: ReadResource#test_read_no_project_path().
  TestGetSupportedSchemes: GetSupportedSchemes#
  TestGetSupportedResourceTypes: GetSupportedResourceTypes#
  TestGetSupportedStatsTypes: GetSupportedStatsTypes#
  TestStringRepresentations: StringRepresentations#
---
# Module: [`tests/unit/mcp/test_resources/test_project_stats_resource.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py)

## Classes
### `MockAnyUrl`
- def: [`tests/unit/mcp/test_resources/test_project_stats_resource.py:57`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L57)
- signature: `class MockAnyUrl:`
- protocol/private: `__str__`[`L58`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L58)
- used by: (1 test-only callers)

### `TestExtractStatsType`
- def: [`tests/unit/mcp/test_resources/test_project_stats_resource.py:64`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L64)
- doc: Test _extract_stats_type method
- signature: `class TestExtractStatsType:`
- members:
  - `resource(self)` — [`L68`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L68) — Create resource instance
  - `test_extract_invalid_uri_raises_error(self, resource)` — [`L79`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L79) — Test that invalid URI raises ValueError
  - `test_extract_valid_stats_type(self, resource)` — [`L72`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L72) — Test extracting valid stats type
- uses (calls/refs, reference-scoped): [`ProjectStatsResource`](../../../../tree_sitter_analyzer/mcp/resources/project_stats_resource.md#ProjectStatsResource)

### `TestGenerateComplexityStats`
- def: [`tests/unit/mcp/test_resources/test_project_stats_resource.py:322`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L322)
- doc: Test _generate_complexity_stats method
- signature: `class TestGenerateComplexityStats:`
- members:
  - `resource(self)` — [`L326`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L326) — Create resource instance
  - `test_generate_complexity_no_project_path(self, resource)` — [`L352`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L352) — Test generating complexity without project path raises error
  - `test_generate_complexity_success(self, resource, tmp_path)` — [`L340`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L340) — Test generating complexity statistics
  - `tmp_path(self)` — [`L331`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L331) — Create temporary directory with test files
- uses (calls/refs, reference-scoped): [`ProjectStatsResource`](../../../../tree_sitter_analyzer/mcp/resources/project_stats_resource.md#ProjectStatsResource)

### `TestGenerateFilesStats`
- def: [`tests/unit/mcp/test_resources/test_project_stats_resource.py:359`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L359)
- doc: Test _generate_files_stats method
- signature: `class TestGenerateFilesStats:`
- members:
  - `resource(self)` — [`L363`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L363) — Create resource instance
  - `test_generate_files_no_project_path(self, resource)` — [`L400`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L400) — Test generating files without project path raises error
  - `test_generate_files_sorted(self, resource, tmp_path)` — [`L388`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L388) — Test files are sorted by line count
  - `test_generate_files_success(self, resource, tmp_path)` — [`L378`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L378) — Test generating file statistics
  - `tmp_path(self)` — [`L368`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L368) — Create temporary directory with test files
- uses (calls/refs, reference-scoped): [`ProjectStatsResource`](../../../../tree_sitter_analyzer/mcp/resources/project_stats_resource.md#ProjectStatsResource)

### `TestGenerateLanguagesStats`
- def: [`tests/unit/mcp/test_resources/test_project_stats_resource.py:276`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L276)
- doc: Test _generate_languages_stats method
- signature: `class TestGenerateLanguagesStats:`
- members:
  - `resource(self)` — [`L280`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L280) — Create resource instance
  - `test_generate_languages_no_project_path(self, resource)` — [`L315`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L315) — Test generating languages without project path raises error
  - `test_generate_languages_percentage(self, resource, tmp_path)` — [`L305`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L305) — Test language percentage calculation
  - `test_generate_languages_success(self, resource, tmp_path)` — [`L295`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L295) — Test generating language statistics
  - `tmp_path(self)` — [`L285`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L285) — Create temporary directory with test files
- uses (calls/refs, reference-scoped): [`ProjectStatsResource`](../../../../tree_sitter_analyzer/mcp/resources/project_stats_resource.md#ProjectStatsResource)

### `TestGenerateOverviewStats`
- def: [`tests/unit/mcp/test_resources/test_project_stats_resource.py:237`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L237)
- doc: Test _generate_overview_stats method
- signature: `class TestGenerateOverviewStats:`
- members:
  - `resource(self)` — [`L241`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L241) — Create resource instance
  - `test_generate_overview_no_project_path(self, resource)` — [`L269`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L269) — Test generating overview without project path raises error
  - `test_generate_overview_success(self, resource, tmp_path)` — [`L257`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L257) — Test generating overview statistics
  - `tmp_path(self)` — [`L246`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L246) — Create temporary directory with test files
- uses (calls/refs, reference-scoped): [`ProjectStatsResource`](../../../../tree_sitter_analyzer/mcp/resources/project_stats_resource.md#ProjectStatsResource)

### `TestGetLanguageFromFile`
- def: [`tests/unit/mcp/test_resources/test_project_stats_resource.py:198`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L198)
- doc: Test _get_language_from_file method
- signature: `class TestGetLanguageFromFile:`
- members:
  - `resource(self)` — [`L202`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L202) — Create resource instance
  - `test_get_javascript_language(self, resource, tmp_path)` — [`L220`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L220) — Test getting language from JavaScript file
  - `test_get_python_language(self, resource, tmp_path)` — [`L212`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L212) — Test getting language from Python file
  - `test_get_unknown_language(self, resource, tmp_path)` — [`L228`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L228) — Test getting language from unknown file type
  - `tmp_path(self)` — [`L207`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L207) — Create temporary directory
- uses (calls/refs, reference-scoped): [`ProjectStatsResource`](../../../../tree_sitter_analyzer/mcp/resources/project_stats_resource.md#ProjectStatsResource)

### `TestGetSupportedResourceTypes`
- def: [`tests/unit/mcp/test_resources/test_project_stats_resource.py:496`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L496)
- doc: Test get_supported_resource_types method
- signature: `class TestGetSupportedResourceTypes:`
- members:
  - `test_get_supported_resource_types(self)` — [`L499`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L499) — Test getting supported resource types
- uses (calls/refs, reference-scoped): [`ProjectStatsResource`](../../../../tree_sitter_analyzer/mcp/resources/project_stats_resource.md#ProjectStatsResource), [`get_supported_resource_types`](../../../../tree_sitter_analyzer/mcp/resources/project_stats_resource.md#ProjectStatsResource.get_supported_resource_types)

### `TestGetSupportedSchemes`
- def: [`tests/unit/mcp/test_resources/test_project_stats_resource.py:484`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L484)
- doc: Test get_supported_schemes method
- signature: `class TestGetSupportedSchemes:`
- members:
  - `test_get_supported_schemes(self)` — [`L487`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L487) — Test getting supported URI schemes
- uses (calls/refs, reference-scoped): [`ProjectStatsResource`](../../../../tree_sitter_analyzer/mcp/resources/project_stats_resource.md#ProjectStatsResource), [`get_supported_schemes`](../../../../tree_sitter_analyzer/mcp/resources/project_stats_resource.md#ProjectStatsResource.get_supported_schemes)

### `TestGetSupportedStatsTypes`
- def: [`tests/unit/mcp/test_resources/test_project_stats_resource.py:508`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L508)
- doc: Test get_supported_stats_types method
- signature: `class TestGetSupportedStatsTypes:`
- members:
  - `test_get_supported_stats_types(self)` — [`L511`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L511) — Test getting supported statistics types
- uses (calls/refs, reference-scoped): [`ProjectStatsResource`](../../../../tree_sitter_analyzer/mcp/resources/project_stats_resource.md#ProjectStatsResource), [`get_supported_stats_types`](../../../../tree_sitter_analyzer/mcp/resources/project_stats_resource.md#ProjectStatsResource.get_supported_stats_types)

### `TestIsSupportedCodeFile`
- def: [`tests/unit/mcp/test_resources/test_project_stats_resource.py:160`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L160)
- doc: Test _is_supported_code_file method
- signature: `class TestIsSupportedCodeFile:`
- members:
  - `resource(self)` — [`L164`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L164) — Create resource instance
  - `test_is_supported_javascript_file(self, resource, tmp_path)` — [`L181`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L181) — Test JavaScript file is supported
  - `test_is_supported_python_file(self, resource, tmp_path)` — [`L174`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L174) — Test Python file is supported
  - `test_unsupported_file(self, resource, tmp_path)` — [`L188`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L188) — Test unsupported file type
  - `tmp_path(self)` — [`L169`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L169) — Create temporary directory
- uses (calls/refs, reference-scoped): [`ProjectStatsResource`](../../../../tree_sitter_analyzer/mcp/resources/project_stats_resource.md#ProjectStatsResource)

### `TestMatchesUri`
- def: [`tests/unit/mcp/test_resources/test_project_stats_resource.py:41`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L41)
- doc: Test matches_uri method — resource-specific edge cases.
- signature: `class TestMatchesUri:`
- members:
  - `resource(self)` — [`L49`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L49) — Create resource instance
  - `test_matches_uri_with_anyurl_type(self, resource)` — [`L53`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L53) — Test matching URI with AnyUrl type (string conversion)
- uses (calls/refs, reference-scoped): [`ProjectStatsResource`](../../../../tree_sitter_analyzer/mcp/resources/project_stats_resource.md#ProjectStatsResource)  (1 test-only)

### `TestProjectPathProperty`
- def: [`tests/unit/mcp/test_resources/test_project_stats_resource.py:85`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L85)
- doc: Test project_path property
- signature: `class TestProjectPathProperty:`
- members:
  - `test_get_project_root_default(self)` — [`L88`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L88) — Test getting default project root
  - `test_set_project_root(self)` — [`L93`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L93) — Test setting project root
- uses (calls/refs, reference-scoped): [`ProjectStatsResource`](../../../../tree_sitter_analyzer/mcp/resources/project_stats_resource.md#ProjectStatsResource), [`project_root`](../../../../tree_sitter_analyzer/mcp/resources/project_stats_resource.md#ProjectStatsResource.project_root)

### `TestProjectStatsResourceInit`
- def: [`tests/unit/mcp/test_resources/test_project_stats_resource.py:19`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L19)
- doc: Test ProjectStatsResource initialization — stats-specific fields.
- signature: `class TestProjectStatsResourceInit:`
- members:
  - `test_project_path_initially_none(self)` — [`L34`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L34) — Test that _project_path is None on init and analysis_engine is set.
  - `test_supported_stats_types(self)` — [`L26`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L26) — Test supported statistics types
- uses (calls/refs, reference-scoped): [`ProjectStatsResource`](../../../../tree_sitter_analyzer/mcp/resources/project_stats_resource.md#ProjectStatsResource), [`_project_path`](../../../../tree_sitter_analyzer/mcp/resources/project_stats_resource.md#ProjectStatsResource._project_path), [`_supported_stats_types`](../../../../tree_sitter_analyzer/mcp/resources/project_stats_resource.md#ProjectStatsResource._supported_stats_types), [`analysis_engine`](../../../../tree_sitter_analyzer/mcp/resources/project_stats_resource.md#ProjectStatsResource.analysis_engine)

### `TestReadResource`
- def: [`tests/unit/mcp/test_resources/test_project_stats_resource.py:407`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L407)
- doc: Test read_resource method
- signature: `class TestReadResource:`
- members:
  - `resource(self)` — [`L411`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L411) — Create resource instance
  - `test_read_complexity_resource(self, resource, tmp_path)` — [`L444`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L444) — Test reading complexity resource
  - `test_read_files_resource(self, resource, tmp_path)` — [`L454`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L454) — Test reading files resource
  - `test_read_invalid_uri(self, resource)` — [`L464`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L464) — Test reading resource with invalid URI
  - `test_read_languages_resource(self, resource, tmp_path)` — [`L434`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L434) — Test reading languages resource
  - `test_read_no_project_path(self, resource)` — [`L477`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L477) — Test reading resource without project path raises error
  - `test_read_overview_resource(self, resource, tmp_path)` — [`L424`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L424) — Test reading overview resource
  - `test_read_unsupported_stats_type(self, resource)` — [`L470`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L470) — Test reading resource with unsupported stats type
  - `tmp_path(self)` — [`L416`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L416) — Create temporary directory with test files
- uses (calls/refs, reference-scoped): [`ProjectStatsResource`](../../../../tree_sitter_analyzer/mcp/resources/project_stats_resource.md#ProjectStatsResource)

### `TestSetProjectPath`
- def: [`tests/unit/mcp/test_resources/test_project_stats_resource.py:100`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L100)
- doc: Test set_project_path method
- signature: `class TestSetProjectPath:`
- members:
  - `resource(self)` — [`L104`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L104) — Create resource instance
  - `test_set_empty_path_raises_error(self, resource)` — [`L113`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L113) — Test that empty path raises ValueError
  - `test_set_non_string_path_raises_error(self, resource)` — [`L118`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L118) — Test that non-string path raises TypeError
  - `test_set_valid_project_path(self, resource)` — [`L108`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L108) — Test setting a valid project path
- uses (calls/refs, reference-scoped): [`ProjectStatsResource`](../../../../tree_sitter_analyzer/mcp/resources/project_stats_resource.md#ProjectStatsResource)

### `TestStringRepresentations`
- def: [`tests/unit/mcp/test_resources/test_project_stats_resource.py:523`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L523)
- doc: Test __str__ and __repr__ methods
- signature: `class TestStringRepresentations:`
- members:
  - `test_repr_representation(self)` — [`L534`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L534) — Test detailed string representation
  - `test_str_representation(self)` — [`L526`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L526) — Test string representation
- uses (calls/refs, reference-scoped): [`ProjectStatsResource`](../../../../tree_sitter_analyzer/mcp/resources/project_stats_resource.md#ProjectStatsResource)

### `TestValidateProjectPath`
- def: [`tests/unit/mcp/test_resources/test_project_stats_resource.py:124`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L124)
- doc: Test _validate_project_path method
- signature: `class TestValidateProjectPath:`
- members:
  - `resource(self)` — [`L128`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L128) — Create resource instance
  - `test_validate_file_path_raises_error(self, resource, tmp_path)` — [`L143`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L143) — Test that file path (not directory) raises error
  - `test_validate_nonexistent_path_raises_error(self, resource, tmp_path)` — [`L137`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L137) — Test that non-existent path raises FileNotFoundError
  - `test_validate_path_not_set_raises_error(self, resource)` — [`L132`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L132) — Test that unset path raises ValueError
  - `test_validate_valid_directory(self, resource, tmp_path)` — [`L153`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_resources/test_project_stats_resource.py#L153) — Test validating a valid directory
- uses (calls/refs, reference-scoped): [`ProjectStatsResource`](../../../../tree_sitter_analyzer/mcp/resources/project_stats_resource.md#ProjectStatsResource)

