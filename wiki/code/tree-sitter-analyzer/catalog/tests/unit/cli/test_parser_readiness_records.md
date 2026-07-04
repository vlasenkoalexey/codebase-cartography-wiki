---
title: 'Module: tests/unit/cli/test_parser_readiness_records.py'
type: catalog
provenance: extracted
module: tests/unit/cli/test_parser_readiness_records.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.cli.test_parser_readiness_records`/
symbols:
  TestBuildLanguageRecords.test_single_language: TestBuildLanguageRecords#test_single_language().
  TestBuildLanguageRecords.test_multiple_languages: TestBuildLanguageRecords#test_multiple_languages().
  TestBuildLanguageRecords.test_empty_languages: TestBuildLanguageRecords#test_empty_languages().
  _make_inputs: _make_inputs().
  TestLoaderAliases.test_csharp_aliases: TestLoaderAliases#test_csharp_aliases().
  TestLoaderAliases.test_typescript_aliases: TestLoaderAliases#test_typescript_aliases().
  TestLoaderAliases.test_yaml_aliases: TestLoaderAliases#test_yaml_aliases().
  TestScoreWeights.test_total_is_100: TestScoreWeights#test_total_is_100().
  TestScoreWeights.test_parser_dependency_declared_highest: TestScoreWeights#test_parser_dependency_declared_highest().
  TestLoaderKeys.test_known_alias: TestLoaderKeys#test_known_alias().
  TestLoaderKeys.test_unknown_returns_self: TestLoaderKeys#test_unknown_returns_self().
  TestModuleIsInstalled.test_os_installed: TestModuleIsInstalled#test_os_installed().
  TestModuleIsInstalled.test_empty_string: TestModuleIsInstalled#test_empty_string().
  TestModuleIsInstalled.test_nonexistent_module: TestModuleIsInstalled#test_nonexistent_module().
  TestModuleNameForLanguage.test_from_loader_modules: TestModuleNameForLanguage#test_from_loader_modules().
  TestModuleNameForLanguage.test_csharp_uses_alias: TestModuleNameForLanguage#test_csharp_uses_alias().
  TestModuleNameForLanguage.test_from_parser_package: TestModuleNameForLanguage#test_from_parser_package().
  TestModuleNameForLanguage.test_empty_when_nothing: TestModuleNameForLanguage#test_empty_when_nothing().
  TestHasLoaderMapping.test_present: TestHasLoaderMapping#test_present().
  TestHasLoaderMapping.test_alias_present: TestHasLoaderMapping#test_alias_present().
  TestHasLoaderMapping.test_absent: TestHasLoaderMapping#test_absent().
  TestPathMatchesLanguage.test_exact_match: TestPathMatchesLanguage#test_exact_match().
  TestPathMatchesLanguage.test_no_match: TestPathMatchesLanguage#test_no_match().
  TestPathMatchesLanguage.test_underscore_split: TestPathMatchesLanguage#test_underscore_split().
  TestCountMatchingFiles.test_count_in_directory: TestCountMatchingFiles#test_count_in_directory().
  TestCountMatchingFiles.test_empty_directory: TestCountMatchingFiles#test_empty_directory().
  TestCountMatchingFiles.test_nonexistent_directory: TestCountMatchingFiles#test_nonexistent_directory().
  TestArtifactSignals.test_returns_dict: TestArtifactSignals#test_returns_dict().
  TestArtifactSignals.test_no_tests: TestArtifactSignals#test_no_tests().
  TestArtifactSignals.test_with_tests: TestArtifactSignals#test_with_tests().
  TestMetadataSignals.test_all_missing: TestMetadataSignals#test_all_missing().
  TestMetadataSignals.test_all_present: TestMetadataSignals#test_all_present().
  TestReadinessScore.test_all_true: TestReadinessScore#test_all_true().
  TestReadinessScore.test_all_false: TestReadinessScore#test_all_false().
  TestReadinessScore.test_partial: TestReadinessScore#test_partial().
  TestIsSupported.test_supported: TestIsSupported#test_supported().
  TestIsSupported.test_missing_unit_tests: TestIsSupported#test_missing_unit_tests().
  TestIsSupported.test_missing_loader: TestIsSupported#test_missing_loader().
  TestIsSupported.test_missing_golden_master: TestIsSupported#test_missing_golden_master().
  TestReadinessStatus.test_supported: TestReadinessStatus#test_supported().
  TestReadinessStatus.test_needs_hardening: TestReadinessStatus#test_needs_hardening().
  TestReadinessStatus.test_candidate: TestReadinessStatus#test_candidate().
  TestReadinessStatus.test_missing_parser_package: TestReadinessStatus#test_missing_parser_package().
  TestReadinessStatus.test_plugin_without_parser_package_is_missing_parser_package: TestReadinessStatus#test_plugin_without_parser_package_is_missing_parser_package().
  TestUnknownUpstreamSignals.test_returns_dict: TestUnknownUpstreamSignals#test_returns_dict().
  TestSemanticVersionText.test_none: TestSemanticVersionText#test_none().
  TestSemanticVersionText.test_tuple: TestSemanticVersionText#test_tuple().
  TestSemanticVersionText.test_single: TestSemanticVersionText#test_single().
  TestPackagedFileSignal.test_none_root: TestPackagedFileSignal#test_none_root().
  TestPackagedFileSignal.test_nonexistent_root: TestPackagedFileSignal#test_nonexistent_root().
  TestPackagedFileSignal.test_file_found: TestPackagedFileSignal#test_file_found().
  TestPackagedFileSignal.test_file_not_found: TestPackagedFileSignal#test_file_not_found().
  TestScannerSignal.test_none_root: TestScannerSignal#test_none_root().
  TestScannerSignal.test_scanner_c_found: TestScannerSignal#test_scanner_c_found().
  TestScannerSignal.test_scanner_cc_found: TestScannerSignal#test_scanner_cc_found().
  TestScannerSignal.test_no_scanner: TestScannerSignal#test_no_scanner().
  TestRelativeDisplay.test_relative: TestRelativeDisplay#test_relative().
  TestRelativeDisplay.test_outside_root: TestRelativeDisplay#test_outside_root().
  TestLanguageRecordMetadata.test_fields: TestLanguageRecordMetadata#test_fields().
  TestLanguageRecordMetadata.test_empty_parser_info: TestLanguageRecordMetadata#test_empty_parser_info().
  TestLanguageRecordActions.test_has_signals_and_steps: TestLanguageRecordActions#test_has_signals_and_steps().
  TestNextSteps.test_all_false_gives_many_steps: TestNextSteps#test_all_false_gives_many_steps().
  TestNextSteps.test_all_true_few_steps: TestNextSteps#test_all_true_few_steps().
  TestUpstreamNextSteps.test_requires_online_check: TestUpstreamNextSteps#test_requires_online_check().
  TestUpstreamNextSteps.test_unknown_abi_adds_step: TestUpstreamNextSteps#test_unknown_abi_adds_step().
  TestFirstProjectUrl.test_empty: TestFirstProjectUrl#test_empty().
  TestFirstProjectUrl.test_returns_first: TestFirstProjectUrl#test_returns_first().
  TestMaintenanceCheckUrl.test_maintenance_urls_releases: TestMaintenanceCheckUrl#test_maintenance_urls_releases().
  TestMaintenanceCheckUrl.test_maintenance_urls_fallback_repo: TestMaintenanceCheckUrl#test_maintenance_urls_fallback_repo().
  TestMaintenanceCheckUrl.test_fallback_to_project_urls: TestMaintenanceCheckUrl#test_fallback_to_project_urls().
  TestVerificationCommands.test_returns_list: TestVerificationCommands#test_returns_list().
  TestVerificationCommands.test_contains_pytest: TestVerificationCommands#test_contains_pytest().
  TestVerificationCommands.test_contains_parser_readiness: TestVerificationCommands#test_contains_parser_readiness().
  TestBuildLanguageRecord.test_returns_complete_record: TestBuildLanguageRecord#test_returns_complete_record().
  TestBuildLanguageRecord.test_missing_language_has_low_score: TestBuildLanguageRecord#test_missing_language_has_low_score().
  tmp_project: tmp_project().
  TestLoaderAliases: TestLoaderAliases#
  TestScoreWeights: TestScoreWeights#
  TestLoaderKeys: TestLoaderKeys#
  TestModuleIsInstalled: TestModuleIsInstalled#
  TestModuleNameForLanguage: TestModuleNameForLanguage#
  TestHasLoaderMapping: TestHasLoaderMapping#
  TestPathMatchesLanguage: TestPathMatchesLanguage#
  TestCountMatchingFiles: TestCountMatchingFiles#
  TestArtifactSignals: TestArtifactSignals#
  TestMetadataSignals: TestMetadataSignals#
  TestReadinessScore: TestReadinessScore#
  TestIsSupported: TestIsSupported#
  TestReadinessStatus: TestReadinessStatus#
  TestUnknownUpstreamSignals: TestUnknownUpstreamSignals#
  TestSemanticVersionText: TestSemanticVersionText#
  TestPackagedFileSignal: TestPackagedFileSignal#
  TestScannerSignal: TestScannerSignal#
  TestRelativeDisplay: TestRelativeDisplay#
  TestLanguageRecordMetadata: TestLanguageRecordMetadata#
  TestLanguageRecordActions: TestLanguageRecordActions#
  TestNextSteps: TestNextSteps#
  TestUpstreamNextSteps: TestUpstreamNextSteps#
  TestFirstProjectUrl: TestFirstProjectUrl#
  TestMaintenanceCheckUrl: TestMaintenanceCheckUrl#
  TestVerificationCommands: TestVerificationCommands#
  TestBuildLanguageRecords: TestBuildLanguageRecords#
  TestBuildLanguageRecord: TestBuildLanguageRecord#
---
# Module: [`tests/unit/cli/test_parser_readiness_records.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py)

## Classes
### `TestArtifactSignals`
- def: [`tests/unit/cli/test_parser_readiness_records.py:155`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L155)
- signature: `class TestArtifactSignals:`
- members:
  - `test_no_tests(self, tmp_path)` — [`L164`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L164)
  - `test_returns_dict(self, tmp_path)` — [`L156`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L156)
  - `test_with_tests(self, tmp_project)` — [`L169`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L169)
- uses (calls/refs, reference-scoped): [`_artifact_signals`](../../../tree_sitter_analyzer/cli/parser_readiness_records.md#_artifact_signals)

### `TestBuildLanguageRecord`
- def: [`tests/unit/cli/test_parser_readiness_records.py:600`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L600)
- signature: `class TestBuildLanguageRecord:`
- members:
  - `test_missing_language_has_low_score(self, tmp_path)` — [`L616`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L616)
  - `test_returns_complete_record(self, tmp_path)` — [`L601`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L601)
- uses (calls/refs, reference-scoped): [`_build_language_record`](../../../tree_sitter_analyzer/cli/parser_readiness_records.md#_build_language_record)

### `TestBuildLanguageRecords`
- def: [`tests/unit/cli/test_parser_readiness_records.py:574`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L574)
- signature: `class TestBuildLanguageRecords:`
- members:
  - `test_empty_languages(self, tmp_path)` — [`L595`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L595)
  - `test_multiple_languages(self, tmp_path)` — [`L585`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L585)
  - `test_single_language(self, tmp_path)` — [`L575`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L575)
- uses (calls/refs, reference-scoped): [`build_language_records`](../../../tree_sitter_analyzer/cli/parser_readiness_records.md#build_language_records)  (1 test-only)

### `TestCountMatchingFiles`
- def: [`tests/unit/cli/test_parser_readiness_records.py:141`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L141)
- signature: `class TestCountMatchingFiles:`
- members:
  - `test_count_in_directory(self, tmp_path)` — [`L142`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L142)
  - `test_empty_directory(self, tmp_path)` — [`L148`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L148)
  - `test_nonexistent_directory(self, tmp_path)` — [`L151`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L151)
- uses (calls/refs, reference-scoped): [`_count_matching_files`](../../../tree_sitter_analyzer/cli/parser_readiness_records.md#_count_matching_files)

### `TestFirstProjectUrl`
- def: [`tests/unit/cli/test_parser_readiness_records.py:533`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L533)
- signature: `class TestFirstProjectUrl:`
- members:
  - `test_empty(self)` — [`L534`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L534)
  - `test_returns_first(self)` — [`L537`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L537)
- uses (calls/refs, reference-scoped): [`_first_project_url`](../../../tree_sitter_analyzer/cli/parser_readiness_records.md#_first_project_url)

### `TestHasLoaderMapping`
- def: [`tests/unit/cli/test_parser_readiness_records.py:119`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L119)
- signature: `class TestHasLoaderMapping:`
- members:
  - `test_absent(self)` — [`L126`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L126)
  - `test_alias_present(self)` — [`L123`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L123)
  - `test_present(self)` — [`L120`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L120)
- uses (calls/refs, reference-scoped): [`_has_loader_mapping`](../../../tree_sitter_analyzer/cli/parser_readiness_records.md#_has_loader_mapping)

### `TestIsSupported`
- def: [`tests/unit/cli/test_parser_readiness_records.py:231`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L231)
- signature: `class TestIsSupported:`
- members:
  - `test_missing_golden_master(self)` — [`L274`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L274)
  - `test_missing_loader(self)` — [`L260`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L260)
  - `test_missing_unit_tests(self)` — [`L246`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L246)
  - `test_supported(self)` — [`L232`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L232)
- uses (calls/refs, reference-scoped): [`_is_supported`](../../../tree_sitter_analyzer/cli/parser_readiness_records.md#_is_supported)

### `TestLanguageRecordActions`
- def: [`tests/unit/cli/test_parser_readiness_records.py:454`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L454)
- signature: `class TestLanguageRecordActions:`
- members:
  - `test_has_signals_and_steps(self)` — [`L455`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L455)
- uses (calls/refs, reference-scoped): [`_language_record_actions`](../../../tree_sitter_analyzer/cli/parser_readiness_records.md#_language_record_actions)

### `TestLanguageRecordMetadata`
- def: [`tests/unit/cli/test_parser_readiness_records.py:425`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L425)
- signature: `class TestLanguageRecordMetadata:`
- members:
  - `test_empty_parser_info(self)` — [`L445`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L445)
  - `test_fields(self)` — [`L426`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L426)
- uses (calls/refs, reference-scoped): [`_language_record_metadata`](../../../tree_sitter_analyzer/cli/parser_readiness_records.md#_language_record_metadata)

### `TestLoaderAliases`
- def: [`tests/unit/cli/test_parser_readiness_records.py:59`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L59)
- signature: `class TestLoaderAliases:`
- members:
  - `test_csharp_aliases(self)` — [`L60`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L60)
  - `test_typescript_aliases(self)` — [`L63`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L63)
  - `test_yaml_aliases(self)` — [`L66`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L66)
- uses (calls/refs, reference-scoped): [`LOADER_ALIASES`](../../../tree_sitter_analyzer/cli/parser_readiness_records.md#LOADER_ALIASES)

### `TestLoaderKeys`
- def: [`tests/unit/cli/test_parser_readiness_records.py:78`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L78)
- signature: `class TestLoaderKeys:`
- members:
  - `test_known_alias(self)` — [`L79`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L79)
  - `test_unknown_returns_self(self)` — [`L82`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L82)
- uses (calls/refs, reference-scoped): [`_loader_keys`](../../../tree_sitter_analyzer/cli/parser_readiness_records.md#_loader_keys)

### `TestMaintenanceCheckUrl`
- def: [`tests/unit/cli/test_parser_readiness_records.py:542`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L542)
- signature: `class TestMaintenanceCheckUrl:`
- members:
  - `test_fallback_to_project_urls(self)` — [`L551`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L551)
  - `test_maintenance_urls_fallback_repo(self)` — [`L547`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L547)
  - `test_maintenance_urls_releases(self)` — [`L543`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L543)
- uses (calls/refs, reference-scoped): [`_maintenance_check_url`](../../../tree_sitter_analyzer/cli/parser_readiness_records.md#_maintenance_check_url)

### `TestMetadataSignals`
- def: [`tests/unit/cli/test_parser_readiness_records.py:177`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L177)
- signature: `class TestMetadataSignals:`
- members:
  - `test_all_missing(self)` — [`L178`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L178)
  - `test_all_present(self)` — [`L184`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L184)
- uses (calls/refs, reference-scoped): [`_metadata_signals`](../../../tree_sitter_analyzer/cli/parser_readiness_records.md#_metadata_signals)

### `TestModuleIsInstalled`
- def: [`tests/unit/cli/test_parser_readiness_records.py:86`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L86)
- signature: `class TestModuleIsInstalled:`
- members:
  - `test_empty_string(self)` — [`L90`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L90)
  - `test_nonexistent_module(self)` — [`L93`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L93)
  - `test_os_installed(self)` — [`L87`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L87)
- uses (calls/refs, reference-scoped): [`_module_is_installed`](../../../tree_sitter_analyzer/cli/parser_readiness_records.md#_module_is_installed)

### `TestModuleNameForLanguage`
- def: [`tests/unit/cli/test_parser_readiness_records.py:97`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L97)
- signature: `class TestModuleNameForLanguage:`
- members:
  - `test_csharp_uses_alias(self)` — [`L104`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L104)
  - `test_empty_when_nothing(self)` — [`L114`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L114)
  - `test_from_loader_modules(self)` — [`L98`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L98)
  - `test_from_parser_package(self)` — [`L108`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L108)
- uses (calls/refs, reference-scoped): [`_module_name_for_language`](../../../tree_sitter_analyzer/cli/parser_readiness_records.md#_module_name_for_language)

### `TestNextSteps`
- def: [`tests/unit/cli/test_parser_readiness_records.py:475`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L475)
- signature: `class TestNextSteps:`
- members:
  - `test_all_false_gives_many_steps(self)` — [`L476`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L476)
  - `test_all_true_few_steps(self)` — [`L493`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L493)
- uses (calls/refs, reference-scoped): [`_next_steps`](../../../tree_sitter_analyzer/cli/parser_readiness_records.md#_next_steps)

### `TestPackagedFileSignal`
- def: [`tests/unit/cli/test_parser_readiness_records.py:366`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L366)
- signature: `class TestPackagedFileSignal:`
- members:
  - `test_file_found(self, tmp_path)` — [`L376`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L376)
  - `test_file_not_found(self, tmp_path)` — [`L383`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L383)
  - `test_none_root(self)` — [`L367`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L367)
  - `test_nonexistent_root(self, tmp_path)` — [`L370`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L370)
- uses (calls/refs, reference-scoped): [`_packaged_file_signal`](../../../tree_sitter_analyzer/cli/parser_readiness_records.md#_packaged_file_signal)

### `TestPathMatchesLanguage`
- def: [`tests/unit/cli/test_parser_readiness_records.py:130`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L130)
- signature: `class TestPathMatchesLanguage:`
- members:
  - `test_exact_match(self)` — [`L131`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L131)
  - `test_no_match(self)` — [`L134`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L134)
  - `test_underscore_split(self)` — [`L137`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L137)
- uses (calls/refs, reference-scoped): [`_path_matches_language`](../../../tree_sitter_analyzer/cli/parser_readiness_records.md#_path_matches_language)

### `TestReadinessScore`
- def: [`tests/unit/cli/test_parser_readiness_records.py:196`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L196)
- signature: `class TestReadinessScore:`
- members:
  - `test_all_false(self)` — [`L208`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L208)
  - `test_all_true(self)` — [`L197`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L197)
  - `test_partial(self)` — [`L219`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L219)
- uses (calls/refs, reference-scoped): [`_readiness_score`](../../../tree_sitter_analyzer/cli/parser_readiness_records.md#_readiness_score)

### `TestReadinessStatus`
- def: [`tests/unit/cli/test_parser_readiness_records.py:289`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L289)
- signature: `class TestReadinessStatus:`
- members:
  - `test_candidate(self)` — [`L312`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L312)
  - `test_missing_parser_package(self)` — [`L323`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L323)
  - `test_needs_hardening(self)` — [`L301`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L301)
  - `test_plugin_without_parser_package_is_missing_parser_package(self)` — [`L334`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L334)
  - `test_supported(self)` — [`L290`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L290)
- uses (calls/refs, reference-scoped): [`_readiness_status`](../../../tree_sitter_analyzer/cli/parser_readiness_records.md#_readiness_status)

### `TestRelativeDisplay`
- def: [`tests/unit/cli/test_parser_readiness_records.py:414`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L414)
- signature: `class TestRelativeDisplay:`
- members:
  - `test_outside_root(self, tmp_path)` — [`L419`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L419)
  - `test_relative(self, tmp_path)` — [`L415`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L415)
- uses (calls/refs, reference-scoped): [`_relative_display`](../../../tree_sitter_analyzer/cli/parser_readiness_records.md#_relative_display)

### `TestScannerSignal`
- def: [`tests/unit/cli/test_parser_readiness_records.py:389`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L389)
- signature: `class TestScannerSignal:`
- members:
  - `test_no_scanner(self, tmp_path)` — [`L407`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L407)
  - `test_none_root(self)` — [`L390`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L390)
  - `test_scanner_c_found(self, tmp_path)` — [`L393`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L393)
  - `test_scanner_cc_found(self, tmp_path)` — [`L400`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L400)
- uses (calls/refs, reference-scoped): [`_scanner_signal`](../../../tree_sitter_analyzer/cli/parser_readiness_records.md#_scanner_signal)

### `TestScoreWeights`
- def: [`tests/unit/cli/test_parser_readiness_records.py:70`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L70)
- signature: `class TestScoreWeights:`
- members:
  - `test_parser_dependency_declared_highest(self)` — [`L74`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L74)
  - `test_total_is_100(self)` — [`L71`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L71)
- uses (calls/refs, reference-scoped): [`SCORE_WEIGHTS`](../../../tree_sitter_analyzer/cli/parser_readiness_records.md#SCORE_WEIGHTS)

### `TestSemanticVersionText`
- def: [`tests/unit/cli/test_parser_readiness_records.py:355`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L355)
- signature: `class TestSemanticVersionText:`
- members:
  - `test_none(self)` — [`L356`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L356)
  - `test_single(self)` — [`L362`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L362)
  - `test_tuple(self)` — [`L359`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L359)
- uses (calls/refs, reference-scoped): [`_semantic_version_text`](../../../tree_sitter_analyzer/cli/parser_readiness_records.md#_semantic_version_text)

### `TestUnknownUpstreamSignals`
- def: [`tests/unit/cli/test_parser_readiness_records.py:346`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L346)
- signature: `class TestUnknownUpstreamSignals:`
- members:
  - `test_returns_dict(self)` — [`L347`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L347)
- uses (calls/refs, reference-scoped): [`_unknown_upstream_signals`](../../../tree_sitter_analyzer/cli/parser_readiness_records.md#_unknown_upstream_signals)

### `TestUpstreamNextSteps`
- def: [`tests/unit/cli/test_parser_readiness_records.py:510`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L510)
- signature: `class TestUpstreamNextSteps:`
- members:
  - `test_requires_online_check(self)` — [`L511`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L511)
  - `test_unknown_abi_adds_step(self)` — [`L522`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L522)
- uses (calls/refs, reference-scoped): [`_upstream_next_steps`](../../../tree_sitter_analyzer/cli/parser_readiness_records.md#_upstream_next_steps)

### `TestVerificationCommands`
- def: [`tests/unit/cli/test_parser_readiness_records.py:559`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L559)
- signature: `class TestVerificationCommands:`
- members:
  - `test_contains_parser_readiness(self)` — [`L569`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L569)
  - `test_contains_pytest(self)` — [`L565`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L565)
  - `test_returns_list(self)` — [`L560`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L560)
- uses (calls/refs, reference-scoped): [`_verification_commands`](../../../tree_sitter_analyzer/cli/parser_readiness_records.md#_verification_commands)

## Functions
- `_make_inputs(parser_packages=None, plugin_entrypoints=None, loader_modules=None)` — [`L47`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L47)
- `tmp_project(tmp_path)` — [`L40`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_parser_readiness_records.py#L40)

