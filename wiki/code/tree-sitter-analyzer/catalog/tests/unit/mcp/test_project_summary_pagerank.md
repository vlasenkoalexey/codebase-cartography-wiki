---
title: 'Module: tests/unit/mcp/test_project_summary_pagerank.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_project_summary_pagerank.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_project_summary_pagerank`/
symbols:
  TestSummaryToonFormat.test_critical_section_present_when_data_available: TestSummaryToonFormat#test_critical_section_present_when_data_available().
  TestSummaryToonFormat.test_notes_appear_when_set: TestSummaryToonFormat#test_notes_appear_when_set().
  TestSummaryToonFormat.test_notes_omitted_when_empty: TestSummaryToonFormat#test_notes_omitted_when_empty().
  TestNoBugSilentDrop.test_large_dir_without_description_appears: TestNoBugSilentDrop#test_large_dir_without_description_appears().
  TestNoBugSilentDrop.test_context_dir_appears_under_context_section: TestNoBugSilentDrop#test_context_dir_appears_under_context_section().
  TestNoBugSilentDrop.test_all_top_level_dirs_present: TestNoBugSilentDrop#test_all_top_level_dirs_present().
  TestPageRank.test_beanfactory_ranks_highest: TestPageRank#test_beanfactory_ranks_highest().
  TestPageRank.test_pagerank_returns_top_n: TestPageRank#test_pagerank_returns_top_n().
  TestPageRank.test_pagerank_includes_inbound_refs: TestPageRank#test_pagerank_includes_inbound_refs().
  TestPageRank.test_exception_in_pagerank_returns_empty: TestPageRank#test_exception_in_pagerank_returns_empty().
  TestSummaryToonFormat.test_contains_project_name: TestSummaryToonFormat#test_contains_project_name().
  TestSummaryToonFormat.test_contains_scale_line: TestSummaryToonFormat#test_contains_scale_line().
  TestSummaryToonFormat.test_no_entry_na_line: TestSummaryToonFormat#test_no_entry_na_line().
  TestSummaryToonFormat.test_output_under_30_lines: TestSummaryToonFormat#test_output_under_30_lines().
  TestIncrementalUpdate.test_unchanged_project_skips_reparse: TestIncrementalUpdate#test_unchanged_project_skips_reparse().
  TestIncrementalUpdate.test_changed_file_triggers_reparse: TestIncrementalUpdate#test_changed_file_triggers_reparse().
  TestIncrementalUpdate.test_force_refresh_rebuilds: TestIncrementalUpdate#test_force_refresh_rebuilds().
  TestFirstPartyFiltering.test_pagerank_after_filtering_has_no_noise: TestFirstPartyFiltering#test_pagerank_after_filtering_has_no_noise().
  TestClassifyDir.test_context_has_readme_and_build_file: TestClassifyDir#test_context_has_readme_and_build_file().
  TestClassifyDir.test_context_with_package_json: TestClassifyDir#test_context_with_package_json().
  TestClassifyDir.test_tooling_by_name: TestClassifyDir#test_tooling_by_name().
  TestClassifyDir.test_core_plain_src: TestClassifyDir#test_core_plain_src().
  TestClassifyDir.test_core_no_readme: TestClassifyDir#test_core_no_readme().
  TestDescribeDir.test_reads_init_py_docstring: TestDescribeDir#test_reads_init_py_docstring().
  TestDescribeDir.test_falls_back_to_readme: TestDescribeDir#test_falls_back_to_readme().
  TestDescribeDir.test_convention_table_still_works: TestDescribeDir#test_convention_table_still_works().
  TestDescribeDir.test_no_description_returns_empty_not_crashes: TestDescribeDir#test_no_description_returns_empty_not_crashes().
  TestEdgeExtraction.test_java_import_creates_edge: TestEdgeExtraction#test_java_import_creates_edge().
  TestEdgeExtraction.test_java_extends_creates_edge: TestEdgeExtraction#test_java_extends_creates_edge().
  TestEdgeExtraction.test_java_implements_creates_edge: TestEdgeExtraction#test_java_implements_creates_edge().
  TestEdgeExtraction.test_unknown_file_returns_empty: TestEdgeExtraction#test_unknown_file_returns_empty().
  TestPageRank.test_empty_edges_returns_empty: TestPageRank#test_empty_edges_returns_empty().
  TestGetProjectSummaryReadsToon.test_reads_existing_toon: TestGetProjectSummaryReadsToon#test_reads_existing_toon().
  TestGetProjectSummaryReadsToon.test_builds_if_toon_missing: TestGetProjectSummaryReadsToon#test_builds_if_toon_missing().
  TestFirstPartyFiltering.test_stdlib_import_excluded: TestFirstPartyFiltering#test_stdlib_import_excluded().
  TestFirstPartyFiltering.test_annotation_import_excluded: TestFirstPartyFiltering#test_annotation_import_excluded().
  TestFirstPartyFiltering.test_first_party_import_kept: TestFirstPartyFiltering#test_first_party_import_kept().
  TestFirstPartyFiltering.test_extends_implements_not_filtered: TestFirstPartyFiltering#test_extends_implements_not_filtered().
  TestFirstPartyFiltering.test_no_pom_extends_kept: TestFirstPartyFiltering#test_no_pom_extends_kept().
  TestFirstPartyFiltering.test_gradle_project_extends_kept: TestFirstPartyFiltering#test_gradle_project_extends_kept().
  TestBugfixes.test_html_stripped_from_readme_excerpt: TestBugfixes#test_html_stripped_from_readme_excerpt().
  TestBugfixes.test_html_stripped_from_describe_dir: TestBugfixes#test_html_stripped_from_describe_dir().
  TestBugfixes.test_buildsrc_classified_as_core: TestBugfixes#test_buildsrc_classified_as_core().
  TestBugfixes.test_github_dir_classified_as_core: TestBugfixes#test_github_dir_classified_as_core().
  TestDetectJavaRootPackages.test_reads_pom_groupid: TestDetectJavaRootPackages#test_reads_pom_groupid().
  TestDetectJavaRootPackages.test_reads_gradle_group: TestDetectJavaRootPackages#test_reads_gradle_group().
  TestDetectJavaRootPackages.test_no_build_file_returns_empty: TestDetectJavaRootPackages#test_no_build_file_returns_empty().
  TestDetectJavaRootPackages.test_multi_module_collects_all: TestDetectJavaRootPackages#test_multi_module_collects_all().
  TestPageRank._raise: TestPageRank#_raise().
  simple_project: simple_project().
  multi_module_project: multi_module_project().
  java_project: java_project().
  TestClassifyDir: TestClassifyDir#
  TestDescribeDir: TestDescribeDir#
  TestNoBugSilentDrop: TestNoBugSilentDrop#
  TestEdgeExtraction: TestEdgeExtraction#
  TestPageRank: TestPageRank#
  TestSummaryToonFormat: TestSummaryToonFormat#
  TestIncrementalUpdate: TestIncrementalUpdate#
  TestGetProjectSummaryReadsToon: TestGetProjectSummaryReadsToon#
  java_project_with_noise: java_project_with_noise().
  gradle_project: gradle_project().
  TestDetectJavaRootPackages: TestDetectJavaRootPackages#
  TestFirstPartyFiltering: TestFirstPartyFiltering#
  TestBugfixes: TestBugfixes#
---
# Module: [`tests/unit/mcp/test_project_summary_pagerank.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_summary_pagerank.py)

## Classes
### `TestBugfixes`
- def: [`tests/unit/mcp/test_project_summary_pagerank.py:732`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_summary_pagerank.py#L732)
- doc: HTML tag cleanup and buildSrc classification.
- signature: `class TestBugfixes:`
- members:
  - `test_buildsrc_classified_as_core(self, tmp_path: Path)` — [`L753`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_summary_pagerank.py#L753)
  - `test_github_dir_classified_as_core(self, tmp_path: Path)` — [`L761`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_summary_pagerank.py#L761)
  - `test_html_stripped_from_describe_dir(self, tmp_path: Path)` — [`L744`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_summary_pagerank.py#L744)
  - `test_html_stripped_from_readme_excerpt(self, tmp_path: Path)` — [`L735`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_summary_pagerank.py#L735)
- uses (calls/refs, reference-scoped): [`ProjectIndexManager`](../../../tree_sitter_analyzer/mcp/utils/project_index/_manager.md#ProjectIndexManager), [`_classify_dir`](../../../tree_sitter_analyzer/mcp/utils/project_index/_manager.md#ProjectIndexManager._classify_dir), [`_describe_dir`](../../../tree_sitter_analyzer/mcp/utils/project_index/_manager.md#ProjectIndexManager._describe_dir), [`_extract_readme_excerpt`](../../../tree_sitter_analyzer/mcp/utils/project_index/_manager.md#ProjectIndexManager._extract_readme_excerpt)

### `TestClassifyDir`
- def: [`tests/unit/mcp/test_project_summary_pagerank.py:123`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_summary_pagerank.py#L123)
- doc: _classify_dir returns core / context / tooling.
- signature: `class TestClassifyDir:`
- members:
  - `test_context_has_readme_and_build_file(self, tmp_path: Path)` — [`L126`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_summary_pagerank.py#L126)
  - `test_context_with_package_json(self, tmp_path: Path)` — [`L134`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_summary_pagerank.py#L134)
  - `test_core_no_readme(self, tmp_path: Path)` — [`L156`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_summary_pagerank.py#L156)
  - `test_core_plain_src(self, tmp_path: Path)` — [`L150`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_summary_pagerank.py#L150)
  - `test_tooling_by_name(self, tmp_path: Path)` — [`L142`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_summary_pagerank.py#L142)
- uses (calls/refs, reference-scoped): [`ProjectIndexManager`](../../../tree_sitter_analyzer/mcp/utils/project_index/_manager.md#ProjectIndexManager), [`_classify_dir`](../../../tree_sitter_analyzer/mcp/utils/project_index/_manager.md#ProjectIndexManager._classify_dir)

### `TestDescribeDir`
- def: [`tests/unit/mcp/test_project_summary_pagerank.py:170`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_summary_pagerank.py#L170)
- doc: _describe_dir reads README.md as fallback; never returns empty for
- signature: `class TestDescribeDir:`
- members:
  - `test_convention_table_still_works(self, tmp_path: Path)` — [`L190`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_summary_pagerank.py#L190)
  - `test_falls_back_to_readme(self, tmp_path: Path)` — [`L181`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_summary_pagerank.py#L181)
  - `test_no_description_returns_empty_not_crashes(self, tmp_path: Path)` — [`L197`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_summary_pagerank.py#L197)
  - `test_reads_init_py_docstring(self, tmp_path: Path)` — [`L174`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_summary_pagerank.py#L174)
- uses (calls/refs, reference-scoped): [`ProjectIndexManager`](../../../tree_sitter_analyzer/mcp/utils/project_index/_manager.md#ProjectIndexManager), [`_describe_dir`](../../../tree_sitter_analyzer/mcp/utils/project_index/_manager.md#ProjectIndexManager._describe_dir)

### `TestDetectJavaRootPackages`
- def: [`tests/unit/mcp/test_project_summary_pagerank.py:576`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_summary_pagerank.py#L576)
- doc: Java root package detection via edge_extractors.java module.
- signature: `class TestDetectJavaRootPackages:`
- members:
  - `test_multi_module_collects_all(self, tmp_path: Path)` — [`L603`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_summary_pagerank.py#L603) — Multi-module Maven project: collects groupIds from sub-poms.
  - `test_no_build_file_returns_empty(self, tmp_path: Path)` — [`L595`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_summary_pagerank.py#L595)
  - `test_reads_gradle_group(self, gradle_project: Path)` — [`L587`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_summary_pagerank.py#L587)
  - `test_reads_pom_groupid(self, java_project_with_noise: Path)` — [`L579`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_summary_pagerank.py#L579)
- uses (calls/refs, reference-scoped): [`_detect_java_root_packages`](../../../tree_sitter_analyzer/mcp/utils/edge_extractors/java.md#_detect_java_root_packages)

### `TestEdgeExtraction`
- def: [`tests/unit/mcp/test_project_summary_pagerank.py:253`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_summary_pagerank.py#L253)
- doc: _extract_edges_from_file parses import/extends/implements.
- signature: `class TestEdgeExtraction:`
- members:
  - `test_java_extends_creates_edge(self, java_project: Path)` — [`L263`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_summary_pagerank.py#L263)
  - `test_java_implements_creates_edge(self, java_project: Path)` — [`L270`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_summary_pagerank.py#L270)
  - `test_java_import_creates_edge(self, java_project: Path)` — [`L256`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_summary_pagerank.py#L256)
  - `test_unknown_file_returns_empty(self, tmp_path: Path)` — [`L277`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_summary_pagerank.py#L277)
- uses (calls/refs, reference-scoped): [`ProjectIndexManager`](../../../tree_sitter_analyzer/mcp/utils/project_index/_manager.md#ProjectIndexManager), [`_extract_edges_from_file`](../../../tree_sitter_analyzer/mcp/utils/project_index/_manager.md#ProjectIndexManager._extract_edges_from_file)

### `TestFirstPartyFiltering`
- def: [`tests/unit/mcp/test_project_summary_pagerank.py:627`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_summary_pagerank.py#L627)
- doc: Edges from stdlib/third-party imports are excluded; first-party kept.
- signature: `class TestFirstPartyFiltering:`
- members:
  - `test_annotation_import_excluded(self, java_project_with_noise: Path)` — [`L641`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_summary_pagerank.py#L641) — javax.annotation.Nullable should NOT create an edge.
  - `test_extends_implements_not_filtered(self, java_project_with_noise: Path)` — [`L661`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_summary_pagerank.py#L661) — extends/implements edges are always kept (no package info).
  - `test_first_party_import_kept(self, java_project_with_noise: Path)` — [`L652`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_summary_pagerank.py#L652) — com.example.BeanFactory should create an edge.
  - `test_gradle_project_extends_kept(self, gradle_project: Path)` — [`L710`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_summary_pagerank.py#L710) — Gradle project: extends edges from first-party classes kept.
  - `test_no_pom_extends_kept(self, tmp_path: Path)` — [`L692`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_summary_pagerank.py#L692) — Without pom.xml, extends edges still created (no filtering needed).
  - `test_pagerank_after_filtering_has_no_noise(self, java_project_with_noise: Path)` — [`L672`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_summary_pagerank.py#L672) — Full pipeline: build → PageRank top nodes should be project classes only.
  - `test_stdlib_import_excluded(self, java_project_with_noise: Path)` — [`L630`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_summary_pagerank.py#L630) — java.util.List should NOT create an edge.
- uses (calls/refs, reference-scoped): [`ProjectIndexManager`](../../../tree_sitter_analyzer/mcp/utils/project_index/_manager.md#ProjectIndexManager), [`_extract_edges_from_file`](../../../tree_sitter_analyzer/mcp/utils/project_index/_manager.md#ProjectIndexManager._extract_edges_from_file), [`_compute_pagerank`](../../../tree_sitter_analyzer/mcp/utils/project_index/_manager.md#ProjectIndexManager._compute_pagerank)

### `TestGetProjectSummaryReadsToon`
- def: [`tests/unit/mcp/test_project_summary_pagerank.py:468`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_summary_pagerank.py#L468)
- doc: get_project_summary reads pre-built summary.toon, no recomputation.
- signature: `class TestGetProjectSummaryReadsToon:`
- members:
  - `test_builds_if_toon_missing(self, simple_project: Path)` — [`L483`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_summary_pagerank.py#L483) — If summary.toon doesn't exist, builds it on demand.
  - `test_reads_existing_toon(self, simple_project: Path)` — [`L471`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_summary_pagerank.py#L471)
- uses (calls/refs, reference-scoped): [`execute`](../../../tree_sitter_analyzer/mcp/tools/get_project_summary_tool.md#GetProjectSummaryTool.execute), [`GetProjectSummaryTool`](../../../tree_sitter_analyzer/mcp/tools/get_project_summary_tool.md#GetProjectSummaryTool)

### `TestIncrementalUpdate`
- def: [`tests/unit/mcp/test_project_summary_pagerank.py:419`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_summary_pagerank.py#L419)
- doc: build_project_index only re-parses changed files.
- signature: `class TestIncrementalUpdate:`
- members:
  - `test_changed_file_triggers_reparse(self, simple_project: Path)` — [`L438`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_summary_pagerank.py#L438)
  - `test_force_refresh_rebuilds(self, simple_project: Path)` — [`L452`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_summary_pagerank.py#L452)
  - `test_unchanged_project_skips_reparse(self, simple_project: Path)` — [`L422`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_summary_pagerank.py#L422)
- uses (calls/refs, reference-scoped): [`ProjectIndexManager`](../../../tree_sitter_analyzer/mcp/utils/project_index/_manager.md#ProjectIndexManager), [`build`](../../../tree_sitter_analyzer/mcp/utils/project_index/_manager.md#ProjectIndexManager.build), [`updated_at`](../../../tree_sitter_analyzer/mcp/utils/project_index/_models.md#ProjectIndex.updated_at)

### `TestNoBugSilentDrop`
- def: [`tests/unit/mcp/test_project_summary_pagerank.py:210`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_summary_pagerank.py#L210)
- doc: Regression: dirs with no description must still appear in summary.toon.
- signature: `class TestNoBugSilentDrop:`
- members:
  - `test_all_top_level_dirs_present(self, multi_module_project: Path)` — [`L239`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_summary_pagerank.py#L239)
  - `test_context_dir_appears_under_context_section(self, multi_module_project: Path)` — [`L228`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_summary_pagerank.py#L228)
  - `test_large_dir_without_description_appears(self, tmp_path: Path)` — [`L213`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_summary_pagerank.py#L213) — A dir with 1000 files but no __init__.py / README must appear.
- uses (calls/refs, reference-scoped): [`ProjectIndexManager`](../../../tree_sitter_analyzer/mcp/utils/project_index/_manager.md#ProjectIndexManager), [`build`](../../../tree_sitter_analyzer/mcp/utils/project_index/_manager.md#ProjectIndexManager.build), [`render_toon`](../../../tree_sitter_analyzer/mcp/utils/project_index/_manager.md#ProjectIndexManager.render_toon)

### `TestPageRank`
- def: [`tests/unit/mcp/test_project_summary_pagerank.py:290`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_summary_pagerank.py#L290)
- doc: _compute_pagerank returns critical_nodes sorted by score.
- signature: `class TestPageRank:`
- members:
  - `test_beanfactory_ranks_highest(self, java_project: Path)` — [`L293`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_summary_pagerank.py#L293) — BeanFactory is imported by 3 files — must rank highest.
  - `test_empty_edges_returns_empty(self, tmp_path: Path)` — [`L330`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_summary_pagerank.py#L330)
  - `test_exception_in_pagerank_returns_empty(self, tmp_path: Path)` — [`L335`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_summary_pagerank.py#L335) — If an unexpected error occurs, gracefully return empty list.
  - `test_pagerank_includes_inbound_refs(self, java_project: Path)` — [`L316`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_summary_pagerank.py#L316)
  - `test_pagerank_returns_top_n(self, java_project: Path)` — [`L306`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_summary_pagerank.py#L306)
- protocol/private: `_raise`[`L343`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_summary_pagerank.py#L343)
- uses (calls/refs, reference-scoped): [`ProjectIndexManager`](../../../tree_sitter_analyzer/mcp/utils/project_index/_manager.md#ProjectIndexManager), [`_extract_edges_from_file`](../../../tree_sitter_analyzer/mcp/utils/project_index/_manager.md#ProjectIndexManager._extract_edges_from_file), [`_compute_pagerank`](../../../tree_sitter_analyzer/mcp/utils/project_index/_manager.md#ProjectIndexManager._compute_pagerank)

### `TestSummaryToonFormat`
- def: [`tests/unit/mcp/test_project_summary_pagerank.py:360`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_summary_pagerank.py#L360)
- doc: render_toon produces the correct TOON structure.
- signature: `class TestSummaryToonFormat:`
- members:
  - `test_contains_project_name(self, simple_project: Path)` — [`L363`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_summary_pagerank.py#L363)
  - `test_contains_scale_line(self, simple_project: Path)` — [`L369`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_summary_pagerank.py#L369)
  - `test_critical_section_present_when_data_available(self, java_project: Path)` — [`L375`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_summary_pagerank.py#L375)
  - `test_no_entry_na_line(self, simple_project: Path)` — [`L384`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_summary_pagerank.py#L384) — entry: n/a must not appear — omit the line instead.
  - `test_notes_appear_when_set(self, simple_project: Path)` — [`L392`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_summary_pagerank.py#L392)
  - `test_notes_omitted_when_empty(self, simple_project: Path)` — [`L399`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_summary_pagerank.py#L399)
  - `test_output_under_30_lines(self, simple_project: Path)` — [`L406`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_summary_pagerank.py#L406)
- uses (calls/refs, reference-scoped): [`ProjectIndexManager`](../../../tree_sitter_analyzer/mcp/utils/project_index/_manager.md#ProjectIndexManager), [`build`](../../../tree_sitter_analyzer/mcp/utils/project_index/_manager.md#ProjectIndexManager.build), [`render_toon`](../../../tree_sitter_analyzer/mcp/utils/project_index/_manager.md#ProjectIndexManager.render_toon), [`custom_notes`](../../../tree_sitter_analyzer/mcp/utils/project_index/_models.md#ProjectIndex.custom_notes), [`critical_nodes`](../../../tree_sitter_analyzer/mcp/utils/project_index/_models.md#ProjectIndex.critical_nodes)

## Functions
- `gradle_project(tmp_path: Path)` — [`L554`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_summary_pagerank.py#L554) — Java project with build.gradle instead of pom.xml.
- `java_project(tmp_path: Path)` — [`L83`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_summary_pagerank.py#L83) — Minimal Java project for edge extraction tests.
- `java_project_with_noise(tmp_path: Path)` — [`L503`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_summary_pagerank.py#L503) — Java project with pom.xml groupId + stdlib/third-party imports.
- `multi_module_project(tmp_path: Path)` — [`L51`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_summary_pagerank.py#L51) — Project with core + context (external repo) + tooling dirs.
- `simple_project(tmp_path: Path)` — [`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_project_summary_pagerank.py#L38) — Minimal Python project — no external dependencies.

