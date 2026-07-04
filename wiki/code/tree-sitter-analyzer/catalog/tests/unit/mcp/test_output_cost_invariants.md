---
title: 'Module: tests/unit/mcp/test_output_cost_invariants.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_output_cost_invariants.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_output_cost_invariants`/
symbols:
  _make_synthetic_uml_response: _make_synthetic_uml_response().
  test_viz_boundary_toon_disjoint: test_viz_boundary_toon_disjoint().
  test_toon_strip_no_bulk_at_top_level: test_toon_strip_no_bulk_at_top_level().
  _DECISION_TOOLS: _DECISION_TOOLS.
  test_nav_impact_toon_no_bulk_at_top_level: test_nav_impact_toon_no_bulk_at_top_level().
  test_class_diagram_scoped_smaller_than_unscoped: test_class_diagram_scoped_smaller_than_unscoped().
  _measure: _measure().
  test_outline_wide_class_methods_bounded_by_cap: test_outline_wide_class_methods_bounded_by_cap().
  _make_synthetic_callers_payload: _make_synthetic_callers_payload().
  _is_bulk: _is_bulk().
  _make_synthetic_similarity_compact_response: _make_synthetic_similarity_compact_response().
  test_compact_only_strictly_reduces_default_toon: test_compact_only_strictly_reduces_default_toon().
  test_viz_uml_toon_no_bulk_duplication: test_viz_uml_toon_no_bulk_duplication().
  test_viz_graph_toon_no_mermaid_duplication: test_viz_graph_toon_no_mermaid_duplication().
  test_viz_uml_toon_smaller_than_json: test_viz_uml_toon_smaller_than_json().
  test_viz_graph_toon_smaller_than_json: test_viz_graph_toon_smaller_than_json().
  test_nav_impact_toon_smaller_than_json: test_nav_impact_toon_smaller_than_json().
  test_class_diagram_scoped_smaller_than_unscoped.FakeExporterProvider.uml_exporter: test_class_diagram_scoped_smaller_than_unscoped().FakeExporterProvider#uml_exporter().
  test_similarity_summary_smaller_than_full_bodies: test_similarity_summary_smaller_than_full_bodies().
  test_content_truncation_structural_fields: test_content_truncation_structural_fields().
  test_content_no_truncation_structural_fields: test_content_no_truncation_structural_fields().
  test_content_default_cap_bytes_smaller_than_uncapped: test_content_default_cap_bytes_smaller_than_uncapped().
  test_viz_boundary_toon_disjoint.cap_decorator: test_viz_boundary_toon_disjoint().cap_decorator().
  _make_synthetic_similarity_response: _make_synthetic_similarity_response().
  _make_synthetic_content_response: _make_synthetic_content_response().
  test_viz_boundary_toon_disjoint.run_test: test_viz_boundary_toon_disjoint().run_test().
  test_viz_boundary_toon_disjoint.run_test.fake_execute: test_viz_boundary_toon_disjoint().run_test().fake_execute().
  test_toon_meets_its_efficiency_premise: test_toon_meets_its_efficiency_premise().
  test_viz_similarity_toon_no_groups_duplication: test_viz_similarity_toon_no_groups_duplication().
  test_similarity_summary_no_snippet_fields: test_similarity_summary_no_snippet_fields().
  test_similarity_compact_has_sample_files: test_similarity_compact_has_sample_files().
  test_similarity_full_has_snippet_fields: test_similarity_full_has_snippet_fields().
  test_callers_truncation_structural_fields: test_callers_truncation_structural_fields().
  test_callers_no_truncation_structural_fields: test_callers_no_truncation_structural_fields().
  test_callers_default_cap_bytes_smaller_than_unlimited: test_callers_default_cap_bytes_smaller_than_unlimited().
  _bytes: _bytes().
  _BULK_THRESHOLD_BYTES: _BULK_THRESHOLD_BYTES.
  _make_synthetic_nav_impact_response: _make_synthetic_nav_impact_response().
  _BULK_SHAPES._BULK_SHAPES: _BULK_SHAPES._BULK_SHAPES.
  _SAMPLE: _SAMPLE.
  test_viz_boundary_toon_disjoint.cap_decorator.decorator: test_viz_boundary_toon_disjoint().cap_decorator().decorator().
  test_class_diagram_scoped_smaller_than_unscoped.FakeHierarchyAll: test_class_diagram_scoped_smaller_than_unscoped().FakeHierarchyAll#
  test_class_diagram_scoped_smaller_than_unscoped.SentinelCache: test_class_diagram_scoped_smaller_than_unscoped().SentinelCache#
  test_class_diagram_scoped_smaller_than_unscoped.FakeExporterProvider: test_class_diagram_scoped_smaller_than_unscoped().FakeExporterProvider#
  _make_synthetic_similarity_group: _make_synthetic_similarity_group().
  _make_synthetic_similarity_compact_group: _make_synthetic_similarity_compact_group().
  test_class_diagram_scoped_smaller_than_unscoped.FakeHierarchyAll.__init__: test_class_diagram_scoped_smaller_than_unscoped().FakeHierarchyAll#__init__().
  test_class_diagram_scoped_smaller_than_unscoped.FakeHierarchyAll.build: test_class_diagram_scoped_smaller_than_unscoped().FakeHierarchyAll#build().
  test_class_diagram_scoped_smaller_than_unscoped.FakeHierarchyAll.all_classes: test_class_diagram_scoped_smaller_than_unscoped().FakeHierarchyAll#all_classes().
  test_class_diagram_scoped_smaller_than_unscoped.FakeExporterProvider.__init__: test_class_diagram_scoped_smaller_than_unscoped().FakeExporterProvider#__init__().
---
# Module: [`tests/unit/mcp/test_output_cost_invariants.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_output_cost_invariants.py)

## Classes
### `FakeExporterProvider`
- def: [`tests/unit/mcp/test_output_cost_invariants.py:785`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_output_cost_invariants.py#L785)
- signature: `class FakeExporterProvider:`
- members:
  - `uml_exporter(self)` — [`L789`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_output_cost_invariants.py#L789)
- protocol/private: `__init__`[`L786`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_output_cost_invariants.py#L786)
- uses (calls/refs, reference-scoped): [`UMLExporter`](../../../tree_sitter_analyzer/uml_export.md#UMLExporter)  (1 test-only)
- used by: (1 test-only callers)

### `FakeHierarchyAll`
- def: [`tests/unit/mcp/test_output_cost_invariants.py:771`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_output_cost_invariants.py#L771)
- signature: `class FakeHierarchyAll:`
- members:
  - `all_classes(self)` — [`L778`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_output_cost_invariants.py#L778)
  - `build(self)` — [`L775`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_output_cost_invariants.py#L775)
- protocol/private: `__init__`[`L772`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_output_cost_invariants.py#L772)
- used by: (1 test-only callers)

### `SentinelCache`
- def: [`tests/unit/mcp/test_output_cost_invariants.py:782`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_output_cost_invariants.py#L782)
- signature: `class SentinelCache:`
- used by: (1 test-only callers)

## Functions
- `_bytes(payload: dict)` — [`L41`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_output_cost_invariants.py#L41)
- `_is_bulk(value: object)` — [`L388`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_output_cost_invariants.py#L388) — Return True when ``value`` is a list/dict that exceeds the bulk threshold.
- `_make_synthetic_callers_payload(n_callers: int, limit: int)` — [`L1014`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_output_cost_invariants.py#L1014) — Synthetic callers_tool response dict for n_callers callers, capped at limit.
- `_make_synthetic_content_response(n_shown: int, n_total: int, cap: int)` — [`L1131`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_output_cost_invariants.py#L1131) — Synthetic search_content respond_full payload — no tmp paths.
- `_make_synthetic_nav_impact_response(n: int = 50)` — [`L616`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_output_cost_invariants.py#L616) — Build a realistic nav action=impact / function_impact response dict.
- `_make_synthetic_similarity_compact_group(i: int)` — [`L886`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_output_cost_invariants.py#L886) — Compact summary group — no functions list, just sample_files (#801 fix).
- `_make_synthetic_similarity_compact_response()` — [`L897`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_output_cost_invariants.py#L897) — Deterministic compact response — groups have sample_files, not functions[].
- `_make_synthetic_similarity_group(i: int, include_snippet: bool)` — [`L839`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_output_cost_invariants.py#L839) — One synthetic clone group with 3 function entries.
- `_make_synthetic_similarity_response(include_snippets: bool)` — [`L862`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_output_cost_invariants.py#L862) — Deterministic full-bodies similarity response.
- `_make_synthetic_uml_response(n_classes: int = 20)` — [`L132`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_output_cost_invariants.py#L132) — Build a synthetic UML response dict (mimics CodeGraphUMLTool.execute output).
- `_measure(tmp_path, tool_cls, needs_file: bool, **extra)` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_output_cost_invariants.py#L45) — Return (json_bytes, toon_bytes) for one tool invocation pair.
- `cap_decorator(name)` — [`L327`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_output_cost_invariants.py#L327)
- `decorator(func)` — [`L328`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_output_cost_invariants.py#L328)
- `fake_execute(_args)` — [`L350`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_output_cost_invariants.py#L350)
- `run_test()` — [`L349`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_output_cost_invariants.py#L349)
- `test_callers_default_cap_bytes_smaller_than_unlimited()` — [`L1079`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_output_cost_invariants.py#L1079) — DF-13 rule-11 differential: default (50/200) bytes < unlimited (200/200).
- `test_callers_no_truncation_structural_fields()` — [`L1069`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_output_cost_invariants.py#L1069) — DF-13: 10 callers with default cap 50 → truncated=False, all listed.
- `test_callers_truncation_structural_fields()` — [`L1055`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_output_cost_invariants.py#L1055) — DF-13: default (50/200) response carries correct truncation fields.
- `test_class_diagram_scoped_smaller_than_unscoped(monkeypatch)` — [`L746`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_output_cost_invariants.py#L746) — Scoped class diagram bytes < unscoped bytes (rule-11 differential invariant).
- `test_compact_only_strictly_reduces_default_toon(tmp_path, tool_cls, needs_file, tool_id)` — [`L101`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_output_cost_invariants.py#L101) — RFC-0012 Phase 1's reason to exist, as an invariant: compact < default.
- `test_content_default_cap_bytes_smaller_than_uncapped()` — [`L1194`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_output_cost_invariants.py#L1194) — DF-1 rule-11 differential: capped (50/80) bytes < uncapped (80/80).
- `test_content_no_truncation_structural_fields()` — [`L1180`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_output_cost_invariants.py#L1180) — DF-1: 30 matches with default cap 50 → truncated=False, all listed.
- `test_content_truncation_structural_fields()` — [`L1165`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_output_cost_invariants.py#L1165) — DF-1: capped (50/80) response carries correct truncation fields.
- `test_nav_impact_toon_no_bulk_at_top_level()` — [`L670`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_output_cost_invariants.py#L670) — Issue #439 (reopened): nav impact TOON must strip all bulk fields.
- `test_nav_impact_toon_smaller_than_json()` — [`L709`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_output_cost_invariants.py#L709) — Rule-11 ratchet: nav impact TOON bytes < JSON bytes (50-row payload).
- `test_outline_wide_class_methods_bounded_by_cap(tmp_path)` — [`L1227`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_output_cost_invariants.py#L1227) — #571: a single wide class must not detonate the outline response.
- `test_similarity_compact_has_sample_files()` — [`L961`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_output_cost_invariants.py#L961) — Structural invariant: compact groups must contain 'sample_files' key (#801).
- `test_similarity_full_has_snippet_fields()` — [`L978`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_output_cost_invariants.py#L978) — Structural invariant: full-bodies groups must contain 'snippet' key.
- `test_similarity_summary_no_snippet_fields()` — [`L943`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_output_cost_invariants.py#L943) — Structural invariant: compact groups must not contain 'snippet' or 'functions' keys.
- `test_similarity_summary_smaller_than_full_bodies()` — [`L914`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_output_cost_invariants.py#L914) — Rule-11 differential invariant: compact response < full-bodies response.
- `test_toon_meets_its_efficiency_premise(tmp_path, tool_cls, needs_file, tool_id, compact)` — [`L86`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_output_cost_invariants.py#L86) — The §1 premise as an executable invariant: TOON must be <= JSON.
- `test_toon_strip_no_bulk_at_top_level(field_name: str, bulk_value: object)` — [`L553`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_output_cost_invariants.py#L553) — Global structural invariant: no bulk list/dict survives TOON formatting.
- `test_viz_boundary_toon_disjoint()` — [`L288`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_output_cost_invariants.py#L288) — Through the handle_call_tool boundary: viz TOON top-level keys ∩ bulk keys == ∅.
- `test_viz_graph_toon_no_mermaid_duplication()` — [`L181`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_output_cost_invariants.py#L181) — action=graph: mermaid must not appear at top level of TOON response.
- `test_viz_graph_toon_smaller_than_json()` — [`L264`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_output_cost_invariants.py#L264) — Rule-11 ratchet: viz graph TOON bytes < JSON bytes (currently xfail — no duplication,
- `test_viz_similarity_toon_no_groups_duplication()` — [`L199`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_output_cost_invariants.py#L199) — action=similarity: groups must not appear at top level of TOON response.
- `test_viz_uml_toon_no_bulk_duplication()` — [`L154`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_output_cost_invariants.py#L154) — After the fix: nodes/edges/mermaid must NOT appear at top level of TOON response.
- `test_viz_uml_toon_smaller_than_json()` — [`L228`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_output_cost_invariants.py#L228) — Rule-11 differential invariant: viz UML TOON bytes < JSON bytes.

## Module values
- `_BULK_SHAPES` — [`L408`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_output_cost_invariants.py#L408)
- `_BULK_THRESHOLD_BYTES` — [`L385`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_output_cost_invariants.py#L385)
- `_DECISION_TOOLS` — [`L60`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_output_cost_invariants.py#L60)
- `_SAMPLE` — [`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_output_cost_invariants.py#L38)

