---
title: 'Module: tests/integration/formatters/test_data_manager.py'
type: catalog
provenance: extracted
module: tests/integration/formatters/test_data_manager.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.formatters.test_data_manager`/
symbols:
  FormatTestDataGenerator._create_metadata: FormatTestDataGenerator#_create_metadata().
  FormatTestDataGenerator.generate_test_data: FormatTestDataGenerator#generate_test_data().
  TestDataValidator.validate_test_data_set: TestDataValidator#validate_test_data_set().
  FormatTestDataRepository.get_test_data: FormatTestDataRepository#get_test_data().
  FormatTestDataManager.get_test_data_for_scenario: FormatTestDataManager#get_test_data_for_scenario().
  FormatTestDataManager.cleanup_invalid_data: FormatTestDataManager#cleanup_invalid_data().
  TestDataValidator._validate_consistency: TestDataValidator#_validate_consistency().
  FormatTestDataManager.repository: FormatTestDataManager#repository.
  FormatTestDataManager.create_test_data_suite: FormatTestDataManager#create_test_data_suite().
  FormatTestDataManager.validate_repository: FormatTestDataManager#validate_repository().
  FormatTestDataGenerator._generate_name: FormatTestDataGenerator#_generate_name().
  FormatTestDataSet.metadata: FormatTestDataSet#metadata.
  TestDataValidator._validate_metadata: TestDataValidator#_validate_metadata().
  get_language_templates: get_language_templates().
  store_test_data_set: store_test_data_set().
  FormatTestDataRepository.search_test_data: FormatTestDataRepository#search_test_data().
  FormatTestDataManager.import_test_data_suite: FormatTestDataManager#import_test_data_suite().
  FormatTestDataSet: FormatTestDataSet#
  FormatTestDataGenerator._generate_source_code: FormatTestDataGenerator#_generate_source_code().
  FormatTestDataRepository.db_path: FormatTestDataRepository#db_path.
  FormatTestDataRepository.data_path: FormatTestDataRepository#data_path.
  export_test_data_suite_data: export_test_data_suite_data().
  _export_test_data_sets: _export_test_data_sets().
  FormatTestDataMetadata: FormatTestDataMetadata#
  FormatTestDataRepository.store_test_data: FormatTestDataRepository#store_test_data().
  FormatTestDataMetadata.id: FormatTestDataMetadata#id.
  FormatTestDataMetadata.language: FormatTestDataMetadata#language.
  FormatTestDataSet.source_code: FormatTestDataSet#source_code.
  FormatTestDataGenerator._generate_complex_code: FormatTestDataGenerator#_generate_complex_code().
  FormatTestDataRepository._init_database: FormatTestDataRepository#_init_database().
  FormatTestDataManager._remove_test_data: FormatTestDataManager#_remove_test_data().
  import_test_data_suite_data: import_test_data_suite_data().
  _load_exported_test_data: _load_exported_test_data().
  search_test_data_sets: search_test_data_sets().
  FormatTestDataManager.generator: FormatTestDataManager#generator.
  FormatTestDataRepository.repository_path: FormatTestDataRepository#repository_path.
  FormatTestDataManager.validator: FormatTestDataManager#validator.
  FormatTestDataManager.export_test_data_suite: FormatTestDataManager#export_test_data_suite().
  FormatTestDataManager: FormatTestDataManager#
  _import_one_test_data_set: _import_one_test_data_set().
  FormatTestDataSet.expected_outputs: FormatTestDataSet#expected_outputs.
  FormatTestDataGenerator.language_templates: FormatTestDataGenerator#language_templates.
  FormatTestDataGenerator.__init__: FormatTestDataGenerator#__init__().
  FormatTestDataRepository.record_usage: FormatTestDataRepository#record_usage().
  FormatTestDataRepository.get_usage_statistics: FormatTestDataRepository#get_usage_statistics().
  FormatTestDataMetadata.name: FormatTestDataMetadata#name.
  FormatTestDataMetadata.description: FormatTestDataMetadata#description.
  FormatTestDataMetadata.complexity_level: FormatTestDataMetadata#complexity_level.
  FormatTestDataMetadata.element_counts: FormatTestDataMetadata#element_counts.
  FormatTestDataSet.test_scenarios: FormatTestDataSet#test_scenarios.
  _write_expected_outputs: _write_expected_outputs().
  _write_metadata: _write_metadata().
  TEST_DATA_TABLE_SCHEMAS: TEST_DATA_TABLE_SCHEMAS.
  FormatTestDataMetadata.format_types: FormatTestDataMetadata#format_types.
  FormatTestDataMetadata.file_size_bytes: FormatTestDataMetadata#file_size_bytes.
  FormatTestDataMetadata.created_timestamp: FormatTestDataMetadata#created_timestamp.
  FormatTestDataMetadata.version: FormatTestDataMetadata#version.
  FormatTestDataMetadata.tags: FormatTestDataMetadata#tags.
  FormatTestDataMetadata.source_hash: FormatTestDataMetadata#source_hash.
  FormatTestDataMetadata.validation_status: FormatTestDataMetadata#validation_status.
  FormatTestDataGenerator: FormatTestDataGenerator#
  FormatTestDataGenerator._get_default_element_counts: FormatTestDataGenerator#_get_default_element_counts().
  FormatTestDataGenerator._generate_expected_outputs: FormatTestDataGenerator#_generate_expected_outputs().
  FormatTestDataGenerator._generate_test_scenarios: FormatTestDataGenerator#_generate_test_scenarios().
  FormatTestDataRepository: FormatTestDataRepository#
  FormatTestDataRepository._get_file_extension: FormatTestDataRepository#_get_file_extension().
  TestDataValidator: TestDataValidator#
  TestDataValidator._validate_source_code: TestDataValidator#_validate_source_code().
  TestDataValidator._validate_expected_outputs: TestDataValidator#_validate_expected_outputs().
  TestDataValidator._count_elements_in_source: TestDataValidator#_count_elements_in_source().
  _get_python_templates: _get_python_templates().
  _get_java_templates: _get_java_templates().
  _get_javascript_templates: _get_javascript_templates().
  _get_typescript_templates: _get_typescript_templates().
  _select_export_metadata: _select_export_metadata().
  _write_export_source_file: _write_export_source_file().
  _write_export_manifest: _write_export_manifest().
  _load_export_manifest: _load_export_manifest().
  _read_exported_source: _read_exported_source().
  _read_exported_outputs: _read_exported_outputs().
  _write_repository_source_file: _write_repository_source_file().
  _build_search_query: _build_search_query().
  _metadata_from_row: _metadata_from_row().
  _upsert_test_data_record: _upsert_test_data_record().
  FormatTestDataRepository.__init__: FormatTestDataRepository#__init__().
  FormatTestDataManager.__init__: FormatTestDataManager#__init__().
---
# Module: [`tests/integration/formatters/test_data_manager.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py)

## Classes
### `FormatTestDataGenerator`
- def: [`tests/integration/formatters/test_data_manager.py:91`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L91)
- doc: Generates test data for various scenarios
- signature: `class FormatTestDataGenerator:`
- members:
  - `_create_metadata(self, language: str, complexity: str, element_counts: dict[str, int], source_code: str)` — [`L211`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L211) — Create metadata for test data
  - `_generate_complex_code(self, language: str, element_counts: dict[str, int])` — [`L169`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L169) — Generate complex code with specified element counts
  - `_generate_expected_outputs(self, source_code: str, language: str)` — [`L239`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L239) — Generate expected outputs (simplified - would use actual analyzer)
  - `_generate_name(self, prefix: str)` — [`L206`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L206) — Generate random name with prefix
  - `_generate_source_code(self, language: str, complexity: str, element_counts: dict[str, int])` — [`L142`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L142) — Generate source code based on specifications
  - `_generate_test_scenarios(self, language: str, complexity: str)` — [`L250`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L250) — Generate test scenarios for the data
  - `_get_default_element_counts(self, complexity: str)` — [`L133`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L133) — Get default element counts based on complexity
  - `generate_test_data(self, language: str, complexity: str = "medium", element_counts: dict[str, int] | None = None)` — [`L97`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L97) — Generate test data for specified language and complexity
  - `language_templates` — [`L95`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L95)
- protocol/private: `__init__`[`L94`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L94)
- uses (calls/refs, reference-scoped): (20 test-only callers)
- used by: (4 test-only callers)

### `FormatTestDataManager`
- def: [`tests/integration/formatters/test_data_manager.py:649`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L649)
- doc: Main interface for test data management
- signature: `class FormatTestDataManager:`
- members:
  - `_remove_test_data(self, test_data_id: str)` — [`L772`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L772) — Remove test data from repository
  - `cleanup_invalid_data(self)` — [`L754`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L754) — Remove invalid test data from repository
  - `create_test_data_suite(self, languages: list[str], complexities: list[str] = None, count_per_combination: int = 3)` — [`L657`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L657) — Create comprehensive test data suite
  - `export_test_data_suite(self, output_path: str, filters: dict[str, Any] | None = None)` — [`L800`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L800) — Export test data suite for sharing or backup
  - `get_test_data_for_scenario(self, language: str, complexity: str = "medium", scenario_type: str = "basic")` — [`L701`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L701) — Get test data suitable for specific testing scenario
  - `import_test_data_suite(self, import_path: str)` — [`L806`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L806) — Import test data suite from export
  - `validate_repository(self)` — [`L720`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L720) — Validate entire test data repository
  - `generator` — [`L653`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L653)
  - `repository` — [`L654`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L654)
  - `validator` — [`L655`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L655)
- protocol/private: `__init__`[`L652`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L652)
- uses (calls/refs, reference-scoped): (14 test-only callers)
- used by: (2 test-only callers)

### `FormatTestDataMetadata`
- def: [`tests/integration/formatters/test_data_manager.py:63`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L63)
- doc: Metadata for test data
- signature: `class FormatTestDataMetadata:`
- members:
  - `complexity_level` — [`L71`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L71)
  - `created_timestamp` — [`L74`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L74)
  - `description` — [`L68`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L68)
  - `element_counts` — [`L73`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L73)
  - `file_size_bytes` — [`L72`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L72)
  - `format_types` — [`L70`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L70)
  - `id` — [`L66`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L66)
  - `language` — [`L69`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L69)
  - `name` — [`L67`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L67)
  - `source_hash` — [`L77`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L77)
  - `tags` — [`L76`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L76)
  - `validation_status` — [`L78`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L78)
  - `version` — [`L75`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L75)
- used by: (12 test-only callers)

### `FormatTestDataRepository`
- def: [`tests/integration/formatters/test_data_manager.py:282`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L282)
- doc: Repository for managing test data storage and retrieval
- signature: `class FormatTestDataRepository:`
- members:
  - `_get_file_extension(self, language: str)` — [`L439`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L439) — Get file extension for language
  - `_init_database(self)` — [`L295`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L295) — Initialize test data database
  - `get_test_data(self, test_data_id: str)` — [`L307`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L307) — Retrieve test data set by ID
  - `get_usage_statistics(self)` — [`L391`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L391) — Get test data usage statistics
  - `record_usage(self, test_data_id: str, test_type: str, result: str)` — [`L374`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L374) — Record test data usage
  - `search_test_data(self, language: str | None = None, complexity: str | None = None, tags: list[str] | None = None, limit: int = 100)` — [`L357`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L357) — Search for test data sets
  - `store_test_data(self, test_data_set: FormatTestDataSet)` — [`L303`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L303) — Store test data set in repository
  - `data_path` — [`L290`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L290)
  - `db_path` — [`L289`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L289)
  - `repository_path` — [`L286`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L286)
- protocol/private: `__init__`[`L285`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L285)
- uses (calls/refs, reference-scoped): (9 test-only callers)
- used by: (7 test-only callers)

### `FormatTestDataSet`
- def: [`tests/integration/formatters/test_data_manager.py:82`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L82)
- doc: Complete test data set
- signature: `class FormatTestDataSet:`
- members:
  - `expected_outputs` — [`L87`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L87)
  - `metadata` — [`L85`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L85)
  - `source_code` — [`L86`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L86)
  - `test_scenarios` — [`L88`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L88)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (8 test-only callers)

### `TestDataValidator`
- def: [`tests/integration/formatters/test_data_manager.py:452`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L452)
- doc: Validates test data quality and consistency
- signature: `class TestDataValidator:`
- members:
  - `_count_elements_in_source(self, source_code: str, language: str)` — [`L616`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L616) — Count elements in source code
  - `_validate_consistency(self, test_data_set: FormatTestDataSet)` — [`L590`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L590) — Validate internal consistency
  - `_validate_expected_outputs(self, expected_outputs: dict[str, str])` — [`L563`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L563) — Validate expected outputs
  - `_validate_metadata(self, metadata: FormatTestDataMetadata)` — [`L479`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L479) — Validate metadata quality
  - `_validate_source_code(self, source_code: str, language: str)` — [`L521`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L521) — Validate source code quality
  - `validate_test_data_set(self, test_data_set: FormatTestDataSet)` — [`L455`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L455) — Validate test data set quality
- uses (calls/refs, reference-scoped): (9 test-only callers)
- used by: (4 test-only callers)

## Functions
- `_build_search_query(language: str | None, complexity: str | None, tags: list[str] | None, limit: int)` — [`L1277`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L1277)
- `_export_test_data_sets(repository: Any, output_path: Path, test_data_list: list[Any])` — [`L1075`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L1075)
- `_get_java_templates()` — [`L864`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L864)
- `_get_javascript_templates()` — [`L917`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L917)
- `_get_python_templates()` — [`L826`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L826)
- `_get_typescript_templates()` — [`L964`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L964)
- `_import_one_test_data_set(repository: Any, import_path: Path, test_data_id: str, metadata_type: Any, data_set_type: Any)` — [`L1160`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L1160)
- `_load_export_manifest(import_path: Path)` — [`L1148`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L1148)
- `_load_exported_test_data(repository: Any, test_dir: Path, metadata_type: Any, data_set_type: Any)` — [`L1192`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L1192)
- `_metadata_from_row(row: tuple[Any, ...], metadata_type: type)` — [`L1303`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L1303)
- `_read_exported_outputs(test_dir: Path)` — [`L1220`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L1220)
- `_read_exported_source(repository: Any, test_dir: Path, language: str)` — [`L1214`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L1214)
- `_select_export_metadata(repository: Any, filters: dict[str, Any] | None)` — [`L1061`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L1061)
- `_upsert_test_data_record(db_path: Path, data_dir: Path, test_data_set: Any)` — [`L1321`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L1321)
- `_write_expected_outputs(export_dir: Path, expected_outputs: dict[str, str])` — [`L1105`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L1105)
- `_write_export_manifest(output_path: Path, exported_count: int, filters: dict[str, Any] | None, test_data_list: list[Any])` — [`L1128`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L1128)
- `_write_export_source_file(repository: Any, export_dir: Path, language: str, source_code: str)` — [`L1097`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L1097)
- `_write_metadata(export_dir: Path, test_data: Any)` — [`L1115`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L1115)
- `_write_repository_source_file(data_dir: Path, test_data_set: Any, extension_for_language: Callable[[str], str])` — [`L1248`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L1248)
- `export_test_data_suite_data(repository: Any, output_path: str, filters: dict[str, Any] | None = None)` — [`L1017`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L1017) — Export repository test data to a portable directory.
- `get_language_templates()` — [`L816`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L816) — Return source templates keyed by language name.
- `import_test_data_suite_data(repository: Any, import_path: str, metadata_type: Any, data_set_type: Any)` — [`L1031`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L1031) — Import repository test data from a portable export directory.
- `search_test_data_sets(db_path: Path, metadata_type: type, language: str | None = None, complexity: str | None = None, tags: list[str] | None = None, limit: int = 100)` — [`L1258`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L1258) — Search repository metadata records with optional filters.
- `store_test_data_set(repository: Any, test_data_set: Any)` — [`L1233`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L1233) — Persist a test data set and return its id.

## Module values
- `TEST_DATA_TABLE_SCHEMAS` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/test_data_manager.py#L21)

