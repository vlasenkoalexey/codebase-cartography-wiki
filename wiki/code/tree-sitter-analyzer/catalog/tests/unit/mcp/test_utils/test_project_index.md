---
title: 'Module: tests/unit/mcp/test_utils/test_project_index.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_utils/test_project_index.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_utils.test_project_index`/
symbols:
  TestProjectIndexDataclass.test_project_index_creation: TestProjectIndexDataclass#test_project_index_creation().
  TestProjectIndexManagerSaveLoad.test_save_and_load_roundtrip: TestProjectIndexManagerSaveLoad#test_save_and_load_roundtrip().
  TestProjectIndexManagerFdFallback.test_fd_fallback_to_os_walk: TestProjectIndexManagerFdFallback#test_fd_fallback_to_os_walk().
  TestProjectIndexManagerBuild.test_build_creates_index: TestProjectIndexManagerBuild#test_build_creates_index().
  TestProjectIndexManagerBuild.test_schema_version_set_in_index: TestProjectIndexManagerBuild#test_schema_version_set_in_index().
  TestProjectIndexManagerSaveLoad.test_schema_version_mismatch_returns_none: TestProjectIndexManagerSaveLoad#test_schema_version_mismatch_returns_none().
  TestProjectIndexManagerStaleness.test_is_stale_old_index: TestProjectIndexManagerStaleness#test_is_stale_old_index().
  TestProjectIndexManagerStaleness.test_is_stale_exactly_at_boundary: TestProjectIndexManagerStaleness#test_is_stale_exactly_at_boundary().
  TestProjectIndexManagerStaleness.test_is_stale_custom_max_age: TestProjectIndexManagerStaleness#test_is_stale_custom_max_age().
  TestProjectIndexManagerBuild.test_language_distribution_correct: TestProjectIndexManagerBuild#test_language_distribution_correct().
  TestProjectIndexManagerBuild.test_artifact_dirs_excluded: TestProjectIndexManagerBuild#test_artifact_dirs_excluded().
  TestProjectIndexManagerBuild.test_key_files_identified: TestProjectIndexManagerBuild#test_key_files_identified().
  TestProjectIndexManagerBuild.test_entry_points_identified: TestProjectIndexManagerBuild#test_entry_points_identified().
  TestProjectIndexManagerBuild.test_readme_excerpt_extracted: TestProjectIndexManagerBuild#test_readme_excerpt_extracted().
  TestProjectIndexManagerBuild.test_module_descriptions_from_init: TestProjectIndexManagerBuild#test_module_descriptions_from_init().
  TestProjectIndexManagerBuild.test_updated_at_recent: TestProjectIndexManagerBuild#test_updated_at_recent().
  TestProjectIndexManagerSaveLoad.test_save_creates_parent_directory: TestProjectIndexManagerSaveLoad#test_save_creates_parent_directory().
  TestProjectIndexManagerStaleness.test_is_stale_fresh_index: TestProjectIndexManagerStaleness#test_is_stale_fresh_index().
  TestProjectIndexManagerInitialization.test_init_stores_project_root: TestProjectIndexManagerInitialization#test_init_stores_project_root().
  TestProjectIndexManagerInitialization.test_cache_file_constant: TestProjectIndexManagerInitialization#test_cache_file_constant().
  TestProjectIndexManagerInitialization.test_schema_version_set: TestProjectIndexManagerInitialization#test_schema_version_set().
  TestProjectIndexManagerSaveLoad.test_load_returns_none_when_missing: TestProjectIndexManagerSaveLoad#test_load_returns_none_when_missing().
  TestProjectIndexManagerSaveLoad.test_load_returns_none_for_invalid_json: TestProjectIndexManagerSaveLoad#test_load_returns_none_for_invalid_json().
  TestProjectIndexManagerFdFallback.test_os_walk_skips_artifact_dirs: TestProjectIndexManagerFdFallback#test_os_walk_skips_artifact_dirs().
  manager: manager().
  TestProjectIndexManagerFdFallback.mock_run: TestProjectIndexManagerFdFallback#mock_run().
  simple_project: simple_project().
  TestProjectIndexManagerInitialization: TestProjectIndexManagerInitialization#
  TestProjectIndexManagerBuild: TestProjectIndexManagerBuild#
  TestProjectIndexManagerSaveLoad: TestProjectIndexManagerSaveLoad#
  TestProjectIndexManagerStaleness: TestProjectIndexManagerStaleness#
  TestProjectIndexManagerFdFallback: TestProjectIndexManagerFdFallback#
  TestProjectIndexDataclass: TestProjectIndexDataclass#
---
# Module: [`tests/unit/mcp/test_utils/test_project_index.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_project_index.py)

## Classes
### `TestProjectIndexDataclass`
- def: [`tests/unit/mcp/test_utils/test_project_index.py:301`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_project_index.py#L301)
- doc: Tests for the ProjectIndex dataclass.
- signature: `class TestProjectIndexDataclass:`
- members:
  - `test_project_index_creation(self)` — [`L304`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_project_index.py#L304) — Test that a ProjectIndex can be created with all required fields.
- uses (calls/refs, reference-scoped): [`ProjectIndex`](../../../../tree_sitter_analyzer/mcp/utils/project_index/_models.md#ProjectIndex), [`custom_notes`](../../../../tree_sitter_analyzer/mcp/utils/project_index/_models.md#ProjectIndex.custom_notes), [`language_distribution`](../../../../tree_sitter_analyzer/mcp/utils/project_index/_models.md#ProjectIndex.language_distribution), [`updated_at`](../../../../tree_sitter_analyzer/mcp/utils/project_index/_models.md#ProjectIndex.updated_at), [`file_count`](../../../../tree_sitter_analyzer/mcp/utils/project_index/_models.md#ProjectIndex.file_count), [`entry_points`](../../../../tree_sitter_analyzer/mcp/utils/project_index/_models.md#ProjectIndex.entry_points), [`module_descriptions`](../../../../tree_sitter_analyzer/mcp/utils/project_index/_models.md#ProjectIndex.module_descriptions), [`readme_excerpt`](../../../../tree_sitter_analyzer/mcp/utils/project_index/_models.md#ProjectIndex.readme_excerpt), [`key_files`](../../../../tree_sitter_analyzer/mcp/utils/project_index/_models.md#ProjectIndex.key_files), [`top_level_structure`](../../../../tree_sitter_analyzer/mcp/utils/project_index/_models.md#ProjectIndex.top_level_structure), [`project_root`](../../../../tree_sitter_analyzer/mcp/utils/project_index/_models.md#ProjectIndex.project_root), [`schema_version`](../../../../tree_sitter_analyzer/mcp/utils/project_index/_models.md#ProjectIndex.schema_version), [`created_at`](../../../../tree_sitter_analyzer/mcp/utils/project_index/_models.md#ProjectIndex.created_at)

### `TestProjectIndexManagerBuild`
- def: [`tests/unit/mcp/test_utils/test_project_index.py:85`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_project_index.py#L85)
- doc: Tests for ProjectIndexManager.build().
- signature: `class TestProjectIndexManagerBuild:`
- members:
  - `test_artifact_dirs_excluded(self, manager: ProjectIndexManager)` — [`L111`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_project_index.py#L111) — Test that __pycache__ directories are not in top_level_structure.
  - `test_build_creates_index(self, manager: ProjectIndexManager)` — [`L88`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_project_index.py#L88) — Test that build() returns a valid ProjectIndex.
  - `test_entry_points_identified(self, manager: ProjectIndexManager)` — [`L124`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_project_index.py#L124) — Test that __main__.py appears in entry_points.
  - `test_key_files_identified(self, manager: ProjectIndexManager)` — [`L117`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_project_index.py#L117) — Test that pyproject.toml and README.md appear in key_files.
  - `test_language_distribution_correct(self, manager: ProjectIndexManager)` — [`L100`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_project_index.py#L100) — Test that Python and TypeScript files are counted correctly.
  - `test_module_descriptions_from_init(self, manager: ProjectIndexManager)` — [`L135`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_project_index.py#L135) — Test that __init__.py docstrings are captured in module_descriptions.
  - `test_readme_excerpt_extracted(self, manager: ProjectIndexManager)` — [`L129`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_project_index.py#L129) — Test that a meaningful excerpt is extracted from README.md.
  - `test_schema_version_set_in_index(self, manager: ProjectIndexManager)` — [`L142`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_project_index.py#L142) — Test that the built index has the correct schema version.
  - `test_updated_at_recent(self, manager: ProjectIndexManager)` — [`L147`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_project_index.py#L147) — Test that updated_at is set to approximately now.
- uses (calls/refs, reference-scoped): [`ProjectIndexManager`](../../../../tree_sitter_analyzer/mcp/utils/project_index/_manager.md#ProjectIndexManager), [`build`](../../../../tree_sitter_analyzer/mcp/utils/project_index/_manager.md#ProjectIndexManager.build), [`ProjectIndex`](../../../../tree_sitter_analyzer/mcp/utils/project_index/_models.md#ProjectIndex), [`language_distribution`](../../../../tree_sitter_analyzer/mcp/utils/project_index/_models.md#ProjectIndex.language_distribution), [`updated_at`](../../../../tree_sitter_analyzer/mcp/utils/project_index/_models.md#ProjectIndex.updated_at), [`file_count`](../../../../tree_sitter_analyzer/mcp/utils/project_index/_models.md#ProjectIndex.file_count), [`entry_points`](../../../../tree_sitter_analyzer/mcp/utils/project_index/_models.md#ProjectIndex.entry_points), [`module_descriptions`](../../../../tree_sitter_analyzer/mcp/utils/project_index/_models.md#ProjectIndex.module_descriptions), [`readme_excerpt`](../../../../tree_sitter_analyzer/mcp/utils/project_index/_models.md#ProjectIndex.readme_excerpt), [`key_files`](../../../../tree_sitter_analyzer/mcp/utils/project_index/_models.md#ProjectIndex.key_files), [`top_level_structure`](../../../../tree_sitter_analyzer/mcp/utils/project_index/_models.md#ProjectIndex.top_level_structure), [`SCHEMA_VERSION`](../../../../tree_sitter_analyzer/mcp/utils/project_index/_manager.md#ProjectIndexManager.SCHEMA_VERSION), [`schema_version`](../../../../tree_sitter_analyzer/mcp/utils/project_index/_models.md#ProjectIndex.schema_version)

### `TestProjectIndexManagerFdFallback`
- def: [`tests/unit/mcp/test_utils/test_project_index.py:247`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_project_index.py#L247)
- doc: Tests for fd fallback to os.walk.
- signature: `class TestProjectIndexManagerFdFallback:`
- members:
  - `mock_run(cmd: list[str], **kwargs: object)` — [`L259`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_project_index.py#L259)
  - `test_fd_fallback_to_os_walk(self, manager: ProjectIndexManager, simple_project: Path)` — [`L250`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_project_index.py#L250) — Test that when fd is not available, os.walk is used as fallback.
  - `test_os_walk_skips_artifact_dirs(self, tmp_path: Path)` — [`L271`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_project_index.py#L271) — Test that os.walk fallback skips artifact directories like __pycache__.
- uses (calls/refs, reference-scoped): [`ProjectIndexManager`](../../../../tree_sitter_analyzer/mcp/utils/project_index/_manager.md#ProjectIndexManager), [`build`](../../../../tree_sitter_analyzer/mcp/utils/project_index/_manager.md#ProjectIndexManager.build), [`language_distribution`](../../../../tree_sitter_analyzer/mcp/utils/project_index/_models.md#ProjectIndex.language_distribution), [`file_count`](../../../../tree_sitter_analyzer/mcp/utils/project_index/_models.md#ProjectIndex.file_count), [`_list_files`](../../../../tree_sitter_analyzer/mcp/utils/project_index/_manager.md#ProjectIndexManager._list_files)

### `TestProjectIndexManagerInitialization`
- def: [`tests/unit/mcp/test_utils/test_project_index.py:67`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_project_index.py#L67)
- doc: Tests for ProjectIndexManager initialization.
- signature: `class TestProjectIndexManagerInitialization:`
- members:
  - `test_cache_file_constant(self)` — [`L75`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_project_index.py#L75) — Test that CACHE_FILE is the expected relative path.
  - `test_init_stores_project_root(self, simple_project: Path)` — [`L70`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_project_index.py#L70) — Test that the manager stores the project_root.
  - `test_schema_version_set(self)` — [`L79`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_project_index.py#L79) — Test that SCHEMA_VERSION is defined.
- uses (calls/refs, reference-scoped): [`ProjectIndexManager`](../../../../tree_sitter_analyzer/mcp/utils/project_index/_manager.md#ProjectIndexManager), [`project_root`](../../../../tree_sitter_analyzer/mcp/utils/project_index/_manager.md#ProjectIndexManager.project_root), [`SCHEMA_VERSION`](../../../../tree_sitter_analyzer/mcp/utils/project_index/_manager.md#ProjectIndexManager.SCHEMA_VERSION), [`CACHE_FILE`](../../../../tree_sitter_analyzer/mcp/utils/project_index/_manager.md#ProjectIndexManager.CACHE_FILE)

### `TestProjectIndexManagerSaveLoad`
- def: [`tests/unit/mcp/test_utils/test_project_index.py:155`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_project_index.py#L155)
- doc: Tests for save/load round-trips.
- signature: `class TestProjectIndexManagerSaveLoad:`
- members:
  - `test_load_returns_none_for_invalid_json(self, manager: ProjectIndexManager, simple_project: Path)` — [`L197`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_project_index.py#L197) — Test that corrupt JSON causes load() to return None.
  - `test_load_returns_none_when_missing(self, tmp_path: Path)` — [`L173`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_project_index.py#L173) — Test that load() returns None when the cache file doesn't exist.
  - `test_save_and_load_roundtrip(self, manager: ProjectIndexManager, simple_project: Path)` — [`L158`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_project_index.py#L158) — Test that saving and loading an index preserves all fields.
  - `test_save_creates_parent_directory(self, tmp_path: Path)` — [`L208`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_project_index.py#L208) — Test that save() creates the cache directory if it doesn't exist.
  - `test_schema_version_mismatch_returns_none(self, manager: ProjectIndexManager, simple_project: Path)` — [`L179`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_project_index.py#L179) — Test that a schema version mismatch causes load() to return None.
- uses (calls/refs, reference-scoped): [`ProjectIndexManager`](../../../../tree_sitter_analyzer/mcp/utils/project_index/_manager.md#ProjectIndexManager), [`build`](../../../../tree_sitter_analyzer/mcp/utils/project_index/_manager.md#ProjectIndexManager.build), [`load`](../../../../tree_sitter_analyzer/mcp/utils/project_index/_manager.md#ProjectIndexManager.load), [`save`](../../../../tree_sitter_analyzer/mcp/utils/project_index/_manager.md#ProjectIndexManager.save), [`custom_notes`](../../../../tree_sitter_analyzer/mcp/utils/project_index/_models.md#ProjectIndex.custom_notes), [`language_distribution`](../../../../tree_sitter_analyzer/mcp/utils/project_index/_models.md#ProjectIndex.language_distribution), [`file_count`](../../../../tree_sitter_analyzer/mcp/utils/project_index/_models.md#ProjectIndex.file_count), [`schema_version`](../../../../tree_sitter_analyzer/mcp/utils/project_index/_models.md#ProjectIndex.schema_version)

### `TestProjectIndexManagerStaleness`
- def: [`tests/unit/mcp/test_utils/test_project_index.py:218`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_project_index.py#L218)
- doc: Tests for is_stale().
- signature: `class TestProjectIndexManagerStaleness:`
- members:
  - `test_is_stale_custom_max_age(self, manager: ProjectIndexManager)` — [`L239`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_project_index.py#L239) — Test that a custom max_age_hours parameter is respected.
  - `test_is_stale_exactly_at_boundary(self, manager: ProjectIndexManager)` — [`L233`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_project_index.py#L233) — Test boundary: exactly 24h old is stale.
  - `test_is_stale_fresh_index(self, manager: ProjectIndexManager)` — [`L221`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_project_index.py#L221) — Test that a freshly built index is not stale.
  - `test_is_stale_old_index(self, manager: ProjectIndexManager)` — [`L226`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_project_index.py#L226) — Test that an index older than 24 hours is stale.
- uses (calls/refs, reference-scoped): [`ProjectIndexManager`](../../../../tree_sitter_analyzer/mcp/utils/project_index/_manager.md#ProjectIndexManager), [`build`](../../../../tree_sitter_analyzer/mcp/utils/project_index/_manager.md#ProjectIndexManager.build), [`updated_at`](../../../../tree_sitter_analyzer/mcp/utils/project_index/_models.md#ProjectIndex.updated_at), [`is_stale`](../../../../tree_sitter_analyzer/mcp/utils/project_index/_manager.md#ProjectIndexManager.is_stale)

## Functions
- `manager(simple_project: Path)` — [`L62`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_project_index.py#L62) — Create a ProjectIndexManager for the simple project.
- `simple_project(tmp_path: Path)` — [`L27`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_project_index.py#L27) — Create a simple project structure for testing.

