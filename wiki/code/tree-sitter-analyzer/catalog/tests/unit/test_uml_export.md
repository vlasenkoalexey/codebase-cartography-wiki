---
title: 'Module: tests/unit/test_uml_export.py'
type: catalog
provenance: extracted
module: tests/unit/test_uml_export.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_uml_export`/
symbols:
  test_sequence_diagram_uses_call_path_and_marks_static_approximation: test_sequence_diagram_uses_call_path_and_marks_static_approximation().
  test_class_diagram_uses_internal_and_common_external_bases: test_class_diagram_uses_internal_and_common_external_bases().
  test_package_diagram_aggregates_import_edges: test_package_diagram_aggregates_import_edges().
  test_component_diagram_aggregates_top_level_components: test_component_diagram_aggregates_top_level_components().
  test_class_diagram_closes_owned_cache_and_falls_back_to_nodes: test_class_diagram_closes_owned_cache_and_falls_back_to_nodes().
  test_render_class_mermaid_uses_inheritance_arrows: test_render_class_mermaid_uses_inheritance_arrows().
  test_render_flowchart_mermaid_labels_weighted_edges: test_render_flowchart_mermaid_labels_weighted_edges().
  test_render_flowchart_mermaid_supports_unlabeled_edges: test_render_flowchart_mermaid_supports_unlabeled_edges().
  test_clamp_edges_merges_duplicates_and_reports_truncation: test_clamp_edges_merges_duplicates_and_reports_truncation().
  test_render_sequence_mermaid_uses_first_call_path: test_render_sequence_mermaid_uses_first_call_path().
  test_render_sequence_mermaid_empty_path_is_explicit: test_render_sequence_mermaid_empty_path_is_explicit().
  test_render_sequence_mermaid_empty_hops_are_explicit: test_render_sequence_mermaid_empty_hops_are_explicit().
  test_render_sequence_mermaid_skips_incomplete_hops: test_render_sequence_mermaid_skips_incomplete_hops().
  test_package_name_groups_file_paths: test_package_name_groups_file_paths().
  test_component_name_groups_project_components: test_component_name_groups_project_components().
  test_sequence_diagram_uses_call_path_and_marks_static_approximation.FakeCallPathFinder.find_path: test_sequence_diagram_uses_call_path_and_marks_static_approximation().FakeCallPathFinder#find_path().
  test_sequence_diagram_uses_call_path_and_marks_static_approximation.FakeCallPathResult: test_sequence_diagram_uses_call_path_and_marks_static_approximation().FakeCallPathResult#
  test_class_diagram_uses_internal_and_common_external_bases.FakeHierarchy: test_class_diagram_uses_internal_and_common_external_bases().FakeHierarchy#
  test_class_diagram_closes_owned_cache_and_falls_back_to_nodes.FakeCache: test_class_diagram_closes_owned_cache_and_falls_back_to_nodes().FakeCache#
  test_class_diagram_closes_owned_cache_and_falls_back_to_nodes.FakeHierarchy: test_class_diagram_closes_owned_cache_and_falls_back_to_nodes().FakeHierarchy#
  test_package_diagram_aggregates_import_edges.FakeImportGraph: test_package_diagram_aggregates_import_edges().FakeImportGraph#
  test_component_diagram_aggregates_top_level_components.FakeImportGraph: test_component_diagram_aggregates_top_level_components().FakeImportGraph#
  test_sequence_diagram_uses_call_path_and_marks_static_approximation.FakeCallPathFinder: test_sequence_diagram_uses_call_path_and_marks_static_approximation().FakeCallPathFinder#
  test_class_diagram_uses_internal_and_common_external_bases.FakeHierarchy.__init__: test_class_diagram_uses_internal_and_common_external_bases().FakeHierarchy#__init__().
  FakeHierarchy.cache: FakeHierarchy#cache.
  test_class_diagram_uses_internal_and_common_external_bases.FakeHierarchy.build: test_class_diagram_uses_internal_and_common_external_bases().FakeHierarchy#build().
  test_class_diagram_uses_internal_and_common_external_bases.FakeHierarchy.all_classes: test_class_diagram_uses_internal_and_common_external_bases().FakeHierarchy#all_classes().
  test_class_diagram_closes_owned_cache_and_falls_back_to_nodes.FakeCache.__init__: test_class_diagram_closes_owned_cache_and_falls_back_to_nodes().FakeCache#__init__().
  test_class_diagram_closes_owned_cache_and_falls_back_to_nodes.FakeCache.close: test_class_diagram_closes_owned_cache_and_falls_back_to_nodes().FakeCache#close().
  test_class_diagram_closes_owned_cache_and_falls_back_to_nodes.FakeHierarchy.__init__: test_class_diagram_closes_owned_cache_and_falls_back_to_nodes().FakeHierarchy#__init__().
  test_class_diagram_closes_owned_cache_and_falls_back_to_nodes.FakeHierarchy.build: test_class_diagram_closes_owned_cache_and_falls_back_to_nodes().FakeHierarchy#build().
  test_class_diagram_closes_owned_cache_and_falls_back_to_nodes.FakeHierarchy.all_classes: test_class_diagram_closes_owned_cache_and_falls_back_to_nodes().FakeHierarchy#all_classes().
  test_package_diagram_aggregates_import_edges.FakeImportGraph.__init__: test_package_diagram_aggregates_import_edges().FakeImportGraph#__init__().
  test_package_diagram_aggregates_import_edges.FakeImportGraph.build: test_package_diagram_aggregates_import_edges().FakeImportGraph#build().
  test_component_diagram_aggregates_top_level_components.FakeImportGraph.__init__: test_component_diagram_aggregates_top_level_components().FakeImportGraph#__init__().
  test_component_diagram_aggregates_top_level_components.FakeImportGraph.build: test_component_diagram_aggregates_top_level_components().FakeImportGraph#build().
  test_sequence_diagram_uses_call_path_and_marks_static_approximation.FakeCallPathResult.truncated: test_sequence_diagram_uses_call_path_and_marks_static_approximation().FakeCallPathResult#truncated.
  test_sequence_diagram_uses_call_path_and_marks_static_approximation.FakeCallPathResult.to_dict: test_sequence_diagram_uses_call_path_and_marks_static_approximation().FakeCallPathResult#to_dict().
  test_sequence_diagram_uses_call_path_and_marks_static_approximation.FakeCallPathFinder.__init__: test_sequence_diagram_uses_call_path_and_marks_static_approximation().FakeCallPathFinder#__init__().
---
# Module: [`tests/unit/test_uml_export.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_export.py)

## Classes
### `FakeCache`
- def: [`tests/unit/test_uml_export.py:161`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_export.py#L161)
- signature: `class FakeCache:`
- members:
  - `close(self)` — [`L165`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_export.py#L165)
- protocol/private: `__init__`[`L162`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_export.py#L162)
- used by: (1 test-only callers)

### `FakeCallPathFinder`
- def: [`tests/unit/test_uml_export.py:277`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_export.py#L277)
- signature: `class FakeCallPathFinder:`
- members:
  - `find_path(self, source_function: str, target_function: str, max_depth: int, max_paths: int)` — [`L282`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_export.py#L282)
- protocol/private: `__init__`[`L278`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_export.py#L278)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `FakeCallPathResult`
- def: [`tests/unit/test_uml_export.py:262`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_export.py#L262)
- signature: `class FakeCallPathResult:`
- members:
  - `to_dict(self)` — [`L265`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_export.py#L265)
  - `truncated` — [`L263`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_export.py#L263)
- used by: (1 test-only callers)

### `FakeHierarchy`
- def: [`tests/unit/test_uml_export.py:168`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_export.py#L168)
- signature: `class FakeHierarchy:`
- members:
  - `all_classes(self)` — [`L140`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_export.py#L140)
  - `all_classes(self)` — [`L175`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_export.py#L175)
  - `build(self)` — [`L137`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_export.py#L137)
  - `build(self)` — [`L172`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_export.py#L172)
  - `cache` — [`L135`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_export.py#L135)
- protocol/private: `__init__`[`L134`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_export.py#L134), `__init__`[`L169`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_export.py#L169)
- used by: (1 test-only callers)

### `FakeImportGraph`
- def: [`tests/unit/test_uml_export.py:228`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_export.py#L228)
- signature: `class FakeImportGraph:`
- members:
  - `build(self)` — [`L199`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_export.py#L199)
  - `build(self)` — [`L232`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_export.py#L232)
- protocol/private: `__init__`[`L196`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_export.py#L196), `__init__`[`L229`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_export.py#L229)
- used by: (1 test-only callers)

## Functions
- `test_clamp_edges_merges_duplicates_and_reports_truncation()` — [`L118`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_export.py#L118)
- `test_class_diagram_closes_owned_cache_and_falls_back_to_nodes(monkeypatch)` — [`L158`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_export.py#L158)
- `test_class_diagram_uses_internal_and_common_external_bases(monkeypatch)` — [`L132`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_export.py#L132)
- `test_component_diagram_aggregates_top_level_components(monkeypatch)` — [`L227`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_export.py#L227)
- `test_component_name_groups_project_components(path: str, expected: str)` — [`L114`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_export.py#L114)
- `test_package_diagram_aggregates_import_edges(monkeypatch)` — [`L194`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_export.py#L194)
- `test_package_name_groups_file_paths(path: str, expected: str)` — [`L100`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_export.py#L100)
- `test_render_class_mermaid_uses_inheritance_arrows()` — [`L22`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_export.py#L22)
- `test_render_flowchart_mermaid_labels_weighted_edges()` — [`L33`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_export.py#L33)
- `test_render_flowchart_mermaid_supports_unlabeled_edges()` — [`L44`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_export.py#L44)
- `test_render_sequence_mermaid_empty_hops_are_explicit()` — [`L75`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_export.py#L75)
- `test_render_sequence_mermaid_empty_path_is_explicit()` — [`L69`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_export.py#L69)
- `test_render_sequence_mermaid_skips_incomplete_hops()` — [`L81`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_export.py#L81)
- `test_render_sequence_mermaid_uses_first_call_path()` — [`L50`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_export.py#L50)
- `test_sequence_diagram_uses_call_path_and_marks_static_approximation(monkeypatch)` — [`L259`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_uml_export.py#L259)

